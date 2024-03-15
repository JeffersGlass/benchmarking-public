
# Results vs. 3.12.0

- fork: python
- ref: v3.11.6
- machine: windows-amd64
- commit hash: 8b6ee5b
- commit date: 2023-10-02
- overall geometric mean: 1.05x slower \*
- HPT reliability: 99.29%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231002-pythonperf1-amd64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 207 ms: 1.05x faster                                        |
| chameleon      | 4.98 ms                                                     | 5.24 ms: 1.05x slower                                       |
| docutils       | 1.66 sec                                                    | 1.60 sec: 1.04x faster                                      |
| tornado_http   | 89.5 ms                                                     | 90.5 ms: 1.01x slower                                       |
| Geometric mean | (ref)                                                       | 1.01x faster                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231002-pythonperf1-amd64-python-v3.11.6-3.11.6-8b6ee5b |
|-------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| async_tree_cpu_io_mixed | 489 ms                                                      | 515 ms: 1.05x slower                                        |
| async_tree_io           | 731 ms                                                      | 778 ms: 1.06x slower                                        |
| async_tree_none         | 291 ms                                                      | 311 ms: 1.07x slower                                        |
| async_tree_memoization  | 339 ms                                                      | 375 ms: 1.10x slower                                        |
| Geometric mean          | (ref)                                                       | 1.07x slower                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231002-pythonperf1-amd64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| float          | 56.8 ms                                                     | 54.3 ms: 1.05x faster                                       |
| nbody          | 71.9 ms                                                     | 69.7 ms: 1.03x faster                                       |
| pidigits       | 152 ms                                                      | 148 ms: 1.03x faster                                        |
| Geometric mean | (ref)                                                       | 1.03x faster                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231002-pythonperf1-amd64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| regex_effbot   | 1.62 ms                                                     | 1.53 ms: 1.06x faster                                       |
| regex_dna      | 126 ms                                                      | 122 ms: 1.04x faster                                        |
| regex_v8       | 14.2 ms                                                     | 14.2 ms: 1.00x faster                                       |
| regex_compile  | 87.5 ms                                                     | 91.7 ms: 1.05x slower                                       |
| Geometric mean | (ref)                                                       | 1.01x faster                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231002-pythonperf1-amd64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| pickle               | 7.43 us                                                     | 6.67 us: 1.11x faster                                       |
| unpickle             | 8.18 us                                                     | 7.67 us: 1.07x faster                                       |
| xml_etree_generate   | 55.8 ms                                                     | 52.9 ms: 1.06x faster                                       |
| json_loads           | 13.9 us                                                     | 13.2 us: 1.05x faster                                       |
| pickle_list          | 2.83 us                                                     | 2.70 us: 1.05x faster                                       |
| unpickle_list        | 2.75 us                                                     | 2.64 us: 1.04x faster                                       |
| xml_etree_iterparse  | 65.2 ms                                                     | 63.3 ms: 1.03x faster                                       |
| tomli_loads          | 1.37 sec                                                    | 1.42 sec: 1.03x slower                                      |
| pickle_pure_python   | 195 us                                                      | 203 us: 1.04x slower                                        |
| xml_etree_parse      | 93.0 ms                                                     | 97.3 ms: 1.05x slower                                       |
| unpickle_pure_python | 133 us                                                      | 151 us: 1.13x slower                                        |
| json_dumps           | 5.70 ms                                                     | 7.74 ms: 1.36x slower                                       |
| Geometric mean       | (ref)                                                       | 1.01x slower                                                |

Benchmark hidden because not significant (2): pickle_dict, xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231002-pythonperf1-amd64-python-v3.11.6-3.11.6-8b6ee5b |
|------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 18.6 ms: 1.05x faster                                       |
| python_startup_no_site | 16.2 ms                                                     | 15.6 ms: 1.04x faster                                       |
| Geometric mean         | (ref)                                                       | 1.05x faster                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231002-pythonperf1-amd64-python-v3.11.6-3.11.6-8b6ee5b |
|-----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| django_template | 22.9 ms                                                     | 23.6 ms: 1.03x slower                                       |
| mako            | 7.09 ms                                                     | 7.31 ms: 1.03x slower                                       |
| Geometric mean  | (ref)                                                       | 1.03x slower                                                |

All benchmarks:
===============

| Benchmark                | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231002-pythonperf1-amd64-python-v3.11.6-3.11.6-8b6ee5b |
|--------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| async_generators         | 239 ms                                                      | 179 ms: 1.34x faster                                        |
| bench_mp_pool            | 69.2 ms                                                     | 58.7 ms: 1.18x faster                                       |
| pathlib                  | 80.5 ms                                                     | 68.5 ms: 1.17x faster                                       |
| pickle                   | 7.43 us                                                     | 6.67 us: 1.11x faster                                       |
| unpickle                 | 8.18 us                                                     | 7.67 us: 1.07x faster                                       |
| create_gc_cycles         | 752 us                                                      | 708 us: 1.06x faster                                        |
| regex_effbot             | 1.62 ms                                                     | 1.53 ms: 1.06x faster                                       |
| xml_etree_generate       | 55.8 ms                                                     | 52.9 ms: 1.06x faster                                       |
| json_loads               | 13.9 us                                                     | 13.2 us: 1.05x faster                                       |
| 2to3                     | 218 ms                                                      | 207 ms: 1.05x faster                                        |
| telco                    | 4.13 ms                                                     | 3.93 ms: 1.05x faster                                       |
| python_startup           | 19.5 ms                                                     | 18.6 ms: 1.05x faster                                       |
| pickle_list              | 2.83 us                                                     | 2.70 us: 1.05x faster                                       |
| float                    | 56.8 ms                                                     | 54.3 ms: 1.05x faster                                       |
| python_startup_no_site   | 16.2 ms                                                     | 15.6 ms: 1.04x faster                                       |
| unpickle_list            | 2.75 us                                                     | 2.64 us: 1.04x faster                                       |
| regex_dna                | 126 ms                                                      | 122 ms: 1.04x faster                                        |
| aiohttp                  | 884 us                                                      | 853 us: 1.04x faster                                        |
| docutils                 | 1.66 sec                                                    | 1.60 sec: 1.04x faster                                      |
| nbody                    | 71.9 ms                                                     | 69.7 ms: 1.03x faster                                       |
| sqlalchemy_declarative   | 86.4 ms                                                     | 83.8 ms: 1.03x faster                                       |
| xml_etree_iterparse      | 65.2 ms                                                     | 63.3 ms: 1.03x faster                                       |
| gc_traversal             | 1.52 ms                                                     | 1.48 ms: 1.03x faster                                       |
| scimark_sor              | 78.8 ms                                                     | 76.8 ms: 1.03x faster                                       |
| pidigits                 | 152 ms                                                      | 148 ms: 1.03x faster                                        |
| fannkuch                 | 247 ms                                                      | 241 ms: 1.02x faster                                        |
| sqlite_synth             | 1.76 us                                                     | 1.72 us: 1.02x faster                                       |
| scimark_fft              | 184 ms                                                      | 181 ms: 1.02x faster                                        |
| regex_v8                 | 14.2 ms                                                     | 14.2 ms: 1.00x faster                                       |
| pprint_safe_repr         | 513 ms                                                      | 517 ms: 1.01x slower                                        |
| spectral_norm            | 66.9 ms                                                     | 67.5 ms: 1.01x slower                                       |
| tornado_http             | 89.5 ms                                                     | 90.5 ms: 1.01x slower                                       |
| nqueens                  | 62.8 ms                                                     | 63.7 ms: 1.02x slower                                       |
| pprint_pformat           | 1.05 sec                                                    | 1.06 sec: 1.02x slower                                      |
| sqlglot_optimize         | 34.5 ms                                                     | 35.1 ms: 1.02x slower                                       |
| crypto_pyaes             | 48.5 ms                                                     | 49.3 ms: 1.02x slower                                       |
| dulwich_log              | 44.3 ms                                                     | 45.0 ms: 1.02x slower                                       |
| meteor_contest           | 74.6 ms                                                     | 76.1 ms: 1.02x slower                                       |
| django_template          | 22.9 ms                                                     | 23.6 ms: 1.03x slower                                       |
| sqlglot_normalize        | 187 ms                                                      | 192 ms: 1.03x slower                                        |
| coroutines               | 14.3 ms                                                     | 14.7 ms: 1.03x slower                                       |
| mako                     | 7.09 ms                                                     | 7.31 ms: 1.03x slower                                       |
| deepcopy                 | 238 us                                                      | 246 us: 1.03x slower                                        |
| pyflate                  | 295 ms                                                      | 305 ms: 1.03x slower                                        |
| tomli_loads              | 1.37 sec                                                    | 1.42 sec: 1.03x slower                                      |
| pickle_pure_python       | 195 us                                                      | 203 us: 1.04x slower                                        |
| xml_etree_parse          | 93.0 ms                                                     | 97.3 ms: 1.05x slower                                       |
| regex_compile            | 87.5 ms                                                     | 91.7 ms: 1.05x slower                                       |
| chameleon                | 4.98 ms                                                     | 5.24 ms: 1.05x slower                                       |
| scimark_lu               | 58.9 ms                                                     | 61.9 ms: 1.05x slower                                       |
| async_tree_cpu_io_mixed  | 489 ms                                                      | 515 ms: 1.05x slower                                        |
| raytrace                 | 192 ms                                                      | 203 ms: 1.05x slower                                        |
| scimark_monte_carlo      | 43.7 ms                                                     | 46.3 ms: 1.06x slower                                       |
| async_tree_io            | 731 ms                                                      | 778 ms: 1.06x slower                                        |
| deepcopy_memo            | 23.7 us                                                     | 25.3 us: 1.07x slower                                       |
| sympy_integrate          | 13.0 ms                                                     | 13.8 ms: 1.07x slower                                       |
| async_tree_none          | 291 ms                                                      | 311 ms: 1.07x slower                                        |
| logging_format           | 6.72 us                                                     | 7.18 us: 1.07x slower                                       |
| logging_simple           | 6.28 us                                                     | 6.72 us: 1.07x slower                                       |
| sympy_str                | 175 ms                                                      | 187 ms: 1.07x slower                                        |
| sympy_expand             | 284 ms                                                      | 305 ms: 1.08x slower                                        |
| richards                 | 28.4 ms                                                     | 30.6 ms: 1.08x slower                                       |
| sqlalchemy_imperative    | 9.29 ms                                                     | 10.3 ms: 1.10x slower                                       |
| async_tree_memoization   | 339 ms                                                      | 375 ms: 1.10x slower                                        |
| hexiom                   | 4.10 ms                                                     | 4.55 ms: 1.11x slower                                       |
| sympy_sum                | 91.5 ms                                                     | 102 ms: 1.11x slower                                        |
| comprehensions           | 14.1 us                                                     | 15.7 us: 1.11x slower                                       |
| go                       | 91.6 ms                                                     | 102 ms: 1.11x slower                                        |
| sqlglot_transpile        | 1.02 ms                                                     | 1.14 ms: 1.12x slower                                       |
| unpickle_pure_python     | 133 us                                                      | 151 us: 1.13x slower                                        |
| chaos                    | 43.3 ms                                                     | 49.7 ms: 1.15x slower                                       |
| sqlglot_parse            | 804 us                                                      | 938 us: 1.17x slower                                        |
| logging_silent           | 60.5 ns                                                     | 70.7 ns: 1.17x slower                                       |
| richards_super           | 32.1 ms                                                     | 38.4 ms: 1.20x slower                                       |
| deltablue                | 2.16 ms                                                     | 2.63 ms: 1.22x slower                                       |
| unpack_sequence          | 37.5 ns                                                     | 46.3 ns: 1.23x slower                                       |
| mdp                      | 1.37 sec                                                    | 1.71 sec: 1.25x slower                                      |
| coverage                 | 40.8 ms                                                     | 53.6 ms: 1.31x slower                                       |
| json_dumps               | 5.70 ms                                                     | 7.74 ms: 1.36x slower                                       |
| asyncio_tcp              | 487 ms                                                      | 728 ms: 1.49x slower                                        |
| generators               | 22.5 ms                                                     | 33.7 ms: 1.50x slower                                       |
| typing_runtime_protocols | 95.1 us                                                     | 324 us: 3.41x slower                                        |
| Geometric mean           | (ref)                                                       | 1.05x slower                                                |

Benchmark hidden because not significant (9): asyncio_tcp_ssl, pycparser, bench_thread_pool, json, scimark_sparse_mat_mult, dask, pickle_dict, xml_etree_process, deepcopy_reduce
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, mypy2
Ignored benchmarks (6) of results/bm-20231002-3.11.6-8b6ee5b/bm-20231002-pythonperf1-amd64-python-v3.11.6-3.11.6-8b6ee5b.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 99.29% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown