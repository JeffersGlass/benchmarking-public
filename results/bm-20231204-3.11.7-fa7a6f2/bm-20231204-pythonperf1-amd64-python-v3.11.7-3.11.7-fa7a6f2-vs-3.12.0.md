
# Results vs. 3.12.0

- fork: python
- ref: v3.11.7
- machine: windows-amd64
- commit hash: fa7a6f2
- commit date: 2023-12-04
- overall geometric mean: 1.04x slower
- HPT reliability: 98.71%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 209 ms: 1.04x faster                                        |
| chameleon      | 4.98 ms                                                     | 5.02 ms: 1.01x slower                                       |
| docutils       | 1.66 sec                                                    | 1.58 sec: 1.05x faster                                      |
| Geometric mean | (ref)                                                       | 1.02x faster                                                |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2 |
|---------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| async_tree_io_tg          | 771 ms                                                      | 783 ms: 1.02x slower                                        |
| async_tree_memoization_tg | 367 ms                                                      | 378 ms: 1.03x slower                                        |
| async_tree_none_tg        | 285 ms                                                      | 294 ms: 1.03x slower                                        |
| async_tree_cpu_io_mixed   | 489 ms                                                      | 523 ms: 1.07x slower                                        |
| async_tree_io             | 731 ms                                                      | 784 ms: 1.07x slower                                        |
| async_tree_none           | 291 ms                                                      | 317 ms: 1.09x slower                                        |
| async_tree_memoization    | 339 ms                                                      | 380 ms: 1.12x slower                                        |
| Geometric mean            | (ref)                                                       | 1.05x slower                                                |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| float          | 56.8 ms                                                     | 54.1 ms: 1.05x faster                                       |
| pidigits       | 152 ms                                                      | 149 ms: 1.02x faster                                        |
| nbody          | 71.9 ms                                                     | 70.8 ms: 1.01x faster                                       |
| Geometric mean | (ref)                                                       | 1.03x faster                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 119 ms: 1.06x faster                                        |
| regex_effbot   | 1.62 ms                                                     | 1.54 ms: 1.05x faster                                       |
| regex_v8       | 14.2 ms                                                     | 13.7 ms: 1.04x faster                                       |
| regex_compile  | 87.5 ms                                                     | 88.3 ms: 1.01x slower                                       |
| Geometric mean | (ref)                                                       | 1.03x faster                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| pickle               | 7.43 us                                                     | 6.55 us: 1.13x faster                                       |
| json_loads           | 13.9 us                                                     | 12.8 us: 1.09x faster                                       |
| pickle_list          | 2.83 us                                                     | 2.66 us: 1.06x faster                                       |
| unpickle_list        | 2.75 us                                                     | 2.60 us: 1.06x faster                                       |
| unpickle             | 8.18 us                                                     | 7.74 us: 1.06x faster                                       |
| xml_etree_generate   | 55.8 ms                                                     | 52.9 ms: 1.06x faster                                       |
| xml_etree_iterparse  | 65.2 ms                                                     | 64.3 ms: 1.01x faster                                       |
| xml_etree_process    | 37.7 ms                                                     | 37.2 ms: 1.01x faster                                       |
| tomli_loads          | 1.37 sec                                                    | 1.40 sec: 1.02x slower                                      |
| pickle_pure_python   | 195 us                                                      | 201 us: 1.03x slower                                        |
| xml_etree_parse      | 93.0 ms                                                     | 98.1 ms: 1.05x slower                                       |
| unpickle_pure_python | 133 us                                                      | 149 us: 1.12x slower                                        |
| json_dumps           | 5.70 ms                                                     | 7.86 ms: 1.38x slower                                       |
| Geometric mean       | (ref)                                                       | 1.01x slower                                                |

Benchmark hidden because not significant (1): pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2 |
|------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| python_startup_no_site | 16.2 ms                                                     | 15.7 ms: 1.04x faster                                       |
| python_startup         | 19.5 ms                                                     | 20.3 ms: 1.04x slower                                       |
| Geometric mean         | (ref)                                                       | 1.00x slower                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2 |
|-----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| mako            | 7.09 ms                                                     | 7.29 ms: 1.03x slower                                       |
| django_template | 22.9 ms                                                     | 23.7 ms: 1.03x slower                                       |
| Geometric mean  | (ref)                                                       | 1.03x slower                                                |

All benchmarks:
===============

