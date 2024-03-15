
# Results vs. 3.12.0

- fork: python
- ref: v3.11.8
- machine: windows-amd64
- commit hash: db85d51
- commit date: 2024-02-06
- overall geometric mean: 1.04x slower \*
- HPT reliability: 98.23%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1-amd64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 206 ms: 1.06x faster                                        |
| chameleon      | 4.98 ms                                                     | 5.18 ms: 1.04x slower                                       |
| docutils       | 1.66 sec                                                    | 1.56 sec: 1.06x faster                                      |
| tornado_http   | 89.5 ms                                                     | 88.0 ms: 1.02x faster                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1-amd64-python-v3.11.8-3.11.8-db85d51 |
|-------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| async_tree_none_tg      | 285 ms                                                      | 292 ms: 1.03x slower                                        |
| async_tree_io_tg        | 771 ms                                                      | 794 ms: 1.03x slower                                        |
| async_tree_cpu_io_mixed | 489 ms                                                      | 521 ms: 1.06x slower                                        |
| async_tree_none         | 291 ms                                                      | 312 ms: 1.07x slower                                        |
| async_tree_io           | 731 ms                                                      | 785 ms: 1.07x slower                                        |
| async_tree_memoization  | 339 ms                                                      | 379 ms: 1.12x slower                                        |
| Geometric mean          | (ref)                                                       | 1.05x slower                                                |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1-amd64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| float          | 56.8 ms                                                     | 53.6 ms: 1.06x faster                                       |
| pidigits       | 152 ms                                                      | 148 ms: 1.03x faster                                        |
| Geometric mean | (ref)                                                       | 1.03x faster                                                |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1-amd64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| regex_effbot   | 1.62 ms                                                     | 1.49 ms: 1.08x faster                                       |
| regex_dna      | 126 ms                                                      | 117 ms: 1.08x faster                                        |
| regex_v8       | 14.2 ms                                                     | 13.6 ms: 1.05x faster                                       |
| regex_compile  | 87.5 ms                                                     | 88.2 ms: 1.01x slower                                       |
| Geometric mean | (ref)                                                       | 1.05x faster                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1-amd64-python-v3.11.8-3.11.8-db85d51 |
|----------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| pickle               | 7.43 us                                                     | 6.78 us: 1.10x faster                                       |
| json_loads           | 13.9 us                                                     | 12.9 us: 1.08x faster                                       |
| xml_etree_generate   | 55.8 ms                                                     | 52.7 ms: 1.06x faster                                       |
| unpickle_list        | 2.75 us                                                     | 2.61 us: 1.05x faster                                       |
| unpickle             | 8.18 us                                                     | 7.78 us: 1.05x faster                                       |
| pickle_list          | 2.83 us                                                     | 2.71 us: 1.04x faster                                       |
| xml_etree_process    | 37.7 ms                                                     | 36.7 ms: 1.03x faster                                       |
| pickle_dict          | 18.4 us                                                     | 18.5 us: 1.00x slower                                       |
| pickle_pure_python   | 195 us                                                      | 201 us: 1.03x slower                                        |
| tomli_loads          | 1.37 sec                                                    | 1.42 sec: 1.04x slower                                      |
| xml_etree_parse      | 93.0 ms                                                     | 102 ms: 1.10x slower                                        |
| unpickle_pure_python | 133 us                                                      | 150 us: 1.12x slower                                        |
| json_dumps           | 5.70 ms                                                     | 7.80 ms: 1.37x slower                                       |
| Geometric mean       | (ref)                                                       | 1.01x slower                                                |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1-amd64-python-v3.11.8-3.11.8-db85d51 |
|------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| python_startup_no_site | 16.2 ms                                                     | 15.3 ms: 1.06x faster                                       |
| python_startup         | 19.5 ms                                                     | 18.4 ms: 1.06x faster                                       |
| Geometric mean         | (ref)                                                       | 1.06x faster                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1-amd64-python-v3.11.8-3.11.8-db85d51 |
|-----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| django_template | 22.9 ms                                                     | 23.9 ms: 1.04x slower                                       |
| mako            | 7.09 ms                                                     | 7.47 ms: 1.05x slower                                       |
| Geometric mean  | (ref)                                                       | 1.05x slower                                                |

All benchmarks:
===============

| Benchmark                | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1-amd64-python-v3.11.8-3.11.8-db85d51 |
|--------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| async_generators         | 239 ms                                                      | 178 ms: 1.35x faster                                        |
| pathlib                  | 80.5 ms                                                     | 66.9 ms: 1.20x faster                                       |
| bench_mp_pool            | 69.2 ms                                                     | 61.4 ms: 1.13x faster                                       |
| mypy2                    | 509 ms                                                      | 452 ms: 1.13x faster                                        |
| pickle                   | 7.43 us                                                     | 6.78 us: 1.10x faster                                       |
| regex_effbot             | 1.62 ms                                                     | 1.49 ms: 1.08x faster                                       |
| regex_dna                | 126 ms                                                      | 117 ms: 1.08x faster                                        |
| json_loads               | 13.9 us                                                     | 12.9 us: 1.08x faster                                       |
| asyncio_tcp_ssl          | 2.10 sec                                                    | 1.96 sec: 1.07x faster                                      |
| python_startup_no_site   | 16.2 ms                                                     | 15.3 ms: 1.06x faster                                       |
| docutils                 | 1.66 sec                                                    | 1.56 sec: 1.06x faster                                      |
| float                    | 56.8 ms                                                     | 53.6 ms: 1.06x faster                                       |
| xml_etree_generate       | 55.8 ms                                                     | 52.7 ms: 1.06x faster                                       |
| python_startup           | 19.5 ms                                                     | 18.4 ms: 1.06x faster                                       |
| 2to3                     | 218 ms                                                      | 206 ms: 1.06x faster                                        |
| unpickle_list            | 2.75 us                                                     | 2.61 us: 1.05x faster                                       |
| create_gc_cycles         | 752 us                                                      | 713 us: 1.05x faster                                        |
| unpickle                 | 8.18 us                                                     | 7.78 us: 1.05x faster                                       |
| telco                    | 4.13 ms                                                     | 3.93 ms: 1.05x faster                                       |
| regex_v8                 | 14.2 ms                                                     | 13.6 ms: 1.05x faster                                       |
| aiohttp                  | 884 us                                                      | 846 us: 1.04x faster                                        |
| pickle_list              | 2.83 us                                                     | 2.71 us: 1.04x faster                                       |
| sqlalchemy_declarative   | 86.4 ms                                                     | 83.4 ms: 1.04x faster                                       |
| pidigits                 | 152 ms                                                      | 148 ms: 1.03x faster                                        |
| xml_etree_process        | 37.7 ms                                                     | 36.7 ms: 1.03x faster                                       |
| scimark_sor              | 78.8 ms                                                     | 76.6 ms: 1.03x faster                                       |
| sqlite_synth             | 1.76 us                                                     | 1.71 us: 1.03x faster                                       |
| gc_traversal             | 1.52 ms                                                     | 1.49 ms: 1.02x faster                                       |
| fannkuch                 | 247 ms                                                      | 241 ms: 1.02x faster                                        |
| pycparser                | 699 ms                                                      | 684 ms: 1.02x faster                                        |
| tornado_http             | 89.5 ms                                                     | 88.0 ms: 1.02x faster                                       |
| crypto_pyaes             | 48.5 ms                                                     | 47.7 ms: 1.02x faster                                       |
| scimark_fft              | 184 ms                                                      | 182 ms: 1.01x faster                                        |
| dulwich_log              | 44.3 ms                                                     | 44.0 ms: 1.01x faster                                       |
| pickle_dict              | 18.4 us                                                     | 18.5 us: 1.00x slower                                       |
| spectral_norm            | 66.9 ms                                                     | 67.3 ms: 1.01x slower                                       |
| regex_compile            | 87.5 ms                                                     | 88.2 ms: 1.01x slower                                       |
| sqlglot_optimize         | 34.5 ms                                                     | 34.9 ms: 1.01x slower                                       |
| deepcopy                 | 238 us                                                      | 242 us: 1.02x slower                                        |
| pprint_safe_repr         | 513 ms                                                      | 522 ms: 1.02x slower                                        |
| deepcopy_reduce          | 2.09 us                                                     | 2.13 us: 1.02x slower                                       |
| pprint_pformat           | 1.05 sec                                                    | 1.07 sec: 1.02x slower                                      |
| scimark_sparse_mat_mult  | 2.56 ms                                                     | 2.61 ms: 1.02x slower                                       |
| async_tree_none_tg       | 285 ms                                                      | 292 ms: 1.03x slower                                        |
| pickle_pure_python       | 195 us                                                      | 201 us: 1.03x slower                                        |
| sqlglot_normalize        | 187 ms                                                      | 192 ms: 1.03x slower                                        |
| async_tree_io_tg         | 771 ms                                                      | 794 ms: 1.03x slower                                        |
| nqueens                  | 62.8 ms                                                     | 64.7 ms: 1.03x slower                                       |
| pyflate                  | 295 ms                                                      | 305 ms: 1.03x slower                                        |
| scimark_lu               | 58.9 ms                                                     | 61.0 ms: 1.04x slower                                       |
| tomli_loads              | 1.37 sec                                                    | 1.42 sec: 1.04x slower                                      |
| deepcopy_memo            | 23.7 us                                                     | 24.6 us: 1.04x slower                                       |
| chameleon                | 4.98 ms                                                     | 5.18 ms: 1.04x slower                                       |
| coroutines               | 14.3 ms                                                     | 14.8 ms: 1.04x slower                                       |
| django_template          | 22.9 ms                                                     | 23.9 ms: 1.04x slower                                       |
| sympy_integrate          | 13.0 ms                                                     | 13.5 ms: 1.04x slower                                       |
| sympy_str                | 175 ms                                                      | 183 ms: 1.05x slower                                        |
| raytrace                 | 192 ms                                                      | 202 ms: 1.05x slower                                        |
| mako                     | 7.09 ms                                                     | 7.47 ms: 1.05x slower                                       |
| sympy_expand             | 284 ms                                                      | 300 ms: 1.06x slower                                        |
| logging_format           | 6.72 us                                                     | 7.13 us: 1.06x slower                                       |
| scimark_monte_carlo      | 43.7 ms                                                     | 46.5 ms: 1.06x slower                                       |
| async_tree_cpu_io_mixed  | 489 ms                                                      | 521 ms: 1.06x slower                                        |
| richards                 | 28.4 ms                                                     | 30.3 ms: 1.07x slower                                       |
| async_tree_none          | 291 ms                                                      | 312 ms: 1.07x slower                                        |
| async_tree_io            | 731 ms                                                      | 785 ms: 1.07x slower                                        |
| logging_simple           | 6.28 us                                                     | 6.75 us: 1.08x slower                                       |
| comprehensions           | 14.1 us                                                     | 15.2 us: 1.08x slower                                       |
| sympy_sum                | 91.5 ms                                                     | 98.5 ms: 1.08x slower                                       |
| xml_etree_parse          | 93.0 ms                                                     | 102 ms: 1.10x slower                                        |
| coverage                 | 40.8 ms                                                     | 44.8 ms: 1.10x slower                                       |
| sqlalchemy_imperative    | 9.29 ms                                                     | 10.2 ms: 1.10x slower                                       |
| hexiom                   | 4.10 ms                                                     | 4.51 ms: 1.10x slower                                       |
| sqlglot_transpile        | 1.02 ms                                                     | 1.14 ms: 1.11x slower                                       |
| async_tree_memoization   | 339 ms                                                      | 379 ms: 1.12x slower                                        |
| chaos                    | 43.3 ms                                                     | 48.5 ms: 1.12x slower                                       |
| unpickle_pure_python     | 133 us                                                      | 150 us: 1.12x slower                                        |
| go                       | 91.6 ms                                                     | 103 ms: 1.13x slower                                        |
| logging_silent           | 60.5 ns                                                     | 69.9 ns: 1.16x slower                                       |
| sqlglot_parse            | 804 us                                                      | 929 us: 1.16x slower                                        |
| richards_super           | 32.1 ms                                                     | 37.6 ms: 1.17x slower                                       |
| mdp                      | 1.37 sec                                                    | 1.61 sec: 1.18x slower                                      |
| deltablue                | 2.16 ms                                                     | 2.62 ms: 1.21x slower                                       |
| unpack_sequence          | 37.5 ns                                                     | 47.3 ns: 1.26x slower                                       |
| json_dumps               | 5.70 ms                                                     | 7.80 ms: 1.37x slower                                       |
| asyncio_tcp              | 487 ms                                                      | 709 ms: 1.45x slower                                        |
| generators               | 22.5 ms                                                     | 33.5 ms: 1.49x slower                                       |
| typing_runtime_protocols | 95.1 us                                                     | 328 us: 3.45x slower                                        |
| Geometric mean           | (ref)                                                       | 1.04x slower                                                |

Benchmark hidden because not significant (8): bench_thread_pool, async_tree_cpu_io_mixed_tg, nbody, dask, meteor_contest, xml_etree_iterparse, async_tree_memoization_tg, json
Ignored benchmarks (6) of results/bm-20240206-3.11.8-db85d51/bm-20240206-pythonperf1-amd64-python-v3.11.8-3.11.8-db85d51.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 98.23% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown