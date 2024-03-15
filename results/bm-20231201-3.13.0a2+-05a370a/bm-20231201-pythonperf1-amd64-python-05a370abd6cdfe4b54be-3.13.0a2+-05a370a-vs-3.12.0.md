
# Results vs. 3.12.0

- fork: python
- ref: 05a370abd6cdfe4b54be
- machine: windows-amd64
- commit hash: 05a370a
- commit date: 2023-12-01
- overall geometric mean: 1.00x slower
- HPT reliability: 89.00%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231201-pythonperf1-amd64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| chameleon      | 4.98 ms                                                     | 5.21 ms: 1.05x slower                                                       |
| docutils       | 1.66 sec                                                    | 1.58 sec: 1.05x faster                                                      |
| tornado_http   | 89.5 ms                                                     | 88.4 ms: 1.01x faster                                                       |
| Geometric mean | (ref)                                                       | 1.00x faster                                                                |

Benchmark hidden because not significant (1): 2to3

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231201-pythonperf1-amd64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 276 ms: 1.06x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 465 ms: 1.05x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 488 ms: 1.03x faster                                                        |
| async_tree_io_tg           | 771 ms                                                      | 781 ms: 1.01x slower                                                        |
| async_tree_io              | 731 ms                                                      | 743 ms: 1.02x slower                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 376 ms: 1.02x slower                                                        |
| async_tree_memoization     | 339 ms                                                      | 352 ms: 1.04x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.00x faster                                                                |

Benchmark hidden because not significant (1): async_tree_none_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231201-pythonperf1-amd64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 56.8 ms                                                     | 54.1 ms: 1.05x faster                                                       |
| pidigits       | 152 ms                                                      | 147 ms: 1.03x faster                                                        |
| nbody          | 71.9 ms                                                     | 75.8 ms: 1.05x slower                                                       |
| Geometric mean | (ref)                                                       | 1.01x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231201-pythonperf1-amd64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 120 ms: 1.06x faster                                                        |
| regex_effbot   | 1.62 ms                                                     | 1.58 ms: 1.02x faster                                                       |
| regex_compile  | 87.5 ms                                                     | 86.6 ms: 1.01x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 14.7 ms: 1.04x slower                                                       |
| Geometric mean | (ref)                                                       | 1.01x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231201-pythonperf1-amd64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle               | 7.43 us                                                     | 6.84 us: 1.09x faster                                                       |
| unpickle_list        | 2.75 us                                                     | 2.66 us: 1.03x faster                                                       |
| json_loads           | 13.9 us                                                     | 13.6 us: 1.02x faster                                                       |
| pickle_dict          | 18.4 us                                                     | 18.2 us: 1.01x faster                                                       |
| pickle_list          | 2.83 us                                                     | 2.81 us: 1.00x faster                                                       |
| xml_etree_parse      | 93.0 ms                                                     | 94.7 ms: 1.02x slower                                                       |
| json_dumps           | 5.70 ms                                                     | 5.86 ms: 1.03x slower                                                       |
| unpickle             | 8.18 us                                                     | 8.44 us: 1.03x slower                                                       |
| xml_etree_generate   | 55.8 ms                                                     | 57.8 ms: 1.03x slower                                                       |
| xml_etree_process    | 37.7 ms                                                     | 39.9 ms: 1.06x slower                                                       |
| unpickle_pure_python | 133 us                                                      | 142 us: 1.07x slower                                                        |
| tomli_loads          | 1.37 sec                                                    | 1.51 sec: 1.11x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.01x slower                                                                |

