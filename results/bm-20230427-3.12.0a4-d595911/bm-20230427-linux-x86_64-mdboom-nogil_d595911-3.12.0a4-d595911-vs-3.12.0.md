
# Results vs. 3.12.0

- fork: mdboom
- ref: nogil_d595911
- machine: linux-x86_64
- commit hash: d595911
- commit date: 2023-04-27
- overall geometric mean: 1.02x slower \*
- HPT reliability: 95.45%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.27x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230427-linux-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 287 ms: 1.05x slower                                           |
| chameleon      | 7.41 ms                                                | 7.73 ms: 1.04x slower                                          |
| Geometric mean | (ref)                                                  | 1.04x slower                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230427-linux-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_io           | 1.16 sec                                               | 580 ms: 1.99x faster                                           |
| async_tree_none         | 472 ms                                                 | 289 ms: 1.63x faster                                           |
| async_tree_memoization  | 578 ms                                                 | 362 ms: 1.60x faster                                           |
| async_tree_cpu_io_mixed | 726 ms                                                 | 514 ms: 1.41x faster                                           |
| Geometric mean          | (ref)                                                  | 1.65x faster                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230427-linux-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| float          | 84.7 ms                                                | 67.0 ms: 1.26x faster                                          |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x faster                                           |
| nbody          | 97.0 ms                                                | 103 ms: 1.07x slower                                           |
| Geometric mean | (ref)                                                  | 1.06x faster                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230427-linux-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_v8       | 23.1 ms                                                | 22.0 ms: 1.05x faster                                          |
| regex_effbot   | 3.61 ms                                                | 3.52 ms: 1.03x faster                                          |
| regex_compile  | 148 ms                                                 | 151 ms: 1.02x slower                                           |
| regex_dna      | 212 ms                                                 | 219 ms: 1.03x slower                                           |
| Geometric mean | (ref)                                                  | 1.01x faster                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230427-linux-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| xml_etree_parse      | 159 ms                                                 | 133 ms: 1.20x faster                                           |
| pickle_dict          | 35.5 us                                                | 29.9 us: 1.19x faster                                          |
| pickle               | 11.6 us                                                | 9.82 us: 1.18x faster                                          |
| pickle_list          | 5.08 us                                                | 4.47 us: 1.14x faster                                          |
| xml_etree_generate   | 89.2 ms                                                | 83.3 ms: 1.07x faster                                          |
| unpickle             | 15.9 us                                                | 15.3 us: 1.04x faster                                          |
| pickle_pure_python   | 324 us                                                 | 315 us: 1.03x faster                                           |
| xml_etree_process    | 61.7 ms                                                | 60.5 ms: 1.02x faster                                          |
| json_loads           | 28.5 us                                                | 28.1 us: 1.01x faster                                          |
| unpickle_list        | 5.29 us                                                | 5.35 us: 1.01x slower                                          |
| tomli_loads          | 2.33 sec                                               | 2.39 sec: 1.03x slower                                         |
| unpickle_pure_python | 230 us                                                 | 237 us: 1.03x slower                                           |
| xml_etree_iterparse  | 107 ms                                                 | 121 ms: 1.13x slower                                           |
| Geometric mean       | (ref)                                                  | 1.04x faster                                                   |

