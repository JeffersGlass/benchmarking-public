
# Results vs. 3.11.0

- fork: python
- ref: v3.12.0rc2
- machine: windows-amd64
- commit hash: 40913a5
- commit date: 2023-09-05
- overall geometric mean: 1.06x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230905-pythonperf1-amd64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 216 ms: 1.01x slower                                              |
| tornado_http   | 92.8 ms                                                     | 88.4 ms: 1.05x faster                                             |
| Geometric mean | (ref)                                                       | 1.01x faster                                                      |

Benchmark hidden because not significant (1): docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230905-pythonperf1-amd64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|-------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| async_tree_memoization  | 399 ms                                                      | 339 ms: 1.18x faster                                              |
| async_tree_none         | 332 ms                                                      | 291 ms: 1.14x faster                                              |
| async_tree_io           | 808 ms                                                      | 722 ms: 1.12x faster                                              |
| async_tree_cpu_io_mixed | 530 ms                                                      | 480 ms: 1.10x faster                                              |
| Geometric mean          | (ref)                                                       | 1.14x faster                                                      |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230905-pythonperf1-amd64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 69.0 ms: 1.02x faster                                             |
| Geometric mean | (ref)                                                       | 1.01x faster                                                      |

Benchmark hidden because not significant (2): pidigits, float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230905-pythonperf1-amd64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 87.5 ms: 1.04x faster                                             |
| regex_v8       | 14.2 ms                                                     | 13.7 ms: 1.04x faster                                             |
| regex_dna      | 116 ms                                                      | 119 ms: 1.02x slower                                              |
| regex_effbot   | 1.50 ms                                                     | 1.58 ms: 1.05x slower                                             |
| Geometric mean | (ref)                                                       | 1.00x faster                                                      |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230905-pythonperf1-amd64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.66 ms: 1.43x faster                                             |
| unpickle_pure_python | 157 us                                                      | 130 us: 1.20x faster                                              |
| pickle_pure_python   | 208 us                                                      | 191 us: 1.09x faster                                              |
| xml_etree_parse      | 97.6 ms                                                     | 89.7 ms: 1.09x faster                                             |
| tomli_loads          | 1.46 sec                                                    | 1.37 sec: 1.06x faster                                            |
| xml_etree_iterparse  | 65.6 ms                                                     | 62.8 ms: 1.04x faster                                             |
| pickle_dict          | 18.5 us                                                     | 18.3 us: 1.01x faster                                             |
| xml_etree_process    | 37.2 ms                                                     | 37.9 ms: 1.02x slower                                             |
| pickle_list          | 2.70 us                                                     | 2.75 us: 1.02x slower                                             |
| unpickle_list        | 2.59 us                                                     | 2.65 us: 1.02x slower                                             |
| json_loads           | 13.0 us                                                     | 13.6 us: 1.05x slower                                             |
| pickle               | 6.64 us                                                     | 6.97 us: 1.05x slower                                             |
| xml_etree_generate   | 52.5 ms                                                     | 55.4 ms: 1.05x slower                                             |
| unpickle             | 7.57 us                                                     | 8.05 us: 1.06x slower                                             |
| Geometric mean       | (ref)                                                       | 1.04x faster                                                      |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230905-pythonperf1-amd64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 16.3 ms: 1.03x faster                                             |
| python_startup         | 19.8 ms                                                     | 19.3 ms: 1.03x faster                                             |
| Geometric mean         | (ref)                                                       | 1.03x faster                                                      |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230905-pythonperf1-amd64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|-----------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 7.00 ms: 1.08x faster                                             |

All benchmarks:
===============

