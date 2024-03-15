
# Results vs. 3.10.4

- fork: mdboom
- ref: nogil_d595911
- machine: linux-x86_64
- commit hash: d595911
- commit date: 2023-04-27
- overall geometric mean: 1.28x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.22x faster
- Memory change: 1.45x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230427-linux-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 287 ms: 1.22x faster                                           |
| chameleon      | 9.68 ms                                                | 7.73 ms: 1.25x faster                                          |
| html5lib       | 88.9 ms                                                | 68.3 ms: 1.30x faster                                          |
| Geometric mean | (ref)                                                  | 1.26x faster                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230427-linux-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_io           | 1.77 sec                                               | 580 ms: 3.05x faster                                           |
| async_tree_none         | 728 ms                                                 | 289 ms: 2.52x faster                                           |
| async_tree_memoization  | 870 ms                                                 | 362 ms: 2.40x faster                                           |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 514 ms: 1.98x faster                                           |
| Geometric mean          | (ref)                                                  | 2.46x faster                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230427-linux-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| float          | 117 ms                                                 | 67.0 ms: 1.75x faster                                          |
| nbody          | 154 ms                                                 | 103 ms: 1.48x faster                                           |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                           |
| Geometric mean | (ref)                                                  | 1.38x faster                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230427-linux-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_v8       | 27.8 ms                                                | 22.0 ms: 1.26x faster                                          |
| regex_compile  | 188 ms                                                 | 151 ms: 1.25x faster                                           |
| regex_dna      | 227 ms                                                 | 219 ms: 1.03x faster                                           |
| regex_effbot   | 3.63 ms                                                | 3.52 ms: 1.03x faster                                          |
| Geometric mean | (ref)                                                  | 1.14x faster                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230427-linux-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 315 us: 1.54x faster                                           |
| unpickle_pure_python | 331 us                                                 | 237 us: 1.40x faster                                           |
| json_dumps           | 14.2 ms                                                | 10.5 ms: 1.36x faster                                          |
| tomli_loads          | 3.14 sec                                               | 2.39 sec: 1.31x faster                                         |
| xml_etree_process    | 79.1 ms                                                | 60.5 ms: 1.31x faster                                          |
| xml_etree_parse      | 168 ms                                                 | 133 ms: 1.26x faster                                           |
| xml_etree_generate   | 99.4 ms                                                | 83.3 ms: 1.19x faster                                          |
| pickle_list          | 5.08 us                                                | 4.47 us: 1.13x faster                                          |
| json_loads           | 31.2 us                                                | 28.1 us: 1.11x faster                                          |
| pickle               | 10.7 us                                                | 9.82 us: 1.09x faster                                          |
| pickle_dict          | 29.6 us                                                | 29.9 us: 1.01x slower                                          |
| unpickle_list        | 5.20 us                                                | 5.35 us: 1.03x slower                                          |
| xml_etree_iterparse  | 115 ms                                                 | 121 ms: 1.04x slower                                           |
| unpickle             | 14.4 us                                                | 15.3 us: 1.06x slower                                          |
| Geometric mean       | (ref)                                                  | 1.17x faster                                                   |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230427-linux-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 9.33 ms: 1.56x faster                                          |
| python_startup_no_site | 5.93 ms                                                | 6.70 ms: 1.13x slower                                          |
| Geometric mean         | (ref)                                                  | 1.18x faster                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230427-linux-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| genshi_text    | 31.8 ms                                                | 24.3 ms: 1.31x faster                                          |
| genshi_xml     | 66.0 ms                                                | 51.9 ms: 1.27x faster                                          |
| mako           | 16.3 ms                                                | 13.6 ms: 1.20x faster                                          |
| Geometric mean | (ref)                                                  | 1.26x faster                                                   |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230427-linux-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_io            | 1.77 sec                                               | 580 ms: 3.05x faster                                           |
| async_tree_none          | 728 ms                                                 | 289 ms: 2.52x faster                                           |
| async_tree_memoization   | 870 ms                                                 | 362 ms: 2.40x faster                                           |
| deltablue                | 7.91 ms                                                | 3.67 ms: 2.16x faster                                          |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 514 ms: 1.98x faster                                           |
| scimark_sor              | 220 ms                                                 | 125 ms: 1.75x faster                                           |
| float                    | 117 ms                                                 | 67.0 ms: 1.75x faster                                          |
| logging_silent           | 190 ns                                                 | 109 ns: 1.74x faster                                           |
| asyncio_tcp              | 922 ms                                                 | 535 ms: 1.72x faster                                           |
| go                       | 240 ms                                                 | 147 ms: 1.63x faster                                           |
| richards                 | 79.3 ms                                                | 48.8 ms: 1.63x faster                                          |
| richards_super           | 94.7 ms                                                | 60.2 ms: 1.57x faster                                          |
| python_startup           | 14.6 ms                                                | 9.33 ms: 1.56x faster                                          |
| crypto_pyaes             | 128 ms                                                 | 81.9 ms: 1.56x faster                                          |
| scimark_monte_carlo      | 118 ms                                                 | 76.1 ms: 1.55x faster                                          |
| pickle_pure_python       | 484 us                                                 | 315 us: 1.54x faster                                           |
| hexiom                   | 10.4 ms                                                | 6.85 ms: 1.52x faster                                          |
| spectral_norm            | 170 ms                                                 | 112 ms: 1.51x faster                                           |
| pyflate                  | 716 ms                                                 | 475 ms: 1.51x faster                                           |
| chaos                    | 115 ms                                                 | 76.6 ms: 1.51x faster                                          |
| nbody                    | 154 ms                                                 | 103 ms: 1.48x faster                                           |
| raytrace                 | 507 ms                                                 | 346 ms: 1.47x faster                                           |
| deepcopy_memo            | 58.5 us                                                | 40.1 us: 1.46x faster                                          |
| scimark_lu               | 176 ms                                                 | 125 ms: 1.41x faster                                           |
| coroutines               | 35.1 ms                                                | 25.1 ms: 1.40x faster                                          |
| unpickle_pure_python     | 331 us                                                 | 237 us: 1.40x faster                                           |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.85 sec: 1.39x faster                                         |
| pycparser                | 1.58 sec                                               | 1.14 sec: 1.38x faster                                         |
| json_dumps               | 14.2 ms                                                | 10.5 ms: 1.36x faster                                          |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.91 ms: 1.32x faster                                          |
| pprint_safe_repr         | 1.02 sec                                               | 772 ms: 1.32x faster                                           |
| pprint_pformat           | 2.10 sec                                               | 1.60 sec: 1.32x faster                                         |
| tomli_loads              | 3.14 sec                                               | 2.39 sec: 1.31x faster                                         |
| genshi_text              | 31.8 ms                                                | 24.3 ms: 1.31x faster                                          |
| sqlglot_transpile        | 2.57 ms                                                | 1.97 ms: 1.31x faster                                          |
| xml_etree_process        | 79.1 ms                                                | 60.5 ms: 1.31x faster                                          |
| html5lib                 | 88.9 ms                                                | 68.3 ms: 1.30x faster                                          |
| sqlglot_parse            | 2.17 ms                                                | 1.67 ms: 1.30x faster                                          |
| deepcopy                 | 479 us                                                 | 373 us: 1.28x faster                                           |
| genshi_xml               | 66.0 ms                                                | 51.9 ms: 1.27x faster                                          |
| regex_v8                 | 27.8 ms                                                | 22.0 ms: 1.26x faster                                          |
| xml_etree_parse          | 168 ms                                                 | 133 ms: 1.26x faster                                           |
| sqlglot_normalize        | 143 ms                                                 | 114 ms: 1.26x faster                                           |
| deepcopy_reduce          | 4.17 us                                                | 3.32 us: 1.25x faster                                          |
| chameleon                | 9.68 ms                                                | 7.73 ms: 1.25x faster                                          |
| sqlglot_optimize         | 69.2 ms                                                | 55.4 ms: 1.25x faster                                          |
| regex_compile            | 188 ms                                                 | 151 ms: 1.25x faster                                           |
| scimark_fft              | 466 ms                                                 | 374 ms: 1.25x faster                                           |
| fannkuch                 | 532 ms                                                 | 433 ms: 1.23x faster                                           |
| nqueens                  | 106 ms                                                 | 86.4 ms: 1.22x faster                                          |
| 2to3                     | 348 ms                                                 | 287 ms: 1.22x faster                                           |
| logging_simple           | 8.30 us                                                | 6.89 us: 1.21x faster                                          |
| async_generators         | 444 ms                                                 | 369 ms: 1.20x faster                                           |
| mako                     | 16.3 ms                                                | 13.6 ms: 1.20x faster                                          |
| xml_etree_generate       | 99.4 ms                                                | 83.3 ms: 1.19x faster                                          |
| logging_format           | 9.09 us                                                | 7.75 us: 1.17x faster                                          |
| gc_traversal             | 3.62 ms                                                | 3.11 ms: 1.17x faster                                          |
| unpack_sequence          | 60.0 ns                                                | 51.8 ns: 1.16x faster                                          |
| pickle_list              | 5.08 us                                                | 4.47 us: 1.13x faster                                          |
| sympy_integrate          | 25.8 ms                                                | 22.8 ms: 1.13x faster                                          |
| json                     | 5.69 ms                                                | 5.05 ms: 1.13x faster                                          |
| json_loads               | 31.2 us                                                | 28.1 us: 1.11x faster                                          |
| pickle                   | 10.7 us                                                | 9.82 us: 1.09x faster                                          |
| create_gc_cycles         | 1.62 ms                                                | 1.50 ms: 1.08x faster                                          |
| comprehensions           | 28.8 us                                                | 26.8 us: 1.07x faster                                          |
| telco                    | 7.27 ms                                                | 6.81 ms: 1.07x faster                                          |
| sympy_expand             | 566 ms                                                 | 533 ms: 1.06x faster                                           |
| sympy_str                | 346 ms                                                 | 329 ms: 1.05x faster                                           |
| pathlib                  | 20.5 ms                                                | 19.5 ms: 1.05x faster                                          |
| regex_dna                | 227 ms                                                 | 219 ms: 1.03x faster                                           |
| regex_effbot             | 3.63 ms                                                | 3.52 ms: 1.03x faster                                          |
| sympy_sum                | 196 ms                                                 | 192 ms: 1.03x faster                                           |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                           |
| generators               | 80.1 ms                                                | 78.3 ms: 1.02x faster                                          |
| typing_runtime_protocols | 544 us                                                 | 535 us: 1.02x faster                                           |
| pickle_dict              | 29.6 us                                                | 29.9 us: 1.01x slower                                          |
| unpickle_list            | 5.20 us                                                | 5.35 us: 1.03x slower                                          |
| mdp                      | 2.85 sec                                               | 2.94 sec: 1.03x slower                                         |
| xml_etree_iterparse      | 115 ms                                                 | 121 ms: 1.04x slower                                           |
| meteor_contest           | 120 ms                                                 | 126 ms: 1.06x slower                                           |
| unpickle                 | 14.4 us                                                | 15.3 us: 1.06x slower                                          |
| sqlite_synth             | 3.02 us                                                | 3.33 us: 1.10x slower                                          |
| python_startup_no_site   | 5.93 ms                                                | 6.70 ms: 1.13x slower                                          |
| bench_thread_pool        | 986 us                                                 | 1.64 ms: 1.66x slower                                          |
| Geometric mean           | (ref)                                                  | 1.28x faster                                                   |

Benchmark hidden because not significant (1): bench_mp_pool
Ignored benchmarks (16) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_websockets, coverage, dask, django_template, djangocms, docutils, dulwich_log, flaskblogging, gunicorn, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift, tornado_http


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.25x
- 95% likely to have a speedup of 1.24x
- 99% likely to have a speedup of 1.22x


# Memory

- memory change: 1.45x