Benchmark hidden because not significant (1): json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230427-linux-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup_no_site | 6.94 ms                                                | 6.70 ms: 1.04x faster                                          |
| python_startup         | 9.55 ms                                                | 9.33 ms: 1.02x faster                                          |
| Geometric mean         | (ref)                                                  | 1.03x faster                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230427-linux-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 13.6 ms: 1.14x slower                                          |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230427-linux-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_io            | 1.16 sec                                               | 580 ms: 1.99x faster                                           |
| async_tree_none          | 472 ms                                                 | 289 ms: 1.63x faster                                           |
| async_tree_memoization   | 578 ms                                                 | 362 ms: 1.60x faster                                           |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 514 ms: 1.41x faster                                           |
| float                    | 84.7 ms                                                | 67.0 ms: 1.26x faster                                          |
| async_generators         | 463 ms                                                 | 369 ms: 1.25x faster                                           |
| gc_traversal             | 3.79 ms                                                | 3.11 ms: 1.22x faster                                          |
| xml_etree_parse          | 159 ms                                                 | 133 ms: 1.20x faster                                           |
| pickle_dict              | 35.5 us                                                | 29.9 us: 1.19x faster                                          |
| pickle                   | 11.6 us                                                | 9.82 us: 1.18x faster                                          |
| pickle_list              | 5.08 us                                                | 4.47 us: 1.14x faster                                          |
| xml_etree_generate       | 89.2 ms                                                | 83.3 ms: 1.07x faster                                          |
| regex_v8                 | 23.1 ms                                                | 22.0 ms: 1.05x faster                                          |
| telco                    | 7.10 ms                                                | 6.81 ms: 1.04x faster                                          |
| json                     | 5.26 ms                                                | 5.05 ms: 1.04x faster                                          |
| unpack_sequence          | 54.0 ns                                                | 51.8 ns: 1.04x faster                                          |
| python_startup_no_site   | 6.94 ms                                                | 6.70 ms: 1.04x faster                                          |
| unpickle                 | 15.9 us                                                | 15.3 us: 1.04x faster                                          |
| pycparser                | 1.18 sec                                               | 1.14 sec: 1.03x faster                                         |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 4.91 ms: 1.03x faster                                          |
| scimark_sor              | 129 ms                                                 | 125 ms: 1.03x faster                                           |
| pickle_pure_python       | 324 us                                                 | 315 us: 1.03x faster                                           |
| regex_effbot             | 3.61 ms                                                | 3.52 ms: 1.03x faster                                          |
| python_startup           | 9.55 ms                                                | 9.33 ms: 1.02x faster                                          |
| spectral_norm            | 115 ms                                                 | 112 ms: 1.02x faster                                           |
| scimark_fft              | 382 ms                                                 | 374 ms: 1.02x faster                                           |
| xml_etree_process        | 61.7 ms                                                | 60.5 ms: 1.02x faster                                          |
| deepcopy_memo            | 40.7 us                                                | 40.1 us: 1.02x faster                                          |
| pyflate                  | 482 ms                                                 | 475 ms: 1.02x faster                                           |
| json_loads               | 28.5 us                                                | 28.1 us: 1.01x faster                                          |
| deltablue                | 3.72 ms                                                | 3.67 ms: 1.01x faster                                          |
| deepcopy_reduce          | 3.35 us                                                | 3.32 us: 1.01x faster                                          |
| pprint_safe_repr         | 776 ms                                                 | 772 ms: 1.00x faster                                           |
| pidigits                 | 187 ms                                                 | 187 ms: 1.00x faster                                           |
| deepcopy                 | 371 us                                                 | 373 us: 1.01x slower                                           |
| pathlib                  | 19.3 ms                                                | 19.5 ms: 1.01x slower                                          |
| sqlglot_optimize         | 54.8 ms                                                | 55.4 ms: 1.01x slower                                          |
| unpickle_list            | 5.29 us                                                | 5.35 us: 1.01x slower                                          |
| scimark_monte_carlo      | 75.1 ms                                                | 76.1 ms: 1.01x slower                                          |
| create_gc_cycles         | 1.48 ms                                                | 1.50 ms: 1.02x slower                                          |
| pprint_pformat           | 1.57 sec                                               | 1.60 sec: 1.02x slower                                         |
| regex_compile            | 148 ms                                                 | 151 ms: 1.02x slower                                           |
| tomli_loads              | 2.33 sec                                               | 2.39 sec: 1.03x slower                                         |
| unpickle_pure_python     | 230 us                                                 | 237 us: 1.03x slower                                           |
| sqlglot_normalize        | 110 ms                                                 | 114 ms: 1.03x slower                                           |
| regex_dna                | 212 ms                                                 | 219 ms: 1.03x slower                                           |
| fannkuch                 | 417 ms                                                 | 433 ms: 1.04x slower                                           |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.85 sec: 1.04x slower                                         |
| nqueens                  | 83.3 ms                                                | 86.4 ms: 1.04x slower                                          |
| logging_silent           | 104 ns                                                 | 109 ns: 1.04x slower                                           |
| chameleon                | 7.41 ms                                                | 7.73 ms: 1.04x slower                                          |
| 2to3                     | 274 ms                                                 | 287 ms: 1.05x slower                                           |
| go                       | 139 ms                                                 | 147 ms: 1.06x slower                                           |
| scimark_lu               | 118 ms                                                 | 125 ms: 1.06x slower                                           |
| sympy_integrate          | 21.4 ms                                                | 22.8 ms: 1.06x slower                                          |
| richards                 | 45.8 ms                                                | 48.8 ms: 1.06x slower                                          |
| nbody                    | 97.0 ms                                                | 103 ms: 1.07x slower                                           |
| logging_simple           | 6.46 us                                                | 6.89 us: 1.07x slower                                          |
| hexiom                   | 6.41 ms                                                | 6.85 ms: 1.07x slower                                          |
| logging_format           | 7.23 us                                                | 7.75 us: 1.07x slower                                          |
| coroutines               | 23.2 ms                                                | 25.1 ms: 1.08x slower                                          |
| asyncio_tcp              | 491 ms                                                 | 535 ms: 1.09x slower                                           |
| sympy_str                | 300 ms                                                 | 329 ms: 1.10x slower                                           |
| raytrace                 | 312 ms                                                 | 346 ms: 1.11x slower                                           |
| sympy_expand             | 478 ms                                                 | 533 ms: 1.11x slower                                           |
| mdp                      | 2.63 sec                                               | 2.94 sec: 1.12x slower                                         |
| meteor_contest           | 112 ms                                                 | 126 ms: 1.12x slower                                           |
| xml_etree_iterparse      | 107 ms                                                 | 121 ms: 1.13x slower                                           |
| sympy_sum                | 169 ms                                                 | 192 ms: 1.13x slower                                           |
| mako                     | 11.9 ms                                                | 13.6 ms: 1.14x slower                                          |
| chaos                    | 67.0 ms                                                | 76.6 ms: 1.14x slower                                          |
| sqlglot_transpile        | 1.68 ms                                                | 1.97 ms: 1.17x slower                                          |
| richards_super           | 51.5 ms                                                | 60.2 ms: 1.17x slower                                          |
| sqlite_synth             | 2.83 us                                                | 3.33 us: 1.17x slower                                          |
| sqlglot_parse            | 1.36 ms                                                | 1.67 ms: 1.23x slower                                          |
| comprehensions           | 21.8 us                                                | 26.8 us: 1.23x slower                                          |
| bench_thread_pool        | 842 us                                                 | 1.64 ms: 1.95x slower                                          |
| generators               | 31.2 ms                                                | 78.3 ms: 2.51x slower                                          |
| typing_runtime_protocols | 158 us                                                 | 535 us: 3.39x slower                                           |
| Geometric mean           | (ref)                                                  | 1.02x slower                                                   |

Benchmark hidden because not significant (3): crypto_pyaes, bench_mp_pool, json_dumps
Ignored benchmarks (16) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, coverage, dask, django_template, docutils, dulwich_log, gunicorn, mypy2, sqlalchemy_declarative, sqlalchemy_imperative, tornado_http
Ignored benchmarks (3) of results/bm-20230427-3.12.0a4-d595911/bm-20230427-linux-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911.json: genshi_text, genshi_xml, html5lib


# HPT report

- Reliability score: 95.45% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.27x