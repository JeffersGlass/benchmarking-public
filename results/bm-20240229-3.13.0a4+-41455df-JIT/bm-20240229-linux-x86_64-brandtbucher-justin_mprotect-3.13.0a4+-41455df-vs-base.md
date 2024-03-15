# Results vs. base

- fork: brandtbucher
- ref: justin_mprotect
- machine: linux-x86_64
- commit hash: 41455df
- commit date: 2024-02-29
- overall geometric mean: 1.00x faster
- HPT reliability: 80.83%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.92x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df |
|----------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| 2to3           | 276 ms                                                                 | 275 ms: 1.00x faster                                                    |
| chameleon      | 6.81 ms                                                                | 6.77 ms: 1.01x faster                                                   |
| tornado_http   | 96.9 ms                                                                | 96.3 ms: 1.01x faster                                                   |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                            |

Benchmark hidden because not significant (1): docutils

Benchmarks with tag 'asyncio':
==============================

Benchmark hidden because not significant (8): async_tree_io, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_none_tg, async_tree_memoization, async_tree_cpu_io_mixed, async_tree_memoization_tg, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df |
|----------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| nbody          | 94.5 ms                                                                | 93.1 ms: 1.01x faster                                                   |
| pidigits       | 187 ms                                                                 | 187 ms: 1.00x faster                                                    |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                            |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df |
|----------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| regex_v8       | 25.3 ms                                                                | 24.6 ms: 1.03x faster                                                   |
| regex_compile  | 142 ms                                                                 | 141 ms: 1.01x faster                                                    |
| regex_effbot   | 3.69 ms                                                                | 3.82 ms: 1.04x slower                                                   |
| regex_dna      | 222 ms                                                                 | 234 ms: 1.05x slower                                                    |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                            |

Benchmarks with tag 'serialize':
================================

| Benchmark          | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df |
|--------------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| unpickle_list      | 4.91 us                                                                | 4.70 us: 1.04x faster                                                   |
| unpickle           | 15.0 us                                                                | 14.5 us: 1.03x faster                                                   |
| xml_etree_generate | 86.5 ms                                                                | 85.7 ms: 1.01x faster                                                   |
| json_dumps         | 10.4 ms                                                                | 10.3 ms: 1.00x faster                                                   |
| json_loads         | 27.4 us                                                                | 27.6 us: 1.01x slower                                                   |
| tomli_loads        | 2.01 sec                                                               | 2.04 sec: 1.01x slower                                                  |
| pickle_dict        | 33.8 us                                                                | 34.4 us: 1.02x slower                                                   |
| pickle_pure_python | 297 us                                                                 | 305 us: 1.03x slower                                                    |
| pickle_list        | 4.89 us                                                                | 5.14 us: 1.05x slower                                                   |
| Geometric mean     | (ref)                                                                  | 1.00x slower                                                            |

Benchmark hidden because not significant (5): xml_etree_process, xml_etree_iterparse, xml_etree_parse, unpickle_pure_python, pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df |
|------------------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| python_startup_no_site | 11.0 ms                                                                | 9.85 ms: 1.11x faster                                                   |
| python_startup         | 12.3 ms                                                                | 11.2 ms: 1.10x faster                                                   |
| Geometric mean         | (ref)                                                                  | 1.11x faster                                                            |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df |
|-----------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| mako      | 11.0 ms                                                                | 10.8 ms: 1.02x faster                                                   |

All benchmarks:
===============

