
# Results vs. 3.12.0

- fork: python
- ref: b905fad83819ec9102ec
- machine: windows-amd64
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.02x slower
- HPT reliability: 98.24%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 225 ms: 1.03x slower                                                        |
| chameleon      | 4.98 ms                                                     | 5.28 ms: 1.06x slower                                                       |
| docutils       | 1.66 sec                                                    | 1.63 sec: 1.02x faster                                                      |
| tornado_http   | 89.5 ms                                                     | 88.0 ms: 1.02x faster                                                       |
| Geometric mean | (ref)                                                       | 1.01x slower                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 275 ms: 1.06x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 471 ms: 1.04x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 487 ms: 1.03x faster                                                        |
| async_tree_none_tg         | 285 ms                                                      | 289 ms: 1.01x slower                                                        |
| async_tree_io_tg           | 771 ms                                                      | 787 ms: 1.02x slower                                                        |
| async_tree_io              | 731 ms                                                      | 754 ms: 1.03x slower                                                        |
| async_tree_memoization     | 339 ms                                                      | 354 ms: 1.04x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.00x faster                                                                |

Benchmark hidden because not significant (1): async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 152 ms                                                      | 149 ms: 1.02x faster                                                        |
| float          | 56.8 ms                                                     | 57.2 ms: 1.01x slower                                                       |
| nbody          | 71.9 ms                                                     | 83.0 ms: 1.15x slower                                                       |
| Geometric mean | (ref)                                                       | 1.04x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 87.5 ms                                                     | 85.3 ms: 1.03x faster                                                       |
| regex_effbot   | 1.62 ms                                                     | 1.63 ms: 1.01x slower                                                       |
| regex_dna      | 126 ms                                                      | 129 ms: 1.02x slower                                                        |
| regex_v8       | 14.2 ms                                                     | 18.5 ms: 1.30x slower                                                       |
| Geometric mean | (ref)                                                       | 1.07x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 185 us: 1.06x faster                                                        |
| pickle               | 7.43 us                                                     | 7.09 us: 1.05x faster                                                       |
| xml_etree_process    | 37.7 ms                                                     | 38.2 ms: 1.01x slower                                                       |
| xml_etree_generate   | 55.8 ms                                                     | 56.7 ms: 1.01x slower                                                       |
| pickle_dict          | 18.4 us                                                     | 18.7 us: 1.01x slower                                                       |
| json_dumps           | 5.70 ms                                                     | 5.78 ms: 1.02x slower                                                       |
| unpickle_list        | 2.75 us                                                     | 2.82 us: 1.03x slower                                                       |
| tomli_loads          | 1.37 sec                                                    | 1.42 sec: 1.04x slower                                                      |
| xml_etree_iterparse  | 65.2 ms                                                     | 67.7 ms: 1.04x slower                                                       |
| pickle_list          | 2.83 us                                                     | 2.93 us: 1.04x slower                                                       |
| unpickle             | 8.18 us                                                     | 8.60 us: 1.05x slower                                                       |
| unpickle_pure_python | 133 us                                                      | 143 us: 1.08x slower                                                        |
| Geometric mean       | (ref)                                                       | 1.02x slower                                                                |

Benchmark hidden because not significant (2): json_loads, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 20.8 ms: 1.07x slower                                                       |
| python_startup_no_site | 16.2 ms                                                     | 18.4 ms: 1.13x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.10x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 7.44 ms: 1.05x slower                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 74.2 us: 1.28x faster                                                       |
| mypy2                      | 509 ms                                                      | 432 ms: 1.18x faster                                                        |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.86 sec: 1.13x faster                                                      |
| sqlite_synth               | 1.76 us                                                     | 1.60 us: 1.10x faster                                                       |
| raytrace                   | 192 ms                                                      | 176 ms: 1.10x faster                                                        |
| comprehensions             | 14.1 us                                                     | 13.1 us: 1.08x faster                                                       |
| logging_silent             | 60.5 ns                                                     | 56.8 ns: 1.06x faster                                                       |
| coroutines                 | 14.3 ms                                                     | 13.4 ms: 1.06x faster                                                       |
| async_tree_none            | 291 ms                                                      | 275 ms: 1.06x faster                                                        |
| pickle_pure_python         | 195 us                                                      | 185 us: 1.06x faster                                                        |
| pickle                     | 7.43 us                                                     | 7.09 us: 1.05x faster                                                       |
| deepcopy_reduce            | 2.09 us                                                     | 2.01 us: 1.04x faster                                                       |
| sympy_str                  | 175 ms                                                      | 168 ms: 1.04x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 471 ms: 1.04x faster                                                        |
| sympy_sum                  | 91.5 ms                                                     | 88.2 ms: 1.04x faster                                                       |
| deepcopy                   | 238 us                                                      | 230 us: 1.04x faster                                                        |
| generators                 | 22.5 ms                                                     | 21.7 ms: 1.04x faster                                                       |
| json                       | 3.05 ms                                                     | 2.95 ms: 1.03x faster                                                       |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 487 ms: 1.03x faster                                                        |
| regex_compile              | 87.5 ms                                                     | 85.3 ms: 1.03x faster                                                       |
| pidigits                   | 152 ms                                                      | 149 ms: 1.02x faster                                                        |
| async_generators           | 239 ms                                                      | 235 ms: 1.02x faster                                                        |
| docutils                   | 1.66 sec                                                    | 1.63 sec: 1.02x faster                                                      |
| tornado_http               | 89.5 ms                                                     | 88.0 ms: 1.02x faster                                                       |
| deepcopy_memo              | 23.7 us                                                     | 23.3 us: 1.02x faster                                                       |
| dulwich_log                | 44.3 ms                                                     | 43.6 ms: 1.02x faster                                                       |
| bench_mp_pool              | 69.2 ms                                                     | 68.2 ms: 1.01x faster                                                       |
| richards_super             | 32.1 ms                                                     | 31.7 ms: 1.01x faster                                                       |
| richards                   | 28.4 ms                                                     | 28.1 ms: 1.01x faster                                                       |
| sqlglot_parse              | 804 us                                                      | 797 us: 1.01x faster                                                        |
| scimark_lu                 | 58.9 ms                                                     | 58.4 ms: 1.01x faster                                                       |
| sympy_expand               | 284 ms                                                      | 282 ms: 1.01x faster                                                        |
| crypto_pyaes               | 48.5 ms                                                     | 48.2 ms: 1.01x faster                                                       |
| sqlglot_transpile          | 1.02 ms                                                     | 1.02 ms: 1.01x faster                                                       |
| go                         | 91.6 ms                                                     | 91.1 ms: 1.00x faster                                                       |
| pathlib                    | 80.5 ms                                                     | 81.0 ms: 1.01x slower                                                       |
| regex_effbot               | 1.62 ms                                                     | 1.63 ms: 1.01x slower                                                       |
| float                      | 56.8 ms                                                     | 57.2 ms: 1.01x slower                                                       |
| pycparser                  | 699 ms                                                      | 707 ms: 1.01x slower                                                        |
| xml_etree_process          | 37.7 ms                                                     | 38.2 ms: 1.01x slower                                                       |
| gc_traversal               | 1.52 ms                                                     | 1.54 ms: 1.01x slower                                                       |
| async_tree_none_tg         | 285 ms                                                      | 289 ms: 1.01x slower                                                        |
| xml_etree_generate         | 55.8 ms                                                     | 56.7 ms: 1.01x slower                                                       |
| pickle_dict                | 18.4 us                                                     | 18.7 us: 1.01x slower                                                       |
| json_dumps                 | 5.70 ms                                                     | 5.78 ms: 1.02x slower                                                       |
| nqueens                    | 62.8 ms                                                     | 63.8 ms: 1.02x slower                                                       |
| regex_dna                  | 126 ms                                                      | 129 ms: 1.02x slower                                                        |
| sqlglot_optimize           | 34.5 ms                                                     | 35.1 ms: 1.02x slower                                                       |
| async_tree_io_tg           | 771 ms                                                      | 787 ms: 1.02x slower                                                        |
| chaos                      | 43.3 ms                                                     | 44.5 ms: 1.03x slower                                                       |
| unpickle_list              | 2.75 us                                                     | 2.82 us: 1.03x slower                                                       |
| logging_format             | 6.72 us                                                     | 6.92 us: 1.03x slower                                                       |
| pprint_safe_repr           | 513 ms                                                      | 529 ms: 1.03x slower                                                        |
| async_tree_io              | 731 ms                                                      | 754 ms: 1.03x slower                                                        |
| 2to3                       | 218 ms                                                      | 225 ms: 1.03x slower                                                        |
| tomli_loads                | 1.37 sec                                                    | 1.42 sec: 1.04x slower                                                      |
| xml_etree_iterparse        | 65.2 ms                                                     | 67.7 ms: 1.04x slower                                                       |
| pickle_list                | 2.83 us                                                     | 2.93 us: 1.04x slower                                                       |
| pprint_pformat             | 1.05 sec                                                    | 1.09 sec: 1.04x slower                                                      |
| sympy_integrate            | 13.0 ms                                                     | 13.5 ms: 1.04x slower                                                       |
| async_tree_memoization     | 339 ms                                                      | 354 ms: 1.04x slower                                                        |
| meteor_contest             | 74.6 ms                                                     | 78.0 ms: 1.04x slower                                                       |
| mako                       | 7.09 ms                                                     | 7.44 ms: 1.05x slower                                                       |
| unpickle                   | 8.18 us                                                     | 8.60 us: 1.05x slower                                                       |
| scimark_sor                | 78.8 ms                                                     | 83.0 ms: 1.05x slower                                                       |
| chameleon                  | 4.98 ms                                                     | 5.28 ms: 1.06x slower                                                       |
| mdp                        | 1.37 sec                                                    | 1.46 sec: 1.06x slower                                                      |
| python_startup             | 19.5 ms                                                     | 20.8 ms: 1.07x slower                                                       |
| unpickle_pure_python       | 133 us                                                      | 143 us: 1.08x slower                                                        |
| scimark_monte_carlo        | 43.7 ms                                                     | 48.0 ms: 1.10x slower                                                       |
| pyflate                    | 295 ms                                                      | 324 ms: 1.10x slower                                                        |
| fannkuch                   | 247 ms                                                      | 272 ms: 1.10x slower                                                        |
| python_startup_no_site     | 16.2 ms                                                     | 18.4 ms: 1.13x slower                                                       |
| scimark_fft                | 184 ms                                                      | 211 ms: 1.14x slower                                                        |
| telco                      | 4.13 ms                                                     | 4.73 ms: 1.15x slower                                                       |
| unpack_sequence            | 37.5 ns                                                     | 43.2 ns: 1.15x slower                                                       |
| nbody                      | 71.9 ms                                                     | 83.0 ms: 1.15x slower                                                       |
| coverage                   | 40.8 ms                                                     | 47.5 ms: 1.16x slower                                                       |
| hexiom                     | 4.10 ms                                                     | 4.79 ms: 1.17x slower                                                       |
| deltablue                  | 2.16 ms                                                     | 2.64 ms: 1.22x slower                                                       |
| spectral_norm              | 66.9 ms                                                     | 82.2 ms: 1.23x slower                                                       |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 3.14 ms: 1.23x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 18.5 ms: 1.30x slower                                                       |
| Geometric mean             | (ref)                                                       | 1.02x slower                                                                |

Benchmark hidden because not significant (9): asyncio_tcp, create_gc_cycles, bench_thread_pool, sqlglot_normalize, logging_simple, json_loads, xml_etree_parse, dask, async_tree_memoization_tg
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 98.24% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown