
# Results vs. 3.12.0

- fork: python
- ref: 742ba6081c92744ba30f
- machine: windows-amd64
- commit hash: 742ba60
- commit date: 2024-01-29
- overall geometric mean: 1.02x faster
- HPT reliability: 99.41%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 221 ms: 1.02x slower                                                        |
| chameleon      | 4.98 ms                                                     | 4.79 ms: 1.04x faster                                                       |
| docutils       | 1.66 sec                                                    | 1.59 sec: 1.04x faster                                                      |
| tornado_http   | 89.5 ms                                                     | 87.6 ms: 1.02x faster                                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 273 ms: 1.07x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 460 ms: 1.06x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 481 ms: 1.04x faster                                                        |
| async_tree_io              | 731 ms                                                      | 741 ms: 1.01x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.02x faster                                                                |

Benchmark hidden because not significant (4): async_tree_memoization_tg, async_tree_none_tg, async_tree_memoization, async_tree_io_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| nbody          | 71.9 ms                                                     | 60.9 ms: 1.18x faster                                                       |
| float          | 56.8 ms                                                     | 51.0 ms: 1.11x faster                                                       |
| Geometric mean | (ref)                                                       | 1.10x faster                                                                |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 87.5 ms                                                     | 81.0 ms: 1.08x faster                                                       |
| regex_dna      | 126 ms                                                      | 124 ms: 1.02x faster                                                        |
| regex_effbot   | 1.62 ms                                                     | 1.60 ms: 1.01x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 21.9 ms: 1.54x slower                                                       |
| Geometric mean | (ref)                                                       | 1.08x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 173 us: 1.13x faster                                                        |
| unpickle_pure_python | 133 us                                                      | 125 us: 1.07x faster                                                        |
| tomli_loads          | 1.37 sec                                                    | 1.29 sec: 1.06x faster                                                      |
| xml_etree_generate   | 55.8 ms                                                     | 53.5 ms: 1.04x faster                                                       |
| pickle_dict          | 18.4 us                                                     | 17.7 us: 1.04x faster                                                       |
| json_dumps           | 5.70 ms                                                     | 5.55 ms: 1.03x faster                                                       |
| pickle               | 7.43 us                                                     | 7.28 us: 1.02x faster                                                       |
| xml_etree_process    | 37.7 ms                                                     | 37.0 ms: 1.02x faster                                                       |
| pickle_list          | 2.83 us                                                     | 2.77 us: 1.02x faster                                                       |
| json_loads           | 13.9 us                                                     | 13.7 us: 1.01x faster                                                       |
| xml_etree_iterparse  | 65.2 ms                                                     | 65.9 ms: 1.01x slower                                                       |
| xml_etree_parse      | 93.0 ms                                                     | 94.6 ms: 1.02x slower                                                       |
| unpickle             | 8.18 us                                                     | 8.54 us: 1.04x slower                                                       |
| unpickle_list        | 2.75 us                                                     | 2.87 us: 1.05x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.02x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 21.3 ms: 1.10x slower                                                       |
| python_startup_no_site | 16.2 ms                                                     | 19.1 ms: 1.18x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.14x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 6.82 ms: 1.04x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 69.9 us: 1.36x faster                                                       |
| comprehensions             | 14.1 us                                                     | 11.4 us: 1.24x faster                                                       |
| nbody                      | 71.9 ms                                                     | 60.9 ms: 1.18x faster                                                       |
| mypy2                      | 509 ms                                                      | 432 ms: 1.18x faster                                                        |
| raytrace                   | 192 ms                                                      | 168 ms: 1.15x faster                                                        |
| richards_super             | 32.1 ms                                                     | 28.1 ms: 1.14x faster                                                       |
| logging_silent             | 60.5 ns                                                     | 53.5 ns: 1.13x faster                                                       |
| richards                   | 28.4 ms                                                     | 25.1 ms: 1.13x faster                                                       |
| pickle_pure_python         | 195 us                                                      | 173 us: 1.13x faster                                                        |
| sqlite_synth               | 1.76 us                                                     | 1.56 us: 1.13x faster                                                       |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.87 sec: 1.12x faster                                                      |
| float                      | 56.8 ms                                                     | 51.0 ms: 1.11x faster                                                       |
| deepcopy_memo              | 23.7 us                                                     | 21.4 us: 1.11x faster                                                       |
| deepcopy_reduce            | 2.09 us                                                     | 1.89 us: 1.11x faster                                                       |
| coroutines                 | 14.3 ms                                                     | 12.9 ms: 1.10x faster                                                       |
| deepcopy                   | 238 us                                                      | 217 us: 1.10x faster                                                        |
| scimark_lu                 | 58.9 ms                                                     | 54.1 ms: 1.09x faster                                                       |
| regex_compile              | 87.5 ms                                                     | 81.0 ms: 1.08x faster                                                       |
| sqlglot_normalize          | 187 ms                                                      | 173 ms: 1.08x faster                                                        |
| sqlglot_parse              | 804 us                                                      | 750 us: 1.07x faster                                                        |
| sympy_str                  | 175 ms                                                      | 164 ms: 1.07x faster                                                        |
| generators                 | 22.5 ms                                                     | 21.1 ms: 1.07x faster                                                       |
| unpickle_pure_python       | 133 us                                                      | 125 us: 1.07x faster                                                        |
| async_tree_none            | 291 ms                                                      | 273 ms: 1.07x faster                                                        |
| logging_simple             | 6.28 us                                                     | 5.89 us: 1.06x faster                                                       |
| nqueens                    | 62.8 ms                                                     | 59.0 ms: 1.06x faster                                                       |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 460 ms: 1.06x faster                                                        |
| tomli_loads                | 1.37 sec                                                    | 1.29 sec: 1.06x faster                                                      |
| scimark_sor                | 78.8 ms                                                     | 74.7 ms: 1.05x faster                                                       |
| logging_format             | 6.72 us                                                     | 6.40 us: 1.05x faster                                                       |
| sqlglot_transpile          | 1.02 ms                                                     | 976 us: 1.05x faster                                                        |
| docutils                   | 1.66 sec                                                    | 1.59 sec: 1.04x faster                                                      |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 481 ms: 1.04x faster                                                        |
| xml_etree_generate         | 55.8 ms                                                     | 53.5 ms: 1.04x faster                                                       |
| bench_thread_pool          | 857 us                                                      | 821 us: 1.04x faster                                                        |
| pickle_dict                | 18.4 us                                                     | 17.7 us: 1.04x faster                                                       |
| chameleon                  | 4.98 ms                                                     | 4.79 ms: 1.04x faster                                                       |
| mako                       | 7.09 ms                                                     | 6.82 ms: 1.04x faster                                                       |
| crypto_pyaes               | 48.5 ms                                                     | 46.9 ms: 1.03x faster                                                       |
| deltablue                  | 2.16 ms                                                     | 2.09 ms: 1.03x faster                                                       |
| sympy_sum                  | 91.5 ms                                                     | 88.8 ms: 1.03x faster                                                       |
| pprint_safe_repr           | 513 ms                                                      | 500 ms: 1.03x faster                                                        |
| json_dumps                 | 5.70 ms                                                     | 5.55 ms: 1.03x faster                                                       |
| dulwich_log                | 44.3 ms                                                     | 43.3 ms: 1.02x faster                                                       |
| tornado_http               | 89.5 ms                                                     | 87.6 ms: 1.02x faster                                                       |
| chaos                      | 43.3 ms                                                     | 42.4 ms: 1.02x faster                                                       |
| pprint_pformat             | 1.05 sec                                                    | 1.02 sec: 1.02x faster                                                      |
| pickle                     | 7.43 us                                                     | 7.28 us: 1.02x faster                                                       |
| xml_etree_process          | 37.7 ms                                                     | 37.0 ms: 1.02x faster                                                       |
| pickle_list                | 2.83 us                                                     | 2.77 us: 1.02x faster                                                       |
| regex_dna                  | 126 ms                                                      | 124 ms: 1.02x faster                                                        |
| sympy_expand               | 284 ms                                                      | 279 ms: 1.02x faster                                                        |
| spectral_norm              | 66.9 ms                                                     | 65.8 ms: 1.02x faster                                                       |
| create_gc_cycles           | 752 us                                                      | 742 us: 1.01x faster                                                        |
| regex_effbot               | 1.62 ms                                                     | 1.60 ms: 1.01x faster                                                       |
| sqlglot_optimize           | 34.5 ms                                                     | 34.1 ms: 1.01x faster                                                       |
| json_loads                 | 13.9 us                                                     | 13.7 us: 1.01x faster                                                       |
| fannkuch                   | 247 ms                                                      | 246 ms: 1.00x faster                                                        |
| xml_etree_iterparse        | 65.2 ms                                                     | 65.9 ms: 1.01x slower                                                       |
| gc_traversal               | 1.52 ms                                                     | 1.54 ms: 1.01x slower                                                       |
| async_tree_io              | 731 ms                                                      | 741 ms: 1.01x slower                                                        |
| 2to3                       | 218 ms                                                      | 221 ms: 1.02x slower                                                        |
| pathlib                    | 80.5 ms                                                     | 81.7 ms: 1.02x slower                                                       |
| xml_etree_parse            | 93.0 ms                                                     | 94.6 ms: 1.02x slower                                                       |
| async_generators           | 239 ms                                                      | 244 ms: 1.02x slower                                                        |
| sympy_integrate            | 13.0 ms                                                     | 13.2 ms: 1.02x slower                                                       |
| unpickle                   | 8.18 us                                                     | 8.54 us: 1.04x slower                                                       |
| scimark_fft                | 184 ms                                                      | 193 ms: 1.05x slower                                                        |
| meteor_contest             | 74.6 ms                                                     | 78.0 ms: 1.05x slower                                                       |
| unpickle_list              | 2.75 us                                                     | 2.87 us: 1.05x slower                                                       |
| go                         | 91.6 ms                                                     | 96.0 ms: 1.05x slower                                                       |
| pyflate                    | 295 ms                                                      | 312 ms: 1.06x slower                                                        |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.76 ms: 1.08x slower                                                       |
| unpack_sequence            | 37.5 ns                                                     | 40.7 ns: 1.09x slower                                                       |
| python_startup             | 19.5 ms                                                     | 21.3 ms: 1.10x slower                                                       |
| coverage                   | 40.8 ms                                                     | 45.5 ms: 1.11x slower                                                       |
| telco                      | 4.13 ms                                                     | 4.67 ms: 1.13x slower                                                       |
| mdp                        | 1.37 sec                                                    | 1.55 sec: 1.13x slower                                                      |
| python_startup_no_site     | 16.2 ms                                                     | 19.1 ms: 1.18x slower                                                       |
| hexiom                     | 4.10 ms                                                     | 5.18 ms: 1.26x slower                                                       |
| scimark_monte_carlo        | 43.7 ms                                                     | 57.0 ms: 1.30x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 21.9 ms: 1.54x slower                                                       |
| Geometric mean             | (ref)                                                       | 1.02x faster                                                                |

Benchmark hidden because not significant (10): async_tree_memoization_tg, pycparser, json, async_tree_none_tg, bench_mp_pool, pidigits, async_tree_memoization, dask, async_tree_io_tg, asyncio_tcp
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.41% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown