
# Results vs. 3.11.0

- fork: mdboom
- ref: match_nogil_gc
- machine: linux-x86_64
- commit hash: 0fd3163
- commit date: 2023-05-31
- overall geometric mean: 1.13x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.07x faster
- Memory change: 1.17x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230531-linux-x86_64-mdboom-match_nogil_gc-3.12.0a4-0fd3163 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 245 ms: 1.08x faster                                            |
| chameleon      | 6.70 ms                                                | 6.37 ms: 1.05x faster                                           |
| docutils       | 2.66 sec                                               | 2.15 sec: 1.24x faster                                          |
| html5lib       | 64.8 ms                                                | 57.8 ms: 1.12x faster                                           |
| Geometric mean | (ref)                                                  | 1.12x faster                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230531-linux-x86_64-mdboom-match_nogil_gc-3.12.0a4-0fd3163 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_io           | 1.29 sec                                               | 534 ms: 2.41x faster                                            |
| async_tree_none         | 528 ms                                                 | 260 ms: 2.03x faster                                            |
| async_tree_memoization  | 639 ms                                                 | 315 ms: 2.03x faster                                            |
| async_tree_cpu_io_mixed | 749 ms                                                 | 469 ms: 1.60x faster                                            |
| Geometric mean          | (ref)                                                  | 1.99x faster                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230531-linux-x86_64-mdboom-match_nogil_gc-3.12.0a4-0fd3163 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| float          | 78.9 ms                                                | 60.7 ms: 1.30x faster                                           |
| nbody          | 96.0 ms                                                | 92.3 ms: 1.04x faster                                           |
| pidigits       | 194 ms                                                 | 189 ms: 1.03x faster                                            |
| Geometric mean | (ref)                                                  | 1.12x faster                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230531-linux-x86_64-mdboom-match_nogil_gc-3.12.0a4-0fd3163 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 131 ms: 1.08x faster                                            |
| regex_v8       | 22.9 ms                                                | 22.1 ms: 1.04x faster                                           |
| regex_effbot   | 3.51 ms                                                | 3.46 ms: 1.01x faster                                           |
| regex_dna      | 205 ms                                                 | 210 ms: 1.03x slower                                            |
| Geometric mean | (ref)                                                  | 1.02x faster                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230531-linux-x86_64-mdboom-match_nogil_gc-3.12.0a4-0fd3163 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 9.55 ms: 1.40x faster                                           |
| xml_etree_parse      | 164 ms                                                 | 122 ms: 1.35x faster                                            |
| xml_etree_iterparse  | 108 ms                                                 | 80.9 ms: 1.34x faster                                           |
| json_loads           | 29.2 us                                                | 23.7 us: 1.23x faster                                           |
| unpickle_pure_python | 242 us                                                 | 198 us: 1.22x faster                                            |
| tomli_loads          | 2.30 sec                                               | 1.98 sec: 1.16x faster                                          |
| pickle_pure_python   | 320 us                                                 | 282 us: 1.13x faster                                            |
| pickle_list          | 4.59 us                                                | 4.05 us: 1.13x faster                                           |
| pickle_dict          | 34.6 us                                                | 31.2 us: 1.11x faster                                           |
| xml_etree_generate   | 81.1 ms                                                | 73.4 ms: 1.10x faster                                           |
| xml_etree_process    | 56.9 ms                                                | 51.6 ms: 1.10x faster                                           |
| pickle               | 11.0 us                                                | 10.2 us: 1.08x faster                                           |
| unpickle             | 13.8 us                                                | 13.0 us: 1.06x faster                                           |
| unpickle_list        | 5.21 us                                                | 4.95 us: 1.05x faster                                           |
| Geometric mean       | (ref)                                                  | 1.17x faster                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230531-linux-x86_64-mdboom-match_nogil_gc-3.12.0a4-0fd3163 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 8.24 ms: 1.04x faster                                           |
| python_startup_no_site | 6.01 ms                                                | 5.93 ms: 1.01x faster                                           |
| Geometric mean         | (ref)                                                  | 1.03x faster                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230531-linux-x86_64-mdboom-match_nogil_gc-3.12.0a4-0fd3163 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| genshi_xml      | 53.4 ms                                                | 45.9 ms: 1.16x faster                                           |
| genshi_text     | 22.5 ms                                                | 20.2 ms: 1.12x faster                                           |
| mako            | 10.7 ms                                                | 9.69 ms: 1.10x faster                                           |
| django_template | 33.5 ms                                                | 32.9 ms: 1.02x faster                                           |
| Geometric mean  | (ref)                                                  | 1.10x faster                                                    |

All benchmarks:
===============

| Benchmark                | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230531-linux-x86_64-mdboom-match_nogil_gc-3.12.0a4-0fd3163 |
|--------------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_io            | 1.29 sec                                               | 534 ms: 2.41x faster                                            |
| async_tree_none          | 528 ms                                                 | 260 ms: 2.03x faster                                            |
| async_tree_memoization   | 639 ms                                                 | 315 ms: 2.03x faster                                            |
| asyncio_tcp_ssl          | 3.11 sec                                               | 1.79 sec: 1.74x faster                                          |
| asyncio_tcp              | 875 ms                                                 | 511 ms: 1.71x faster                                            |
| async_tree_cpu_io_mixed  | 749 ms                                                 | 469 ms: 1.60x faster                                            |
| json_dumps               | 13.3 ms                                                | 9.55 ms: 1.40x faster                                           |
| xml_etree_parse          | 164 ms                                                 | 122 ms: 1.35x faster                                            |
| xml_etree_iterparse      | 108 ms                                                 | 80.9 ms: 1.34x faster                                           |
| float                    | 78.9 ms                                                | 60.7 ms: 1.30x faster                                           |
| deltablue                | 3.92 ms                                                | 3.11 ms: 1.26x faster                                           |
| logging_silent           | 111 ns                                                 | 89.6 ns: 1.24x faster                                           |
| docutils                 | 2.66 sec                                               | 2.15 sec: 1.24x faster                                          |
| json_loads               | 29.2 us                                                | 23.7 us: 1.23x faster                                           |
| unpickle_pure_python     | 242 us                                                 | 198 us: 1.22x faster                                            |
| scimark_sparse_mat_mult  | 5.03 ms                                                | 4.12 ms: 1.22x faster                                           |
| gc_traversal             | 4.01 ms                                                | 3.38 ms: 1.19x faster                                           |
| deepcopy_memo            | 40.2 us                                                | 33.8 us: 1.19x faster                                           |
| richards                 | 49.8 ms                                                | 42.5 ms: 1.17x faster                                           |
| richards_super           | 61.9 ms                                                | 52.9 ms: 1.17x faster                                           |
| genshi_xml               | 53.4 ms                                                | 45.9 ms: 1.16x faster                                           |
| tomli_loads              | 2.30 sec                                               | 1.98 sec: 1.16x faster                                          |
| dask                     | 365 ms                                                 | 317 ms: 1.15x faster                                            |
| json                     | 5.24 ms                                                | 4.59 ms: 1.14x faster                                           |
| spectral_norm            | 108 ms                                                 | 94.7 ms: 1.14x faster                                           |
| scimark_sor              | 121 ms                                                 | 106 ms: 1.14x faster                                            |
| hexiom                   | 6.89 ms                                                | 6.06 ms: 1.14x faster                                           |
| pickle_pure_python       | 320 us                                                 | 282 us: 1.13x faster                                            |
| nqueens                  | 87.9 ms                                                | 77.6 ms: 1.13x faster                                           |
| pickle_list              | 4.59 us                                                | 4.05 us: 1.13x faster                                           |
| pycparser                | 1.19 sec                                               | 1.06 sec: 1.12x faster                                          |
| html5lib                 | 64.8 ms                                                | 57.8 ms: 1.12x faster                                           |
| typing_runtime_protocols | 520 us                                                 | 463 us: 1.12x faster                                            |
| mdp                      | 2.77 sec                                               | 2.48 sec: 1.12x faster                                          |
| genshi_text              | 22.5 ms                                                | 20.2 ms: 1.12x faster                                           |
| scimark_fft              | 345 ms                                                 | 309 ms: 1.12x faster                                            |
| pprint_pformat           | 1.55 sec                                               | 1.39 sec: 1.11x faster                                          |
| pickle_dict              | 34.6 us                                                | 31.2 us: 1.11x faster                                           |
| pprint_safe_repr         | 747 ms                                                 | 676 ms: 1.10x faster                                            |
| xml_etree_generate       | 81.1 ms                                                | 73.4 ms: 1.10x faster                                           |
| scimark_lu               | 116 ms                                                 | 105 ms: 1.10x faster                                            |
| async_generators         | 374 ms                                                 | 338 ms: 1.10x faster                                            |
| xml_etree_process        | 56.9 ms                                                | 51.6 ms: 1.10x faster                                           |
| deepcopy                 | 365 us                                                 | 332 us: 1.10x faster                                            |
| fannkuch                 | 405 ms                                                 | 368 ms: 1.10x faster                                            |
| mako                     | 10.7 ms                                                | 9.69 ms: 1.10x faster                                           |
| scimark_monte_carlo      | 70.7 ms                                                | 65.2 ms: 1.09x faster                                           |
| go                       | 149 ms                                                 | 137 ms: 1.08x faster                                            |
| deepcopy_reduce          | 3.22 us                                                | 2.97 us: 1.08x faster                                           |
| pickle                   | 11.0 us                                                | 10.2 us: 1.08x faster                                           |
| raytrace                 | 309 ms                                                 | 286 ms: 1.08x faster                                            |
| 2to3                     | 264 ms                                                 | 245 ms: 1.08x faster                                            |
| pyflate                  | 434 ms                                                 | 403 ms: 1.08x faster                                            |
| regex_compile            | 141 ms                                                 | 131 ms: 1.08x faster                                            |
| logging_simple           | 6.22 us                                                | 5.80 us: 1.07x faster                                           |
| sqlglot_optimize         | 55.3 ms                                                | 51.6 ms: 1.07x faster                                           |
| sympy_expand             | 484 ms                                                 | 455 ms: 1.07x faster                                            |
| sympy_integrate          | 21.5 ms                                                | 20.2 ms: 1.06x faster                                           |
| unpickle                 | 13.8 us                                                | 13.0 us: 1.06x faster                                           |
| sympy_str                | 297 ms                                                 | 281 ms: 1.06x faster                                            |
| logging_format           | 6.81 us                                                | 6.44 us: 1.06x faster                                           |
| unpickle_list            | 5.21 us                                                | 4.95 us: 1.05x faster                                           |
| bench_thread_pool        | 834 us                                                 | 792 us: 1.05x faster                                            |
| chameleon                | 6.70 ms                                                | 6.37 ms: 1.05x faster                                           |
| telco                    | 6.86 ms                                                | 6.52 ms: 1.05x faster                                           |
| sqlglot_transpile        | 1.75 ms                                                | 1.67 ms: 1.05x faster                                           |
| chaos                    | 71.9 ms                                                | 68.8 ms: 1.04x faster                                           |
| sqlglot_normalize        | 113 ms                                                 | 108 ms: 1.04x faster                                            |
| crypto_pyaes             | 76.7 ms                                                | 73.7 ms: 1.04x faster                                           |
| nbody                    | 96.0 ms                                                | 92.3 ms: 1.04x faster                                           |
| sqlglot_parse            | 1.43 ms                                                | 1.38 ms: 1.04x faster                                           |
| python_startup           | 8.56 ms                                                | 8.24 ms: 1.04x faster                                           |
| sympy_sum                | 169 ms                                                 | 163 ms: 1.04x faster                                            |
| coroutines               | 27.0 ms                                                | 26.1 ms: 1.04x faster                                           |
| regex_v8                 | 22.9 ms                                                | 22.1 ms: 1.04x faster                                           |
| pidigits                 | 194 ms                                                 | 189 ms: 1.03x faster                                            |
| django_template          | 33.5 ms                                                | 32.9 ms: 1.02x faster                                           |
| pathlib                  | 18.5 ms                                                | 18.2 ms: 1.02x faster                                           |
| dulwich_log              | 64.6 ms                                                | 63.5 ms: 1.02x faster                                           |
| thrift                   | 784 us                                                 | 772 us: 1.02x faster                                            |
| python_startup_no_site   | 6.01 ms                                                | 5.93 ms: 1.01x faster                                           |
| regex_effbot             | 3.51 ms                                                | 3.46 ms: 1.01x faster                                           |
| djangocms                | 33.5 us                                                | 33.1 us: 1.01x faster                                           |
| comprehensions           | 23.6 us                                                | 23.9 us: 1.01x slower                                           |
| create_gc_cycles         | 1.43 ms                                                | 1.46 ms: 1.02x slower                                           |
| regex_dna                | 205 ms                                                 | 210 ms: 1.03x slower                                            |
| sqlite_synth             | 2.57 us                                                | 2.67 us: 1.04x slower                                           |
| generators               | 74.9 ms                                                | 79.1 ms: 1.06x slower                                           |
| coverage                 | 78.8 ms                                                | 99.2 ms: 1.26x slower                                           |
| Geometric mean           | (ref)                                                  | 1.13x faster                                                    |

Benchmark hidden because not significant (3): bench_mp_pool, meteor_contest, unpack_sequence
Ignored benchmarks (13) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, flaskblogging, gunicorn, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, tornado_http


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.09x
- 95% likely to have a speedup of 1.08x
- 99% likely to have a speedup of 1.07x


# Memory

- memory change: 1.17x