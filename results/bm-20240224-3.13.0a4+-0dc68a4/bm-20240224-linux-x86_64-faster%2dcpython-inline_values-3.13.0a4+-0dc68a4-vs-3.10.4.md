# Results vs. 3.10.4

- fork: faster-cpython
- ref: inline_values
- machine: linux-x86_64
- commit hash: 0dc68a4
- commit date: 2024-02-24
- overall geometric mean: 1.36x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.29x faster
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 262 ms: 1.33x faster                                                      |
| chameleon      | 9.68 ms                                                | 6.72 ms: 1.44x faster                                                     |
| docutils       | 3.30 sec                                               | 2.60 sec: 1.27x faster                                                    |
| tornado_http   | 136 ms                                                 | 94.1 ms: 1.45x faster                                                     |
| Geometric mean | (ref)                                                  | 1.37x faster                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|-------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 477 ms: 1.53x faster                                                      |
| async_tree_io           | 1.77 sec                                               | 1.16 sec: 1.52x faster                                                    |
| async_tree_memoization  | 870 ms                                                 | 575 ms: 1.51x faster                                                      |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 725 ms: 1.40x faster                                                      |
| Geometric mean          | (ref)                                                  | 1.49x faster                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 90.6 ms: 1.69x faster                                                     |
| float          | 117 ms                                                 | 79.5 ms: 1.47x faster                                                     |
| pidigits       | 191 ms                                                 | 203 ms: 1.07x slower                                                      |
| Geometric mean | (ref)                                                  | 1.33x faster                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 130 ms: 1.44x faster                                                      |
| regex_v8       | 27.8 ms                                                | 25.0 ms: 1.11x faster                                                     |
| regex_dna      | 227 ms                                                 | 215 ms: 1.06x faster                                                      |
| regex_effbot   | 3.63 ms                                                | 3.55 ms: 1.02x faster                                                     |
| Geometric mean | (ref)                                                  | 1.15x faster                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 294 us: 1.65x faster                                                      |
| unpickle_pure_python | 331 us                                                 | 212 us: 1.56x faster                                                      |
| tomli_loads          | 3.14 sec                                               | 2.15 sec: 1.46x faster                                                    |
| json_dumps           | 14.2 ms                                                | 10.3 ms: 1.37x faster                                                     |
| xml_etree_process    | 79.1 ms                                                | 58.2 ms: 1.36x faster                                                     |
| xml_etree_generate   | 99.4 ms                                                | 85.3 ms: 1.17x faster                                                     |
| json_loads           | 31.2 us                                                | 27.6 us: 1.13x faster                                                     |
| xml_etree_iterparse  | 115 ms                                                 | 105 ms: 1.10x faster                                                      |
| unpickle_list        | 5.20 us                                                | 4.74 us: 1.10x faster                                                     |
| xml_etree_parse      | 168 ms                                                 | 159 ms: 1.06x faster                                                      |
| pickle_list          | 5.08 us                                                | 5.30 us: 1.04x slower                                                     |
| unpickle             | 14.4 us                                                | 15.5 us: 1.08x slower                                                     |
| pickle               | 10.7 us                                                | 11.9 us: 1.11x slower                                                     |
| pickle_dict          | 29.6 us                                                | 35.3 us: 1.19x slower                                                     |
| Geometric mean       | (ref)                                                  | 1.16x faster                                                              |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.42x faster                                                     |
| python_startup_no_site | 5.93 ms                                                | 8.82 ms: 1.49x slower                                                     |
| Geometric mean         | (ref)                                                  | 1.02x slower                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|-----------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.2 ms: 1.46x faster                                                     |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|--------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 110 us: 4.96x faster                                                      |
| generators               | 80.1 ms                                                | 28.6 ms: 2.80x faster                                                     |
| deltablue                | 7.91 ms                                                | 3.17 ms: 2.50x faster                                                     |
| raytrace                 | 507 ms                                                 | 256 ms: 1.98x faster                                                      |
| chaos                    | 115 ms                                                 | 59.2 ms: 1.95x faster                                                     |
| logging_silent           | 190 ns                                                 | 99.7 ns: 1.90x faster                                                     |
| asyncio_tcp              | 922 ms                                                 | 489 ms: 1.89x faster                                                      |
| scimark_sor              | 220 ms                                                 | 119 ms: 1.84x faster                                                      |
| richards_super           | 94.7 ms                                                | 52.6 ms: 1.80x faster                                                     |
| comprehensions           | 28.8 us                                                | 16.0 us: 1.80x faster                                                     |
| crypto_pyaes             | 128 ms                                                 | 71.2 ms: 1.80x faster                                                     |
| scimark_monte_carlo      | 118 ms                                                 | 66.7 ms: 1.77x faster                                                     |
| sqlglot_parse            | 2.17 ms                                                | 1.23 ms: 1.77x faster                                                     |
| go                       | 240 ms                                                 | 137 ms: 1.75x faster                                                      |
| nbody                    | 154 ms                                                 | 90.6 ms: 1.69x faster                                                     |
| hexiom                   | 10.4 ms                                                | 6.16 ms: 1.69x faster                                                     |
| richards                 | 79.3 ms                                                | 47.3 ms: 1.68x faster                                                     |
| sqlglot_transpile        | 2.57 ms                                                | 1.55 ms: 1.66x faster                                                     |
| pickle_pure_python       | 484 us                                                 | 294 us: 1.65x faster                                                      |
| coroutines               | 35.1 ms                                                | 21.5 ms: 1.63x faster                                                     |
| pyflate                  | 716 ms                                                 | 449 ms: 1.59x faster                                                      |
| spectral_norm            | 170 ms                                                 | 107 ms: 1.59x faster                                                      |
| scimark_lu               | 176 ms                                                 | 112 ms: 1.57x faster                                                      |
| unpickle_pure_python     | 331 us                                                 | 212 us: 1.56x faster                                                      |
| deepcopy_memo            | 58.5 us                                                | 38.1 us: 1.53x faster                                                     |
| async_tree_none          | 728 ms                                                 | 477 ms: 1.53x faster                                                      |
| async_tree_io            | 1.77 sec                                               | 1.16 sec: 1.52x faster                                                    |
| async_tree_memoization   | 870 ms                                                 | 575 ms: 1.51x faster                                                      |
| logging_format           | 9.09 us                                                | 6.12 us: 1.49x faster                                                     |
| logging_simple           | 8.30 us                                                | 5.63 us: 1.47x faster                                                     |
| float                    | 117 ms                                                 | 79.5 ms: 1.47x faster                                                     |
| mako                     | 16.3 ms                                                | 11.2 ms: 1.46x faster                                                     |
| tomli_loads              | 3.14 sec                                               | 2.15 sec: 1.46x faster                                                    |
| tornado_http             | 136 ms                                                 | 94.1 ms: 1.45x faster                                                     |
| regex_compile            | 188 ms                                                 | 130 ms: 1.44x faster                                                      |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.78 sec: 1.44x faster                                                    |
| chameleon                | 9.68 ms                                                | 6.72 ms: 1.44x faster                                                     |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.42x faster                                                     |
| pprint_pformat           | 2.10 sec                                               | 1.48 sec: 1.42x faster                                                    |
| pprint_safe_repr         | 1.02 sec                                               | 723 ms: 1.41x faster                                                      |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 725 ms: 1.40x faster                                                      |
| deepcopy                 | 479 us                                                 | 343 us: 1.40x faster                                                      |
| fannkuch                 | 532 ms                                                 | 384 ms: 1.39x faster                                                      |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.71 ms: 1.37x faster                                                     |
| json_dumps               | 14.2 ms                                                | 10.3 ms: 1.37x faster                                                     |
| deepcopy_reduce          | 4.17 us                                                | 3.05 us: 1.37x faster                                                     |
| xml_etree_process        | 79.1 ms                                                | 58.2 ms: 1.36x faster                                                     |
| sqlglot_normalize        | 143 ms                                                 | 106 ms: 1.35x faster                                                      |
| pycparser                | 1.58 sec                                               | 1.18 sec: 1.34x faster                                                    |
| 2to3                     | 348 ms                                                 | 262 ms: 1.33x faster                                                      |
| sympy_sum                | 196 ms                                                 | 148 ms: 1.32x faster                                                      |
| nqueens                  | 106 ms                                                 | 80.5 ms: 1.31x faster                                                     |
| sympy_integrate          | 25.8 ms                                                | 19.7 ms: 1.31x faster                                                     |
| sqlglot_optimize         | 69.2 ms                                                | 52.9 ms: 1.31x faster                                                     |
| sympy_str                | 346 ms                                                 | 267 ms: 1.30x faster                                                      |
| scimark_fft              | 466 ms                                                 | 361 ms: 1.29x faster                                                      |
| dulwich_log              | 84.3 ms                                                | 66.5 ms: 1.27x faster                                                     |
| docutils                 | 3.30 sec                                               | 2.60 sec: 1.27x faster                                                    |
| sympy_expand             | 566 ms                                                 | 452 ms: 1.25x faster                                                      |
| bench_thread_pool        | 986 us                                                 | 820 us: 1.20x faster                                                      |
| unpack_sequence          | 60.0 ns                                                | 50.5 ns: 1.19x faster                                                     |
| xml_etree_generate       | 99.4 ms                                                | 85.3 ms: 1.17x faster                                                     |
| meteor_contest           | 120 ms                                                 | 104 ms: 1.15x faster                                                      |
| mdp                      | 2.85 sec                                               | 2.50 sec: 1.14x faster                                                    |
| json_loads               | 31.2 us                                                | 27.6 us: 1.13x faster                                                     |
| json                     | 5.69 ms                                                | 5.08 ms: 1.12x faster                                                     |
| pathlib                  | 20.5 ms                                                | 18.3 ms: 1.12x faster                                                     |
| regex_v8                 | 27.8 ms                                                | 25.0 ms: 1.11x faster                                                     |
| xml_etree_iterparse      | 115 ms                                                 | 105 ms: 1.10x faster                                                      |
| unpickle_list            | 5.20 us                                                | 4.74 us: 1.10x faster                                                     |
| xml_etree_parse          | 168 ms                                                 | 159 ms: 1.06x faster                                                      |
| regex_dna                | 227 ms                                                 | 215 ms: 1.06x faster                                                      |
| sqlite_synth             | 3.02 us                                                | 2.88 us: 1.05x faster                                                     |
| create_gc_cycles         | 1.62 ms                                                | 1.56 ms: 1.04x faster                                                     |
| regex_effbot             | 3.63 ms                                                | 3.55 ms: 1.02x faster                                                     |
| asyncio_websockets       | 559 ms                                                 | 551 ms: 1.01x faster                                                      |
| async_generators         | 444 ms                                                 | 448 ms: 1.01x slower                                                      |
| gc_traversal             | 3.62 ms                                                | 3.73 ms: 1.03x slower                                                     |
| pickle_list              | 5.08 us                                                | 5.30 us: 1.04x slower                                                     |
| pidigits                 | 191 ms                                                 | 203 ms: 1.07x slower                                                      |
| unpickle                 | 14.4 us                                                | 15.5 us: 1.08x slower                                                     |
| pickle                   | 10.7 us                                                | 11.9 us: 1.11x slower                                                     |
| telco                    | 7.27 ms                                                | 8.42 ms: 1.16x slower                                                     |
| pickle_dict              | 29.6 us                                                | 35.3 us: 1.19x slower                                                     |
| coverage                 | 79.4 ms                                                | 97.1 ms: 1.22x slower                                                     |
| python_startup_no_site   | 5.93 ms                                                | 8.82 ms: 1.49x slower                                                     |
| Geometric mean           | (ref)                                                  | 1.36x faster                                                              |

Benchmark hidden because not significant (2): mypy2, bench_mp_pool
Ignored benchmarks (13) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240224-3.13.0a4+-0dc68a4/bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.32x
- 95% likely to have a speedup of 1.31x
- 99% likely to have a speedup of 1.29x


# Memory

- memory change: 1.07x