| Benchmark                 | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2 |
|---------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| async_generators          | 239 ms                                                      | 172 ms: 1.39x faster                                        |
| bench_mp_pool             | 69.2 ms                                                     | 60.8 ms: 1.14x faster                                       |
| pickle                    | 7.43 us                                                     | 6.55 us: 1.13x faster                                       |
| pathlib                   | 80.5 ms                                                     | 71.2 ms: 1.13x faster                                       |
| mypy2                     | 509 ms                                                      | 454 ms: 1.12x faster                                        |
| json_loads                | 13.9 us                                                     | 12.8 us: 1.09x faster                                       |
| pickle_list               | 2.83 us                                                     | 2.66 us: 1.06x faster                                       |
| regex_dna                 | 126 ms                                                      | 119 ms: 1.06x faster                                        |
| telco                     | 4.13 ms                                                     | 3.89 ms: 1.06x faster                                       |
| unpickle_list             | 2.75 us                                                     | 2.60 us: 1.06x faster                                       |
| scimark_sor               | 78.8 ms                                                     | 74.5 ms: 1.06x faster                                       |
| unpickle                  | 8.18 us                                                     | 7.74 us: 1.06x faster                                       |
| xml_etree_generate        | 55.8 ms                                                     | 52.9 ms: 1.06x faster                                       |
| docutils                  | 1.66 sec                                                    | 1.58 sec: 1.05x faster                                      |
| regex_effbot              | 1.62 ms                                                     | 1.54 ms: 1.05x faster                                       |
| float                     | 56.8 ms                                                     | 54.1 ms: 1.05x faster                                       |
| 2to3                      | 218 ms                                                      | 209 ms: 1.04x faster                                        |
| create_gc_cycles          | 752 us                                                      | 721 us: 1.04x faster                                        |
| gc_traversal              | 1.52 ms                                                     | 1.46 ms: 1.04x faster                                       |
| regex_v8                  | 14.2 ms                                                     | 13.7 ms: 1.04x faster                                       |
| python_startup_no_site    | 16.2 ms                                                     | 15.7 ms: 1.04x faster                                       |
| sqlite_synth              | 1.76 us                                                     | 1.70 us: 1.04x faster                                       |
| aiohttp                   | 884 us                                                      | 854 us: 1.04x faster                                        |
| sqlalchemy_declarative    | 86.4 ms                                                     | 83.7 ms: 1.03x faster                                       |
| scimark_fft               | 184 ms                                                      | 179 ms: 1.03x faster                                        |
| deepcopy_reduce           | 2.09 us                                                     | 2.04 us: 1.03x faster                                       |
| pidigits                  | 152 ms                                                      | 149 ms: 1.02x faster                                        |
| bench_thread_pool         | 857 us                                                      | 842 us: 1.02x faster                                        |
| nbody                     | 71.9 ms                                                     | 70.8 ms: 1.01x faster                                       |
| xml_etree_iterparse       | 65.2 ms                                                     | 64.3 ms: 1.01x faster                                       |
| xml_etree_process         | 37.7 ms                                                     | 37.2 ms: 1.01x faster                                       |
| spectral_norm             | 66.9 ms                                                     | 66.3 ms: 1.01x faster                                       |
| pprint_safe_repr          | 513 ms                                                      | 509 ms: 1.01x faster                                        |
| fannkuch                  | 247 ms                                                      | 245 ms: 1.01x faster                                        |
| crypto_pyaes              | 48.5 ms                                                     | 48.6 ms: 1.00x slower                                       |
| chameleon                 | 4.98 ms                                                     | 5.02 ms: 1.01x slower                                       |
| regex_compile             | 87.5 ms                                                     | 88.3 ms: 1.01x slower                                       |
| sqlglot_optimize          | 34.5 ms                                                     | 34.9 ms: 1.01x slower                                       |
| deepcopy                  | 238 us                                                      | 242 us: 1.01x slower                                        |
| async_tree_io_tg          | 771 ms                                                      | 783 ms: 1.02x slower                                        |
| scimark_monte_carlo       | 43.7 ms                                                     | 44.4 ms: 1.02x slower                                       |
| dulwich_log               | 44.3 ms                                                     | 45.0 ms: 1.02x slower                                       |
| meteor_contest            | 74.6 ms                                                     | 75.9 ms: 1.02x slower                                       |
| nqueens                   | 62.8 ms                                                     | 64.1 ms: 1.02x slower                                       |
| tomli_loads               | 1.37 sec                                                    | 1.40 sec: 1.02x slower                                      |
| sqlglot_normalize         | 187 ms                                                      | 192 ms: 1.02x slower                                        |
| pickle_pure_python        | 195 us                                                      | 201 us: 1.03x slower                                        |
| mako                      | 7.09 ms                                                     | 7.29 ms: 1.03x slower                                       |
| async_tree_memoization_tg | 367 ms                                                      | 378 ms: 1.03x slower                                        |
| django_template           | 22.9 ms                                                     | 23.7 ms: 1.03x slower                                       |
| async_tree_none_tg        | 285 ms                                                      | 294 ms: 1.03x slower                                        |
| pyflate                   | 295 ms                                                      | 305 ms: 1.04x slower                                        |
| deepcopy_memo             | 23.7 us                                                     | 24.7 us: 1.04x slower                                       |
| sympy_integrate           | 13.0 ms                                                     | 13.5 ms: 1.04x slower                                       |
| scimark_lu                | 58.9 ms                                                     | 61.5 ms: 1.04x slower                                       |
| python_startup            | 19.5 ms                                                     | 20.3 ms: 1.04x slower                                       |
| coroutines                | 14.3 ms                                                     | 14.9 ms: 1.05x slower                                       |
| raytrace                  | 192 ms                                                      | 202 ms: 1.05x slower                                        |
| sympy_str                 | 175 ms                                                      | 184 ms: 1.05x slower                                        |
| xml_etree_parse           | 93.0 ms                                                     | 98.1 ms: 1.05x slower                                       |
| richards                  | 28.4 ms                                                     | 30.2 ms: 1.06x slower                                       |
| asyncio_tcp_ssl           | 2.10 sec                                                    | 2.23 sec: 1.06x slower                                      |
| sympy_expand              | 284 ms                                                      | 303 ms: 1.07x slower                                        |
| async_tree_cpu_io_mixed   | 489 ms                                                      | 523 ms: 1.07x slower                                        |
| async_tree_io             | 731 ms                                                      | 784 ms: 1.07x slower                                        |
| coverage                  | 40.8 ms                                                     | 43.9 ms: 1.07x slower                                       |
| logging_simple            | 6.28 us                                                     | 6.76 us: 1.08x slower                                       |
| logging_format            | 6.72 us                                                     | 7.25 us: 1.08x slower                                       |
| sympy_sum                 | 91.5 ms                                                     | 98.9 ms: 1.08x slower                                       |
| hexiom                    | 4.10 ms                                                     | 4.45 ms: 1.08x slower                                       |
| async_tree_none           | 291 ms                                                      | 317 ms: 1.09x slower                                        |
| sqlalchemy_imperative     | 9.29 ms                                                     | 10.2 ms: 1.10x slower                                       |
| sqlglot_transpile         | 1.02 ms                                                     | 1.13 ms: 1.11x slower                                       |
| comprehensions            | 14.1 us                                                     | 15.7 us: 1.11x slower                                       |
| unpickle_pure_python      | 133 us                                                      | 149 us: 1.12x slower                                        |
| async_tree_memoization    | 339 ms                                                      | 380 ms: 1.12x slower                                        |
| go                        | 91.6 ms                                                     | 103 ms: 1.12x slower                                        |
| chaos                     | 43.3 ms                                                     | 49.1 ms: 1.13x slower                                       |
| logging_silent            | 60.5 ns                                                     | 69.6 ns: 1.15x slower                                       |
| sqlglot_parse             | 804 us                                                      | 933 us: 1.16x slower                                        |
| richards_super            | 32.1 ms                                                     | 38.2 ms: 1.19x slower                                       |
| mdp                       | 1.37 sec                                                    | 1.65 sec: 1.20x slower                                      |
| deltablue                 | 2.16 ms                                                     | 2.62 ms: 1.21x slower                                       |
| unpack_sequence           | 37.5 ns                                                     | 47.9 ns: 1.28x slower                                       |
| json_dumps                | 5.70 ms                                                     | 7.86 ms: 1.38x slower                                       |
| asyncio_tcp               | 487 ms                                                      | 730 ms: 1.50x slower                                        |
| generators                | 22.5 ms                                                     | 34.0 ms: 1.51x slower                                       |
| typing_runtime_protocols  | 95.1 us                                                     | 327 us: 3.43x slower                                        |
| Geometric mean            | (ref)                                                       | 1.04x slower                                                |

Benchmark hidden because not significant (8): async_tree_cpu_io_mixed_tg, pycparser, pprint_pformat, scimark_sparse_mat_mult, pickle_dict, tornado_http, dask, json
Ignored benchmarks (6) of results/bm-20231204-3.11.7-fa7a6f2/bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 98.71% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown