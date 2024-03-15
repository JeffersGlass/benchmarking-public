
# Results vs. 3.12.0

- fork: python
- ref: 2f0ec7fa9450caeac820
- machine: linux-x86_64
- commit hash: 2f0ec7f
- commit date: 2023-12-17
- overall geometric mean: 1.01x slower
- HPT reliability: 92.27%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.88x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 295 ms: 1.03x slower                                                         |
| chameleon      | 7.23 ms                                                      | 7.40 ms: 1.02x slower                                                        |
| docutils       | 2.87 sec                                                     | 2.84 sec: 1.01x faster                                                       |
| tornado_http   | 121 ms                                                       | 118 ms: 1.03x faster                                                         |
| Geometric mean | (ref)                                                        | 1.00x slower                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark        | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none  | 452 ms                                                       | 432 ms: 1.05x faster                                                         |
| async_tree_io_tg | 1.05 sec                                                     | 1.07 sec: 1.02x slower                                                       |
| async_tree_io    | 1.04 sec                                                     | 1.07 sec: 1.03x slower                                                       |
| Geometric mean   | (ref)                                                        | 1.00x slower                                                                 |

Benchmark hidden because not significant (5): async_tree_cpu_io_mixed, async_tree_none_tg, async_tree_memoization, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 264 ms: 1.00x faster                                                         |
| float          | 76.6 ms                                                      | 78.8 ms: 1.03x slower                                                        |
| nbody          | 88.0 ms                                                      | 91.2 ms: 1.04x slower                                                        |
| Geometric mean | (ref)                                                        | 1.02x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 144 ms                                                       | 141 ms: 1.02x faster                                                         |
| regex_dna      | 239 ms                                                       | 256 ms: 1.07x slower                                                         |
| regex_v8       | 23.6 ms                                                      | 26.1 ms: 1.10x slower                                                        |
| Geometric mean | (ref)                                                        | 1.04x slower                                                                 |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_list          | 4.43 us                                                      | 4.19 us: 1.06x faster                                                        |
| pickle               | 10.5 us                                                      | 9.99 us: 1.05x faster                                                        |
| pickle_pure_python   | 318 us                                                       | 310 us: 1.03x faster                                                         |
| pickle_dict          | 32.5 us                                                      | 31.8 us: 1.02x faster                                                        |
| unpickle             | 14.8 us                                                      | 14.5 us: 1.02x faster                                                        |
| xml_etree_process    | 58.4 ms                                                      | 57.9 ms: 1.01x faster                                                        |
| xml_etree_generate   | 86.1 ms                                                      | 85.4 ms: 1.01x faster                                                        |
| unpickle_list        | 4.66 us                                                      | 4.69 us: 1.01x slower                                                        |
| json_dumps           | 10.2 ms                                                      | 10.5 ms: 1.02x slower                                                        |
| xml_etree_parse      | 144 ms                                                       | 148 ms: 1.03x slower                                                         |
| xml_etree_iterparse  | 103 ms                                                       | 106 ms: 1.03x slower                                                         |
| json_loads           | 24.4 us                                                      | 25.7 us: 1.05x slower                                                        |
| tomli_loads          | 2.16 sec                                                     | 2.28 sec: 1.06x slower                                                       |
| unpickle_pure_python | 210 us                                                       | 222 us: 1.06x slower                                                         |
| Geometric mean       | (ref)                                                        | 1.00x slower                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 12.6 ms: 1.08x slower                                                        |
| python_startup_no_site | 8.64 ms                                                      | 11.0 ms: 1.27x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.17x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 10.1 ms: 1.01x slower                                                        |

All benchmarks:
===============

