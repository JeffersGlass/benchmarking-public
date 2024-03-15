
# Results vs. 3.12.0

- fork: python
- ref: 2f0ec7fa9450caeac820
- machine: windows-amd64
- commit hash: 2f0ec7f
- commit date: 2023-12-17
- overall geometric mean: 1.05x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 215 ms: 1.01x faster                                                        |
| chameleon      | 4.98 ms                                                     | 4.86 ms: 1.03x faster                                                       |
| docutils       | 1.66 sec                                                    | 1.56 sec: 1.06x faster                                                      |
| tornado_http   | 89.5 ms                                                     | 87.7 ms: 1.02x faster                                                       |
| Geometric mean | (ref)                                                       | 1.03x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 266 ms: 1.10x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 448 ms: 1.09x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 463 ms: 1.08x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 352 ms: 1.04x faster                                                        |
| async_tree_none_tg         | 285 ms                                                      | 275 ms: 1.04x faster                                                        |
| async_tree_io_tg           | 771 ms                                                      | 748 ms: 1.03x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.05x faster                                                                |

Benchmark hidden because not significant (2): async_tree_io, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 56.8 ms                                                     | 51.9 ms: 1.10x faster                                                       |
| nbody          | 71.9 ms                                                     | 69.5 ms: 1.04x faster                                                       |
| pidigits       | 152 ms                                                      | 150 ms: 1.02x faster                                                        |
| Geometric mean | (ref)                                                       | 1.05x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 87.5 ms                                                     | 77.9 ms: 1.12x faster                                                       |
| regex_dna      | 126 ms                                                      | 122 ms: 1.04x faster                                                        |
| regex_effbot   | 1.62 ms                                                     | 1.61 ms: 1.01x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 15.3 ms: 1.07x slower                                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 181 us: 1.08x faster                                                        |
| pickle               | 7.43 us                                                     | 7.02 us: 1.06x faster                                                       |
| xml_etree_generate   | 55.8 ms                                                     | 53.1 ms: 1.05x faster                                                       |
| json_dumps           | 5.70 ms                                                     | 5.49 ms: 1.04x faster                                                       |
| unpickle_pure_python | 133 us                                                      | 129 us: 1.04x faster                                                        |
| xml_etree_iterparse  | 65.2 ms                                                     | 63.0 ms: 1.03x faster                                                       |
| xml_etree_process    | 37.7 ms                                                     | 36.7 ms: 1.03x faster                                                       |
| json_loads           | 13.9 us                                                     | 13.6 us: 1.03x faster                                                       |
| unpickle_list        | 2.75 us                                                     | 2.69 us: 1.02x faster                                                       |
| xml_etree_parse      | 93.0 ms                                                     | 92.0 ms: 1.01x faster                                                       |
| pickle_dict          | 18.4 us                                                     | 18.3 us: 1.01x faster                                                       |
| unpickle             | 8.18 us                                                     | 8.32 us: 1.02x slower                                                       |
| tomli_loads          | 1.37 sec                                                    | 1.40 sec: 1.02x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.02x faster                                                                |

