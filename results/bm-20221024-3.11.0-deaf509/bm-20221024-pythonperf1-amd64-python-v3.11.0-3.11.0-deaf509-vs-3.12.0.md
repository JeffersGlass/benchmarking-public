
# Results vs. 3.12.0

- fork: python
- ref: v3.11.0
- machine: windows-amd64
- commit hash: deaf509
- commit date: 2022-10-24
- overall geometric mean: 1.06x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 214 ms: 1.02x faster                                        |
| chameleon      | 4.98 ms                                                     | 5.26 ms: 1.06x slower                                       |
| docutils       | 1.66 sec                                                    | 1.64 sec: 1.01x faster                                      |
| tornado_http   | 89.5 ms                                                     | 92.8 ms: 1.04x slower                                       |
| Geometric mean | (ref)                                                       | 1.01x slower                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 |
|----------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 523 ms: 1.04x slower                                        |
| async_tree_io_tg           | 771 ms                                                      | 829 ms: 1.07x slower                                        |
| async_tree_none_tg         | 285 ms                                                      | 309 ms: 1.08x slower                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 530 ms: 1.08x slower                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 405 ms: 1.10x slower                                        |
| async_tree_io              | 731 ms                                                      | 808 ms: 1.10x slower                                        |
| async_tree_none            | 291 ms                                                      | 332 ms: 1.14x slower                                        |
| async_tree_memoization     | 339 ms                                                      | 399 ms: 1.18x slower                                        |
| Geometric mean             | (ref)                                                       | 1.10x slower                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| float          | 56.8 ms                                                     | 54.4 ms: 1.04x faster                                       |
| nbody          | 71.9 ms                                                     | 70.3 ms: 1.02x faster                                       |
| pidigits       | 152 ms                                                      | 150 ms: 1.01x faster                                        |
| Geometric mean | (ref)                                                       | 1.03x faster                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 116 ms: 1.09x faster                                        |
| regex_effbot   | 1.62 ms                                                     | 1.50 ms: 1.08x faster                                       |
| regex_v8       | 14.2 ms                                                     | 14.2 ms: 1.00x faster                                       |
| regex_compile  | 87.5 ms                                                     | 91.0 ms: 1.04x slower                                       |
| Geometric mean | (ref)                                                       | 1.03x faster                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 |
|----------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| pickle               | 7.43 us                                                     | 6.64 us: 1.12x faster                                       |
| unpickle             | 8.18 us                                                     | 7.57 us: 1.08x faster                                       |
| json_loads           | 13.9 us                                                     | 13.0 us: 1.07x faster                                       |
| xml_etree_generate   | 55.8 ms                                                     | 52.5 ms: 1.06x faster                                       |
| unpickle_list        | 2.75 us                                                     | 2.59 us: 1.06x faster                                       |
| pickle_list          | 2.83 us                                                     | 2.70 us: 1.05x faster                                       |
| xml_etree_process    | 37.7 ms                                                     | 37.2 ms: 1.01x faster                                       |
| pickle_dict          | 18.4 us                                                     | 18.5 us: 1.00x slower                                       |
| xml_etree_parse      | 93.0 ms                                                     | 97.6 ms: 1.05x slower                                       |
| tomli_loads          | 1.37 sec                                                    | 1.46 sec: 1.06x slower                                      |
| pickle_pure_python   | 195 us                                                      | 208 us: 1.07x slower                                        |
| unpickle_pure_python | 133 us                                                      | 157 us: 1.18x slower                                        |
| json_dumps           | 5.70 ms                                                     | 8.09 ms: 1.42x slower                                       |
| Geometric mean       | (ref)                                                       | 1.02x slower                                                |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 |
|------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 19.8 ms: 1.02x slower                                       |
| python_startup_no_site | 16.2 ms                                                     | 16.8 ms: 1.04x slower                                       |
| Geometric mean         | (ref)                                                       | 1.03x slower                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 |
|-----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| django_template | 22.9 ms                                                     | 24.4 ms: 1.07x slower                                       |
| mako            | 7.09 ms                                                     | 7.58 ms: 1.07x slower                                       |
| Geometric mean  | (ref)                                                       | 1.07x slower                                                |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 |
|----------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| async_generators           | 239 ms                                                      | 177 ms: 1.35x faster                                        |
| pathlib                    | 80.5 ms                                                     | 70.9 ms: 1.14x faster                                       |
| pickle                     | 7.43 us                                                     | 6.64 us: 1.12x faster                                       |
| mypy2                      | 509 ms                                                      | 459 ms: 1.11x faster                                        |
| bench_mp_pool              | 69.2 ms                                                     | 63.2 ms: 1.09x faster                                       |
| regex_dna                  | 126 ms                                                      | 116 ms: 1.09x faster                                        |
| unpickle                   | 8.18 us                                                     | 7.57 us: 1.08x faster                                       |
| regex_effbot               | 1.62 ms                                                     | 1.50 ms: 1.08x faster                                       |
| json_loads                 | 13.9 us                                                     | 13.0 us: 1.07x faster                                       |
| xml_etree_generate         | 55.8 ms                                                     | 52.5 ms: 1.06x faster                                       |
| unpickle_list              | 2.75 us                                                     | 2.59 us: 1.06x faster                                       |
| create_gc_cycles           | 752 us                                                      | 713 us: 1.05x faster                                        |
| pickle_list                | 2.83 us                                                     | 2.70 us: 1.05x faster                                       |
| float                      | 56.8 ms                                                     | 54.4 ms: 1.04x faster                                       |
| scimark_fft                | 184 ms                                                      | 179 ms: 1.03x faster                                        |
| nbody                      | 71.9 ms                                                     | 70.3 ms: 1.02x faster                                       |
| 2to3                       | 218 ms                                                      | 214 ms: 1.02x faster                                        |
| gc_traversal               | 1.52 ms                                                     | 1.49 ms: 1.02x faster                                       |
| telco                      | 4.13 ms                                                     | 4.06 ms: 1.02x faster                                       |
| deepcopy_reduce            | 2.09 us                                                     | 2.06 us: 1.02x faster                                       |
| pidigits                   | 152 ms                                                      | 150 ms: 1.01x faster                                        |
| xml_etree_process          | 37.7 ms                                                     | 37.2 ms: 1.01x faster                                       |
| docutils                   | 1.66 sec                                                    | 1.64 sec: 1.01x faster                                      |
| sqlalchemy_declarative     | 86.4 ms                                                     | 85.6 ms: 1.01x faster                                       |
| scimark_sor                | 78.8 ms                                                     | 78.1 ms: 1.01x faster                                       |
| regex_v8                   | 14.2 ms                                                     | 14.2 ms: 1.00x faster                                       |
| pickle_dict                | 18.4 us                                                     | 18.5 us: 1.00x slower                                       |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.58 ms: 1.01x slower                                       |
| crypto_pyaes               | 48.5 ms                                                     | 48.9 ms: 1.01x slower                                       |
| meteor_contest             | 74.6 ms                                                     | 75.2 ms: 1.01x slower                                       |
| python_startup             | 19.5 ms                                                     | 19.8 ms: 1.02x slower                                       |
| sqlglot_normalize          | 187 ms                                                      | 190 ms: 1.02x slower                                        |
| bench_thread_pool          | 857 us                                                      | 872 us: 1.02x slower                                        |
| spectral_norm              | 66.9 ms                                                     | 68.3 ms: 1.02x slower                                       |
| fannkuch                   | 247 ms                                                      | 253 ms: 1.03x slower                                        |
| pycparser                  | 699 ms                                                      | 720 ms: 1.03x slower                                        |
| pprint_safe_repr           | 513 ms                                                      | 529 ms: 1.03x slower                                        |
| python_startup_no_site     | 16.2 ms                                                     | 16.8 ms: 1.04x slower                                       |
| deepcopy                   | 238 us                                                      | 246 us: 1.04x slower                                        |
| scimark_monte_carlo        | 43.7 ms                                                     | 45.3 ms: 1.04x slower                                       |
| tornado_http               | 89.5 ms                                                     | 92.8 ms: 1.04x slower                                       |
| dask                       | 263 ms                                                      | 273 ms: 1.04x slower                                        |
| pprint_pformat             | 1.05 sec                                                    | 1.09 sec: 1.04x slower                                      |
| regex_compile              | 87.5 ms                                                     | 91.0 ms: 1.04x slower                                       |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 523 ms: 1.04x slower                                        |
| dulwich_log                | 44.3 ms                                                     | 46.4 ms: 1.05x slower                                       |
| xml_etree_parse            | 93.0 ms                                                     | 97.6 ms: 1.05x slower                                       |
| coroutines                 | 14.3 ms                                                     | 15.0 ms: 1.05x slower                                       |
| sympy_expand               | 284 ms                                                      | 299 ms: 1.05x slower                                        |
| chameleon                  | 4.98 ms                                                     | 5.26 ms: 1.06x slower                                       |
| sympy_str                  | 175 ms                                                      | 185 ms: 1.06x slower                                        |
| pyflate                    | 295 ms                                                      | 312 ms: 1.06x slower                                        |
| coverage                   | 40.8 ms                                                     | 43.4 ms: 1.06x slower                                       |
| tomli_loads                | 1.37 sec                                                    | 1.46 sec: 1.06x slower                                      |
| django_template            | 22.9 ms                                                     | 24.4 ms: 1.07x slower                                       |
| pickle_pure_python         | 195 us                                                      | 208 us: 1.07x slower                                        |
| logging_format             | 6.72 us                                                     | 7.16 us: 1.07x slower                                       |
| scimark_lu                 | 58.9 ms                                                     | 62.8 ms: 1.07x slower                                       |
| mako                       | 7.09 ms                                                     | 7.58 ms: 1.07x slower                                       |
| async_tree_io_tg           | 771 ms                                                      | 829 ms: 1.07x slower                                        |
| async_tree_none_tg         | 285 ms                                                      | 309 ms: 1.08x slower                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 530 ms: 1.08x slower                                        |
| sympy_integrate            | 13.0 ms                                                     | 14.0 ms: 1.08x slower                                       |
| nqueens                    | 62.8 ms                                                     | 68.3 ms: 1.09x slower                                       |
| logging_simple             | 6.28 us                                                     | 6.86 us: 1.09x slower                                       |
| sympy_sum                  | 91.5 ms                                                     | 100 ms: 1.09x slower                                        |
| deepcopy_memo              | 23.7 us                                                     | 26.0 us: 1.10x slower                                       |
| async_tree_memoization_tg  | 367 ms                                                      | 405 ms: 1.10x slower                                        |
| go                         | 91.6 ms                                                     | 101 ms: 1.10x slower                                        |
| async_tree_io              | 731 ms                                                      | 808 ms: 1.10x slower                                        |
| richards                   | 28.4 ms                                                     | 31.4 ms: 1.11x slower                                       |
| comprehensions             | 14.1 us                                                     | 15.6 us: 1.11x slower                                       |
| raytrace                   | 192 ms                                                      | 213 ms: 1.11x slower                                        |
| hexiom                     | 4.10 ms                                                     | 4.55 ms: 1.11x slower                                       |
| chaos                      | 43.3 ms                                                     | 48.4 ms: 1.12x slower                                       |
| sqlalchemy_imperative      | 9.29 ms                                                     | 10.4 ms: 1.12x slower                                       |
| sqlglot_transpile          | 1.02 ms                                                     | 1.16 ms: 1.14x slower                                       |
| async_tree_none            | 291 ms                                                      | 332 ms: 1.14x slower                                        |
| mdp                        | 1.37 sec                                                    | 1.59 sec: 1.16x slower                                      |
| async_tree_memoization     | 339 ms                                                      | 399 ms: 1.18x slower                                        |
| unpickle_pure_python       | 133 us                                                      | 157 us: 1.18x slower                                        |
| sqlglot_parse              | 804 us                                                      | 953 us: 1.19x slower                                        |
| logging_silent             | 60.5 ns                                                     | 71.8 ns: 1.19x slower                                       |
| richards_super             | 32.1 ms                                                     | 38.7 ms: 1.21x slower                                       |
| deltablue                  | 2.16 ms                                                     | 2.70 ms: 1.25x slower                                       |
| unpack_sequence            | 37.5 ns                                                     | 46.9 ns: 1.25x slower                                       |
| json_dumps                 | 5.70 ms                                                     | 8.09 ms: 1.42x slower                                       |
| asyncio_tcp                | 487 ms                                                      | 726 ms: 1.49x slower                                        |
| generators                 | 22.5 ms                                                     | 34.0 ms: 1.51x slower                                       |
| typing_runtime_protocols   | 95.1 us                                                     | 326 us: 3.43x slower                                        |
| Geometric mean             | (ref)                                                       | 1.06x slower                                                |

Benchmark hidden because not significant (6): asyncio_tcp_ssl, json, aiohttp, sqlglot_optimize, sqlite_synth, xml_etree_iterparse
Ignored benchmarks (6) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.03x
- 95% likely to have a slowdown of 1.03x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: unknown