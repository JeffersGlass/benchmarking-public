
# Results vs. 3.12.0

- fork: python
- ref: 52eade22237eef1f3843
- machine: windows-amd64
- commit hash: 52eade2
- commit date: 2024-01-20
- overall geometric mean: 1.04x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 213 ms: 1.02x faster                                                        |
| chameleon      | 4.98 ms                                                     | 4.90 ms: 1.02x faster                                                       |
| docutils       | 1.66 sec                                                    | 1.53 sec: 1.08x faster                                                      |
| tornado_http   | 89.5 ms                                                     | 86.2 ms: 1.04x faster                                                       |
| Geometric mean | (ref)                                                       | 1.04x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 264 ms: 1.10x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 446 ms: 1.10x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 465 ms: 1.08x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 347 ms: 1.06x faster                                                        |
| async_tree_none_tg         | 285 ms                                                      | 272 ms: 1.05x faster                                                        |
| async_tree_io_tg           | 771 ms                                                      | 751 ms: 1.03x faster                                                        |
| async_tree_io              | 731 ms                                                      | 716 ms: 1.02x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.05x faster                                                                |

Benchmark hidden because not significant (1): async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 56.8 ms                                                     | 51.3 ms: 1.11x faster                                                       |
| pidigits       | 152 ms                                                      | 147 ms: 1.04x faster                                                        |
| nbody          | 71.9 ms                                                     | 72.8 ms: 1.01x slower                                                       |
| Geometric mean | (ref)                                                       | 1.04x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 87.5 ms                                                     | 78.0 ms: 1.12x faster                                                       |
| regex_dna      | 126 ms                                                      | 117 ms: 1.08x faster                                                        |
| regex_effbot   | 1.62 ms                                                     | 1.56 ms: 1.04x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 14.5 ms: 1.02x slower                                                       |
| Geometric mean | (ref)                                                       | 1.05x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 180 us: 1.09x faster                                                        |
| unpickle_pure_python | 133 us                                                      | 128 us: 1.04x faster                                                        |
| pickle               | 7.43 us                                                     | 7.18 us: 1.04x faster                                                       |
| xml_etree_generate   | 55.8 ms                                                     | 54.3 ms: 1.03x faster                                                       |
| xml_etree_iterparse  | 65.2 ms                                                     | 63.5 ms: 1.03x faster                                                       |
| xml_etree_process    | 37.7 ms                                                     | 36.8 ms: 1.03x faster                                                       |
| unpickle_list        | 2.75 us                                                     | 2.69 us: 1.02x faster                                                       |
| json_loads           | 13.9 us                                                     | 13.6 us: 1.02x faster                                                       |
| json_dumps           | 5.70 ms                                                     | 5.59 ms: 1.02x faster                                                       |
| pickle_dict          | 18.4 us                                                     | 18.3 us: 1.00x faster                                                       |
| tomli_loads          | 1.37 sec                                                    | 1.42 sec: 1.04x slower                                                      |
| unpickle             | 8.18 us                                                     | 8.73 us: 1.07x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.01x faster                                                                |

Benchmark hidden because not significant (2): pickle_list, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 20.5 ms: 1.05x slower                                                       |
| python_startup_no_site | 16.2 ms                                                     | 18.3 ms: 1.13x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.09x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 6.48 ms: 1.09x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| comprehensions             | 14.1 us                                                     | 10.6 us: 1.33x faster                                                       |
| typing_runtime_protocols   | 95.1 us                                                     | 71.9 us: 1.32x faster                                                       |
| mypy2                      | 509 ms                                                      | 413 ms: 1.23x faster                                                        |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.82 sec: 1.15x faster                                                      |
| raytrace                   | 192 ms                                                      | 169 ms: 1.14x faster                                                        |
| crypto_pyaes               | 48.5 ms                                                     | 43.1 ms: 1.12x faster                                                       |
| regex_compile              | 87.5 ms                                                     | 78.0 ms: 1.12x faster                                                       |
| sqlite_synth               | 1.76 us                                                     | 1.57 us: 1.12x faster                                                       |
| sympy_sum                  | 91.5 ms                                                     | 82.4 ms: 1.11x faster                                                       |
| spectral_norm              | 66.9 ms                                                     | 60.4 ms: 1.11x faster                                                       |
| float                      | 56.8 ms                                                     | 51.3 ms: 1.11x faster                                                       |
| async_tree_none            | 291 ms                                                      | 264 ms: 1.10x faster                                                        |
| sympy_str                  | 175 ms                                                      | 159 ms: 1.10x faster                                                        |
| logging_silent             | 60.5 ns                                                     | 55.0 ns: 1.10x faster                                                       |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 446 ms: 1.10x faster                                                        |
| mako                       | 7.09 ms                                                     | 6.48 ms: 1.09x faster                                                       |
| pickle_pure_python         | 195 us                                                      | 180 us: 1.09x faster                                                        |
| coroutines                 | 14.3 ms                                                     | 13.1 ms: 1.09x faster                                                       |
| docutils                   | 1.66 sec                                                    | 1.53 sec: 1.08x faster                                                      |
| regex_dna                  | 126 ms                                                      | 117 ms: 1.08x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 465 ms: 1.08x faster                                                        |
| chaos                      | 43.3 ms                                                     | 40.1 ms: 1.08x faster                                                       |
| deepcopy_reduce            | 2.09 us                                                     | 1.94 us: 1.08x faster                                                       |
| dulwich_log                | 44.3 ms                                                     | 41.4 ms: 1.07x faster                                                       |
| scimark_monte_carlo        | 43.7 ms                                                     | 40.9 ms: 1.07x faster                                                       |
| nqueens                    | 62.8 ms                                                     | 58.9 ms: 1.07x faster                                                       |
| deltablue                  | 2.16 ms                                                     | 2.03 ms: 1.07x faster                                                       |
| go                         | 91.6 ms                                                     | 86.0 ms: 1.06x faster                                                       |
| deepcopy                   | 238 us                                                      | 224 us: 1.06x faster                                                        |
| hexiom                     | 4.10 ms                                                     | 3.87 ms: 1.06x faster                                                       |
| json                       | 3.05 ms                                                     | 2.88 ms: 1.06x faster                                                       |
| deepcopy_memo              | 23.7 us                                                     | 22.4 us: 1.06x faster                                                       |
| async_tree_memoization_tg  | 367 ms                                                      | 347 ms: 1.06x faster                                                        |
| scimark_lu                 | 58.9 ms                                                     | 55.7 ms: 1.06x faster                                                       |
| sympy_integrate            | 13.0 ms                                                     | 12.3 ms: 1.05x faster                                                       |
| sqlglot_normalize          | 187 ms                                                      | 178 ms: 1.05x faster                                                        |
| create_gc_cycles           | 752 us                                                      | 715 us: 1.05x faster                                                        |
| async_tree_none_tg         | 285 ms                                                      | 272 ms: 1.05x faster                                                        |
| meteor_contest             | 74.6 ms                                                     | 71.5 ms: 1.04x faster                                                       |
| pprint_safe_repr           | 513 ms                                                      | 493 ms: 1.04x faster                                                        |
| sympy_expand               | 284 ms                                                      | 273 ms: 1.04x faster                                                        |
| unpickle_pure_python       | 133 us                                                      | 128 us: 1.04x faster                                                        |
| tornado_http               | 89.5 ms                                                     | 86.2 ms: 1.04x faster                                                       |
| pprint_pformat             | 1.05 sec                                                    | 1.01 sec: 1.04x faster                                                      |
| bench_mp_pool              | 69.2 ms                                                     | 66.7 ms: 1.04x faster                                                       |
| dask                       | 263 ms                                                      | 253 ms: 1.04x faster                                                        |
| regex_effbot               | 1.62 ms                                                     | 1.56 ms: 1.04x faster                                                       |
| pickle                     | 7.43 us                                                     | 7.18 us: 1.04x faster                                                       |
| pidigits                   | 152 ms                                                      | 147 ms: 1.04x faster                                                        |
| logging_format             | 6.72 us                                                     | 6.50 us: 1.03x faster                                                       |
| richards                   | 28.4 ms                                                     | 27.5 ms: 1.03x faster                                                       |
| asyncio_tcp                | 487 ms                                                      | 472 ms: 1.03x faster                                                        |
| logging_simple             | 6.28 us                                                     | 6.08 us: 1.03x faster                                                       |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.48 ms: 1.03x faster                                                       |
| generators                 | 22.5 ms                                                     | 21.9 ms: 1.03x faster                                                       |
| scimark_fft                | 184 ms                                                      | 179 ms: 1.03x faster                                                        |
| xml_etree_generate         | 55.8 ms                                                     | 54.3 ms: 1.03x faster                                                       |
| richards_super             | 32.1 ms                                                     | 31.2 ms: 1.03x faster                                                       |
| xml_etree_iterparse        | 65.2 ms                                                     | 63.5 ms: 1.03x faster                                                       |
| pyflate                    | 295 ms                                                      | 287 ms: 1.03x faster                                                        |
| async_tree_io_tg           | 771 ms                                                      | 751 ms: 1.03x faster                                                        |
| xml_etree_process          | 37.7 ms                                                     | 36.8 ms: 1.03x faster                                                       |
| sqlglot_parse              | 804 us                                                      | 785 us: 1.02x faster                                                        |
| 2to3                       | 218 ms                                                      | 213 ms: 1.02x faster                                                        |
| mdp                        | 1.37 sec                                                    | 1.34 sec: 1.02x faster                                                      |
| sqlglot_transpile          | 1.02 ms                                                     | 999 us: 1.02x faster                                                        |
| bench_thread_pool          | 857 us                                                      | 838 us: 1.02x faster                                                        |
| unpickle_list              | 2.75 us                                                     | 2.69 us: 1.02x faster                                                       |
| async_tree_io              | 731 ms                                                      | 716 ms: 1.02x faster                                                        |
| json_loads                 | 13.9 us                                                     | 13.6 us: 1.02x faster                                                       |
| gc_traversal               | 1.52 ms                                                     | 1.49 ms: 1.02x faster                                                       |
| json_dumps                 | 5.70 ms                                                     | 5.59 ms: 1.02x faster                                                       |
| async_generators           | 239 ms                                                      | 235 ms: 1.02x faster                                                        |
| sqlglot_optimize           | 34.5 ms                                                     | 33.9 ms: 1.02x faster                                                       |
| chameleon                  | 4.98 ms                                                     | 4.90 ms: 1.02x faster                                                       |
| pathlib                    | 80.5 ms                                                     | 79.2 ms: 1.02x faster                                                       |
| fannkuch                   | 247 ms                                                      | 244 ms: 1.01x faster                                                        |
| pickle_dict                | 18.4 us                                                     | 18.3 us: 1.00x faster                                                       |
| nbody                      | 71.9 ms                                                     | 72.8 ms: 1.01x slower                                                       |
| scimark_sor                | 78.8 ms                                                     | 80.2 ms: 1.02x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 14.5 ms: 1.02x slower                                                       |
| tomli_loads                | 1.37 sec                                                    | 1.42 sec: 1.04x slower                                                      |
| python_startup             | 19.5 ms                                                     | 20.5 ms: 1.05x slower                                                       |
| unpack_sequence            | 37.5 ns                                                     | 39.8 ns: 1.06x slower                                                       |
| unpickle                   | 8.18 us                                                     | 8.73 us: 1.07x slower                                                       |
| python_startup_no_site     | 16.2 ms                                                     | 18.3 ms: 1.13x slower                                                       |
| coverage                   | 40.8 ms                                                     | 46.2 ms: 1.13x slower                                                       |
| telco                      | 4.13 ms                                                     | 4.80 ms: 1.16x slower                                                       |
| Geometric mean             | (ref)                                                       | 1.04x faster                                                                |

Benchmark hidden because not significant (4): async_tree_memoization, pickle_list, xml_etree_parse, pycparser
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: unknown