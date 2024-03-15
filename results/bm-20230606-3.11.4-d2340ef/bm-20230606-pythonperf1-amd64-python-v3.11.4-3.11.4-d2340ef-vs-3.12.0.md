
# Results vs. 3.12.0

- fork: python
- ref: v3.11.4
- machine: windows-amd64
- commit hash: d2340ef
- commit date: 2023-06-06
- overall geometric mean: 1.08x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 221 ms: 1.01x slower                                        |
| chameleon      | 4.98 ms                                                     | 5.44 ms: 1.09x slower                                       |
| tornado_http   | 89.5 ms                                                     | 103 ms: 1.16x slower                                        |
| Geometric mean | (ref)                                                       | 1.06x slower                                                |

Benchmark hidden because not significant (1): docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef |
|-------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| async_tree_cpu_io_mixed | 489 ms                                                      | 522 ms: 1.07x slower                                        |
| async_tree_io           | 731 ms                                                      | 813 ms: 1.11x slower                                        |
| async_tree_none         | 291 ms                                                      | 334 ms: 1.15x slower                                        |
| async_tree_memoization  | 339 ms                                                      | 392 ms: 1.16x slower                                        |
| Geometric mean          | (ref)                                                       | 1.12x slower                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| nbody          | 71.9 ms                                                     | 70.4 ms: 1.02x faster                                       |
| pidigits       | 152 ms                                                      | 151 ms: 1.01x faster                                        |
| Geometric mean | (ref)                                                       | 1.01x faster                                                |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| regex_effbot   | 1.62 ms                                                     | 1.52 ms: 1.07x faster                                       |
| regex_dna      | 126 ms                                                      | 120 ms: 1.05x faster                                        |
| regex_v8       | 14.2 ms                                                     | 13.9 ms: 1.02x faster                                       |
| regex_compile  | 87.5 ms                                                     | 92.8 ms: 1.06x slower                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef |
|----------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| pickle               | 7.43 us                                                     | 6.74 us: 1.10x faster                                       |
| json_loads           | 13.9 us                                                     | 13.3 us: 1.05x faster                                       |
| xml_etree_generate   | 55.8 ms                                                     | 53.8 ms: 1.04x faster                                       |
| unpickle_list        | 2.75 us                                                     | 2.73 us: 1.01x faster                                       |
| xml_etree_process    | 37.7 ms                                                     | 37.9 ms: 1.00x slower                                       |
| pickle_dict          | 18.4 us                                                     | 18.8 us: 1.02x slower                                       |
| pickle_pure_python   | 195 us                                                      | 201 us: 1.03x slower                                        |
| xml_etree_parse      | 93.0 ms                                                     | 96.4 ms: 1.04x slower                                       |
| tomli_loads          | 1.37 sec                                                    | 1.43 sec: 1.05x slower                                      |
| unpickle_pure_python | 133 us                                                      | 153 us: 1.15x slower                                        |
| json_dumps           | 5.70 ms                                                     | 7.92 ms: 1.39x slower                                       |
| Geometric mean       | (ref)                                                       | 1.03x slower                                                |

Benchmark hidden because not significant (3): pickle_list, xml_etree_iterparse, unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef |
|------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 20.6 ms: 1.06x slower                                       |
| python_startup_no_site | 16.2 ms                                                     | 17.5 ms: 1.08x slower                                       |
| Geometric mean         | (ref)                                                       | 1.07x slower                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef |
|-----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| django_template | 22.9 ms                                                     | 24.5 ms: 1.07x slower                                       |
| mako            | 7.09 ms                                                     | 7.67 ms: 1.08x slower                                       |
| Geometric mean  | (ref)                                                       | 1.07x slower                                                |

All benchmarks:
===============

