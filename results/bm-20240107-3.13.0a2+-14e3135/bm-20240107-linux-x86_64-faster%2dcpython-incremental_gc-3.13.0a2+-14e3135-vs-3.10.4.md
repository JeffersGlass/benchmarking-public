
# Results vs. 3.10.4

- fork: faster-cpython
- ref: incremental_gc
- machine: linux-x86_64
- commit hash: 14e3135
- commit date: 2024-01-07
- overall geometric mean: 1.36x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.28x faster
- Memory change: 1.08x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 270 ms: 1.29x faster                                                       |
| chameleon      | 9.68 ms                                                | 6.97 ms: 1.39x faster                                                      |
| docutils       | 3.30 sec                                               | 2.53 sec: 1.31x faster                                                     |
| tornado_http   | 136 ms                                                 | 93.6 ms: 1.46x faster                                                      |
| Geometric mean | (ref)                                                  | 1.36x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_io           | 1.77 sec                                               | 804 ms: 2.20x faster                                                       |
| async_tree_none         | 728 ms                                                 | 356 ms: 2.05x faster                                                       |
| async_tree_memoization  | 870 ms                                                 | 459 ms: 1.90x faster                                                       |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 625 ms: 1.63x faster                                                       |
| Geometric mean          | (ref)                                                  | 1.93x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 91.6 ms: 1.68x faster                                                      |
| float          | 117 ms                                                 | 85.8 ms: 1.36x faster                                                      |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                                       |
| Geometric mean | (ref)                                                  | 1.33x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 131 ms: 1.44x faster                                                       |
| regex_v8       | 27.8 ms                                                | 25.5 ms: 1.09x faster                                                      |
| Geometric mean | (ref)                                                  | 1.12x faster                                                               |

Benchmark hidden because not significant (2): regex_dna, regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 298 us: 1.63x faster                                                       |
| unpickle_pure_python | 331 us                                                 | 216 us: 1.53x faster                                                       |
| tomli_loads          | 3.14 sec                                               | 2.17 sec: 1.45x faster                                                     |
| json_dumps           | 14.2 ms                                                | 10.5 ms: 1.35x faster                                                      |
| xml_etree_process    | 79.1 ms                                                | 60.7 ms: 1.30x faster                                                      |
| xml_etree_generate   | 99.4 ms                                                | 90.2 ms: 1.10x faster                                                      |
| json_loads           | 31.2 us                                                | 28.4 us: 1.10x faster                                                      |
| pickle_list          | 5.08 us                                                | 5.00 us: 1.02x faster                                                      |
| unpickle             | 14.4 us                                                | 14.9 us: 1.03x slower                                                      |
| unpickle_list        | 5.20 us                                                | 5.47 us: 1.05x slower                                                      |
| pickle               | 10.7 us                                                | 11.5 us: 1.08x slower                                                      |
| xml_etree_iterparse  | 115 ms                                                 | 130 ms: 1.13x slower                                                       |
| pickle_dict          | 29.6 us                                                | 34.6 us: 1.17x slower                                                      |
| xml_etree_parse      | 168 ms                                                 | 205 ms: 1.22x slower                                                       |
| Geometric mean       | (ref)                                                  | 1.11x faster                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                      |
| python_startup_no_site | 5.93 ms                                                | 8.55 ms: 1.44x slower                                                      |
| Geometric mean         | (ref)                                                  | 1.00x slower                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.4 ms: 1.43x faster                                                      |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 112 us: 4.86x faster                                                       |
| generators               | 80.1 ms                                                | 29.7 ms: 2.69x faster                                                      |
| deltablue                | 7.91 ms                                                | 3.22 ms: 2.46x faster                                                      |
| async_tree_io            | 1.77 sec                                               | 804 ms: 2.20x faster                                                       |
| async_tree_none          | 728 ms                                                 | 356 ms: 2.05x faster                                                       |
| asyncio_tcp              | 922 ms                                                 | 475 ms: 1.94x faster                                                       |
| raytrace                 | 507 ms                                                 | 263 ms: 1.93x faster                                                       |
| chaos                    | 115 ms                                                 | 60.1 ms: 1.92x faster                                                      |
| async_tree_memoization   | 870 ms                                                 | 459 ms: 1.90x faster                                                       |
| scimark_sor              | 220 ms                                                 | 119 ms: 1.84x faster                                                       |
| logging_silent           | 190 ns                                                 | 104 ns: 1.82x faster                                                       |
| crypto_pyaes             | 128 ms                                                 | 72.0 ms: 1.77x faster                                                      |
| comprehensions           | 28.8 us                                                | 16.3 us: 1.77x faster                                                      |
| richards_super           | 94.7 ms                                                | 54.0 ms: 1.76x faster                                                      |
| scimark_monte_carlo      | 118 ms                                                 | 68.3 ms: 1.73x faster                                                      |
| go                       | 240 ms                                                 | 140 ms: 1.71x faster                                                       |
| sqlglot_parse            | 2.17 ms                                                | 1.27 ms: 1.70x faster                                                      |
| hexiom                   | 10.4 ms                                                | 6.20 ms: 1.68x faster                                                      |
| nbody                    | 154 ms                                                 | 91.6 ms: 1.68x faster                                                      |
| richards                 | 79.3 ms                                                | 47.6 ms: 1.67x faster                                                      |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 625 ms: 1.63x faster                                                       |
| pickle_pure_python       | 484 us                                                 | 298 us: 1.63x faster                                                       |
| sqlglot_transpile        | 2.57 ms                                                | 1.59 ms: 1.62x faster                                                      |
| scimark_lu               | 176 ms                                                 | 112 ms: 1.57x faster                                                       |
| spectral_norm            | 170 ms                                                 | 109 ms: 1.55x faster                                                       |
| unpickle_pure_python     | 331 us                                                 | 216 us: 1.53x faster                                                       |
| pyflate                  | 716 ms                                                 | 468 ms: 1.53x faster                                                       |
| coroutines               | 35.1 ms                                                | 22.9 ms: 1.53x faster                                                      |
| deepcopy_memo            | 58.5 us                                                | 38.3 us: 1.52x faster                                                      |
| logging_simple           | 8.30 us                                                | 5.69 us: 1.46x faster                                                      |
| tornado_http             | 136 ms                                                 | 93.6 ms: 1.46x faster                                                      |
| tomli_loads              | 3.14 sec                                               | 2.17 sec: 1.45x faster                                                     |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.78 sec: 1.45x faster                                                     |
| logging_format           | 9.09 us                                                | 6.30 us: 1.44x faster                                                      |
| regex_compile            | 188 ms                                                 | 131 ms: 1.44x faster                                                       |
| unpack_sequence          | 60.0 ns                                                | 41.8 ns: 1.44x faster                                                      |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                      |
| mako                     | 16.3 ms                                                | 11.4 ms: 1.43x faster                                                      |
| pprint_pformat           | 2.10 sec                                               | 1.49 sec: 1.41x faster                                                     |
| pprint_safe_repr         | 1.02 sec                                               | 727 ms: 1.40x faster                                                       |
| chameleon                | 9.68 ms                                                | 6.97 ms: 1.39x faster                                                      |
| deepcopy                 | 479 us                                                 | 347 us: 1.38x faster                                                       |
| pycparser                | 1.58 sec                                               | 1.15 sec: 1.37x faster                                                     |
| float                    | 117 ms                                                 | 85.8 ms: 1.36x faster                                                      |
| json_dumps               | 14.2 ms                                                | 10.5 ms: 1.35x faster                                                      |
| sqlglot_normalize        | 143 ms                                                 | 106 ms: 1.34x faster                                                       |
| sympy_sum                | 196 ms                                                 | 147 ms: 1.33x faster                                                       |
| deepcopy_reduce          | 4.17 us                                                | 3.13 us: 1.33x faster                                                      |
| sympy_integrate          | 25.8 ms                                                | 19.5 ms: 1.32x faster                                                      |
| nqueens                  | 106 ms                                                 | 80.7 ms: 1.31x faster                                                      |
| docutils                 | 3.30 sec                                               | 2.53 sec: 1.31x faster                                                     |
| xml_etree_process        | 79.1 ms                                                | 60.7 ms: 1.30x faster                                                      |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.98 ms: 1.30x faster                                                      |
| sympy_str                | 346 ms                                                 | 267 ms: 1.30x faster                                                       |
| sqlglot_optimize         | 69.2 ms                                                | 53.6 ms: 1.29x faster                                                      |
| 2to3                     | 348 ms                                                 | 270 ms: 1.29x faster                                                       |
| fannkuch                 | 532 ms                                                 | 415 ms: 1.28x faster                                                       |
| scimark_fft              | 466 ms                                                 | 364 ms: 1.28x faster                                                       |
| dulwich_log              | 84.3 ms                                                | 66.3 ms: 1.27x faster                                                      |
| sympy_expand             | 566 ms                                                 | 453 ms: 1.25x faster                                                       |
| dask                     | 441 ms                                                 | 355 ms: 1.24x faster                                                       |
| mypy2                    | 894 ms                                                 | 745 ms: 1.20x faster                                                       |
| bench_thread_pool        | 986 us                                                 | 831 us: 1.19x faster                                                       |
| create_gc_cycles         | 1.62 ms                                                | 1.44 ms: 1.13x faster                                                      |
| pathlib                  | 20.5 ms                                                | 18.4 ms: 1.11x faster                                                      |
| meteor_contest           | 120 ms                                                 | 108 ms: 1.10x faster                                                       |
| xml_etree_generate       | 99.4 ms                                                | 90.2 ms: 1.10x faster                                                      |
| json_loads               | 31.2 us                                                | 28.4 us: 1.10x faster                                                      |
| regex_v8                 | 27.8 ms                                                | 25.5 ms: 1.09x faster                                                      |
| json                     | 5.69 ms                                                | 5.24 ms: 1.09x faster                                                      |
| sqlite_synth             | 3.02 us                                                | 2.84 us: 1.06x faster                                                      |
| mdp                      | 2.85 sec                                               | 2.72 sec: 1.05x faster                                                     |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                                       |
| pickle_list              | 5.08 us                                                | 5.00 us: 1.02x faster                                                      |
| asyncio_websockets       | 559 ms                                                 | 553 ms: 1.01x faster                                                       |
| async_generators         | 444 ms                                                 | 442 ms: 1.00x faster                                                       |
| unpickle                 | 14.4 us                                                | 14.9 us: 1.03x slower                                                      |
| unpickle_list            | 5.20 us                                                | 5.47 us: 1.05x slower                                                      |
| pickle                   | 10.7 us                                                | 11.5 us: 1.08x slower                                                      |
| gc_traversal             | 3.62 ms                                                | 3.93 ms: 1.08x slower                                                      |
| xml_etree_iterparse      | 115 ms                                                 | 130 ms: 1.13x slower                                                       |
| pickle_dict              | 29.6 us                                                | 34.6 us: 1.17x slower                                                      |
| coverage                 | 79.4 ms                                                | 94.6 ms: 1.19x slower                                                      |
| telco                    | 7.27 ms                                                | 8.66 ms: 1.19x slower                                                      |
| xml_etree_parse          | 168 ms                                                 | 205 ms: 1.22x slower                                                       |
| python_startup_no_site   | 5.93 ms                                                | 8.55 ms: 1.44x slower                                                      |
| Geometric mean           | (ref)                                                  | 1.36x faster                                                               |

Benchmark hidden because not significant (3): regex_dna, bench_mp_pool, regex_effbot
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240107-3.13.0a2+-14e3135/bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.30x
- 95% likely to have a speedup of 1.29x
- 99% likely to have a speedup of 1.28x


# Memory

- memory change: 1.08x