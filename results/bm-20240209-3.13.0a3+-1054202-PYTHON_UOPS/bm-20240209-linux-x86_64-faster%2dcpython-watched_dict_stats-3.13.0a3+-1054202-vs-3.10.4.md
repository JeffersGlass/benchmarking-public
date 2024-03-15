
# Results vs. 3.10.4

- fork: faster-cpython
- ref: watched_dict_stats
- machine: linux-x86_64
- commit hash: 1054202
- commit date: 2024-02-09
- overall geometric mean: 1.27x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.19x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 282 ms: 1.23x faster                                                           |
| chameleon      | 9.68 ms                                                | 7.40 ms: 1.31x faster                                                          |
| docutils       | 3.30 sec                                               | 2.71 sec: 1.22x faster                                                         |
| tornado_http   | 136 ms                                                 | 98.6 ms: 1.38x faster                                                          |
| Geometric mean | (ref)                                                  | 1.28x faster                                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 450 ms: 1.62x faster                                                           |
| async_tree_memoization  | 870 ms                                                 | 577 ms: 1.51x faster                                                           |
| async_tree_io           | 1.77 sec                                               | 1.19 sec: 1.48x faster                                                         |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 725 ms: 1.40x faster                                                           |
| Geometric mean          | (ref)                                                  | 1.50x faster                                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| float          | 117 ms                                                 | 91.4 ms: 1.28x faster                                                          |
| nbody          | 154 ms                                                 | 121 ms: 1.27x faster                                                           |
| pidigits       | 191 ms                                                 | 188 ms: 1.02x faster                                                           |
| Geometric mean | (ref)                                                  | 1.18x faster                                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 150 ms: 1.26x faster                                                           |
| regex_v8       | 27.8 ms                                                | 25.1 ms: 1.11x faster                                                          |
| regex_dna      | 227 ms                                                 | 228 ms: 1.00x slower                                                           |
| regex_effbot   | 3.63 ms                                                | 3.77 ms: 1.04x slower                                                          |
| Geometric mean | (ref)                                                  | 1.07x faster                                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 298 us: 1.63x faster                                                           |
| unpickle_pure_python | 331 us                                                 | 232 us: 1.42x faster                                                           |
| json_dumps           | 14.2 ms                                                | 10.6 ms: 1.34x faster                                                          |
| xml_etree_process    | 79.1 ms                                                | 60.6 ms: 1.31x faster                                                          |
| tomli_loads          | 3.14 sec                                               | 2.62 sec: 1.20x faster                                                         |
| json_loads           | 31.2 us                                                | 27.7 us: 1.13x faster                                                          |
| xml_etree_generate   | 99.4 ms                                                | 88.5 ms: 1.12x faster                                                          |
| xml_etree_parse      | 168 ms                                                 | 159 ms: 1.06x faster                                                           |
| xml_etree_iterparse  | 115 ms                                                 | 109 ms: 1.06x faster                                                           |
| unpickle_list        | 5.20 us                                                | 5.03 us: 1.03x faster                                                          |
| pickle_list          | 5.08 us                                                | 5.25 us: 1.03x slower                                                          |
| unpickle             | 14.4 us                                                | 15.3 us: 1.06x slower                                                          |
| pickle               | 10.7 us                                                | 11.6 us: 1.09x slower                                                          |
| pickle_dict          | 29.6 us                                                | 34.7 us: 1.17x slower                                                          |
| Geometric mean       | (ref)                                                  | 1.12x faster                                                                   |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                          |
| python_startup_no_site | 5.93 ms                                                | 8.75 ms: 1.48x slower                                                          |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|-----------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 13.9 ms: 1.17x faster                                                          |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 115 us: 4.75x faster                                                           |
| generators               | 80.1 ms                                                | 29.4 ms: 2.73x faster                                                          |
| deltablue                | 7.91 ms                                                | 3.48 ms: 2.28x faster                                                          |
| asyncio_tcp              | 922 ms                                                 | 492 ms: 1.87x faster                                                           |
| logging_silent           | 190 ns                                                 | 101 ns: 1.87x faster                                                           |
| scimark_sor              | 220 ms                                                 | 121 ms: 1.81x faster                                                           |
| raytrace                 | 507 ms                                                 | 298 ms: 1.70x faster                                                           |
| richards_super           | 94.7 ms                                                | 55.7 ms: 1.70x faster                                                          |
| sqlglot_parse            | 2.17 ms                                                | 1.33 ms: 1.63x faster                                                          |
| pickle_pure_python       | 484 us                                                 | 298 us: 1.63x faster                                                           |
| async_tree_none          | 728 ms                                                 | 450 ms: 1.62x faster                                                           |
| richards                 | 79.3 ms                                                | 49.3 ms: 1.61x faster                                                          |
| coroutines               | 35.1 ms                                                | 22.1 ms: 1.58x faster                                                          |
| chaos                    | 115 ms                                                 | 73.2 ms: 1.58x faster                                                          |
| sqlglot_transpile        | 2.57 ms                                                | 1.67 ms: 1.54x faster                                                          |
| go                       | 240 ms                                                 | 156 ms: 1.54x faster                                                           |
| scimark_lu               | 176 ms                                                 | 116 ms: 1.52x faster                                                           |
| crypto_pyaes             | 128 ms                                                 | 84.5 ms: 1.51x faster                                                          |
| async_tree_memoization   | 870 ms                                                 | 577 ms: 1.51x faster                                                           |
| async_tree_io            | 1.77 sec                                               | 1.19 sec: 1.48x faster                                                         |
| deepcopy_memo            | 58.5 us                                                | 39.7 us: 1.47x faster                                                          |
| scimark_monte_carlo      | 118 ms                                                 | 81.1 ms: 1.46x faster                                                          |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                          |
| unpickle_pure_python     | 331 us                                                 | 232 us: 1.42x faster                                                           |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.81 sec: 1.42x faster                                                         |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 725 ms: 1.40x faster                                                           |
| tornado_http             | 136 ms                                                 | 98.6 ms: 1.38x faster                                                          |
| logging_simple           | 8.30 us                                                | 6.03 us: 1.38x faster                                                          |
| pyflate                  | 716 ms                                                 | 526 ms: 1.36x faster                                                           |
| deepcopy                 | 479 us                                                 | 353 us: 1.36x faster                                                           |
| comprehensions           | 28.8 us                                                | 21.4 us: 1.35x faster                                                          |
| logging_format           | 9.09 us                                                | 6.78 us: 1.34x faster                                                          |
| json_dumps               | 14.2 ms                                                | 10.6 ms: 1.34x faster                                                          |
| deepcopy_reduce          | 4.17 us                                                | 3.14 us: 1.33x faster                                                          |
| chameleon                | 9.68 ms                                                | 7.40 ms: 1.31x faster                                                          |
| xml_etree_process        | 79.1 ms                                                | 60.6 ms: 1.31x faster                                                          |
| pycparser                | 1.58 sec                                               | 1.23 sec: 1.28x faster                                                         |
| float                    | 117 ms                                                 | 91.4 ms: 1.28x faster                                                          |
| pprint_safe_repr         | 1.02 sec                                               | 799 ms: 1.27x faster                                                           |
| nbody                    | 154 ms                                                 | 121 ms: 1.27x faster                                                           |
| pprint_pformat           | 2.10 sec                                               | 1.66 sec: 1.27x faster                                                         |
| regex_compile            | 188 ms                                                 | 150 ms: 1.26x faster                                                           |
| sqlglot_normalize        | 143 ms                                                 | 115 ms: 1.24x faster                                                           |
| 2to3                     | 348 ms                                                 | 282 ms: 1.23x faster                                                           |
| hexiom                   | 10.4 ms                                                | 8.44 ms: 1.23x faster                                                          |
| dulwich_log              | 84.3 ms                                                | 69.0 ms: 1.22x faster                                                          |
| docutils                 | 3.30 sec                                               | 2.71 sec: 1.22x faster                                                         |
| sympy_integrate          | 25.8 ms                                                | 21.3 ms: 1.21x faster                                                          |
| fannkuch                 | 532 ms                                                 | 440 ms: 1.21x faster                                                           |
| sympy_sum                | 196 ms                                                 | 163 ms: 1.20x faster                                                           |
| tomli_loads              | 3.14 sec                                               | 2.62 sec: 1.20x faster                                                         |
| dask                     | 441 ms                                                 | 370 ms: 1.19x faster                                                           |
| sqlglot_optimize         | 69.2 ms                                                | 58.4 ms: 1.19x faster                                                          |
| spectral_norm            | 170 ms                                                 | 144 ms: 1.18x faster                                                           |
| sympy_str                | 346 ms                                                 | 294 ms: 1.17x faster                                                           |
| mako                     | 16.3 ms                                                | 13.9 ms: 1.17x faster                                                          |
| bench_thread_pool        | 986 us                                                 | 846 us: 1.17x faster                                                           |
| sympy_expand             | 566 ms                                                 | 494 ms: 1.14x faster                                                           |
| json_loads               | 31.2 us                                                | 27.7 us: 1.13x faster                                                          |
| xml_etree_generate       | 99.4 ms                                                | 88.5 ms: 1.12x faster                                                          |
| json                     | 5.69 ms                                                | 5.11 ms: 1.11x faster                                                          |
| pathlib                  | 20.5 ms                                                | 18.4 ms: 1.11x faster                                                          |
| regex_v8                 | 27.8 ms                                                | 25.1 ms: 1.11x faster                                                          |
| create_gc_cycles         | 1.62 ms                                                | 1.48 ms: 1.10x faster                                                          |
| nqueens                  | 106 ms                                                 | 97.6 ms: 1.08x faster                                                          |
| mdp                      | 2.85 sec                                               | 2.64 sec: 1.08x faster                                                         |
| xml_etree_parse          | 168 ms                                                 | 159 ms: 1.06x faster                                                           |
| meteor_contest           | 120 ms                                                 | 113 ms: 1.06x faster                                                           |
| xml_etree_iterparse      | 115 ms                                                 | 109 ms: 1.06x faster                                                           |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 6.11 ms: 1.06x faster                                                          |
| scimark_fft              | 466 ms                                                 | 440 ms: 1.06x faster                                                           |
| unpack_sequence          | 60.0 ns                                                | 57.1 ns: 1.05x faster                                                          |
| sqlite_synth             | 3.02 us                                                | 2.88 us: 1.05x faster                                                          |
| unpickle_list            | 5.20 us                                                | 5.03 us: 1.03x faster                                                          |
| pidigits                 | 191 ms                                                 | 188 ms: 1.02x faster                                                           |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                           |
| regex_dna                | 227 ms                                                 | 228 ms: 1.00x slower                                                           |
| async_generators         | 444 ms                                                 | 449 ms: 1.01x slower                                                           |
| gc_traversal             | 3.62 ms                                                | 3.71 ms: 1.02x slower                                                          |
| pickle_list              | 5.08 us                                                | 5.25 us: 1.03x slower                                                          |
| regex_effbot             | 3.63 ms                                                | 3.77 ms: 1.04x slower                                                          |
| unpickle                 | 14.4 us                                                | 15.3 us: 1.06x slower                                                          |
| pickle                   | 10.7 us                                                | 11.6 us: 1.09x slower                                                          |
| pickle_dict              | 29.6 us                                                | 34.7 us: 1.17x slower                                                          |
| telco                    | 7.27 ms                                                | 8.65 ms: 1.19x slower                                                          |
| coverage                 | 79.4 ms                                                | 94.8 ms: 1.19x slower                                                          |
| python_startup_no_site   | 5.93 ms                                                | 8.75 ms: 1.48x slower                                                          |
| Geometric mean           | (ref)                                                  | 1.27x faster                                                                   |

Benchmark hidden because not significant (2): mypy2, bench_mp_pool
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240209-3.13.0a3+-1054202-PYTHON_UOPS/bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.21x
- 95% likely to have a speedup of 1.20x
- 99% likely to have a speedup of 1.19x


# Memory

- memory change: 1.06x