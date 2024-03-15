
# Results vs. 3.11.0

- fork: python
- ref: v3.12.0
- machine: windows-amd64
- commit hash: 0fb18b0
- commit date: 2023-10-02
- overall geometric mean: 1.06x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 218 ms: 1.02x slower                                        |
| chameleon      | 5.26 ms                                                     | 4.98 ms: 1.06x faster                                       |
| docutils       | 1.64 sec                                                    | 1.66 sec: 1.01x slower                                      |
| tornado_http   | 92.8 ms                                                     | 89.5 ms: 1.04x faster                                       |
| Geometric mean | (ref)                                                       | 1.01x faster                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 |
|----------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| async_tree_memoization     | 399 ms                                                      | 339 ms: 1.18x faster                                        |
| async_tree_none            | 332 ms                                                      | 291 ms: 1.14x faster                                        |
| async_tree_io              | 808 ms                                                      | 731 ms: 1.10x faster                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 367 ms: 1.10x faster                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 489 ms: 1.08x faster                                        |
| async_tree_none_tg         | 309 ms                                                      | 285 ms: 1.08x faster                                        |
| async_tree_io_tg           | 829 ms                                                      | 771 ms: 1.07x faster                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 502 ms: 1.04x faster                                        |
| Geometric mean             | (ref)                                                       | 1.10x faster                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| pidigits       | 150 ms                                                      | 152 ms: 1.01x slower                                        |
| nbody          | 70.3 ms                                                     | 71.9 ms: 1.02x slower                                       |
| float          | 54.4 ms                                                     | 56.8 ms: 1.04x slower                                       |
| Geometric mean | (ref)                                                       | 1.03x slower                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 87.5 ms: 1.04x faster                                       |
| regex_v8       | 14.2 ms                                                     | 14.2 ms: 1.00x slower                                       |
| regex_effbot   | 1.50 ms                                                     | 1.62 ms: 1.08x slower                                       |
| regex_dna      | 116 ms                                                      | 126 ms: 1.09x slower                                        |
| Geometric mean | (ref)                                                       | 1.03x slower                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 |
|----------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.70 ms: 1.42x faster                                       |
| unpickle_pure_python | 157 us                                                      | 133 us: 1.18x faster                                        |
| pickle_pure_python   | 208 us                                                      | 195 us: 1.07x faster                                        |
| tomli_loads          | 1.46 sec                                                    | 1.37 sec: 1.06x faster                                      |
| xml_etree_parse      | 97.6 ms                                                     | 93.0 ms: 1.05x faster                                       |
| pickle_dict          | 18.5 us                                                     | 18.4 us: 1.00x faster                                       |
| xml_etree_process    | 37.2 ms                                                     | 37.7 ms: 1.01x slower                                       |
| pickle_list          | 2.70 us                                                     | 2.83 us: 1.05x slower                                       |
| unpickle_list        | 2.59 us                                                     | 2.75 us: 1.06x slower                                       |
| xml_etree_generate   | 52.5 ms                                                     | 55.8 ms: 1.06x slower                                       |
| json_loads           | 13.0 us                                                     | 13.9 us: 1.07x slower                                       |
| unpickle             | 7.57 us                                                     | 8.18 us: 1.08x slower                                       |
| pickle               | 6.64 us                                                     | 7.43 us: 1.12x slower                                       |
| Geometric mean       | (ref)                                                       | 1.02x faster                                                |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 |
|------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 16.2 ms: 1.04x faster                                       |
| python_startup         | 19.8 ms                                                     | 19.5 ms: 1.02x faster                                       |
| Geometric mean         | (ref)                                                       | 1.03x faster                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 |
|-----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| mako            | 7.58 ms                                                     | 7.09 ms: 1.07x faster                                       |
| django_template | 24.4 ms                                                     | 22.9 ms: 1.07x faster                                       |
| Geometric mean  | (ref)                                                       | 1.07x faster                                                |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 |
|----------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 95.1 us: 3.43x faster                                       |
| generators                 | 34.0 ms                                                     | 22.5 ms: 1.51x faster                                       |
| asyncio_tcp                | 726 ms                                                      | 487 ms: 1.49x faster                                        |
| json_dumps                 | 8.09 ms                                                     | 5.70 ms: 1.42x faster                                       |
| unpack_sequence            | 46.9 ns                                                     | 37.5 ns: 1.25x faster                                       |
| deltablue                  | 2.70 ms                                                     | 2.16 ms: 1.25x faster                                       |
| richards_super             | 38.7 ms                                                     | 32.1 ms: 1.21x faster                                       |
| logging_silent             | 71.8 ns                                                     | 60.5 ns: 1.19x faster                                       |
| sqlglot_parse              | 953 us                                                      | 804 us: 1.19x faster                                        |
| unpickle_pure_python       | 157 us                                                      | 133 us: 1.18x faster                                        |
| async_tree_memoization     | 399 ms                                                      | 339 ms: 1.18x faster                                        |
| mdp                        | 1.59 sec                                                    | 1.37 sec: 1.16x faster                                      |
| async_tree_none            | 332 ms                                                      | 291 ms: 1.14x faster                                        |
| sqlglot_transpile          | 1.16 ms                                                     | 1.02 ms: 1.14x faster                                       |
| sqlalchemy_imperative      | 10.4 ms                                                     | 9.29 ms: 1.12x faster                                       |
| chaos                      | 48.4 ms                                                     | 43.3 ms: 1.12x faster                                       |
| hexiom                     | 4.55 ms                                                     | 4.10 ms: 1.11x faster                                       |
| raytrace                   | 213 ms                                                      | 192 ms: 1.11x faster                                        |
| comprehensions             | 15.6 us                                                     | 14.1 us: 1.11x faster                                       |
| richards                   | 31.4 ms                                                     | 28.4 ms: 1.11x faster                                       |
| async_tree_io              | 808 ms                                                      | 731 ms: 1.10x faster                                        |
| go                         | 101 ms                                                      | 91.6 ms: 1.10x faster                                       |
| async_tree_memoization_tg  | 405 ms                                                      | 367 ms: 1.10x faster                                        |
| deepcopy_memo              | 26.0 us                                                     | 23.7 us: 1.10x faster                                       |
| sympy_sum                  | 100 ms                                                      | 91.5 ms: 1.09x faster                                       |
| logging_simple             | 6.86 us                                                     | 6.28 us: 1.09x faster                                       |
| nqueens                    | 68.3 ms                                                     | 62.8 ms: 1.09x faster                                       |
| sympy_integrate            | 14.0 ms                                                     | 13.0 ms: 1.08x faster                                       |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 489 ms: 1.08x faster                                        |
| async_tree_none_tg         | 309 ms                                                      | 285 ms: 1.08x faster                                        |
| async_tree_io_tg           | 829 ms                                                      | 771 ms: 1.07x faster                                        |
| mako                       | 7.58 ms                                                     | 7.09 ms: 1.07x faster                                       |
| scimark_lu                 | 62.8 ms                                                     | 58.9 ms: 1.07x faster                                       |
| logging_format             | 7.16 us                                                     | 6.72 us: 1.07x faster                                       |
| pickle_pure_python         | 208 us                                                      | 195 us: 1.07x faster                                        |
| django_template            | 24.4 ms                                                     | 22.9 ms: 1.07x faster                                       |
| tomli_loads                | 1.46 sec                                                    | 1.37 sec: 1.06x faster                                      |
| coverage                   | 43.4 ms                                                     | 40.8 ms: 1.06x faster                                       |
| pyflate                    | 312 ms                                                      | 295 ms: 1.06x faster                                        |
| sympy_str                  | 185 ms                                                      | 175 ms: 1.06x faster                                        |
| chameleon                  | 5.26 ms                                                     | 4.98 ms: 1.06x faster                                       |
| sympy_expand               | 299 ms                                                      | 284 ms: 1.05x faster                                        |
| coroutines                 | 15.0 ms                                                     | 14.3 ms: 1.05x faster                                       |
| xml_etree_parse            | 97.6 ms                                                     | 93.0 ms: 1.05x faster                                       |
| dulwich_log                | 46.4 ms                                                     | 44.3 ms: 1.05x faster                                       |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 502 ms: 1.04x faster                                        |
| regex_compile              | 91.0 ms                                                     | 87.5 ms: 1.04x faster                                       |
| pprint_pformat             | 1.09 sec                                                    | 1.05 sec: 1.04x faster                                      |
| dask                       | 273 ms                                                      | 263 ms: 1.04x faster                                        |
| tornado_http               | 92.8 ms                                                     | 89.5 ms: 1.04x faster                                       |
| scimark_monte_carlo        | 45.3 ms                                                     | 43.7 ms: 1.04x faster                                       |
| deepcopy                   | 246 us                                                      | 238 us: 1.04x faster                                        |
| python_startup_no_site     | 16.8 ms                                                     | 16.2 ms: 1.04x faster                                       |
| pprint_safe_repr           | 529 ms                                                      | 513 ms: 1.03x faster                                        |
| pycparser                  | 720 ms                                                      | 699 ms: 1.03x faster                                        |
| fannkuch                   | 253 ms                                                      | 247 ms: 1.03x faster                                        |
| spectral_norm              | 68.3 ms                                                     | 66.9 ms: 1.02x faster                                       |
| bench_thread_pool          | 872 us                                                      | 857 us: 1.02x faster                                        |
| sqlglot_normalize          | 190 ms                                                      | 187 ms: 1.02x faster                                        |
| python_startup             | 19.8 ms                                                     | 19.5 ms: 1.02x faster                                       |
| meteor_contest             | 75.2 ms                                                     | 74.6 ms: 1.01x faster                                       |
| crypto_pyaes               | 48.9 ms                                                     | 48.5 ms: 1.01x faster                                       |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.56 ms: 1.01x faster                                       |
| pickle_dict                | 18.5 us                                                     | 18.4 us: 1.00x faster                                       |
| regex_v8                   | 14.2 ms                                                     | 14.2 ms: 1.00x slower                                       |
| scimark_sor                | 78.1 ms                                                     | 78.8 ms: 1.01x slower                                       |
| sqlalchemy_declarative     | 85.6 ms                                                     | 86.4 ms: 1.01x slower                                       |
| docutils                   | 1.64 sec                                                    | 1.66 sec: 1.01x slower                                      |
| xml_etree_process          | 37.2 ms                                                     | 37.7 ms: 1.01x slower                                       |
| pidigits                   | 150 ms                                                      | 152 ms: 1.01x slower                                        |
| deepcopy_reduce            | 2.06 us                                                     | 2.09 us: 1.02x slower                                       |
| telco                      | 4.06 ms                                                     | 4.13 ms: 1.02x slower                                       |
| gc_traversal               | 1.49 ms                                                     | 1.52 ms: 1.02x slower                                       |
| 2to3                       | 214 ms                                                      | 218 ms: 1.02x slower                                        |
| nbody                      | 70.3 ms                                                     | 71.9 ms: 1.02x slower                                       |
| scimark_fft                | 179 ms                                                      | 184 ms: 1.03x slower                                        |
| float                      | 54.4 ms                                                     | 56.8 ms: 1.04x slower                                       |
| pickle_list                | 2.70 us                                                     | 2.83 us: 1.05x slower                                       |
| create_gc_cycles           | 713 us                                                      | 752 us: 1.05x slower                                        |
| unpickle_list              | 2.59 us                                                     | 2.75 us: 1.06x slower                                       |
| xml_etree_generate         | 52.5 ms                                                     | 55.8 ms: 1.06x slower                                       |
| json_loads                 | 13.0 us                                                     | 13.9 us: 1.07x slower                                       |
| regex_effbot               | 1.50 ms                                                     | 1.62 ms: 1.08x slower                                       |
| unpickle                   | 7.57 us                                                     | 8.18 us: 1.08x slower                                       |
| regex_dna                  | 116 ms                                                      | 126 ms: 1.09x slower                                        |
| bench_mp_pool              | 63.2 ms                                                     | 69.2 ms: 1.09x slower                                       |
| mypy2                      | 459 ms                                                      | 509 ms: 1.11x slower                                        |
| pickle                     | 6.64 us                                                     | 7.43 us: 1.12x slower                                       |
| pathlib                    | 70.9 ms                                                     | 80.5 ms: 1.14x slower                                       |
| async_generators           | 177 ms                                                      | 239 ms: 1.35x slower                                        |
| Geometric mean             | (ref)                                                       | 1.06x faster                                                |

Benchmark hidden because not significant (6): xml_etree_iterparse, sqlite_synth, sqlglot_optimize, aiohttp, json, asyncio_tcp_ssl
Ignored benchmarks (6) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: unknown