| Benchmark                | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef |
|--------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| async_generators         | 239 ms                                                      | 184 ms: 1.30x faster                                        |
| pickle                   | 7.43 us                                                     | 6.74 us: 1.10x faster                                       |
| regex_effbot             | 1.62 ms                                                     | 1.52 ms: 1.07x faster                                       |
| regex_dna                | 126 ms                                                      | 120 ms: 1.05x faster                                        |
| json_loads               | 13.9 us                                                     | 13.3 us: 1.05x faster                                       |
| bench_mp_pool            | 69.2 ms                                                     | 66.1 ms: 1.05x faster                                       |
| sqlalchemy_declarative   | 86.4 ms                                                     | 82.7 ms: 1.04x faster                                       |
| pathlib                  | 80.5 ms                                                     | 77.5 ms: 1.04x faster                                       |
| xml_etree_generate       | 55.8 ms                                                     | 53.8 ms: 1.04x faster                                       |
| telco                    | 4.13 ms                                                     | 4.00 ms: 1.03x faster                                       |
| scimark_sor              | 78.8 ms                                                     | 76.9 ms: 1.02x faster                                       |
| regex_v8                 | 14.2 ms                                                     | 13.9 ms: 1.02x faster                                       |
| nbody                    | 71.9 ms                                                     | 70.4 ms: 1.02x faster                                       |
| create_gc_cycles         | 752 us                                                      | 740 us: 1.02x faster                                        |
| unpickle_list            | 2.75 us                                                     | 2.73 us: 1.01x faster                                       |
| pidigits                 | 152 ms                                                      | 151 ms: 1.01x faster                                        |
| scimark_fft              | 184 ms                                                      | 184 ms: 1.00x faster                                        |
| xml_etree_process        | 37.7 ms                                                     | 37.9 ms: 1.00x slower                                       |
| pprint_pformat           | 1.05 sec                                                    | 1.05 sec: 1.01x slower                                      |
| 2to3                     | 218 ms                                                      | 221 ms: 1.01x slower                                        |
| scimark_sparse_mat_mult  | 2.56 ms                                                     | 2.60 ms: 1.02x slower                                       |
| pickle_dict              | 18.4 us                                                     | 18.8 us: 1.02x slower                                       |
| sqlglot_optimize         | 34.5 ms                                                     | 35.2 ms: 1.02x slower                                       |
| crypto_pyaes             | 48.5 ms                                                     | 49.7 ms: 1.02x slower                                       |
| pickle_pure_python       | 195 us                                                      | 201 us: 1.03x slower                                        |
| sqlglot_normalize        | 187 ms                                                      | 193 ms: 1.03x slower                                        |
| scimark_monte_carlo      | 43.7 ms                                                     | 45.1 ms: 1.03x slower                                       |
| deepcopy                 | 238 us                                                      | 246 us: 1.03x slower                                        |
| xml_etree_parse          | 93.0 ms                                                     | 96.4 ms: 1.04x slower                                       |
| nqueens                  | 62.8 ms                                                     | 65.1 ms: 1.04x slower                                       |
| meteor_contest           | 74.6 ms                                                     | 77.4 ms: 1.04x slower                                       |
| pycparser                | 699 ms                                                      | 726 ms: 1.04x slower                                        |
| coroutines               | 14.3 ms                                                     | 14.8 ms: 1.04x slower                                       |
| dulwich_log              | 44.3 ms                                                     | 46.4 ms: 1.05x slower                                       |
| tomli_loads              | 1.37 sec                                                    | 1.43 sec: 1.05x slower                                      |
| pyflate                  | 295 ms                                                      | 310 ms: 1.05x slower                                        |
| sympy_expand             | 284 ms                                                      | 299 ms: 1.05x slower                                        |
| aiohttp                  | 884 us                                                      | 936 us: 1.06x slower                                        |
| regex_compile            | 87.5 ms                                                     | 92.8 ms: 1.06x slower                                       |
| python_startup           | 19.5 ms                                                     | 20.6 ms: 1.06x slower                                       |
| django_template          | 22.9 ms                                                     | 24.5 ms: 1.07x slower                                       |
| async_tree_cpu_io_mixed  | 489 ms                                                      | 522 ms: 1.07x slower                                        |
| sympy_str                | 175 ms                                                      | 187 ms: 1.07x slower                                        |
| fannkuch                 | 247 ms                                                      | 263 ms: 1.07x slower                                        |
| logging_simple           | 6.28 us                                                     | 6.71 us: 1.07x slower                                       |
| sympy_integrate          | 13.0 ms                                                     | 13.9 ms: 1.08x slower                                       |
| scimark_lu               | 58.9 ms                                                     | 63.4 ms: 1.08x slower                                       |
| python_startup_no_site   | 16.2 ms                                                     | 17.5 ms: 1.08x slower                                       |
| raytrace                 | 192 ms                                                      | 208 ms: 1.08x slower                                        |
| deepcopy_memo            | 23.7 us                                                     | 25.6 us: 1.08x slower                                       |
| logging_format           | 6.72 us                                                     | 7.26 us: 1.08x slower                                       |
| mako                     | 7.09 ms                                                     | 7.67 ms: 1.08x slower                                       |
| chameleon                | 4.98 ms                                                     | 5.44 ms: 1.09x slower                                       |
| dask                     | 263 ms                                                      | 287 ms: 1.09x slower                                        |
| richards                 | 28.4 ms                                                     | 31.0 ms: 1.09x slower                                       |
| go                       | 91.6 ms                                                     | 100 ms: 1.10x slower                                        |
| bench_thread_pool        | 857 us                                                      | 941 us: 1.10x slower                                        |
| comprehensions           | 14.1 us                                                     | 15.6 us: 1.11x slower                                       |
| hexiom                   | 4.10 ms                                                     | 4.55 ms: 1.11x slower                                       |
| async_tree_io            | 731 ms                                                      | 813 ms: 1.11x slower                                        |
| spectral_norm            | 66.9 ms                                                     | 74.7 ms: 1.12x slower                                       |
| sqlalchemy_imperative    | 9.29 ms                                                     | 10.4 ms: 1.12x slower                                       |
| sqlglot_transpile        | 1.02 ms                                                     | 1.15 ms: 1.12x slower                                       |
| sympy_sum                | 91.5 ms                                                     | 103 ms: 1.12x slower                                        |
| chaos                    | 43.3 ms                                                     | 48.8 ms: 1.13x slower                                       |
| unpickle_pure_python     | 133 us                                                      | 153 us: 1.15x slower                                        |
| async_tree_none          | 291 ms                                                      | 334 ms: 1.15x slower                                        |
| asyncio_tcp_ssl          | 2.10 sec                                                    | 2.41 sec: 1.15x slower                                      |
| json                     | 3.05 ms                                                     | 3.51 ms: 1.15x slower                                       |
| tornado_http             | 89.5 ms                                                     | 103 ms: 1.16x slower                                        |
| async_tree_memoization   | 339 ms                                                      | 392 ms: 1.16x slower                                        |
| sqlglot_parse            | 804 us                                                      | 936 us: 1.16x slower                                        |
| logging_silent           | 60.5 ns                                                     | 72.1 ns: 1.19x slower                                       |
| richards_super           | 32.1 ms                                                     | 38.6 ms: 1.20x slower                                       |
| deltablue                | 2.16 ms                                                     | 2.71 ms: 1.26x slower                                       |
| mdp                      | 1.37 sec                                                    | 1.76 sec: 1.28x slower                                      |
| unpack_sequence          | 37.5 ns                                                     | 48.1 ns: 1.28x slower                                       |
| coverage                 | 40.8 ms                                                     | 55.6 ms: 1.36x slower                                       |
| json_dumps               | 5.70 ms                                                     | 7.92 ms: 1.39x slower                                       |
| generators               | 22.5 ms                                                     | 34.5 ms: 1.53x slower                                       |
| asyncio_tcp              | 487 ms                                                      | 932 ms: 1.91x slower                                        |
| typing_runtime_protocols | 95.1 us                                                     | 326 us: 3.43x slower                                        |
| Geometric mean           | (ref)                                                       | 1.08x slower                                                |

Benchmark hidden because not significant (9): pickle_list, xml_etree_iterparse, unpickle, gc_traversal, float, deepcopy_reduce, sqlite_synth, docutils, pprint_safe_repr
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, mypy2
Ignored benchmarks (6) of results/bm-20230606-3.11.4-d2340ef/bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.03x
- 95% likely to have a slowdown of 1.03x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: unknown