| Benchmark                | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df |
|--------------------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| bench_mp_pool            | 28.0 ms                                                                | 24.0 ms: 1.17x faster                                                   |
| python_startup_no_site   | 11.0 ms                                                                | 9.85 ms: 1.11x faster                                                   |
| python_startup           | 12.3 ms                                                                | 11.2 ms: 1.10x faster                                                   |
| gc_traversal             | 4.04 ms                                                                | 3.80 ms: 1.06x faster                                                   |
| unpickle_list            | 4.91 us                                                                | 4.70 us: 1.04x faster                                                   |
| pyflate                  | 489 ms                                                                 | 471 ms: 1.04x faster                                                    |
| unpickle                 | 15.0 us                                                                | 14.5 us: 1.03x faster                                                   |
| regex_v8                 | 25.3 ms                                                                | 24.6 ms: 1.03x faster                                                   |
| richards_super           | 53.1 ms                                                                | 51.7 ms: 1.03x faster                                                   |
| spectral_norm            | 113 ms                                                                 | 110 ms: 1.03x faster                                                    |
| typing_runtime_protocols | 112 us                                                                 | 110 us: 1.03x faster                                                    |
| mako                     | 11.0 ms                                                                | 10.8 ms: 1.02x faster                                                   |
| asyncio_tcp              | 486 ms                                                                 | 475 ms: 1.02x faster                                                    |
| chaos                    | 63.6 ms                                                                | 62.3 ms: 1.02x faster                                                   |
| async_generators         | 468 ms                                                                 | 460 ms: 1.02x faster                                                    |
| nbody                    | 94.5 ms                                                                | 93.1 ms: 1.01x faster                                                   |
| json                     | 5.12 ms                                                                | 5.05 ms: 1.01x faster                                                   |
| logging_format           | 6.23 us                                                                | 6.16 us: 1.01x faster                                                   |
| richards                 | 46.0 ms                                                                | 45.5 ms: 1.01x faster                                                   |
| xml_etree_generate       | 86.5 ms                                                                | 85.7 ms: 1.01x faster                                                   |
| deltablue                | 3.41 ms                                                                | 3.38 ms: 1.01x faster                                                   |
| chameleon                | 6.81 ms                                                                | 6.77 ms: 1.01x faster                                                   |
| tornado_http             | 96.9 ms                                                                | 96.3 ms: 1.01x faster                                                   |
| fannkuch                 | 394 ms                                                                 | 392 ms: 1.01x faster                                                    |
| hexiom                   | 7.05 ms                                                                | 7.01 ms: 1.01x faster                                                   |
| regex_compile            | 142 ms                                                                 | 141 ms: 1.01x faster                                                    |
| mdp                      | 2.77 sec                                                               | 2.76 sec: 1.01x faster                                                  |
| generators               | 29.5 ms                                                                | 29.3 ms: 1.01x faster                                                   |
| 2to3                     | 276 ms                                                                 | 275 ms: 1.00x faster                                                    |
| json_dumps               | 10.4 ms                                                                | 10.3 ms: 1.00x faster                                                   |
| bench_thread_pool        | 844 us                                                                 | 841 us: 1.00x faster                                                    |
| sqlglot_optimize         | 55.7 ms                                                                | 55.5 ms: 1.00x faster                                                   |
| pidigits                 | 187 ms                                                                 | 187 ms: 1.00x faster                                                    |
| deepcopy                 | 346 us                                                                 | 348 us: 1.00x slower                                                    |
| dulwich_log              | 68.4 ms                                                                | 68.7 ms: 1.00x slower                                                   |
| json_loads               | 27.4 us                                                                | 27.6 us: 1.01x slower                                                   |
| logging_simple           | 5.62 us                                                                | 5.65 us: 1.01x slower                                                   |
| sqlglot_parse            | 1.28 ms                                                                | 1.29 ms: 1.01x slower                                                   |
| scimark_fft              | 335 ms                                                                 | 337 ms: 1.01x slower                                                    |
| raytrace                 | 287 ms                                                                 | 289 ms: 1.01x slower                                                    |
| coverage                 | 95.4 ms                                                                | 96.4 ms: 1.01x slower                                                   |
| sqlite_synth             | 2.82 us                                                                | 2.85 us: 1.01x slower                                                   |
| create_gc_cycles         | 1.50 ms                                                                | 1.51 ms: 1.01x slower                                                   |
| tomli_loads              | 2.01 sec                                                               | 2.04 sec: 1.01x slower                                                  |
| scimark_lu               | 128 ms                                                                 | 129 ms: 1.01x slower                                                    |
| telco                    | 8.24 ms                                                                | 8.36 ms: 1.02x slower                                                   |
| coroutines               | 22.3 ms                                                                | 22.7 ms: 1.02x slower                                                   |
| scimark_monte_carlo      | 69.5 ms                                                                | 70.7 ms: 1.02x slower                                                   |
| pickle_dict              | 33.8 us                                                                | 34.4 us: 1.02x slower                                                   |
| logging_silent           | 99.5 ns                                                                | 102 ns: 1.03x slower                                                    |
| pickle_pure_python       | 297 us                                                                 | 305 us: 1.03x slower                                                    |
| pycparser                | 1.17 sec                                                               | 1.21 sec: 1.03x slower                                                  |
| scimark_sparse_mat_mult  | 4.68 ms                                                                | 4.85 ms: 1.04x slower                                                   |
| regex_effbot             | 3.69 ms                                                                | 3.82 ms: 1.04x slower                                                   |
| pickle_list              | 4.89 us                                                                | 5.14 us: 1.05x slower                                                   |
| regex_dna                | 222 ms                                                                 | 234 ms: 1.05x slower                                                    |
| unpack_sequence          | 86.3 ns                                                                | 96.7 ns: 1.12x slower                                                   |
| Geometric mean           | (ref)                                                                  | 1.00x faster                                                            |

Benchmark hidden because not significant (36): go, mypy2, sympy_sum, async_tree_io, xml_etree_process, docutils, async_tree_cpu_io_mixed_tg, async_tree_io_tg, asyncio_tcp_ssl, comprehensions, deepcopy_memo, sympy_integrate, sympy_str, async_tree_none_tg, sympy_expand, dask, xml_etree_iterparse, meteor_contest, asyncio_websockets, scimark_sor, xml_etree_parse, sqlglot_normalize, pprint_pformat, float, nqueens, crypto_pyaes, deepcopy_reduce, async_tree_memoization, async_tree_cpu_io_mixed, sqlglot_transpile, pathlib, async_tree_memoization_tg, pprint_safe_repr, unpickle_pure_python, async_tree_none, pickle


# HPT report

- Reliability score: 80.83% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.92x