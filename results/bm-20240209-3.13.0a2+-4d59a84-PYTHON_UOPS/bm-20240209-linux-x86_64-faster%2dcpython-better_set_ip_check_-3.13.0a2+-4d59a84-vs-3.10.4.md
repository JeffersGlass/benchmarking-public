
# Results vs. 3.10.4

- fork: faster-cpython
- ref: better_set_ip_check_
- machine: linux-x86_64
- commit hash: 4d59a84
- commit date: 2024-02-09
- overall geometric mean: 1.27x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.20x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 282 ms: 1.24x faster                                                             |
| chameleon      | 9.68 ms                                                | 7.34 ms: 1.32x faster                                                            |
| docutils       | 3.30 sec                                               | 2.70 sec: 1.22x faster                                                           |
| tornado_http   | 136 ms                                                 | 98.5 ms: 1.38x faster                                                            |
| Geometric mean | (ref)                                                  | 1.29x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 452 ms: 1.61x faster                                                             |
| async_tree_memoization  | 870 ms                                                 | 576 ms: 1.51x faster                                                             |
| async_tree_io           | 1.77 sec                                               | 1.21 sec: 1.47x faster                                                           |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 724 ms: 1.40x faster                                                             |
| Geometric mean          | (ref)                                                  | 1.50x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 114 ms: 1.35x faster                                                             |
| float          | 117 ms                                                 | 91.8 ms: 1.28x faster                                                            |
| pidigits       | 191 ms                                                 | 188 ms: 1.01x faster                                                             |
| Geometric mean | (ref)                                                  | 1.20x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 151 ms: 1.24x faster                                                             |
| regex_v8       | 27.8 ms                                                | 25.2 ms: 1.10x faster                                                            |
| regex_dna      | 227 ms                                                 | 227 ms: 1.00x slower                                                             |
| Geometric mean | (ref)                                                  | 1.08x faster                                                                     |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 303 us: 1.60x faster                                                             |
| unpickle_pure_python | 331 us                                                 | 233 us: 1.42x faster                                                             |
| json_dumps           | 14.2 ms                                                | 10.6 ms: 1.33x faster                                                            |
| tomli_loads          | 3.14 sec                                               | 2.37 sec: 1.33x faster                                                           |
| xml_etree_process    | 79.1 ms                                                | 60.5 ms: 1.31x faster                                                            |
| xml_etree_generate   | 99.4 ms                                                | 88.8 ms: 1.12x faster                                                            |
| json_loads           | 31.2 us                                                | 28.1 us: 1.11x faster                                                            |
| xml_etree_parse      | 168 ms                                                 | 158 ms: 1.07x faster                                                             |
| xml_etree_iterparse  | 115 ms                                                 | 110 ms: 1.05x faster                                                             |
| unpickle             | 14.4 us                                                | 14.7 us: 1.02x slower                                                            |
| pickle_list          | 5.08 us                                                | 5.26 us: 1.04x slower                                                            |
| pickle               | 10.7 us                                                | 11.4 us: 1.07x slower                                                            |
| pickle_dict          | 29.6 us                                                | 35.8 us: 1.21x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.13x faster                                                                     |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                            |
| python_startup_no_site | 5.93 ms                                                | 8.74 ms: 1.47x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 13.6 ms: 1.20x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 117 us: 4.65x faster                                                             |
| generators               | 80.1 ms                                                | 29.4 ms: 2.72x faster                                                            |
| asyncio_tcp              | 922 ms                                                 | 494 ms: 1.87x faster                                                             |
| logging_silent           | 190 ns                                                 | 107 ns: 1.77x faster                                                             |
| scimark_sor              | 220 ms                                                 | 126 ms: 1.75x faster                                                             |
| deltablue                | 7.91 ms                                                | 4.53 ms: 1.75x faster                                                            |
| raytrace                 | 507 ms                                                 | 297 ms: 1.71x faster                                                             |
| richards_super           | 94.7 ms                                                | 55.7 ms: 1.70x faster                                                            |
| sqlglot_parse            | 2.17 ms                                                | 1.33 ms: 1.63x faster                                                            |
| richards                 | 79.3 ms                                                | 48.9 ms: 1.62x faster                                                            |
| async_tree_none          | 728 ms                                                 | 452 ms: 1.61x faster                                                             |
| chaos                    | 115 ms                                                 | 72.2 ms: 1.60x faster                                                            |
| pickle_pure_python       | 484 us                                                 | 303 us: 1.60x faster                                                             |
| coroutines               | 35.1 ms                                                | 22.4 ms: 1.56x faster                                                            |
| sqlglot_transpile        | 2.57 ms                                                | 1.66 ms: 1.55x faster                                                            |
| crypto_pyaes             | 128 ms                                                 | 83.2 ms: 1.54x faster                                                            |
| go                       | 240 ms                                                 | 156 ms: 1.53x faster                                                             |
| async_tree_memoization   | 870 ms                                                 | 576 ms: 1.51x faster                                                             |
| scimark_lu               | 176 ms                                                 | 119 ms: 1.48x faster                                                             |
| scimark_monte_carlo      | 118 ms                                                 | 79.9 ms: 1.48x faster                                                            |
| async_tree_io            | 1.77 sec                                               | 1.21 sec: 1.47x faster                                                           |
| deepcopy_memo            | 58.5 us                                                | 40.3 us: 1.45x faster                                                            |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                            |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                                           |
| unpickle_pure_python     | 331 us                                                 | 233 us: 1.42x faster                                                             |
| pyflate                  | 716 ms                                                 | 508 ms: 1.41x faster                                                             |
| unpack_sequence          | 60.0 ns                                                | 42.7 ns: 1.41x faster                                                            |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 724 ms: 1.40x faster                                                             |
| comprehensions           | 28.8 us                                                | 20.6 us: 1.40x faster                                                            |
| tornado_http             | 136 ms                                                 | 98.5 ms: 1.38x faster                                                            |
| logging_simple           | 8.30 us                                                | 6.02 us: 1.38x faster                                                            |
| nbody                    | 154 ms                                                 | 114 ms: 1.35x faster                                                             |
| deepcopy                 | 479 us                                                 | 357 us: 1.34x faster                                                             |
| logging_format           | 9.09 us                                                | 6.79 us: 1.34x faster                                                            |
| json_dumps               | 14.2 ms                                                | 10.6 ms: 1.33x faster                                                            |
| deepcopy_reduce          | 4.17 us                                                | 3.14 us: 1.33x faster                                                            |
| tomli_loads              | 3.14 sec                                               | 2.37 sec: 1.33x faster                                                           |
| chameleon                | 9.68 ms                                                | 7.34 ms: 1.32x faster                                                            |
| pycparser                | 1.58 sec                                               | 1.20 sec: 1.32x faster                                                           |
| xml_etree_process        | 79.1 ms                                                | 60.5 ms: 1.31x faster                                                            |
| float                    | 117 ms                                                 | 91.8 ms: 1.28x faster                                                            |
| hexiom                   | 10.4 ms                                                | 8.24 ms: 1.26x faster                                                            |
| pprint_safe_repr         | 1.02 sec                                               | 811 ms: 1.26x faster                                                             |
| sqlglot_normalize        | 143 ms                                                 | 114 ms: 1.25x faster                                                             |
| pprint_pformat           | 2.10 sec                                               | 1.69 sec: 1.25x faster                                                           |
| regex_compile            | 188 ms                                                 | 151 ms: 1.24x faster                                                             |
| 2to3                     | 348 ms                                                 | 282 ms: 1.24x faster                                                             |
| sympy_sum                | 196 ms                                                 | 160 ms: 1.23x faster                                                             |
| dulwich_log              | 84.3 ms                                                | 68.9 ms: 1.22x faster                                                            |
| docutils                 | 3.30 sec                                               | 2.70 sec: 1.22x faster                                                           |
| sympy_integrate          | 25.8 ms                                                | 21.2 ms: 1.22x faster                                                            |
| fannkuch                 | 532 ms                                                 | 437 ms: 1.22x faster                                                             |
| mako                     | 16.3 ms                                                | 13.6 ms: 1.20x faster                                                            |
| sqlglot_optimize         | 69.2 ms                                                | 57.7 ms: 1.20x faster                                                            |
| dask                     | 441 ms                                                 | 368 ms: 1.20x faster                                                             |
| spectral_norm            | 170 ms                                                 | 143 ms: 1.19x faster                                                             |
| sympy_str                | 346 ms                                                 | 292 ms: 1.19x faster                                                             |
| bench_thread_pool        | 986 us                                                 | 850 us: 1.16x faster                                                             |
| sympy_expand             | 566 ms                                                 | 490 ms: 1.16x faster                                                             |
| xml_etree_generate       | 99.4 ms                                                | 88.8 ms: 1.12x faster                                                            |
| nqueens                  | 106 ms                                                 | 95.0 ms: 1.11x faster                                                            |
| json_loads               | 31.2 us                                                | 28.1 us: 1.11x faster                                                            |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.84 ms: 1.11x faster                                                            |
| pathlib                  | 20.5 ms                                                | 18.5 ms: 1.10x faster                                                            |
| create_gc_cycles         | 1.62 ms                                                | 1.47 ms: 1.10x faster                                                            |
| regex_v8                 | 27.8 ms                                                | 25.2 ms: 1.10x faster                                                            |
| json                     | 5.69 ms                                                | 5.26 ms: 1.08x faster                                                            |
| mdp                      | 2.85 sec                                               | 2.67 sec: 1.07x faster                                                           |
| xml_etree_parse          | 168 ms                                                 | 158 ms: 1.07x faster                                                             |
| meteor_contest           | 120 ms                                                 | 113 ms: 1.06x faster                                                             |
| scimark_fft              | 466 ms                                                 | 441 ms: 1.06x faster                                                             |
| xml_etree_iterparse      | 115 ms                                                 | 110 ms: 1.05x faster                                                             |
| sqlite_synth             | 3.02 us                                                | 2.90 us: 1.04x faster                                                            |
| pidigits                 | 191 ms                                                 | 188 ms: 1.01x faster                                                             |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                             |
| regex_dna                | 227 ms                                                 | 227 ms: 1.00x slower                                                             |
| async_generators         | 444 ms                                                 | 450 ms: 1.01x slower                                                             |
| unpickle                 | 14.4 us                                                | 14.7 us: 1.02x slower                                                            |
| gc_traversal             | 3.62 ms                                                | 3.70 ms: 1.02x slower                                                            |
| pickle_list              | 5.08 us                                                | 5.26 us: 1.04x slower                                                            |
| pickle                   | 10.7 us                                                | 11.4 us: 1.07x slower                                                            |
| telco                    | 7.27 ms                                                | 8.57 ms: 1.18x slower                                                            |
| coverage                 | 79.4 ms                                                | 95.4 ms: 1.20x slower                                                            |
| pickle_dict              | 29.6 us                                                | 35.8 us: 1.21x slower                                                            |
| python_startup_no_site   | 5.93 ms                                                | 8.74 ms: 1.47x slower                                                            |
| Geometric mean           | (ref)                                                  | 1.27x faster                                                                     |

Benchmark hidden because not significant (4): mypy2, unpickle_list, bench_mp_pool, regex_effbot
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240209-3.13.0a2+-4d59a84-PYTHON_UOPS/bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.22x
- 95% likely to have a speedup of 1.22x
- 99% likely to have a speedup of 1.20x


# Memory

- memory change: 1.06x