| Benchmark                | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| comprehensions           | 21.9 us                                                      | 16.4 us: 1.33x faster                                                        |
| typing_runtime_protocols | 152 us                                                       | 116 us: 1.31x faster                                                         |
| raytrace                 | 298 ms                                                       | 259 ms: 1.15x faster                                                         |
| crypto_pyaes             | 80.3 ms                                                      | 70.3 ms: 1.14x faster                                                        |
| unpack_sequence          | 53.2 ns                                                      | 48.2 ns: 1.10x faster                                                        |
| async_generators         | 390 ms                                                       | 356 ms: 1.10x faster                                                         |
| sympy_sum                | 162 ms                                                       | 151 ms: 1.07x faster                                                         |
| chaos                    | 64.0 ms                                                      | 60.3 ms: 1.06x faster                                                        |
| pickle_list              | 4.43 us                                                      | 4.19 us: 1.06x faster                                                        |
| scimark_monte_carlo      | 69.0 ms                                                      | 65.3 ms: 1.06x faster                                                        |
| pickle                   | 10.5 us                                                      | 9.99 us: 1.05x faster                                                        |
| generators               | 37.4 ms                                                      | 35.6 ms: 1.05x faster                                                        |
| async_tree_none          | 452 ms                                                       | 432 ms: 1.05x faster                                                         |
| bench_mp_pool            | 4.76 ms                                                      | 4.57 ms: 1.04x faster                                                        |
| sympy_integrate          | 23.9 ms                                                      | 23.1 ms: 1.04x faster                                                        |
| sympy_str                | 302 ms                                                       | 293 ms: 1.03x faster                                                         |
| asyncio_tcp              | 378 ms                                                       | 367 ms: 1.03x faster                                                         |
| mdp                      | 2.57 sec                                                     | 2.49 sec: 1.03x faster                                                       |
| coroutines               | 23.0 ms                                                      | 22.3 ms: 1.03x faster                                                        |
| logging_format           | 7.48 us                                                      | 7.27 us: 1.03x faster                                                        |
| nqueens                  | 89.9 ms                                                      | 87.4 ms: 1.03x faster                                                        |
| tornado_http             | 121 ms                                                       | 118 ms: 1.03x faster                                                         |
| pickle_pure_python       | 318 us                                                       | 310 us: 1.03x faster                                                         |
| sqlite_synth             | 2.77 us                                                      | 2.71 us: 1.02x faster                                                        |
| regex_compile            | 144 ms                                                       | 141 ms: 1.02x faster                                                         |
| logging_simple           | 6.71 us                                                      | 6.56 us: 1.02x faster                                                        |
| pickle_dict              | 32.5 us                                                      | 31.8 us: 1.02x faster                                                        |
| deepcopy_reduce          | 3.37 us                                                      | 3.30 us: 1.02x faster                                                        |
| unpickle                 | 14.8 us                                                      | 14.5 us: 1.02x faster                                                        |
| pprint_pformat           | 1.65 sec                                                     | 1.64 sec: 1.01x faster                                                       |
| docutils                 | 2.87 sec                                                     | 2.84 sec: 1.01x faster                                                       |
| xml_etree_process        | 58.4 ms                                                      | 57.9 ms: 1.01x faster                                                        |
| asyncio_tcp_ssl          | 1.59 sec                                                     | 1.57 sec: 1.01x faster                                                       |
| xml_etree_generate       | 86.1 ms                                                      | 85.4 ms: 1.01x faster                                                        |
| scimark_sparse_mat_mult  | 4.21 ms                                                      | 4.18 ms: 1.01x faster                                                        |
| spectral_norm            | 91.6 ms                                                      | 91.2 ms: 1.00x faster                                                        |
| meteor_contest           | 128 ms                                                       | 128 ms: 1.00x faster                                                         |
| pidigits                 | 265 ms                                                       | 264 ms: 1.00x faster                                                         |
| deepcopy_memo            | 36.8 us                                                      | 36.9 us: 1.00x slower                                                        |
| pathlib                  | 18.9 ms                                                      | 19.0 ms: 1.01x slower                                                        |
| unpickle_list            | 4.66 us                                                      | 4.69 us: 1.01x slower                                                        |
| sqlglot_parse            | 1.38 ms                                                      | 1.39 ms: 1.01x slower                                                        |
| sqlglot_transpile        | 1.78 ms                                                      | 1.80 ms: 1.01x slower                                                        |
| mako                     | 10.0 ms                                                      | 10.1 ms: 1.01x slower                                                        |
| scimark_fft              | 301 ms                                                       | 305 ms: 1.01x slower                                                         |
| async_tree_io_tg         | 1.05 sec                                                     | 1.07 sec: 1.02x slower                                                       |
| create_gc_cycles         | 1.59 ms                                                      | 1.62 ms: 1.02x slower                                                        |
| dask                     | 392 ms                                                       | 400 ms: 1.02x slower                                                         |
| logging_silent           | 94.4 ns                                                      | 96.5 ns: 1.02x slower                                                        |
| json_dumps               | 10.2 ms                                                      | 10.5 ms: 1.02x slower                                                        |
| sqlglot_optimize         | 57.5 ms                                                      | 58.8 ms: 1.02x slower                                                        |
| chameleon                | 7.23 ms                                                      | 7.40 ms: 1.02x slower                                                        |
| gc_traversal             | 3.48 ms                                                      | 3.56 ms: 1.02x slower                                                        |
| dulwich_log              | 65.4 ms                                                      | 67.2 ms: 1.03x slower                                                        |
| xml_etree_parse          | 144 ms                                                       | 148 ms: 1.03x slower                                                         |
| float                    | 76.6 ms                                                      | 78.8 ms: 1.03x slower                                                        |
| async_tree_io            | 1.04 sec                                                     | 1.07 sec: 1.03x slower                                                       |
| json                     | 5.12 ms                                                      | 5.29 ms: 1.03x slower                                                        |
| xml_etree_iterparse      | 103 ms                                                       | 106 ms: 1.03x slower                                                         |
| 2to3                     | 285 ms                                                       | 295 ms: 1.03x slower                                                         |
| nbody                    | 88.0 ms                                                      | 91.2 ms: 1.04x slower                                                        |
| sympy_expand             | 484 ms                                                       | 502 ms: 1.04x slower                                                         |
| json_loads               | 24.4 us                                                      | 25.7 us: 1.05x slower                                                        |
| tomli_loads              | 2.16 sec                                                     | 2.28 sec: 1.06x slower                                                       |
| unpickle_pure_python     | 210 us                                                       | 222 us: 1.06x slower                                                         |
| hexiom                   | 5.96 ms                                                      | 6.35 ms: 1.07x slower                                                        |
| pycparser                | 1.23 sec                                                     | 1.32 sec: 1.07x slower                                                       |
| regex_dna                | 239 ms                                                       | 256 ms: 1.07x slower                                                         |
| python_startup           | 11.6 ms                                                      | 12.6 ms: 1.08x slower                                                        |
| deltablue                | 3.24 ms                                                      | 3.54 ms: 1.09x slower                                                        |
| regex_v8                 | 23.6 ms                                                      | 26.1 ms: 1.10x slower                                                        |
| fannkuch                 | 350 ms                                                       | 395 ms: 1.13x slower                                                         |
| go                       | 150 ms                                                       | 169 ms: 1.13x slower                                                         |
| pyflate                  | 439 ms                                                       | 508 ms: 1.16x slower                                                         |
| coverage                 | 66.7 ms                                                      | 78.0 ms: 1.17x slower                                                        |
| telco                    | 6.96 ms                                                      | 8.15 ms: 1.17x slower                                                        |
| richards_super           | 51.3 ms                                                      | 61.2 ms: 1.19x slower                                                        |
| richards                 | 45.7 ms                                                      | 54.8 ms: 1.20x slower                                                        |
| python_startup_no_site   | 8.64 ms                                                      | 11.0 ms: 1.27x slower                                                        |
| scimark_sor              | 109 ms                                                       | 144 ms: 1.32x slower                                                         |
| Geometric mean           | (ref)                                                        | 1.01x slower                                                                 |

Benchmark hidden because not significant (13): scimark_lu, bench_thread_pool, pprint_safe_repr, async_tree_cpu_io_mixed, async_tree_none_tg, async_tree_memoization, async_tree_cpu_io_mixed_tg, deepcopy, sqlglot_normalize, asyncio_websockets, async_tree_memoization_tg, regex_effbot, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 92.27% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.88x