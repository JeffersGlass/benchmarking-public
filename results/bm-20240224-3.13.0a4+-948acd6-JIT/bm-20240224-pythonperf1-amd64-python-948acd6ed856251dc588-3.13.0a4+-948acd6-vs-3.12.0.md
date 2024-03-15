
# Results vs. 3.12.0

- fork: python
- ref: 948acd6ed856251dc588
- machine: windows-amd64
- commit hash: 948acd6
- commit date: 2024-02-24
- overall geometric mean: 1.02x slower \*
- HPT reliability: 61.52%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 227 ms: 1.04x slower                                                        |
| chameleon      | 4.98 ms                                                     | 4.80 ms: 1.04x faster                                                       |
| tornado_http   | 89.5 ms                                                     | 85.6 ms: 1.05x faster                                                       |
| Geometric mean | (ref)                                                       | 1.01x faster                                                                |

Benchmark hidden because not significant (1): docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 265 ms: 1.10x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 454 ms: 1.08x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 467 ms: 1.07x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 344 ms: 1.07x faster                                                        |
| async_tree_none_tg         | 285 ms                                                      | 272 ms: 1.05x faster                                                        |
| async_tree_io_tg           | 771 ms                                                      | 750 ms: 1.03x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.05x faster                                                                |

Benchmark hidden because not significant (2): async_tree_io, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| nbody          | 71.9 ms                                                     | 61.9 ms: 1.16x faster                                                       |
| float          | 56.8 ms                                                     | 50.0 ms: 1.14x faster                                                       |
| pidigits       | 152 ms                                                      | 152 ms: 1.00x faster                                                        |
| Geometric mean | (ref)                                                       | 1.10x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 119 ms: 1.07x faster                                                        |
| regex_effbot   | 1.62 ms                                                     | 1.57 ms: 1.03x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 16.7 ms: 1.17x slower                                                       |
| regex_compile  | 87.5 ms                                                     | 104 ms: 1.19x slower                                                        |
| Geometric mean | (ref)                                                       | 1.06x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 176 us: 1.11x faster                                                        |
| xml_etree_generate   | 55.8 ms                                                     | 53.3 ms: 1.05x faster                                                       |
| pickle_dict          | 18.4 us                                                     | 17.6 us: 1.05x faster                                                       |
| tomli_loads          | 1.37 sec                                                    | 1.32 sec: 1.04x faster                                                      |
| xml_etree_iterparse  | 65.2 ms                                                     | 63.6 ms: 1.02x faster                                                       |
| xml_etree_process    | 37.7 ms                                                     | 36.9 ms: 1.02x faster                                                       |
| json_dumps           | 5.70 ms                                                     | 5.59 ms: 1.02x faster                                                       |
| pickle               | 7.43 us                                                     | 7.33 us: 1.01x faster                                                       |
| xml_etree_parse      | 93.0 ms                                                     | 92.3 ms: 1.01x faster                                                       |
| json_loads           | 13.9 us                                                     | 13.8 us: 1.01x faster                                                       |
| unpickle_list        | 2.75 us                                                     | 2.78 us: 1.01x slower                                                       |
| unpickle             | 8.18 us                                                     | 8.50 us: 1.04x slower                                                       |
| unpickle_pure_python | 133 us                                                      | 142 us: 1.07x slower                                                        |
| pickle_list          | 2.83 us                                                     | 3.10 us: 1.10x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.01x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 23.2 ms: 1.19x slower                                                       |
| python_startup_no_site | 16.2 ms                                                     | 20.9 ms: 1.29x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.24x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 6.45 ms: 1.10x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 70.8 us: 1.34x faster                                                       |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.80 sec: 1.17x faster                                                      |
| nbody                      | 71.9 ms                                                     | 61.9 ms: 1.16x faster                                                       |
| comprehensions             | 14.1 us                                                     | 12.2 us: 1.15x faster                                                       |
| float                      | 56.8 ms                                                     | 50.0 ms: 1.14x faster                                                       |
| sqlite_synth               | 1.76 us                                                     | 1.57 us: 1.12x faster                                                       |
| mypy2                      | 509 ms                                                      | 459 ms: 1.11x faster                                                        |
| pickle_pure_python         | 195 us                                                      | 176 us: 1.11x faster                                                        |
| async_tree_none            | 291 ms                                                      | 265 ms: 1.10x faster                                                        |
| mako                       | 7.09 ms                                                     | 6.45 ms: 1.10x faster                                                       |
| logging_silent             | 60.5 ns                                                     | 55.4 ns: 1.09x faster                                                       |
| deepcopy_memo              | 23.7 us                                                     | 21.8 us: 1.09x faster                                                       |
| deepcopy_reduce            | 2.09 us                                                     | 1.94 us: 1.08x faster                                                       |
| coroutines                 | 14.3 ms                                                     | 13.2 ms: 1.08x faster                                                       |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 454 ms: 1.08x faster                                                        |
| generators                 | 22.5 ms                                                     | 20.9 ms: 1.08x faster                                                       |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 467 ms: 1.07x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 344 ms: 1.07x faster                                                        |
| regex_dna                  | 126 ms                                                      | 119 ms: 1.07x faster                                                        |
| deepcopy                   | 238 us                                                      | 224 us: 1.06x faster                                                        |
| pathlib                    | 80.5 ms                                                     | 76.1 ms: 1.06x faster                                                       |
| crypto_pyaes               | 48.5 ms                                                     | 46.1 ms: 1.05x faster                                                       |
| async_tree_none_tg         | 285 ms                                                      | 272 ms: 1.05x faster                                                        |
| xml_etree_generate         | 55.8 ms                                                     | 53.3 ms: 1.05x faster                                                       |
| pickle_dict                | 18.4 us                                                     | 17.6 us: 1.05x faster                                                       |
| tornado_http               | 89.5 ms                                                     | 85.6 ms: 1.05x faster                                                       |
| tomli_loads                | 1.37 sec                                                    | 1.32 sec: 1.04x faster                                                      |
| chameleon                  | 4.98 ms                                                     | 4.80 ms: 1.04x faster                                                       |
| spectral_norm              | 66.9 ms                                                     | 64.5 ms: 1.04x faster                                                       |
| regex_effbot               | 1.62 ms                                                     | 1.57 ms: 1.03x faster                                                       |
| async_tree_io_tg           | 771 ms                                                      | 750 ms: 1.03x faster                                                        |
| logging_format             | 6.72 us                                                     | 6.53 us: 1.03x faster                                                       |
| asyncio_tcp                | 487 ms                                                      | 475 ms: 1.03x faster                                                        |
| dulwich_log                | 44.3 ms                                                     | 43.2 ms: 1.03x faster                                                       |
| xml_etree_iterparse        | 65.2 ms                                                     | 63.6 ms: 1.02x faster                                                       |
| logging_simple             | 6.28 us                                                     | 6.13 us: 1.02x faster                                                       |
| xml_etree_process          | 37.7 ms                                                     | 36.9 ms: 1.02x faster                                                       |
| json_dumps                 | 5.70 ms                                                     | 5.59 ms: 1.02x faster                                                       |
| sqlglot_normalize          | 187 ms                                                      | 184 ms: 1.02x faster                                                        |
| create_gc_cycles           | 752 us                                                      | 738 us: 1.02x faster                                                        |
| bench_thread_pool          | 857 us                                                      | 841 us: 1.02x faster                                                        |
| gc_traversal               | 1.52 ms                                                     | 1.50 ms: 1.02x faster                                                       |
| pickle                     | 7.43 us                                                     | 7.33 us: 1.01x faster                                                       |
| xml_etree_parse            | 93.0 ms                                                     | 92.3 ms: 1.01x faster                                                       |
| json_loads                 | 13.9 us                                                     | 13.8 us: 1.01x faster                                                       |
| raytrace                   | 192 ms                                                      | 191 ms: 1.01x faster                                                        |
| pidigits                   | 152 ms                                                      | 152 ms: 1.00x faster                                                        |
| pprint_safe_repr           | 513 ms                                                      | 517 ms: 1.01x slower                                                        |
| deltablue                  | 2.16 ms                                                     | 2.18 ms: 1.01x slower                                                       |
| unpickle_list              | 2.75 us                                                     | 2.78 us: 1.01x slower                                                       |
| sqlglot_transpile          | 1.02 ms                                                     | 1.04 ms: 1.02x slower                                                       |
| pprint_pformat             | 1.05 sec                                                    | 1.07 sec: 1.02x slower                                                      |
| sympy_str                  | 175 ms                                                      | 179 ms: 1.02x slower                                                        |
| sqlglot_parse              | 804 us                                                      | 824 us: 1.02x slower                                                        |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.63 ms: 1.03x slower                                                       |
| sympy_sum                  | 91.5 ms                                                     | 94.2 ms: 1.03x slower                                                       |
| nqueens                    | 62.8 ms                                                     | 64.7 ms: 1.03x slower                                                       |
| meteor_contest             | 74.6 ms                                                     | 76.9 ms: 1.03x slower                                                       |
| unpickle                   | 8.18 us                                                     | 8.50 us: 1.04x slower                                                       |
| 2to3                       | 218 ms                                                      | 227 ms: 1.04x slower                                                        |
| pycparser                  | 699 ms                                                      | 730 ms: 1.04x slower                                                        |
| sqlglot_optimize           | 34.5 ms                                                     | 36.1 ms: 1.05x slower                                                       |
| scimark_fft                | 184 ms                                                      | 194 ms: 1.05x slower                                                        |
| async_generators           | 239 ms                                                      | 255 ms: 1.06x slower                                                        |
| unpickle_pure_python       | 133 us                                                      | 142 us: 1.07x slower                                                        |
| fannkuch                   | 247 ms                                                      | 263 ms: 1.07x slower                                                        |
| sympy_integrate            | 13.0 ms                                                     | 14.0 ms: 1.08x slower                                                       |
| scimark_monte_carlo        | 43.7 ms                                                     | 47.6 ms: 1.09x slower                                                       |
| richards_super             | 32.1 ms                                                     | 35.0 ms: 1.09x slower                                                       |
| sympy_expand               | 284 ms                                                      | 310 ms: 1.09x slower                                                        |
| pickle_list                | 2.83 us                                                     | 3.10 us: 1.10x slower                                                       |
| richards                   | 28.4 ms                                                     | 31.4 ms: 1.11x slower                                                       |
| telco                      | 4.13 ms                                                     | 4.59 ms: 1.11x slower                                                       |
| pyflate                    | 295 ms                                                      | 328 ms: 1.11x slower                                                        |
| regex_v8                   | 14.2 ms                                                     | 16.7 ms: 1.17x slower                                                       |
| coverage                   | 40.8 ms                                                     | 48.0 ms: 1.18x slower                                                       |
| regex_compile              | 87.5 ms                                                     | 104 ms: 1.19x slower                                                        |
| go                         | 91.6 ms                                                     | 109 ms: 1.19x slower                                                        |
| python_startup             | 19.5 ms                                                     | 23.2 ms: 1.19x slower                                                       |
| mdp                        | 1.37 sec                                                    | 1.68 sec: 1.22x slower                                                      |
| python_startup_no_site     | 16.2 ms                                                     | 20.9 ms: 1.29x slower                                                       |
| scimark_sor                | 78.8 ms                                                     | 102 ms: 1.30x slower                                                        |
| scimark_lu                 | 58.9 ms                                                     | 76.6 ms: 1.30x slower                                                       |
| hexiom                     | 4.10 ms                                                     | 6.28 ms: 1.53x slower                                                       |
| unpack_sequence            | 37.5 ns                                                     | 88.5 ns: 2.36x slower                                                       |
| Geometric mean             | (ref)                                                       | 1.02x slower                                                                |

Benchmark hidden because not significant (6): json, async_tree_io, async_tree_memoization, chaos, bench_mp_pool, docutils
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 61.52% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown