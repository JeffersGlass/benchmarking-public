
# Results vs. 3.11.0

- fork: mdboom
- ref: nogil_d595911
- machine: linux-x86_64
- commit hash: d595911
- commit date: 2023-04-27
- overall geometric mean: 1.00x faster \*
- HPT reliability: 97.97%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.35x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230427-linux-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 287 ms: 1.09x slower                                           |
| chameleon      | 6.70 ms                                                | 7.73 ms: 1.15x slower                                          |
| html5lib       | 64.8 ms                                                | 68.3 ms: 1.05x slower                                          |
| Geometric mean | (ref)                                                  | 1.10x slower                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230427-linux-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_io           | 1.29 sec                                               | 580 ms: 2.22x faster                                           |
| async_tree_none         | 528 ms                                                 | 289 ms: 1.83x faster                                           |
| async_tree_memoization  | 639 ms                                                 | 362 ms: 1.77x faster                                           |
| async_tree_cpu_io_mixed | 749 ms                                                 | 514 ms: 1.46x faster                                           |
| Geometric mean          | (ref)                                                  | 1.80x faster                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230427-linux-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| float          | 78.9 ms                                                | 67.0 ms: 1.18x faster                                          |
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                           |
| nbody          | 96.0 ms                                                | 103 ms: 1.08x slower                                           |
| Geometric mean | (ref)                                                  | 1.04x faster                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230427-linux-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_v8       | 22.9 ms                                                | 22.0 ms: 1.04x faster                                          |
| regex_effbot   | 3.51 ms                                                | 3.52 ms: 1.00x slower                                          |
| regex_compile  | 141 ms                                                 | 151 ms: 1.07x slower                                           |
| regex_dna      | 205 ms                                                 | 219 ms: 1.07x slower                                           |
| Geometric mean | (ref)                                                  | 1.03x slower                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230427-linux-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.28x faster                                          |
| xml_etree_parse      | 164 ms                                                 | 133 ms: 1.23x faster                                           |
| pickle_dict          | 34.6 us                                                | 29.9 us: 1.16x faster                                          |
| pickle               | 11.0 us                                                | 9.82 us: 1.12x faster                                          |
| json_loads           | 29.2 us                                                | 28.1 us: 1.04x faster                                          |
| pickle_list          | 4.59 us                                                | 4.47 us: 1.02x faster                                          |
| unpickle_pure_python | 242 us                                                 | 237 us: 1.02x faster                                           |
| pickle_pure_python   | 320 us                                                 | 315 us: 1.02x faster                                           |
| unpickle_list        | 5.21 us                                                | 5.35 us: 1.03x slower                                          |
| xml_etree_generate   | 81.1 ms                                                | 83.3 ms: 1.03x slower                                          |
| tomli_loads          | 2.30 sec                                               | 2.39 sec: 1.04x slower                                         |
| xml_etree_process    | 56.9 ms                                                | 60.5 ms: 1.06x slower                                          |
| unpickle             | 13.8 us                                                | 15.3 us: 1.11x slower                                          |
| xml_etree_iterparse  | 108 ms                                                 | 121 ms: 1.12x slower                                           |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                   |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230427-linux-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 9.33 ms: 1.09x slower                                          |
| python_startup_no_site | 6.01 ms                                                | 6.70 ms: 1.11x slower                                          |
| Geometric mean         | (ref)                                                  | 1.10x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230427-linux-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| genshi_xml     | 53.4 ms                                                | 51.9 ms: 1.03x faster                                          |
| genshi_text    | 22.5 ms                                                | 24.3 ms: 1.08x slower                                          |
| mako           | 10.7 ms                                                | 13.6 ms: 1.27x slower                                          |
| Geometric mean | (ref)                                                  | 1.10x slower                                                   |

All benchmarks:
===============

| Benchmark                | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230427-linux-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_io            | 1.29 sec                                               | 580 ms: 2.22x faster                                           |
| async_tree_none          | 528 ms                                                 | 289 ms: 1.83x faster                                           |
| async_tree_memoization   | 639 ms                                                 | 362 ms: 1.77x faster                                           |
| asyncio_tcp_ssl          | 3.11 sec                                               | 1.85 sec: 1.68x faster                                         |
| asyncio_tcp              | 875 ms                                                 | 535 ms: 1.64x faster                                           |
| async_tree_cpu_io_mixed  | 749 ms                                                 | 514 ms: 1.46x faster                                           |
| gc_traversal             | 4.01 ms                                                | 3.11 ms: 1.29x faster                                          |
| json_dumps               | 13.3 ms                                                | 10.5 ms: 1.28x faster                                          |
| xml_etree_parse          | 164 ms                                                 | 133 ms: 1.23x faster                                           |
| float                    | 78.9 ms                                                | 67.0 ms: 1.18x faster                                          |
| pickle_dict              | 34.6 us                                                | 29.9 us: 1.16x faster                                          |
| pickle                   | 11.0 us                                                | 9.82 us: 1.12x faster                                          |
| coroutines               | 27.0 ms                                                | 25.1 ms: 1.08x faster                                          |
| deltablue                | 3.92 ms                                                | 3.67 ms: 1.07x faster                                          |
| pidigits                 | 194 ms                                                 | 187 ms: 1.04x faster                                           |
| regex_v8                 | 22.9 ms                                                | 22.0 ms: 1.04x faster                                          |
| json                     | 5.24 ms                                                | 5.05 ms: 1.04x faster                                          |
| json_loads               | 29.2 us                                                | 28.1 us: 1.04x faster                                          |
| pycparser                | 1.19 sec                                               | 1.14 sec: 1.04x faster                                         |
| genshi_xml               | 53.4 ms                                                | 51.9 ms: 1.03x faster                                          |
| richards_super           | 61.9 ms                                                | 60.2 ms: 1.03x faster                                          |
| pickle_list              | 4.59 us                                                | 4.47 us: 1.02x faster                                          |
| scimark_sparse_mat_mult  | 5.03 ms                                                | 4.91 ms: 1.02x faster                                          |
| logging_silent           | 111 ns                                                 | 109 ns: 1.02x faster                                           |
| richards                 | 49.8 ms                                                | 48.8 ms: 1.02x faster                                          |
| unpickle_pure_python     | 242 us                                                 | 237 us: 1.02x faster                                           |
| nqueens                  | 87.9 ms                                                | 86.4 ms: 1.02x faster                                          |
| pickle_pure_python       | 320 us                                                 | 315 us: 1.02x faster                                           |
| async_generators         | 374 ms                                                 | 369 ms: 1.01x faster                                           |
| go                       | 149 ms                                                 | 147 ms: 1.01x faster                                           |
| telco                    | 6.86 ms                                                | 6.81 ms: 1.01x faster                                          |
| hexiom                   | 6.89 ms                                                | 6.85 ms: 1.01x faster                                          |
| sqlglot_optimize         | 55.3 ms                                                | 55.4 ms: 1.00x slower                                          |
| regex_effbot             | 3.51 ms                                                | 3.52 ms: 1.00x slower                                          |
| sqlglot_normalize        | 113 ms                                                 | 114 ms: 1.01x slower                                           |
| deepcopy                 | 365 us                                                 | 373 us: 1.02x slower                                           |
| unpickle_list            | 5.21 us                                                | 5.35 us: 1.03x slower                                          |
| pprint_pformat           | 1.55 sec                                               | 1.60 sec: 1.03x slower                                         |
| xml_etree_generate       | 81.1 ms                                                | 83.3 ms: 1.03x slower                                          |
| typing_runtime_protocols | 520 us                                                 | 535 us: 1.03x slower                                           |
| scimark_sor              | 121 ms                                                 | 125 ms: 1.03x slower                                           |
| pprint_safe_repr         | 747 ms                                                 | 772 ms: 1.03x slower                                           |
| deepcopy_reduce          | 3.22 us                                                | 3.32 us: 1.03x slower                                          |
| tomli_loads              | 2.30 sec                                               | 2.39 sec: 1.04x slower                                         |
| spectral_norm            | 108 ms                                                 | 112 ms: 1.04x slower                                           |
| create_gc_cycles         | 1.43 ms                                                | 1.50 ms: 1.05x slower                                          |
| generators               | 74.9 ms                                                | 78.3 ms: 1.05x slower                                          |
| html5lib                 | 64.8 ms                                                | 68.3 ms: 1.05x slower                                          |
| pathlib                  | 18.5 ms                                                | 19.5 ms: 1.06x slower                                          |
| sympy_integrate          | 21.5 ms                                                | 22.8 ms: 1.06x slower                                          |
| mdp                      | 2.77 sec                                               | 2.94 sec: 1.06x slower                                         |
| xml_etree_process        | 56.9 ms                                                | 60.5 ms: 1.06x slower                                          |
| chaos                    | 71.9 ms                                                | 76.6 ms: 1.07x slower                                          |
| crypto_pyaes             | 76.7 ms                                                | 81.9 ms: 1.07x slower                                          |
| fannkuch                 | 405 ms                                                 | 433 ms: 1.07x slower                                           |
| regex_compile            | 141 ms                                                 | 151 ms: 1.07x slower                                           |
| regex_dna                | 205 ms                                                 | 219 ms: 1.07x slower                                           |
| scimark_lu               | 116 ms                                                 | 125 ms: 1.07x slower                                           |
| scimark_monte_carlo      | 70.7 ms                                                | 76.1 ms: 1.08x slower                                          |
| nbody                    | 96.0 ms                                                | 103 ms: 1.08x slower                                           |
| genshi_text              | 22.5 ms                                                | 24.3 ms: 1.08x slower                                          |
| scimark_fft              | 345 ms                                                 | 374 ms: 1.08x slower                                           |
| 2to3                     | 264 ms                                                 | 287 ms: 1.09x slower                                           |
| python_startup           | 8.56 ms                                                | 9.33 ms: 1.09x slower                                          |
| pyflate                  | 434 ms                                                 | 475 ms: 1.09x slower                                           |
| sympy_expand             | 484 ms                                                 | 533 ms: 1.10x slower                                           |
| sympy_str                | 297 ms                                                 | 329 ms: 1.11x slower                                           |
| unpickle                 | 13.8 us                                                | 15.3 us: 1.11x slower                                          |
| logging_simple           | 6.22 us                                                | 6.89 us: 1.11x slower                                          |
| python_startup_no_site   | 6.01 ms                                                | 6.70 ms: 1.11x slower                                          |
| xml_etree_iterparse      | 108 ms                                                 | 121 ms: 1.12x slower                                           |
| raytrace                 | 309 ms                                                 | 346 ms: 1.12x slower                                           |
| sqlglot_transpile        | 1.75 ms                                                | 1.97 ms: 1.12x slower                                          |
| sympy_sum                | 169 ms                                                 | 192 ms: 1.14x slower                                           |
| comprehensions           | 23.6 us                                                | 26.8 us: 1.14x slower                                          |
| logging_format           | 6.81 us                                                | 7.75 us: 1.14x slower                                          |
| chameleon                | 6.70 ms                                                | 7.73 ms: 1.15x slower                                          |
| meteor_contest           | 109 ms                                                 | 126 ms: 1.16x slower                                           |
| sqlglot_parse            | 1.43 ms                                                | 1.67 ms: 1.17x slower                                          |
| unpack_sequence          | 43.5 ns                                                | 51.8 ns: 1.19x slower                                          |
| mako                     | 10.7 ms                                                | 13.6 ms: 1.27x slower                                          |
| sqlite_synth             | 2.57 us                                                | 3.33 us: 1.29x slower                                          |
| bench_thread_pool        | 834 us                                                 | 1.64 ms: 1.97x slower                                          |
| Geometric mean           | (ref)                                                  | 1.00x faster                                                   |

Benchmark hidden because not significant (2): deepcopy_memo, bench_mp_pool
Ignored benchmarks (20) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, coverage, dask, django_template, djangocms, docutils, dulwich_log, flaskblogging, gunicorn, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift, tornado_http


# HPT report

- Reliability score: 97.97% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.35x