| Benchmark                | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230905-pythonperf1-amd64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|--------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| typing_runtime_protocols | 326 us                                                      | 96.2 us: 3.39x faster                                             |
| asyncio_tcp              | 726 ms                                                      | 480 ms: 1.51x faster                                              |
| json_dumps               | 8.09 ms                                                     | 5.66 ms: 1.43x faster                                             |
| generators               | 34.0 ms                                                     | 24.2 ms: 1.40x faster                                             |
| richards_super           | 38.7 ms                                                     | 29.7 ms: 1.30x faster                                             |
| deltablue                | 2.70 ms                                                     | 2.13 ms: 1.27x faster                                             |
| unpack_sequence          | 46.9 ns                                                     | 38.3 ns: 1.22x faster                                             |
| richards                 | 31.4 ms                                                     | 26.0 ms: 1.21x faster                                             |
| unpickle_pure_python     | 157 us                                                      | 130 us: 1.20x faster                                              |
| logging_silent           | 71.8 ns                                                     | 60.3 ns: 1.19x faster                                             |
| sqlglot_parse            | 953 us                                                      | 808 us: 1.18x faster                                              |
| async_tree_memoization   | 399 ms                                                      | 339 ms: 1.18x faster                                              |
| go                       | 101 ms                                                      | 87.0 ms: 1.16x faster                                             |
| mdp                      | 1.59 sec                                                    | 1.39 sec: 1.15x faster                                            |
| async_tree_none          | 332 ms                                                      | 291 ms: 1.14x faster                                              |
| sqlglot_transpile        | 1.16 ms                                                     | 1.02 ms: 1.14x faster                                             |
| chaos                    | 48.4 ms                                                     | 42.6 ms: 1.13x faster                                             |
| hexiom                   | 4.55 ms                                                     | 4.04 ms: 1.13x faster                                             |
| raytrace                 | 213 ms                                                      | 190 ms: 1.12x faster                                              |
| async_tree_io            | 808 ms                                                      | 722 ms: 1.12x faster                                              |
| async_tree_cpu_io_mixed  | 530 ms                                                      | 480 ms: 1.10x faster                                              |
| logging_simple           | 6.86 us                                                     | 6.24 us: 1.10x faster                                             |
| deepcopy_memo            | 26.0 us                                                     | 23.6 us: 1.10x faster                                             |
| scimark_lu               | 62.8 ms                                                     | 57.2 ms: 1.10x faster                                             |
| spectral_norm            | 68.3 ms                                                     | 62.7 ms: 1.09x faster                                             |
| pickle_pure_python       | 208 us                                                      | 191 us: 1.09x faster                                              |
| xml_etree_parse          | 97.6 ms                                                     | 89.7 ms: 1.09x faster                                             |
| dulwich_log              | 46.4 ms                                                     | 42.8 ms: 1.08x faster                                             |
| mako                     | 7.58 ms                                                     | 7.00 ms: 1.08x faster                                             |
| nqueens                  | 68.3 ms                                                     | 63.9 ms: 1.07x faster                                             |
| pyflate                  | 312 ms                                                      | 293 ms: 1.07x faster                                              |
| logging_format           | 7.16 us                                                     | 6.74 us: 1.06x faster                                             |
| tomli_loads              | 1.46 sec                                                    | 1.37 sec: 1.06x faster                                            |
| scimark_monte_carlo      | 45.3 ms                                                     | 42.8 ms: 1.06x faster                                             |
| pycparser                | 720 ms                                                      | 681 ms: 1.06x faster                                              |
| tornado_http             | 92.8 ms                                                     | 88.4 ms: 1.05x faster                                             |
| xml_etree_iterparse      | 65.6 ms                                                     | 62.8 ms: 1.04x faster                                             |
| pprint_pformat           | 1.09 sec                                                    | 1.04 sec: 1.04x faster                                            |
| crypto_pyaes             | 48.9 ms                                                     | 46.9 ms: 1.04x faster                                             |
| pprint_safe_repr         | 529 ms                                                      | 509 ms: 1.04x faster                                              |
| regex_compile            | 91.0 ms                                                     | 87.5 ms: 1.04x faster                                             |
| regex_v8                 | 14.2 ms                                                     | 13.7 ms: 1.04x faster                                             |
| python_startup_no_site   | 16.8 ms                                                     | 16.3 ms: 1.03x faster                                             |
| meteor_contest           | 75.2 ms                                                     | 73.1 ms: 1.03x faster                                             |
| scimark_sparse_mat_mult  | 2.58 ms                                                     | 2.50 ms: 1.03x faster                                             |
| python_startup           | 19.8 ms                                                     | 19.3 ms: 1.03x faster                                             |
| deepcopy                 | 246 us                                                      | 241 us: 1.02x faster                                              |
| aiohttp                  | 883 us                                                      | 863 us: 1.02x faster                                              |
| comprehensions           | 15.6 us                                                     | 15.3 us: 1.02x faster                                             |
| nbody                    | 70.3 ms                                                     | 69.0 ms: 1.02x faster                                             |
| scimark_fft              | 179 ms                                                      | 176 ms: 1.02x faster                                              |
| fannkuch                 | 253 ms                                                      | 249 ms: 1.02x faster                                              |
| sqlglot_normalize        | 190 ms                                                      | 187 ms: 1.02x faster                                              |
| sqlite_synth             | 1.77 us                                                     | 1.74 us: 1.01x faster                                             |
| scimark_sor              | 78.1 ms                                                     | 77.1 ms: 1.01x faster                                             |
| pickle_dict              | 18.5 us                                                     | 18.3 us: 1.01x faster                                             |
| gc_traversal             | 1.49 ms                                                     | 1.51 ms: 1.01x slower                                             |
| 2to3                     | 214 ms                                                      | 216 ms: 1.01x slower                                              |
| xml_etree_process        | 37.2 ms                                                     | 37.9 ms: 1.02x slower                                             |
| regex_dna                | 116 ms                                                      | 119 ms: 1.02x slower                                              |
| pickle_list              | 2.70 us                                                     | 2.75 us: 1.02x slower                                             |
| unpickle_list            | 2.59 us                                                     | 2.65 us: 1.02x slower                                             |
| telco                    | 4.06 ms                                                     | 4.19 ms: 1.03x slower                                             |
| deepcopy_reduce          | 2.06 us                                                     | 2.15 us: 1.04x slower                                             |
| json_loads               | 13.0 us                                                     | 13.6 us: 1.05x slower                                             |
| pickle                   | 6.64 us                                                     | 6.97 us: 1.05x slower                                             |
| regex_effbot             | 1.50 ms                                                     | 1.58 ms: 1.05x slower                                             |
| xml_etree_generate       | 52.5 ms                                                     | 55.4 ms: 1.05x slower                                             |
| unpickle                 | 7.57 us                                                     | 8.05 us: 1.06x slower                                             |
| bench_mp_pool            | 63.2 ms                                                     | 67.3 ms: 1.06x slower                                             |
| pathlib                  | 70.9 ms                                                     | 78.3 ms: 1.11x slower                                             |
| coverage                 | 43.4 ms                                                     | 50.2 ms: 1.16x slower                                             |
| coroutines               | 15.0 ms                                                     | 19.0 ms: 1.27x slower                                             |
| dask                     | 273 ms                                                      | 363 ms: 1.33x slower                                              |
| async_generators         | 177 ms                                                      | 238 ms: 1.35x slower                                              |
| Geometric mean           | (ref)                                                       | 1.06x faster                                                      |

Benchmark hidden because not significant (8): asyncio_tcp_ssl, bench_thread_pool, sqlglot_optimize, pidigits, float, docutils, json, create_gc_cycles
Ignored benchmarks (19) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, chameleon, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: unknown