Benchmark hidden because not significant (2): pickle_pure_python, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231201-pythonperf1-amd64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 20.3 ms: 1.04x slower                                                       |
| python_startup_no_site | 16.2 ms                                                     | 18.2 ms: 1.12x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.08x slower                                                                |

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231201-pythonperf1-amd64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| comprehensions             | 14.1 us                                                     | 11.2 us: 1.26x faster                                                       |
| mypy2                      | 509 ms                                                      | 426 ms: 1.20x faster                                                        |
| typing_runtime_protocols   | 95.1 us                                                     | 80.1 us: 1.19x faster                                                       |
| sqlite_synth               | 1.76 us                                                     | 1.57 us: 1.12x faster                                                       |
| raytrace                   | 192 ms                                                      | 173 ms: 1.11x faster                                                        |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.90 sec: 1.10x faster                                                      |
| pickle                     | 7.43 us                                                     | 6.84 us: 1.09x faster                                                       |
| sympy_sum                  | 91.5 ms                                                     | 85.1 ms: 1.08x faster                                                       |
| sympy_str                  | 175 ms                                                      | 163 ms: 1.07x faster                                                        |
| bench_mp_pool              | 69.2 ms                                                     | 64.7 ms: 1.07x faster                                                       |
| crypto_pyaes               | 48.5 ms                                                     | 45.8 ms: 1.06x faster                                                       |
| regex_dna                  | 126 ms                                                      | 120 ms: 1.06x faster                                                        |
| async_tree_none            | 291 ms                                                      | 276 ms: 1.06x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 465 ms: 1.05x faster                                                        |
| docutils                   | 1.66 sec                                                    | 1.58 sec: 1.05x faster                                                      |
| float                      | 56.8 ms                                                     | 54.1 ms: 1.05x faster                                                       |
| chaos                      | 43.3 ms                                                     | 41.3 ms: 1.05x faster                                                       |
| pidigits                   | 152 ms                                                      | 147 ms: 1.03x faster                                                        |
| unpickle_list              | 2.75 us                                                     | 2.66 us: 1.03x faster                                                       |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 488 ms: 1.03x faster                                                        |
| gc_traversal               | 1.52 ms                                                     | 1.48 ms: 1.03x faster                                                       |
| dulwich_log                | 44.3 ms                                                     | 43.2 ms: 1.03x faster                                                       |
| create_gc_cycles           | 752 us                                                      | 733 us: 1.03x faster                                                        |
| json_loads                 | 13.9 us                                                     | 13.6 us: 1.02x faster                                                       |
| regex_effbot               | 1.62 ms                                                     | 1.58 ms: 1.02x faster                                                       |
| spectral_norm              | 66.9 ms                                                     | 65.6 ms: 1.02x faster                                                       |
| tornado_http               | 89.5 ms                                                     | 88.4 ms: 1.01x faster                                                       |
| async_generators           | 239 ms                                                      | 236 ms: 1.01x faster                                                        |
| sympy_expand               | 284 ms                                                      | 281 ms: 1.01x faster                                                        |
| regex_compile              | 87.5 ms                                                     | 86.6 ms: 1.01x faster                                                       |
| pickle_dict                | 18.4 us                                                     | 18.2 us: 1.01x faster                                                       |
| sympy_integrate            | 13.0 ms                                                     | 12.8 ms: 1.01x faster                                                       |
| scimark_monte_carlo        | 43.7 ms                                                     | 43.3 ms: 1.01x faster                                                       |
| pickle_list                | 2.83 us                                                     | 2.81 us: 1.00x faster                                                       |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.57 ms: 1.01x slower                                                       |
| nqueens                    | 62.8 ms                                                     | 63.1 ms: 1.01x slower                                                       |
| go                         | 91.6 ms                                                     | 92.1 ms: 1.01x slower                                                       |
| sqlglot_normalize          | 187 ms                                                      | 188 ms: 1.01x slower                                                        |
| scimark_fft                | 184 ms                                                      | 186 ms: 1.01x slower                                                        |
| async_tree_io_tg           | 771 ms                                                      | 781 ms: 1.01x slower                                                        |
| async_tree_io              | 731 ms                                                      | 743 ms: 1.02x slower                                                        |
| deepcopy_reduce            | 2.09 us                                                     | 2.13 us: 1.02x slower                                                       |
| xml_etree_parse            | 93.0 ms                                                     | 94.7 ms: 1.02x slower                                                       |
| meteor_contest             | 74.6 ms                                                     | 76.1 ms: 1.02x slower                                                       |
| logging_format             | 6.72 us                                                     | 6.88 us: 1.02x slower                                                       |
| async_tree_memoization_tg  | 367 ms                                                      | 376 ms: 1.02x slower                                                        |
| sqlglot_parse              | 804 us                                                      | 824 us: 1.02x slower                                                        |
| deepcopy                   | 238 us                                                      | 244 us: 1.02x slower                                                        |
| sqlglot_optimize           | 34.5 ms                                                     | 35.4 ms: 1.02x slower                                                       |
| sqlglot_transpile          | 1.02 ms                                                     | 1.05 ms: 1.03x slower                                                       |
| coroutines                 | 14.3 ms                                                     | 14.6 ms: 1.03x slower                                                       |
| json_dumps                 | 5.70 ms                                                     | 5.86 ms: 1.03x slower                                                       |
| unpack_sequence            | 37.5 ns                                                     | 38.5 ns: 1.03x slower                                                       |
| unpickle                   | 8.18 us                                                     | 8.44 us: 1.03x slower                                                       |
| logging_simple             | 6.28 us                                                     | 6.47 us: 1.03x slower                                                       |
| generators                 | 22.5 ms                                                     | 23.3 ms: 1.03x slower                                                       |
| xml_etree_generate         | 55.8 ms                                                     | 57.8 ms: 1.03x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 14.7 ms: 1.04x slower                                                       |
| scimark_lu                 | 58.9 ms                                                     | 61.0 ms: 1.04x slower                                                       |
| async_tree_memoization     | 339 ms                                                      | 352 ms: 1.04x slower                                                        |
| pyflate                    | 295 ms                                                      | 306 ms: 1.04x slower                                                        |
| deltablue                  | 2.16 ms                                                     | 2.25 ms: 1.04x slower                                                       |
| scimark_sor                | 78.8 ms                                                     | 82.0 ms: 1.04x slower                                                       |
| python_startup             | 19.5 ms                                                     | 20.3 ms: 1.04x slower                                                       |
| logging_silent             | 60.5 ns                                                     | 63.1 ns: 1.04x slower                                                       |
| pprint_safe_repr           | 513 ms                                                      | 535 ms: 1.04x slower                                                        |
| pprint_pformat             | 1.05 sec                                                    | 1.09 sec: 1.05x slower                                                      |
| chameleon                  | 4.98 ms                                                     | 5.21 ms: 1.05x slower                                                       |
| hexiom                     | 4.10 ms                                                     | 4.29 ms: 1.05x slower                                                       |
| nbody                      | 71.9 ms                                                     | 75.8 ms: 1.05x slower                                                       |
| xml_etree_process          | 37.7 ms                                                     | 39.9 ms: 1.06x slower                                                       |
| deepcopy_memo              | 23.7 us                                                     | 25.2 us: 1.06x slower                                                       |
| unpickle_pure_python       | 133 us                                                      | 142 us: 1.07x slower                                                        |
| richards_super             | 32.1 ms                                                     | 34.7 ms: 1.08x slower                                                       |
| richards                   | 28.4 ms                                                     | 30.9 ms: 1.09x slower                                                       |
| tomli_loads                | 1.37 sec                                                    | 1.51 sec: 1.11x slower                                                      |
| fannkuch                   | 247 ms                                                      | 275 ms: 1.11x slower                                                        |
| python_startup_no_site     | 16.2 ms                                                     | 18.2 ms: 1.12x slower                                                       |
| coverage                   | 40.8 ms                                                     | 46.0 ms: 1.13x slower                                                       |
| pycparser                  | 699 ms                                                      | 836 ms: 1.20x slower                                                        |
| telco                      | 4.13 ms                                                     | 5.01 ms: 1.21x slower                                                       |
| Geometric mean             | (ref)                                                       | 1.00x slower                                                                |

Benchmark hidden because not significant (11): asyncio_tcp, json, pickle_pure_python, mako, 2to3, pathlib, mdp, xml_etree_iterparse, async_tree_none_tg, dask, bench_thread_pool
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 89.00% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown