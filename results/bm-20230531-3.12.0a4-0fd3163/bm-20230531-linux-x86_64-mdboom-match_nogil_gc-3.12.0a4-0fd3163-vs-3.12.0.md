
# Results vs. 3.12.0

- fork: mdboom
- ref: match_nogil_gc
- machine: linux-x86_64
- commit hash: 0fd3163
- commit date: 2023-05-31
- overall geometric mean: 1.10x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.06x faster
- Memory change: 1.11x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230531-linux-x86_64-mdboom-match_nogil_gc-3.12.0a4-0fd3163 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 245 ms: 1.12x faster                                            |
| chameleon      | 7.41 ms                                                | 6.37 ms: 1.16x faster                                           |
| docutils       | 2.77 sec                                               | 2.15 sec: 1.29x faster                                          |
| Geometric mean | (ref)                                                  | 1.19x faster                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230531-linux-x86_64-mdboom-match_nogil_gc-3.12.0a4-0fd3163 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_io           | 1.16 sec                                               | 534 ms: 2.16x faster                                            |
| async_tree_memoization  | 578 ms                                                 | 315 ms: 1.83x faster                                            |
| async_tree_none         | 472 ms                                                 | 260 ms: 1.81x faster                                            |
| async_tree_cpu_io_mixed | 726 ms                                                 | 469 ms: 1.55x faster                                            |
| Geometric mean          | (ref)                                                  | 1.83x faster                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230531-linux-x86_64-mdboom-match_nogil_gc-3.12.0a4-0fd3163 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| float          | 84.7 ms                                                | 60.7 ms: 1.40x faster                                           |
| nbody          | 97.0 ms                                                | 92.3 ms: 1.05x faster                                           |
| pidigits       | 187 ms                                                 | 189 ms: 1.01x slower                                            |
| Geometric mean | (ref)                                                  | 1.13x faster                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230531-linux-x86_64-mdboom-match_nogil_gc-3.12.0a4-0fd3163 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 131 ms: 1.13x faster                                            |
| regex_v8       | 23.1 ms                                                | 22.1 ms: 1.05x faster                                           |
| regex_effbot   | 3.61 ms                                                | 3.46 ms: 1.04x faster                                           |
| regex_dna      | 212 ms                                                 | 210 ms: 1.01x faster                                            |
| Geometric mean | (ref)                                                  | 1.06x faster                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230531-linux-x86_64-mdboom-match_nogil_gc-3.12.0a4-0fd3163 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| xml_etree_iterparse  | 107 ms                                                 | 80.9 ms: 1.32x faster                                           |
| xml_etree_parse      | 159 ms                                                 | 122 ms: 1.31x faster                                            |
| pickle_list          | 5.08 us                                                | 4.05 us: 1.26x faster                                           |
| unpickle             | 15.9 us                                                | 13.0 us: 1.22x faster                                           |
| xml_etree_generate   | 89.2 ms                                                | 73.4 ms: 1.22x faster                                           |
| json_loads           | 28.5 us                                                | 23.7 us: 1.20x faster                                           |
| xml_etree_process    | 61.7 ms                                                | 51.6 ms: 1.20x faster                                           |
| tomli_loads          | 2.33 sec                                               | 1.98 sec: 1.18x faster                                          |
| unpickle_pure_python | 230 us                                                 | 198 us: 1.16x faster                                            |
| pickle_pure_python   | 324 us                                                 | 282 us: 1.15x faster                                            |
| pickle               | 11.6 us                                                | 10.2 us: 1.14x faster                                           |
| pickle_dict          | 35.5 us                                                | 31.2 us: 1.14x faster                                           |
| json_dumps           | 10.4 ms                                                | 9.55 ms: 1.09x faster                                           |
| unpickle_list        | 5.29 us                                                | 4.95 us: 1.07x faster                                           |
| Geometric mean       | (ref)                                                  | 1.19x faster                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230531-linux-x86_64-mdboom-match_nogil_gc-3.12.0a4-0fd3163 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup_no_site | 6.94 ms                                                | 5.93 ms: 1.17x faster                                           |
| python_startup         | 9.55 ms                                                | 8.24 ms: 1.16x faster                                           |
| Geometric mean         | (ref)                                                  | 1.17x faster                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230531-linux-x86_64-mdboom-match_nogil_gc-3.12.0a4-0fd3163 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| mako            | 11.9 ms                                                | 9.69 ms: 1.23x faster                                           |
| django_template | 34.6 ms                                                | 32.9 ms: 1.05x faster                                           |
| Geometric mean  | (ref)                                                  | 1.14x faster                                                    |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230531-linux-x86_64-mdboom-match_nogil_gc-3.12.0a4-0fd3163 |
|--------------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_io            | 1.16 sec                                               | 534 ms: 2.16x faster                                            |
| async_tree_memoization   | 578 ms                                                 | 315 ms: 1.83x faster                                            |
| async_tree_none          | 472 ms                                                 | 260 ms: 1.81x faster                                            |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 469 ms: 1.55x faster                                            |
| float                    | 84.7 ms                                                | 60.7 ms: 1.40x faster                                           |
| async_generators         | 463 ms                                                 | 338 ms: 1.37x faster                                            |
| xml_etree_iterparse      | 107 ms                                                 | 80.9 ms: 1.32x faster                                           |
| xml_etree_parse          | 159 ms                                                 | 122 ms: 1.31x faster                                            |
| docutils                 | 2.77 sec                                               | 2.15 sec: 1.29x faster                                          |
| pickle_list              | 5.08 us                                                | 4.05 us: 1.26x faster                                           |
| unpack_sequence          | 54.0 ns                                                | 43.6 ns: 1.24x faster                                           |
| scimark_fft              | 382 ms                                                 | 309 ms: 1.24x faster                                            |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 4.12 ms: 1.23x faster                                           |
| mako                     | 11.9 ms                                                | 9.69 ms: 1.23x faster                                           |
| unpickle                 | 15.9 us                                                | 13.0 us: 1.22x faster                                           |
| xml_etree_generate       | 89.2 ms                                                | 73.4 ms: 1.22x faster                                           |
| scimark_sor              | 129 ms                                                 | 106 ms: 1.21x faster                                            |
| spectral_norm            | 115 ms                                                 | 94.7 ms: 1.21x faster                                           |
| deepcopy_memo            | 40.7 us                                                | 33.8 us: 1.20x faster                                           |
| json_loads               | 28.5 us                                                | 23.7 us: 1.20x faster                                           |
| pyflate                  | 482 ms                                                 | 403 ms: 1.20x faster                                            |
| xml_etree_process        | 61.7 ms                                                | 51.6 ms: 1.20x faster                                           |
| deltablue                | 3.72 ms                                                | 3.11 ms: 1.19x faster                                           |
| tomli_loads              | 2.33 sec                                               | 1.98 sec: 1.18x faster                                          |
| dask                     | 372 ms                                                 | 317 ms: 1.17x faster                                            |
| python_startup_no_site   | 6.94 ms                                                | 5.93 ms: 1.17x faster                                           |
| logging_silent           | 104 ns                                                 | 89.6 ns: 1.17x faster                                           |
| chameleon                | 7.41 ms                                                | 6.37 ms: 1.16x faster                                           |
| unpickle_pure_python     | 230 us                                                 | 198 us: 1.16x faster                                            |
| python_startup           | 9.55 ms                                                | 8.24 ms: 1.16x faster                                           |
| scimark_monte_carlo      | 75.1 ms                                                | 65.2 ms: 1.15x faster                                           |
| pickle_pure_python       | 324 us                                                 | 282 us: 1.15x faster                                            |
| pprint_safe_repr         | 776 ms                                                 | 676 ms: 1.15x faster                                            |
| json                     | 5.26 ms                                                | 4.59 ms: 1.15x faster                                           |
| pickle                   | 11.6 us                                                | 10.2 us: 1.14x faster                                           |
| pickle_dict              | 35.5 us                                                | 31.2 us: 1.14x faster                                           |
| fannkuch                 | 417 ms                                                 | 368 ms: 1.13x faster                                            |
| regex_compile            | 148 ms                                                 | 131 ms: 1.13x faster                                            |
| deepcopy_reduce          | 3.35 us                                                | 2.97 us: 1.13x faster                                           |
| pprint_pformat           | 1.57 sec                                               | 1.39 sec: 1.12x faster                                          |
| gc_traversal             | 3.79 ms                                                | 3.38 ms: 1.12x faster                                           |
| logging_format           | 7.23 us                                                | 6.44 us: 1.12x faster                                           |
| scimark_lu               | 118 ms                                                 | 105 ms: 1.12x faster                                            |
| 2to3                     | 274 ms                                                 | 245 ms: 1.12x faster                                            |
| deepcopy                 | 371 us                                                 | 332 us: 1.12x faster                                            |
| pycparser                | 1.18 sec                                               | 1.06 sec: 1.12x faster                                          |
| logging_simple           | 6.46 us                                                | 5.80 us: 1.11x faster                                           |
| crypto_pyaes             | 81.9 ms                                                | 73.7 ms: 1.11x faster                                           |
| raytrace                 | 312 ms                                                 | 286 ms: 1.09x faster                                            |
| telco                    | 7.10 ms                                                | 6.52 ms: 1.09x faster                                           |
| json_dumps               | 10.4 ms                                                | 9.55 ms: 1.09x faster                                           |
| dulwich_log              | 68.5 ms                                                | 63.5 ms: 1.08x faster                                           |
| richards                 | 45.8 ms                                                | 42.5 ms: 1.08x faster                                           |
| nqueens                  | 83.3 ms                                                | 77.6 ms: 1.07x faster                                           |
| unpickle_list            | 5.29 us                                                | 4.95 us: 1.07x faster                                           |
| sympy_str                | 300 ms                                                 | 281 ms: 1.07x faster                                            |
| pathlib                  | 19.3 ms                                                | 18.2 ms: 1.07x faster                                           |
| bench_thread_pool        | 842 us                                                 | 792 us: 1.06x faster                                            |
| sqlglot_optimize         | 54.8 ms                                                | 51.6 ms: 1.06x faster                                           |
| mdp                      | 2.63 sec                                               | 2.48 sec: 1.06x faster                                          |
| sympy_integrate          | 21.4 ms                                                | 20.2 ms: 1.06x faster                                           |
| sqlite_synth             | 2.83 us                                                | 2.67 us: 1.06x faster                                           |
| hexiom                   | 6.41 ms                                                | 6.06 ms: 1.06x faster                                           |
| django_template          | 34.6 ms                                                | 32.9 ms: 1.05x faster                                           |
| sympy_expand             | 478 ms                                                 | 455 ms: 1.05x faster                                            |
| nbody                    | 97.0 ms                                                | 92.3 ms: 1.05x faster                                           |
| regex_v8                 | 23.1 ms                                                | 22.1 ms: 1.05x faster                                           |
| regex_effbot             | 3.61 ms                                                | 3.46 ms: 1.04x faster                                           |
| sympy_sum                | 169 ms                                                 | 163 ms: 1.04x faster                                            |
| meteor_contest           | 112 ms                                                 | 109 ms: 1.03x faster                                            |
| sqlglot_normalize        | 110 ms                                                 | 108 ms: 1.02x faster                                            |
| go                       | 139 ms                                                 | 137 ms: 1.02x faster                                            |
| sqlglot_transpile        | 1.68 ms                                                | 1.67 ms: 1.01x faster                                           |
| create_gc_cycles         | 1.48 ms                                                | 1.46 ms: 1.01x faster                                           |
| regex_dna                | 212 ms                                                 | 210 ms: 1.01x faster                                            |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.79 sec: 1.00x slower                                          |
| pidigits                 | 187 ms                                                 | 189 ms: 1.01x slower                                            |
| sqlglot_parse            | 1.36 ms                                                | 1.38 ms: 1.01x slower                                           |
| richards_super           | 51.5 ms                                                | 52.9 ms: 1.03x slower                                           |
| chaos                    | 67.0 ms                                                | 68.8 ms: 1.03x slower                                           |
| asyncio_tcp              | 491 ms                                                 | 511 ms: 1.04x slower                                            |
| comprehensions           | 21.8 us                                                | 23.9 us: 1.10x slower                                           |
| coroutines               | 23.2 ms                                                | 26.1 ms: 1.12x slower                                           |
| coverage                 | 72.7 ms                                                | 99.2 ms: 1.37x slower                                           |
| generators               | 31.2 ms                                                | 79.1 ms: 2.53x slower                                           |
| typing_runtime_protocols | 158 us                                                 | 463 us: 2.94x slower                                            |
| Geometric mean           | (ref)                                                  | 1.10x faster                                                    |

Benchmark hidden because not significant (1): bench_mp_pool
Ignored benchmarks (11) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, gunicorn, mypy2, sqlalchemy_declarative, sqlalchemy_imperative, tornado_http
Ignored benchmarks (5) of results/bm-20230531-3.12.0a4-0fd3163/bm-20230531-linux-x86_64-mdboom-match_nogil_gc-3.12.0a4-0fd3163.json: djangocms, genshi_text, genshi_xml, html5lib, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.09x
- 95% likely to have a speedup of 1.08x
- 99% likely to have a speedup of 1.06x


# Memory

- memory change: 1.11x