Benchmark hidden because not significant (1): pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 20.6 ms: 1.06x slower                                                       |
| python_startup_no_site | 16.2 ms                                                     | 18.8 ms: 1.16x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.11x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 6.41 ms: 1.11x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| comprehensions             | 14.1 us                                                     | 10.5 us: 1.35x faster                                                       |
| typing_runtime_protocols   | 95.1 us                                                     | 72.3 us: 1.32x faster                                                       |
| mypy2                      | 509 ms                                                      | 414 ms: 1.23x faster                                                        |
| raytrace                   | 192 ms                                                      | 166 ms: 1.16x faster                                                        |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.83 sec: 1.14x faster                                                      |
| sqlite_synth               | 1.76 us                                                     | 1.56 us: 1.13x faster                                                       |
| regex_compile              | 87.5 ms                                                     | 77.9 ms: 1.12x faster                                                       |
| logging_silent             | 60.5 ns                                                     | 53.8 ns: 1.12x faster                                                       |
| crypto_pyaes               | 48.5 ms                                                     | 43.3 ms: 1.12x faster                                                       |
| spectral_norm              | 66.9 ms                                                     | 60.2 ms: 1.11x faster                                                       |
| mako                       | 7.09 ms                                                     | 6.41 ms: 1.11x faster                                                       |
| chaos                      | 43.3 ms                                                     | 39.2 ms: 1.11x faster                                                       |
| sympy_sum                  | 91.5 ms                                                     | 83.3 ms: 1.10x faster                                                       |
| sympy_str                  | 175 ms                                                      | 160 ms: 1.10x faster                                                        |
| async_tree_none            | 291 ms                                                      | 266 ms: 1.10x faster                                                        |
| float                      | 56.8 ms                                                     | 51.9 ms: 1.10x faster                                                       |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 448 ms: 1.09x faster                                                        |
| coroutines                 | 14.3 ms                                                     | 13.1 ms: 1.09x faster                                                       |
| scimark_monte_carlo        | 43.7 ms                                                     | 40.1 ms: 1.09x faster                                                       |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.36 ms: 1.09x faster                                                       |
| deepcopy_memo              | 23.7 us                                                     | 21.9 us: 1.08x faster                                                       |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 463 ms: 1.08x faster                                                        |
| deepcopy                   | 238 us                                                      | 220 us: 1.08x faster                                                        |
| nqueens                    | 62.8 ms                                                     | 58.1 ms: 1.08x faster                                                       |
| hexiom                     | 4.10 ms                                                     | 3.80 ms: 1.08x faster                                                       |
| pickle_pure_python         | 195 us                                                      | 181 us: 1.08x faster                                                        |
| deltablue                  | 2.16 ms                                                     | 2.01 ms: 1.08x faster                                                       |
| deepcopy_reduce            | 2.09 us                                                     | 1.95 us: 1.07x faster                                                       |
| async_generators           | 239 ms                                                      | 224 ms: 1.07x faster                                                        |
| docutils                   | 1.66 sec                                                    | 1.56 sec: 1.06x faster                                                      |
| scimark_lu                 | 58.9 ms                                                     | 55.4 ms: 1.06x faster                                                       |
| pickle                     | 7.43 us                                                     | 7.02 us: 1.06x faster                                                       |
| asyncio_tcp                | 487 ms                                                      | 461 ms: 1.06x faster                                                        |
| dulwich_log                | 44.3 ms                                                     | 41.9 ms: 1.06x faster                                                       |
| sqlglot_normalize          | 187 ms                                                      | 177 ms: 1.06x faster                                                        |
| xml_etree_generate         | 55.8 ms                                                     | 53.1 ms: 1.05x faster                                                       |
| sqlglot_parse              | 804 us                                                      | 765 us: 1.05x faster                                                        |
| pprint_safe_repr           | 513 ms                                                      | 488 ms: 1.05x faster                                                        |
| pprint_pformat             | 1.05 sec                                                    | 996 ms: 1.05x faster                                                        |
| logging_simple             | 6.28 us                                                     | 5.99 us: 1.05x faster                                                       |
| sympy_integrate            | 13.0 ms                                                     | 12.4 ms: 1.04x faster                                                       |
| sqlglot_transpile          | 1.02 ms                                                     | 980 us: 1.04x faster                                                        |
| sympy_expand               | 284 ms                                                      | 272 ms: 1.04x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 352 ms: 1.04x faster                                                        |
| regex_dna                  | 126 ms                                                      | 122 ms: 1.04x faster                                                        |
| logging_format             | 6.72 us                                                     | 6.47 us: 1.04x faster                                                       |
| json_dumps                 | 5.70 ms                                                     | 5.49 ms: 1.04x faster                                                       |
| unpickle_pure_python       | 133 us                                                      | 129 us: 1.04x faster                                                        |
| async_tree_none_tg         | 285 ms                                                      | 275 ms: 1.04x faster                                                        |
| go                         | 91.6 ms                                                     | 88.5 ms: 1.04x faster                                                       |
| nbody                      | 71.9 ms                                                     | 69.5 ms: 1.04x faster                                                       |
| create_gc_cycles           | 752 us                                                      | 727 us: 1.03x faster                                                        |
| xml_etree_iterparse        | 65.2 ms                                                     | 63.0 ms: 1.03x faster                                                       |
| richards                   | 28.4 ms                                                     | 27.5 ms: 1.03x faster                                                       |
| async_tree_io_tg           | 771 ms                                                      | 748 ms: 1.03x faster                                                        |
| richards_super             | 32.1 ms                                                     | 31.2 ms: 1.03x faster                                                       |
| unpack_sequence            | 37.5 ns                                                     | 36.4 ns: 1.03x faster                                                       |
| fannkuch                   | 247 ms                                                      | 240 ms: 1.03x faster                                                        |
| xml_etree_process          | 37.7 ms                                                     | 36.7 ms: 1.03x faster                                                       |
| json_loads                 | 13.9 us                                                     | 13.6 us: 1.03x faster                                                       |
| pyflate                    | 295 ms                                                      | 287 ms: 1.03x faster                                                        |
| chameleon                  | 4.98 ms                                                     | 4.86 ms: 1.03x faster                                                       |
| gc_traversal               | 1.52 ms                                                     | 1.49 ms: 1.02x faster                                                       |
| sqlglot_optimize           | 34.5 ms                                                     | 33.8 ms: 1.02x faster                                                       |
| unpickle_list              | 2.75 us                                                     | 2.69 us: 1.02x faster                                                       |
| meteor_contest             | 74.6 ms                                                     | 73.0 ms: 1.02x faster                                                       |
| tornado_http               | 89.5 ms                                                     | 87.7 ms: 1.02x faster                                                       |
| generators                 | 22.5 ms                                                     | 22.1 ms: 1.02x faster                                                       |
| dask                       | 263 ms                                                      | 258 ms: 1.02x faster                                                        |
| pidigits                   | 152 ms                                                      | 150 ms: 1.02x faster                                                        |
| 2to3                       | 218 ms                                                      | 215 ms: 1.01x faster                                                        |
| scimark_fft                | 184 ms                                                      | 182 ms: 1.01x faster                                                        |
| xml_etree_parse            | 93.0 ms                                                     | 92.0 ms: 1.01x faster                                                       |
| pickle_dict                | 18.4 us                                                     | 18.3 us: 1.01x faster                                                       |
| pathlib                    | 80.5 ms                                                     | 79.8 ms: 1.01x faster                                                       |
| regex_effbot               | 1.62 ms                                                     | 1.61 ms: 1.01x faster                                                       |
| bench_mp_pool              | 69.2 ms                                                     | 69.8 ms: 1.01x slower                                                       |
| scimark_sor                | 78.8 ms                                                     | 79.9 ms: 1.01x slower                                                       |
| unpickle                   | 8.18 us                                                     | 8.32 us: 1.02x slower                                                       |
| tomli_loads                | 1.37 sec                                                    | 1.40 sec: 1.02x slower                                                      |
| mdp                        | 1.37 sec                                                    | 1.41 sec: 1.03x slower                                                      |
| python_startup             | 19.5 ms                                                     | 20.6 ms: 1.06x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 15.3 ms: 1.07x slower                                                       |
| coverage                   | 40.8 ms                                                     | 45.9 ms: 1.12x slower                                                       |
| python_startup_no_site     | 16.2 ms                                                     | 18.8 ms: 1.16x slower                                                       |
| telco                      | 4.13 ms                                                     | 4.92 ms: 1.19x slower                                                       |
| Geometric mean             | (ref)                                                       | 1.05x faster                                                                |

Benchmark hidden because not significant (6): async_tree_io, json, bench_thread_pool, async_tree_memoization, pickle_list, pycparser
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: unknown