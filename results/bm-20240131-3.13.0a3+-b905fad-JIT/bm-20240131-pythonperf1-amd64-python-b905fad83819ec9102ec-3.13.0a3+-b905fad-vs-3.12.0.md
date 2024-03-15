
# Results vs. 3.12.0

- fork: python
- ref: b905fad83819ec9102ec
- machine: windows-amd64
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.02x faster
- HPT reliability: 98.91%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 222 ms: 1.02x slower                                                        |
| chameleon      | 4.98 ms                                                     | 4.72 ms: 1.06x faster                                                       |
| docutils       | 1.66 sec                                                    | 1.60 sec: 1.04x faster                                                      |
| tornado_http   | 89.5 ms                                                     | 86.3 ms: 1.04x faster                                                       |
| Geometric mean | (ref)                                                       | 1.03x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 273 ms: 1.07x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 473 ms: 1.06x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 462 ms: 1.06x faster                                                        |
| async_tree_none_tg         | 285 ms                                                      | 273 ms: 1.04x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 358 ms: 1.02x faster                                                        |
| async_tree_io              | 731 ms                                                      | 749 ms: 1.02x slower                                                        |
| async_tree_memoization     | 339 ms                                                      | 350 ms: 1.03x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.02x faster                                                                |

Benchmark hidden because not significant (1): async_tree_io_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| nbody          | 71.9 ms                                                     | 63.0 ms: 1.14x faster                                                       |
| float          | 56.8 ms                                                     | 52.0 ms: 1.09x faster                                                       |
| pidigits       | 152 ms                                                      | 154 ms: 1.01x slower                                                        |
| Geometric mean | (ref)                                                       | 1.07x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 87.5 ms                                                     | 81.6 ms: 1.07x faster                                                       |
| regex_dna      | 126 ms                                                      | 125 ms: 1.01x faster                                                        |
| regex_v8       | 14.2 ms                                                     | 17.0 ms: 1.19x slower                                                       |
| Geometric mean | (ref)                                                       | 1.02x slower                                                                |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 177 us: 1.11x faster                                                        |
| xml_etree_generate   | 55.8 ms                                                     | 51.8 ms: 1.08x faster                                                       |
| tomli_loads          | 1.37 sec                                                    | 1.28 sec: 1.07x faster                                                      |
| xml_etree_process    | 37.7 ms                                                     | 35.7 ms: 1.05x faster                                                       |
| unpickle_pure_python | 133 us                                                      | 127 us: 1.05x faster                                                        |
| json_dumps           | 5.70 ms                                                     | 5.51 ms: 1.03x faster                                                       |
| pickle               | 7.43 us                                                     | 7.21 us: 1.03x faster                                                       |
| pickle_dict          | 18.4 us                                                     | 17.9 us: 1.03x faster                                                       |
| json_loads           | 13.9 us                                                     | 13.7 us: 1.02x faster                                                       |
| unpickle_list        | 2.75 us                                                     | 2.77 us: 1.01x slower                                                       |
| xml_etree_parse      | 93.0 ms                                                     | 94.0 ms: 1.01x slower                                                       |
| unpickle             | 8.18 us                                                     | 9.00 us: 1.10x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.02x faster                                                                |

Benchmark hidden because not significant (2): xml_etree_iterparse, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 21.6 ms: 1.11x slower                                                       |
| python_startup_no_site | 16.2 ms                                                     | 19.6 ms: 1.21x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.16x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 6.78 ms: 1.05x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 70.2 us: 1.36x faster                                                       |
| comprehensions             | 14.1 us                                                     | 11.6 us: 1.22x faster                                                       |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.74 sec: 1.20x faster                                                      |
| mypy2                      | 509 ms                                                      | 436 ms: 1.17x faster                                                        |
| nbody                      | 71.9 ms                                                     | 63.0 ms: 1.14x faster                                                       |
| logging_silent             | 60.5 ns                                                     | 53.2 ns: 1.14x faster                                                       |
| raytrace                   | 192 ms                                                      | 170 ms: 1.13x faster                                                        |
| sqlite_synth               | 1.76 us                                                     | 1.56 us: 1.13x faster                                                       |
| richards_super             | 32.1 ms                                                     | 28.5 ms: 1.13x faster                                                       |
| richards                   | 28.4 ms                                                     | 25.4 ms: 1.12x faster                                                       |
| generators                 | 22.5 ms                                                     | 20.2 ms: 1.12x faster                                                       |
| pickle_pure_python         | 195 us                                                      | 177 us: 1.11x faster                                                        |
| coroutines                 | 14.3 ms                                                     | 12.9 ms: 1.10x faster                                                       |
| float                      | 56.8 ms                                                     | 52.0 ms: 1.09x faster                                                       |
| deepcopy_memo              | 23.7 us                                                     | 21.8 us: 1.09x faster                                                       |
| xml_etree_generate         | 55.8 ms                                                     | 51.8 ms: 1.08x faster                                                       |
| regex_compile              | 87.5 ms                                                     | 81.6 ms: 1.07x faster                                                       |
| deepcopy                   | 238 us                                                      | 222 us: 1.07x faster                                                        |
| tomli_loads                | 1.37 sec                                                    | 1.28 sec: 1.07x faster                                                      |
| async_tree_none            | 291 ms                                                      | 273 ms: 1.07x faster                                                        |
| deepcopy_reduce            | 2.09 us                                                     | 1.96 us: 1.07x faster                                                       |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 473 ms: 1.06x faster                                                        |
| sqlglot_parse              | 804 us                                                      | 757 us: 1.06x faster                                                        |
| scimark_lu                 | 58.9 ms                                                     | 55.5 ms: 1.06x faster                                                       |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 462 ms: 1.06x faster                                                        |
| chameleon                  | 4.98 ms                                                     | 4.72 ms: 1.06x faster                                                       |
| xml_etree_process          | 37.7 ms                                                     | 35.7 ms: 1.05x faster                                                       |
| nqueens                    | 62.8 ms                                                     | 59.5 ms: 1.05x faster                                                       |
| dulwich_log                | 44.3 ms                                                     | 42.0 ms: 1.05x faster                                                       |
| logging_simple             | 6.28 us                                                     | 5.97 us: 1.05x faster                                                       |
| unpickle_pure_python       | 133 us                                                      | 127 us: 1.05x faster                                                        |
| json                       | 3.05 ms                                                     | 2.91 ms: 1.05x faster                                                       |
| logging_format             | 6.72 us                                                     | 6.42 us: 1.05x faster                                                       |
| mako                       | 7.09 ms                                                     | 6.78 ms: 1.05x faster                                                       |
| async_tree_none_tg         | 285 ms                                                      | 273 ms: 1.04x faster                                                        |
| tornado_http               | 89.5 ms                                                     | 86.3 ms: 1.04x faster                                                       |
| docutils                   | 1.66 sec                                                    | 1.60 sec: 1.04x faster                                                      |
| sqlglot_normalize          | 187 ms                                                      | 180 ms: 1.04x faster                                                        |
| scimark_sor                | 78.8 ms                                                     | 76.1 ms: 1.04x faster                                                       |
| crypto_pyaes               | 48.5 ms                                                     | 46.8 ms: 1.04x faster                                                       |
| sympy_str                  | 175 ms                                                      | 169 ms: 1.04x faster                                                        |
| json_dumps                 | 5.70 ms                                                     | 5.51 ms: 1.03x faster                                                       |
| sqlglot_transpile          | 1.02 ms                                                     | 990 us: 1.03x faster                                                        |
| pickle                     | 7.43 us                                                     | 7.21 us: 1.03x faster                                                       |
| pickle_dict                | 18.4 us                                                     | 17.9 us: 1.03x faster                                                       |
| deltablue                  | 2.16 ms                                                     | 2.10 ms: 1.03x faster                                                       |
| spectral_norm              | 66.9 ms                                                     | 65.2 ms: 1.03x faster                                                       |
| async_tree_memoization_tg  | 367 ms                                                      | 358 ms: 1.02x faster                                                        |
| chaos                      | 43.3 ms                                                     | 42.4 ms: 1.02x faster                                                       |
| pprint_safe_repr           | 513 ms                                                      | 503 ms: 1.02x faster                                                        |
| json_loads                 | 13.9 us                                                     | 13.7 us: 1.02x faster                                                       |
| pycparser                  | 699 ms                                                      | 688 ms: 1.02x faster                                                        |
| sympy_sum                  | 91.5 ms                                                     | 90.3 ms: 1.01x faster                                                       |
| gc_traversal               | 1.52 ms                                                     | 1.50 ms: 1.01x faster                                                       |
| regex_dna                  | 126 ms                                                      | 125 ms: 1.01x faster                                                        |
| pprint_pformat             | 1.05 sec                                                    | 1.03 sec: 1.01x faster                                                      |
| sympy_expand               | 284 ms                                                      | 282 ms: 1.01x faster                                                        |
| fannkuch                   | 247 ms                                                      | 248 ms: 1.01x slower                                                        |
| unpickle_list              | 2.75 us                                                     | 2.77 us: 1.01x slower                                                       |
| xml_etree_parse            | 93.0 ms                                                     | 94.0 ms: 1.01x slower                                                       |
| pidigits                   | 152 ms                                                      | 154 ms: 1.01x slower                                                        |
| 2to3                       | 218 ms                                                      | 222 ms: 1.02x slower                                                        |
| async_tree_io              | 731 ms                                                      | 749 ms: 1.02x slower                                                        |
| sympy_integrate            | 13.0 ms                                                     | 13.4 ms: 1.03x slower                                                       |
| async_tree_memoization     | 339 ms                                                      | 350 ms: 1.03x slower                                                        |
| meteor_contest             | 74.6 ms                                                     | 78.7 ms: 1.06x slower                                                       |
| bench_mp_pool              | 69.2 ms                                                     | 73.2 ms: 1.06x slower                                                       |
| unpack_sequence            | 37.5 ns                                                     | 39.8 ns: 1.06x slower                                                       |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.72 ms: 1.07x slower                                                       |
| pyflate                    | 295 ms                                                      | 315 ms: 1.07x slower                                                        |
| scimark_fft                | 184 ms                                                      | 197 ms: 1.07x slower                                                        |
| go                         | 91.6 ms                                                     | 99.3 ms: 1.08x slower                                                       |
| unpickle                   | 8.18 us                                                     | 9.00 us: 1.10x slower                                                       |
| python_startup             | 19.5 ms                                                     | 21.6 ms: 1.11x slower                                                       |
| telco                      | 4.13 ms                                                     | 4.60 ms: 1.11x slower                                                       |
| coverage                   | 40.8 ms                                                     | 46.6 ms: 1.14x slower                                                       |
| mdp                        | 1.37 sec                                                    | 1.58 sec: 1.15x slower                                                      |
| regex_v8                   | 14.2 ms                                                     | 17.0 ms: 1.19x slower                                                       |
| python_startup_no_site     | 16.2 ms                                                     | 19.6 ms: 1.21x slower                                                       |
| hexiom                     | 4.10 ms                                                     | 5.27 ms: 1.28x slower                                                       |
| scimark_monte_carlo        | 43.7 ms                                                     | 58.0 ms: 1.33x slower                                                       |
| Geometric mean             | (ref)                                                       | 1.02x faster                                                                |

Benchmark hidden because not significant (11): xml_etree_iterparse, create_gc_cycles, dask, pathlib, async_tree_io_tg, regex_effbot, async_generators, sqlglot_optimize, pickle_list, asyncio_tcp, bench_thread_pool
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 98.91% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown