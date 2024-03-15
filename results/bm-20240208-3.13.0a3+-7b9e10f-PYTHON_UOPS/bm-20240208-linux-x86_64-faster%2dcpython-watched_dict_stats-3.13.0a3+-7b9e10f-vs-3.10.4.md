
# Results vs. 3.10.4

- fork: faster-cpython
- ref: watched_dict_stats
- machine: linux-x86_64
- commit hash: 7b9e10f
- commit date: 2024-02-08
- overall geometric mean: 1.29x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.21x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 282 ms: 1.24x faster                                                           |
| chameleon      | 9.68 ms                                                | 7.18 ms: 1.35x faster                                                          |
| docutils       | 3.30 sec                                               | 2.69 sec: 1.22x faster                                                         |
| tornado_http   | 136 ms                                                 | 98.7 ms: 1.38x faster                                                          |
| Geometric mean | (ref)                                                  | 1.30x faster                                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 448 ms: 1.63x faster                                                           |
| async_tree_memoization  | 870 ms                                                 | 574 ms: 1.51x faster                                                           |
| async_tree_io           | 1.77 sec                                               | 1.19 sec: 1.48x faster                                                         |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 721 ms: 1.41x faster                                                           |
| Geometric mean          | (ref)                                                  | 1.51x faster                                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 115 ms: 1.33x faster                                                           |
| float          | 117 ms                                                 | 88.5 ms: 1.32x faster                                                          |
| pidigits       | 191 ms                                                 | 188 ms: 1.02x faster                                                           |
| Geometric mean | (ref)                                                  | 1.22x faster                                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 148 ms: 1.27x faster                                                           |
| regex_v8       | 27.8 ms                                                | 25.0 ms: 1.11x faster                                                          |
| regex_dna      | 227 ms                                                 | 222 ms: 1.02x faster                                                           |
| Geometric mean | (ref)                                                  | 1.09x faster                                                                   |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 298 us: 1.62x faster                                                           |
| unpickle_pure_python | 331 us                                                 | 231 us: 1.43x faster                                                           |
| json_dumps           | 14.2 ms                                                | 10.6 ms: 1.34x faster                                                          |
| xml_etree_process    | 79.1 ms                                                | 59.9 ms: 1.32x faster                                                          |
| tomli_loads          | 3.14 sec                                               | 2.54 sec: 1.24x faster                                                         |
| json_loads           | 31.2 us                                                | 27.7 us: 1.13x faster                                                          |
| xml_etree_generate   | 99.4 ms                                                | 88.1 ms: 1.13x faster                                                          |
| xml_etree_parse      | 168 ms                                                 | 157 ms: 1.07x faster                                                           |
| xml_etree_iterparse  | 115 ms                                                 | 109 ms: 1.06x faster                                                           |
| unpickle_list        | 5.20 us                                                | 4.99 us: 1.04x faster                                                          |
| pickle_list          | 5.08 us                                                | 5.28 us: 1.04x slower                                                          |
| unpickle             | 14.4 us                                                | 15.3 us: 1.07x slower                                                          |
| pickle               | 10.7 us                                                | 11.9 us: 1.11x slower                                                          |
| pickle_dict          | 29.6 us                                                | 35.3 us: 1.19x slower                                                          |
| Geometric mean       | (ref)                                                  | 1.13x faster                                                                   |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                          |
| python_startup_no_site | 5.93 ms                                                | 8.83 ms: 1.49x slower                                                          |
| Geometric mean         | (ref)                                                  | 1.02x slower                                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|-----------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 13.2 ms: 1.24x faster                                                          |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 114 us: 4.77x faster                                                           |
| generators               | 80.1 ms                                                | 29.3 ms: 2.74x faster                                                          |
| deltablue                | 7.91 ms                                                | 3.51 ms: 2.25x faster                                                          |
| asyncio_tcp              | 922 ms                                                 | 488 ms: 1.89x faster                                                           |
| logging_silent           | 190 ns                                                 | 102 ns: 1.85x faster                                                           |
| scimark_sor              | 220 ms                                                 | 123 ms: 1.79x faster                                                           |
| richards_super           | 94.7 ms                                                | 54.3 ms: 1.74x faster                                                          |
| raytrace                 | 507 ms                                                 | 295 ms: 1.72x faster                                                           |
| richards                 | 79.3 ms                                                | 48.3 ms: 1.64x faster                                                          |
| chaos                    | 115 ms                                                 | 70.6 ms: 1.63x faster                                                          |
| async_tree_none          | 728 ms                                                 | 448 ms: 1.63x faster                                                           |
| sqlglot_parse            | 2.17 ms                                                | 1.33 ms: 1.63x faster                                                          |
| pickle_pure_python       | 484 us                                                 | 298 us: 1.62x faster                                                           |
| coroutines               | 35.1 ms                                                | 22.1 ms: 1.59x faster                                                          |
| crypto_pyaes             | 128 ms                                                 | 82.0 ms: 1.56x faster                                                          |
| sqlglot_transpile        | 2.57 ms                                                | 1.67 ms: 1.54x faster                                                          |
| scimark_lu               | 176 ms                                                 | 115 ms: 1.53x faster                                                           |
| scimark_monte_carlo      | 118 ms                                                 | 77.6 ms: 1.52x faster                                                          |
| async_tree_memoization   | 870 ms                                                 | 574 ms: 1.51x faster                                                           |
| unpack_sequence          | 60.0 ns                                                | 39.9 ns: 1.50x faster                                                          |
| async_tree_io            | 1.77 sec                                               | 1.19 sec: 1.48x faster                                                         |
| deepcopy_memo            | 58.5 us                                                | 39.7 us: 1.47x faster                                                          |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                          |
| unpickle_pure_python     | 331 us                                                 | 231 us: 1.43x faster                                                           |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                                         |
| pyflate                  | 716 ms                                                 | 504 ms: 1.42x faster                                                           |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 721 ms: 1.41x faster                                                           |
| comprehensions           | 28.8 us                                                | 20.5 us: 1.40x faster                                                          |
| logging_simple           | 8.30 us                                                | 5.96 us: 1.39x faster                                                          |
| go                       | 240 ms                                                 | 172 ms: 1.39x faster                                                           |
| tornado_http             | 136 ms                                                 | 98.7 ms: 1.38x faster                                                          |
| deepcopy                 | 479 us                                                 | 354 us: 1.36x faster                                                           |
| chameleon                | 9.68 ms                                                | 7.18 ms: 1.35x faster                                                          |
| logging_format           | 9.09 us                                                | 6.76 us: 1.34x faster                                                          |
| json_dumps               | 14.2 ms                                                | 10.6 ms: 1.34x faster                                                          |
| deepcopy_reduce          | 4.17 us                                                | 3.11 us: 1.34x faster                                                          |
| nbody                    | 154 ms                                                 | 115 ms: 1.33x faster                                                           |
| float                    | 117 ms                                                 | 88.5 ms: 1.32x faster                                                          |
| xml_etree_process        | 79.1 ms                                                | 59.9 ms: 1.32x faster                                                          |
| pprint_safe_repr         | 1.02 sec                                               | 790 ms: 1.29x faster                                                           |
| pprint_pformat           | 2.10 sec                                               | 1.64 sec: 1.29x faster                                                         |
| regex_compile            | 188 ms                                                 | 148 ms: 1.27x faster                                                           |
| hexiom                   | 10.4 ms                                                | 8.21 ms: 1.27x faster                                                          |
| pycparser                | 1.58 sec                                               | 1.25 sec: 1.26x faster                                                         |
| mako                     | 16.3 ms                                                | 13.2 ms: 1.24x faster                                                          |
| spectral_norm            | 170 ms                                                 | 137 ms: 1.24x faster                                                           |
| 2to3                     | 348 ms                                                 | 282 ms: 1.24x faster                                                           |
| tomli_loads              | 3.14 sec                                               | 2.54 sec: 1.24x faster                                                         |
| sqlglot_normalize        | 143 ms                                                 | 116 ms: 1.23x faster                                                           |
| sympy_sum                | 196 ms                                                 | 160 ms: 1.23x faster                                                           |
| fannkuch                 | 532 ms                                                 | 433 ms: 1.23x faster                                                           |
| sympy_integrate          | 25.8 ms                                                | 21.0 ms: 1.23x faster                                                          |
| docutils                 | 3.30 sec                                               | 2.69 sec: 1.22x faster                                                         |
| dulwich_log              | 84.3 ms                                                | 69.4 ms: 1.22x faster                                                          |
| dask                     | 441 ms                                                 | 368 ms: 1.20x faster                                                           |
| sqlglot_optimize         | 69.2 ms                                                | 58.0 ms: 1.19x faster                                                          |
| sympy_str                | 346 ms                                                 | 294 ms: 1.18x faster                                                           |
| bench_thread_pool        | 986 us                                                 | 842 us: 1.17x faster                                                           |
| sympy_expand             | 566 ms                                                 | 495 ms: 1.14x faster                                                           |
| nqueens                  | 106 ms                                                 | 93.5 ms: 1.13x faster                                                          |
| json_loads               | 31.2 us                                                | 27.7 us: 1.13x faster                                                          |
| xml_etree_generate       | 99.4 ms                                                | 88.1 ms: 1.13x faster                                                          |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.75 ms: 1.13x faster                                                          |
| pathlib                  | 20.5 ms                                                | 18.3 ms: 1.12x faster                                                          |
| regex_v8                 | 27.8 ms                                                | 25.0 ms: 1.11x faster                                                          |
| create_gc_cycles         | 1.62 ms                                                | 1.46 ms: 1.11x faster                                                          |
| json                     | 5.69 ms                                                | 5.16 ms: 1.10x faster                                                          |
| scimark_fft              | 466 ms                                                 | 425 ms: 1.10x faster                                                           |
| mdp                      | 2.85 sec                                               | 2.62 sec: 1.09x faster                                                         |
| xml_etree_parse          | 168 ms                                                 | 157 ms: 1.07x faster                                                           |
| xml_etree_iterparse      | 115 ms                                                 | 109 ms: 1.06x faster                                                           |
| meteor_contest           | 120 ms                                                 | 113 ms: 1.06x faster                                                           |
| sqlite_synth             | 3.02 us                                                | 2.86 us: 1.06x faster                                                          |
| unpickle_list            | 5.20 us                                                | 4.99 us: 1.04x faster                                                          |
| gc_traversal             | 3.62 ms                                                | 3.49 ms: 1.04x faster                                                          |
| regex_dna                | 227 ms                                                 | 222 ms: 1.02x faster                                                           |
| pidigits                 | 191 ms                                                 | 188 ms: 1.02x faster                                                           |
| asyncio_websockets       | 559 ms                                                 | 551 ms: 1.01x faster                                                           |
| async_generators         | 444 ms                                                 | 460 ms: 1.04x slower                                                           |
| pickle_list              | 5.08 us                                                | 5.28 us: 1.04x slower                                                          |
| unpickle                 | 14.4 us                                                | 15.3 us: 1.07x slower                                                          |
| pickle                   | 10.7 us                                                | 11.9 us: 1.11x slower                                                          |
| coverage                 | 79.4 ms                                                | 94.7 ms: 1.19x slower                                                          |
| pickle_dict              | 29.6 us                                                | 35.3 us: 1.19x slower                                                          |
| telco                    | 7.27 ms                                                | 8.76 ms: 1.21x slower                                                          |
| python_startup_no_site   | 5.93 ms                                                | 8.83 ms: 1.49x slower                                                          |
| Geometric mean           | (ref)                                                  | 1.29x faster                                                                   |

Benchmark hidden because not significant (3): mypy2, bench_mp_pool, regex_effbot
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240208-3.13.0a3+-7b9e10f-PYTHON_UOPS/bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.23x
- 95% likely to have a speedup of 1.22x
- 99% likely to have a speedup of 1.21x


# Memory

- memory change: 1.06x