
# Results vs. 3.12.0

- fork: python
- ref: a768e12f094a9b14a9a1
- machine: windows-amd64
- commit hash: a768e12
- commit date: 2024-01-27
- overall geometric mean: 1.01x slower
- HPT reliability: 69.36%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 222 ms: 1.02x slower                                                        |
| docutils       | 1.66 sec                                                    | 1.60 sec: 1.04x faster                                                      |
| tornado_http   | 89.5 ms                                                     | 86.8 ms: 1.03x faster                                                       |
| Geometric mean | (ref)                                                       | 1.01x faster                                                                |

Benchmark hidden because not significant (1): chameleon

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 489 ms                                                      | 457 ms: 1.07x faster                                                        |
| async_tree_none            | 291 ms                                                      | 278 ms: 1.05x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 481 ms: 1.04x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 354 ms: 1.04x faster                                                        |
| async_tree_io_tg           | 771 ms                                                      | 783 ms: 1.02x slower                                                        |
| async_tree_io              | 731 ms                                                      | 750 ms: 1.03x slower                                                        |
| async_tree_memoization     | 339 ms                                                      | 354 ms: 1.04x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.02x faster                                                                |

Benchmark hidden because not significant (1): async_tree_none_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 152 ms                                                      | 150 ms: 1.02x faster                                                        |
| nbody          | 71.9 ms                                                     | 83.1 ms: 1.16x slower                                                       |
| Geometric mean | (ref)                                                       | 1.05x slower                                                                |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 121 ms: 1.04x faster                                                        |
| regex_effbot   | 1.62 ms                                                     | 1.57 ms: 1.03x faster                                                       |
| regex_compile  | 87.5 ms                                                     | 85.2 ms: 1.03x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 14.8 ms: 1.04x slower                                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 182 us: 1.07x faster                                                        |
| pickle               | 7.43 us                                                     | 7.20 us: 1.03x faster                                                       |
| json_loads           | 13.9 us                                                     | 13.7 us: 1.02x faster                                                       |
| json_dumps           | 5.70 ms                                                     | 5.66 ms: 1.01x faster                                                       |
| xml_etree_generate   | 55.8 ms                                                     | 56.2 ms: 1.01x slower                                                       |
| xml_etree_process    | 37.7 ms                                                     | 38.2 ms: 1.01x slower                                                       |
| pickle_dict          | 18.4 us                                                     | 18.8 us: 1.02x slower                                                       |
| pickle_list          | 2.83 us                                                     | 2.89 us: 1.02x slower                                                       |
| unpickle_pure_python | 133 us                                                      | 137 us: 1.03x slower                                                        |
| unpickle_list        | 2.75 us                                                     | 2.85 us: 1.04x slower                                                       |
| unpickle             | 8.18 us                                                     | 8.52 us: 1.04x slower                                                       |
| xml_etree_iterparse  | 65.2 ms                                                     | 68.0 ms: 1.04x slower                                                       |
| tomli_loads          | 1.37 sec                                                    | 1.43 sec: 1.05x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.01x slower                                                                |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 20.6 ms: 1.06x slower                                                       |
| python_startup_no_site | 16.2 ms                                                     | 18.4 ms: 1.14x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.10x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 7.38 ms: 1.04x slower                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 75.6 us: 1.26x faster                                                       |
| mypy2                      | 509 ms                                                      | 432 ms: 1.18x faster                                                        |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.86 sec: 1.13x faster                                                      |
| raytrace                   | 192 ms                                                      | 170 ms: 1.13x faster                                                        |
| logging_silent             | 60.5 ns                                                     | 54.1 ns: 1.12x faster                                                       |
| sqlite_synth               | 1.76 us                                                     | 1.58 us: 1.12x faster                                                       |
| coroutines                 | 14.3 ms                                                     | 13.1 ms: 1.09x faster                                                       |
| comprehensions             | 14.1 us                                                     | 13.0 us: 1.09x faster                                                       |
| pickle_pure_python         | 195 us                                                      | 182 us: 1.07x faster                                                        |
| generators                 | 22.5 ms                                                     | 21.0 ms: 1.07x faster                                                       |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 457 ms: 1.07x faster                                                        |
| richards                   | 28.4 ms                                                     | 26.8 ms: 1.06x faster                                                       |
| richards_super             | 32.1 ms                                                     | 30.4 ms: 1.06x faster                                                       |
| async_tree_none            | 291 ms                                                      | 278 ms: 1.05x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 481 ms: 1.04x faster                                                        |
| regex_dna                  | 126 ms                                                      | 121 ms: 1.04x faster                                                        |
| deepcopy                   | 238 us                                                      | 229 us: 1.04x faster                                                        |
| json                       | 3.05 ms                                                     | 2.93 ms: 1.04x faster                                                       |
| deepcopy_reduce            | 2.09 us                                                     | 2.01 us: 1.04x faster                                                       |
| async_generators           | 239 ms                                                      | 231 ms: 1.04x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 354 ms: 1.04x faster                                                        |
| docutils                   | 1.66 sec                                                    | 1.60 sec: 1.04x faster                                                      |
| pickle                     | 7.43 us                                                     | 7.20 us: 1.03x faster                                                       |
| tornado_http               | 89.5 ms                                                     | 86.8 ms: 1.03x faster                                                       |
| regex_effbot               | 1.62 ms                                                     | 1.57 ms: 1.03x faster                                                       |
| sympy_str                  | 175 ms                                                      | 170 ms: 1.03x faster                                                        |
| regex_compile              | 87.5 ms                                                     | 85.2 ms: 1.03x faster                                                       |
| sympy_sum                  | 91.5 ms                                                     | 89.6 ms: 1.02x faster                                                       |
| sqlglot_parse              | 804 us                                                      | 789 us: 1.02x faster                                                        |
| json_loads                 | 13.9 us                                                     | 13.7 us: 1.02x faster                                                       |
| pidigits                   | 152 ms                                                      | 150 ms: 1.02x faster                                                        |
| dulwich_log                | 44.3 ms                                                     | 43.7 ms: 1.01x faster                                                       |
| deepcopy_memo              | 23.7 us                                                     | 23.4 us: 1.01x faster                                                       |
| bench_mp_pool              | 69.2 ms                                                     | 68.4 ms: 1.01x faster                                                       |
| logging_simple             | 6.28 us                                                     | 6.22 us: 1.01x faster                                                       |
| sqlglot_transpile          | 1.02 ms                                                     | 1.01 ms: 1.01x faster                                                       |
| json_dumps                 | 5.70 ms                                                     | 5.66 ms: 1.01x faster                                                       |
| xml_etree_generate         | 55.8 ms                                                     | 56.2 ms: 1.01x slower                                                       |
| nqueens                    | 62.8 ms                                                     | 63.5 ms: 1.01x slower                                                       |
| sqlglot_normalize          | 187 ms                                                      | 189 ms: 1.01x slower                                                        |
| xml_etree_process          | 37.7 ms                                                     | 38.2 ms: 1.01x slower                                                       |
| async_tree_io_tg           | 771 ms                                                      | 783 ms: 1.02x slower                                                        |
| 2to3                       | 218 ms                                                      | 222 ms: 1.02x slower                                                        |
| pickle_dict                | 18.4 us                                                     | 18.8 us: 1.02x slower                                                       |
| pickle_list                | 2.83 us                                                     | 2.89 us: 1.02x slower                                                       |
| chaos                      | 43.3 ms                                                     | 44.4 ms: 1.02x slower                                                       |
| async_tree_io              | 731 ms                                                      | 750 ms: 1.03x slower                                                        |
| unpickle_pure_python       | 133 us                                                      | 137 us: 1.03x slower                                                        |
| pprint_safe_repr           | 513 ms                                                      | 528 ms: 1.03x slower                                                        |
| sympy_integrate            | 13.0 ms                                                     | 13.3 ms: 1.03x slower                                                       |
| sqlglot_optimize           | 34.5 ms                                                     | 35.7 ms: 1.03x slower                                                       |
| unpickle_list              | 2.75 us                                                     | 2.85 us: 1.04x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 14.8 ms: 1.04x slower                                                       |
| bench_thread_pool          | 857 us                                                      | 888 us: 1.04x slower                                                        |
| meteor_contest             | 74.6 ms                                                     | 77.5 ms: 1.04x slower                                                       |
| unpickle                   | 8.18 us                                                     | 8.52 us: 1.04x slower                                                       |
| mako                       | 7.09 ms                                                     | 7.38 ms: 1.04x slower                                                       |
| async_tree_memoization     | 339 ms                                                      | 354 ms: 1.04x slower                                                        |
| xml_etree_iterparse        | 65.2 ms                                                     | 68.0 ms: 1.04x slower                                                       |
| tomli_loads                | 1.37 sec                                                    | 1.43 sec: 1.05x slower                                                      |
| pprint_pformat             | 1.05 sec                                                    | 1.09 sec: 1.05x slower                                                      |
| python_startup             | 19.5 ms                                                     | 20.6 ms: 1.06x slower                                                       |
| fannkuch                   | 247 ms                                                      | 266 ms: 1.08x slower                                                        |
| scimark_monte_carlo        | 43.7 ms                                                     | 47.7 ms: 1.09x slower                                                       |
| pyflate                    | 295 ms                                                      | 325 ms: 1.10x slower                                                        |
| mdp                        | 1.37 sec                                                    | 1.53 sec: 1.11x slower                                                      |
| scimark_fft                | 184 ms                                                      | 205 ms: 1.11x slower                                                        |
| unpack_sequence            | 37.5 ns                                                     | 42.1 ns: 1.12x slower                                                       |
| coverage                   | 40.8 ms                                                     | 46.3 ms: 1.13x slower                                                       |
| python_startup_no_site     | 16.2 ms                                                     | 18.4 ms: 1.14x slower                                                       |
| telco                      | 4.13 ms                                                     | 4.75 ms: 1.15x slower                                                       |
| nbody                      | 71.9 ms                                                     | 83.1 ms: 1.16x slower                                                       |
| hexiom                     | 4.10 ms                                                     | 4.80 ms: 1.17x slower                                                       |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 3.07 ms: 1.20x slower                                                       |
| deltablue                  | 2.16 ms                                                     | 2.59 ms: 1.20x slower                                                       |
| spectral_norm              | 66.9 ms                                                     | 80.9 ms: 1.21x slower                                                       |
| Geometric mean             | (ref)                                                       | 1.01x slower                                                                |

Benchmark hidden because not significant (16): asyncio_tcp, async_tree_none_tg, xml_etree_parse, gc_traversal, pathlib, create_gc_cycles, scimark_lu, scimark_sor, go, dask, sympy_expand, crypto_pyaes, logging_format, chameleon, float, pycparser
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 69.36% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown