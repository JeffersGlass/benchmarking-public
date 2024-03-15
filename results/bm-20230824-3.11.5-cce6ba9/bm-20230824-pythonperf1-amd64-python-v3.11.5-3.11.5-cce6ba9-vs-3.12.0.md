
# Results vs. 3.12.0

- fork: python
- ref: v3.11.5
- machine: windows-amd64
- commit hash: cce6ba9
- commit date: 2023-08-24
- overall geometric mean: 1.05x slower \*
- HPT reliability: 98.11%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230824-pythonperf1-amd64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 208 ms: 1.05x faster                                        |
| chameleon      | 4.98 ms                                                     | 5.27 ms: 1.06x slower                                       |
| docutils       | 1.66 sec                                                    | 1.60 sec: 1.04x faster                                      |
| tornado_http   | 89.5 ms                                                     | 90.6 ms: 1.01x slower                                       |
| Geometric mean | (ref)                                                       | 1.00x faster                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230824-pythonperf1-amd64-python-v3.11.5-3.11.5-cce6ba9 |
|-------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| async_tree_cpu_io_mixed | 489 ms                                                      | 516 ms: 1.06x slower                                        |
| async_tree_io           | 731 ms                                                      | 779 ms: 1.07x slower                                        |
| async_tree_none         | 291 ms                                                      | 311 ms: 1.07x slower                                        |
| async_tree_memoization  | 339 ms                                                      | 375 ms: 1.11x slower                                        |
| Geometric mean          | (ref)                                                       | 1.07x slower                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230824-pythonperf1-amd64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| float          | 56.8 ms                                                     | 53.9 ms: 1.05x faster                                       |
| pidigits       | 152 ms                                                      | 148 ms: 1.03x faster                                        |
| nbody          | 71.9 ms                                                     | 70.1 ms: 1.03x faster                                       |
| Geometric mean | (ref)                                                       | 1.04x faster                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230824-pythonperf1-amd64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| regex_effbot   | 1.62 ms                                                     | 1.49 ms: 1.09x faster                                       |
| regex_dna      | 126 ms                                                      | 117 ms: 1.08x faster                                        |
| regex_v8       | 14.2 ms                                                     | 13.8 ms: 1.04x faster                                       |
| regex_compile  | 87.5 ms                                                     | 91.3 ms: 1.04x slower                                       |
| Geometric mean | (ref)                                                       | 1.04x faster                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230824-pythonperf1-amd64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| pickle               | 7.43 us                                                     | 6.86 us: 1.08x faster                                       |
| xml_etree_generate   | 55.8 ms                                                     | 51.8 ms: 1.08x faster                                       |
| json_loads           | 13.9 us                                                     | 13.0 us: 1.07x faster                                       |
| unpickle_list        | 2.75 us                                                     | 2.60 us: 1.06x faster                                       |
| unpickle             | 8.18 us                                                     | 7.92 us: 1.03x faster                                       |
| xml_etree_iterparse  | 65.2 ms                                                     | 63.4 ms: 1.03x faster                                       |
| pickle_list          | 2.83 us                                                     | 2.75 us: 1.03x faster                                       |
| xml_etree_process    | 37.7 ms                                                     | 36.9 ms: 1.02x faster                                       |
| pickle_dict          | 18.4 us                                                     | 18.5 us: 1.01x slower                                       |
| tomli_loads          | 1.37 sec                                                    | 1.41 sec: 1.03x slower                                      |
| pickle_pure_python   | 195 us                                                      | 202 us: 1.03x slower                                        |
| xml_etree_parse      | 93.0 ms                                                     | 97.0 ms: 1.04x slower                                       |
| unpickle_pure_python | 133 us                                                      | 151 us: 1.13x slower                                        |
| json_dumps           | 5.70 ms                                                     | 7.63 ms: 1.34x slower                                       |
| Geometric mean       | (ref)                                                       | 1.01x slower                                                |

Benchmarks with tag 'startup':
==============================

Benchmark hidden because not significant (2): python_startup, python_startup_no_site

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230824-pythonperf1-amd64-python-v3.11.5-3.11.5-cce6ba9 |
|-----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| django_template | 22.9 ms                                                     | 23.9 ms: 1.04x slower                                       |
| mako            | 7.09 ms                                                     | 7.44 ms: 1.05x slower                                       |
| Geometric mean  | (ref)                                                       | 1.04x slower                                                |

All benchmarks:
===============

| Benchmark                | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230824-pythonperf1-amd64-python-v3.11.5-3.11.5-cce6ba9 |
|--------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| async_generators         | 239 ms                                                      | 180 ms: 1.33x faster                                        |
| pathlib                  | 80.5 ms                                                     | 69.7 ms: 1.15x faster                                       |
| bench_mp_pool            | 69.2 ms                                                     | 61.5 ms: 1.12x faster                                       |
| regex_effbot             | 1.62 ms                                                     | 1.49 ms: 1.09x faster                                       |
| pickle                   | 7.43 us                                                     | 6.86 us: 1.08x faster                                       |
| regex_dna                | 126 ms                                                      | 117 ms: 1.08x faster                                        |
| xml_etree_generate       | 55.8 ms                                                     | 51.8 ms: 1.08x faster                                       |
| json_loads               | 13.9 us                                                     | 13.0 us: 1.07x faster                                       |
| create_gc_cycles         | 752 us                                                      | 709 us: 1.06x faster                                        |
| unpickle_list            | 2.75 us                                                     | 2.60 us: 1.06x faster                                       |
| float                    | 56.8 ms                                                     | 53.9 ms: 1.05x faster                                       |
| 2to3                     | 218 ms                                                      | 208 ms: 1.05x faster                                        |
| telco                    | 4.13 ms                                                     | 3.96 ms: 1.04x faster                                       |
| aiohttp                  | 884 us                                                      | 853 us: 1.04x faster                                        |
| docutils                 | 1.66 sec                                                    | 1.60 sec: 1.04x faster                                      |
| regex_v8                 | 14.2 ms                                                     | 13.8 ms: 1.04x faster                                       |
| unpickle                 | 8.18 us                                                     | 7.92 us: 1.03x faster                                       |
| sqlalchemy_declarative   | 86.4 ms                                                     | 83.8 ms: 1.03x faster                                       |
| pidigits                 | 152 ms                                                      | 148 ms: 1.03x faster                                        |
| scimark_sor              | 78.8 ms                                                     | 76.5 ms: 1.03x faster                                       |
| gc_traversal             | 1.52 ms                                                     | 1.48 ms: 1.03x faster                                       |
| xml_etree_iterparse      | 65.2 ms                                                     | 63.4 ms: 1.03x faster                                       |
| pickle_list              | 2.83 us                                                     | 2.75 us: 1.03x faster                                       |
| nbody                    | 71.9 ms                                                     | 70.1 ms: 1.03x faster                                       |
| sqlite_synth             | 1.76 us                                                     | 1.72 us: 1.02x faster                                       |
| xml_etree_process        | 37.7 ms                                                     | 36.9 ms: 1.02x faster                                       |
| deepcopy_reduce          | 2.09 us                                                     | 2.06 us: 1.02x faster                                       |
| scimark_fft              | 184 ms                                                      | 181 ms: 1.02x faster                                        |
| dulwich_log              | 44.3 ms                                                     | 43.6 ms: 1.01x faster                                       |
| crypto_pyaes             | 48.5 ms                                                     | 48.1 ms: 1.01x faster                                       |
| nqueens                  | 62.8 ms                                                     | 62.3 ms: 1.01x faster                                       |
| pickle_dict              | 18.4 us                                                     | 18.5 us: 1.01x slower                                       |
| scimark_sparse_mat_mult  | 2.56 ms                                                     | 2.57 ms: 1.01x slower                                       |
| pprint_pformat           | 1.05 sec                                                    | 1.05 sec: 1.01x slower                                      |
| spectral_norm            | 66.9 ms                                                     | 67.5 ms: 1.01x slower                                       |
| tornado_http             | 89.5 ms                                                     | 90.6 ms: 1.01x slower                                       |
| deepcopy                 | 238 us                                                      | 241 us: 1.01x slower                                        |
| coroutines               | 14.3 ms                                                     | 14.5 ms: 1.02x slower                                       |
| sqlglot_normalize        | 187 ms                                                      | 190 ms: 1.02x slower                                        |
| pyflate                  | 295 ms                                                      | 302 ms: 1.03x slower                                        |
| tomli_loads              | 1.37 sec                                                    | 1.41 sec: 1.03x slower                                      |
| meteor_contest           | 74.6 ms                                                     | 76.8 ms: 1.03x slower                                       |
| pickle_pure_python       | 195 us                                                      | 202 us: 1.03x slower                                        |
| django_template          | 22.9 ms                                                     | 23.9 ms: 1.04x slower                                       |
| xml_etree_parse          | 93.0 ms                                                     | 97.0 ms: 1.04x slower                                       |
| regex_compile            | 87.5 ms                                                     | 91.3 ms: 1.04x slower                                       |
| deepcopy_memo            | 23.7 us                                                     | 24.7 us: 1.04x slower                                       |
| logging_simple           | 6.28 us                                                     | 6.56 us: 1.05x slower                                       |
| sympy_str                | 175 ms                                                      | 183 ms: 1.05x slower                                        |
| mako                     | 7.09 ms                                                     | 7.44 ms: 1.05x slower                                       |
| logging_format           | 6.72 us                                                     | 7.06 us: 1.05x slower                                       |
| sympy_expand             | 284 ms                                                      | 299 ms: 1.05x slower                                        |
| async_tree_cpu_io_mixed  | 489 ms                                                      | 516 ms: 1.06x slower                                        |
| raytrace                 | 192 ms                                                      | 203 ms: 1.06x slower                                        |
| chameleon                | 4.98 ms                                                     | 5.27 ms: 1.06x slower                                       |
| richards                 | 28.4 ms                                                     | 30.1 ms: 1.06x slower                                       |
| sympy_integrate          | 13.0 ms                                                     | 13.7 ms: 1.06x slower                                       |
| scimark_monte_carlo      | 43.7 ms                                                     | 46.5 ms: 1.06x slower                                       |
| scimark_lu               | 58.9 ms                                                     | 62.7 ms: 1.06x slower                                       |
| async_tree_io            | 731 ms                                                      | 779 ms: 1.07x slower                                        |
| async_tree_none          | 291 ms                                                      | 311 ms: 1.07x slower                                        |
| go                       | 91.6 ms                                                     | 98.8 ms: 1.08x slower                                       |
| fannkuch                 | 247 ms                                                      | 268 ms: 1.09x slower                                        |
| sympy_sum                | 91.5 ms                                                     | 100 ms: 1.10x slower                                        |
| async_tree_memoization   | 339 ms                                                      | 375 ms: 1.11x slower                                        |
| sqlglot_transpile        | 1.02 ms                                                     | 1.13 ms: 1.11x slower                                       |
| hexiom                   | 4.10 ms                                                     | 4.55 ms: 1.11x slower                                       |
| sqlalchemy_imperative    | 9.29 ms                                                     | 10.4 ms: 1.12x slower                                       |
| comprehensions           | 14.1 us                                                     | 15.9 us: 1.13x slower                                       |
| unpickle_pure_python     | 133 us                                                      | 151 us: 1.13x slower                                        |
| chaos                    | 43.3 ms                                                     | 49.5 ms: 1.14x slower                                       |
| sqlglot_parse            | 804 us                                                      | 928 us: 1.15x slower                                        |
| logging_silent           | 60.5 ns                                                     | 70.0 ns: 1.16x slower                                       |
| richards_super           | 32.1 ms                                                     | 38.0 ms: 1.18x slower                                       |
| mdp                      | 1.37 sec                                                    | 1.63 sec: 1.19x slower                                      |
| deltablue                | 2.16 ms                                                     | 2.61 ms: 1.21x slower                                       |
| unpack_sequence          | 37.5 ns                                                     | 45.5 ns: 1.21x slower                                       |
| coverage                 | 40.8 ms                                                     | 54.3 ms: 1.33x slower                                       |
| json_dumps               | 5.70 ms                                                     | 7.63 ms: 1.34x slower                                       |
| asyncio_tcp              | 487 ms                                                      | 694 ms: 1.42x slower                                        |
| generators               | 22.5 ms                                                     | 33.8 ms: 1.50x slower                                       |
| typing_runtime_protocols | 95.1 us                                                     | 327 us: 3.44x slower                                        |
| Geometric mean           | (ref)                                                       | 1.05x slower                                                |

Benchmark hidden because not significant (9): asyncio_tcp_ssl, python_startup, pprint_safe_repr, sqlglot_optimize, pycparser, json, bench_thread_pool, dask, python_startup_no_site
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, mypy2
Ignored benchmarks (6) of results/bm-20230824-3.11.5-cce6ba9/bm-20230824-pythonperf1-amd64-python-v3.11.5-3.11.5-cce6ba9.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 98.11% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown