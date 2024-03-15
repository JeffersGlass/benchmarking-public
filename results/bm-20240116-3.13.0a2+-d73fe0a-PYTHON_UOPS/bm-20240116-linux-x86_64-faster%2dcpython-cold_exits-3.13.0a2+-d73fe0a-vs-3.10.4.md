
# Results vs. 3.10.4

- fork: faster-cpython
- ref: cold_exits
- machine: linux-x86_64
- commit hash: d73fe0a
- commit date: 2024-01-16
- overall geometric mean: 1.22x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.14x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 290 ms: 1.20x faster                                                   |
| chameleon      | 9.68 ms                                                | 7.32 ms: 1.32x faster                                                  |
| docutils       | 3.30 sec                                               | 2.85 sec: 1.16x faster                                                 |
| tornado_http   | 136 ms                                                 | 98.0 ms: 1.39x faster                                                  |
| Geometric mean | (ref)                                                  | 1.26x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 450 ms: 1.62x faster                                                   |
| async_tree_memoization  | 870 ms                                                 | 578 ms: 1.51x faster                                                   |
| async_tree_io           | 1.77 sec                                               | 1.21 sec: 1.46x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 722 ms: 1.41x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.50x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 120 ms: 1.28x faster                                                   |
| float          | 117 ms                                                 | 93.4 ms: 1.25x faster                                                  |
| pidigits       | 191 ms                                                 | 189 ms: 1.01x faster                                                   |
| Geometric mean | (ref)                                                  | 1.18x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_v8       | 27.8 ms                                                | 25.2 ms: 1.10x faster                                                  |
| regex_compile  | 188 ms                                                 | 172 ms: 1.10x faster                                                   |
| regex_dna      | 227 ms                                                 | 227 ms: 1.00x slower                                                   |
| Geometric mean | (ref)                                                  | 1.05x faster                                                           |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 299 us: 1.62x faster                                                   |
| json_dumps           | 14.2 ms                                                | 10.6 ms: 1.34x faster                                                  |
| xml_etree_process    | 79.1 ms                                                | 62.2 ms: 1.27x faster                                                  |
| unpickle_pure_python | 331 us                                                 | 278 us: 1.19x faster                                                   |
| tomli_loads          | 3.14 sec                                               | 2.73 sec: 1.15x faster                                                 |
| json_loads           | 31.2 us                                                | 28.4 us: 1.10x faster                                                  |
| xml_etree_generate   | 99.4 ms                                                | 90.8 ms: 1.09x faster                                                  |
| xml_etree_parse      | 168 ms                                                 | 158 ms: 1.07x faster                                                   |
| unpickle_list        | 5.20 us                                                | 4.93 us: 1.06x faster                                                  |
| xml_etree_iterparse  | 115 ms                                                 | 112 ms: 1.03x faster                                                   |
| unpickle             | 14.4 us                                                | 14.8 us: 1.03x slower                                                  |
| pickle_list          | 5.08 us                                                | 5.34 us: 1.05x slower                                                  |
| pickle               | 10.7 us                                                | 11.4 us: 1.07x slower                                                  |
| pickle_dict          | 29.6 us                                                | 37.0 us: 1.25x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.10x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                  |
| python_startup_no_site | 5.93 ms                                                | 8.74 ms: 1.47x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 14.0 ms: 1.17x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 116 us: 4.68x faster                                                   |
| generators               | 80.1 ms                                                | 29.4 ms: 2.73x faster                                                  |
| asyncio_tcp              | 922 ms                                                 | 495 ms: 1.86x faster                                                   |
| logging_silent           | 190 ns                                                 | 106 ns: 1.79x faster                                                   |
| pickle_pure_python       | 484 us                                                 | 299 us: 1.62x faster                                                   |
| async_tree_none          | 728 ms                                                 | 450 ms: 1.62x faster                                                   |
| raytrace                 | 507 ms                                                 | 316 ms: 1.60x faster                                                   |
| coroutines               | 35.1 ms                                                | 22.4 ms: 1.57x faster                                                  |
| deltablue                | 7.91 ms                                                | 5.14 ms: 1.54x faster                                                  |
| chaos                    | 115 ms                                                 | 75.7 ms: 1.52x faster                                                  |
| sqlglot_parse            | 2.17 ms                                                | 1.42 ms: 1.52x faster                                                  |
| crypto_pyaes             | 128 ms                                                 | 84.6 ms: 1.51x faster                                                  |
| async_tree_memoization   | 870 ms                                                 | 578 ms: 1.51x faster                                                   |
| sqlglot_transpile        | 2.57 ms                                                | 1.75 ms: 1.47x faster                                                  |
| scimark_sor              | 220 ms                                                 | 150 ms: 1.47x faster                                                   |
| async_tree_io            | 1.77 sec                                               | 1.21 sec: 1.46x faster                                                 |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.81 sec: 1.42x faster                                                 |
| deepcopy_memo            | 58.5 us                                                | 41.3 us: 1.42x faster                                                  |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 722 ms: 1.41x faster                                                   |
| tornado_http             | 136 ms                                                 | 98.0 ms: 1.39x faster                                                  |
| go                       | 240 ms                                                 | 176 ms: 1.36x faster                                                   |
| deepcopy                 | 479 us                                                 | 358 us: 1.34x faster                                                   |
| json_dumps               | 14.2 ms                                                | 10.6 ms: 1.34x faster                                                  |
| deepcopy_reduce          | 4.17 us                                                | 3.15 us: 1.33x faster                                                  |
| chameleon                | 9.68 ms                                                | 7.32 ms: 1.32x faster                                                  |
| scimark_monte_carlo      | 118 ms                                                 | 89.4 ms: 1.32x faster                                                  |
| comprehensions           | 28.8 us                                                | 22.0 us: 1.31x faster                                                  |
| logging_simple           | 8.30 us                                                | 6.44 us: 1.29x faster                                                  |
| nbody                    | 154 ms                                                 | 120 ms: 1.28x faster                                                   |
| xml_etree_process        | 79.1 ms                                                | 62.2 ms: 1.27x faster                                                  |
| logging_format           | 9.09 us                                                | 7.24 us: 1.26x faster                                                  |
| float                    | 117 ms                                                 | 93.4 ms: 1.25x faster                                                  |
| pyflate                  | 716 ms                                                 | 579 ms: 1.24x faster                                                   |
| pycparser                | 1.58 sec                                               | 1.28 sec: 1.23x faster                                                 |
| richards_super           | 94.7 ms                                                | 77.6 ms: 1.22x faster                                                  |
| 2to3                     | 348 ms                                                 | 290 ms: 1.20x faster                                                   |
| sqlglot_normalize        | 143 ms                                                 | 119 ms: 1.20x faster                                                   |
| sympy_sum                | 196 ms                                                 | 164 ms: 1.20x faster                                                   |
| dask                     | 441 ms                                                 | 370 ms: 1.19x faster                                                   |
| unpickle_pure_python     | 331 us                                                 | 278 us: 1.19x faster                                                   |
| dulwich_log              | 84.3 ms                                                | 71.3 ms: 1.18x faster                                                  |
| sympy_integrate          | 25.8 ms                                                | 21.8 ms: 1.18x faster                                                  |
| pprint_pformat           | 2.10 sec                                               | 1.80 sec: 1.17x faster                                                 |
| mako                     | 16.3 ms                                                | 14.0 ms: 1.17x faster                                                  |
| pprint_safe_repr         | 1.02 sec                                               | 873 ms: 1.17x faster                                                   |
| richards                 | 79.3 ms                                                | 68.4 ms: 1.16x faster                                                  |
| docutils                 | 3.30 sec                                               | 2.85 sec: 1.16x faster                                                 |
| scimark_lu               | 176 ms                                                 | 152 ms: 1.16x faster                                                   |
| bench_thread_pool        | 986 us                                                 | 855 us: 1.15x faster                                                   |
| tomli_loads              | 3.14 sec                                               | 2.73 sec: 1.15x faster                                                 |
| sympy_str                | 346 ms                                                 | 302 ms: 1.14x faster                                                   |
| spectral_norm            | 170 ms                                                 | 149 ms: 1.14x faster                                                   |
| sqlglot_optimize         | 69.2 ms                                                | 61.5 ms: 1.12x faster                                                  |
| sympy_expand             | 566 ms                                                 | 503 ms: 1.12x faster                                                   |
| hexiom                   | 10.4 ms                                                | 9.28 ms: 1.12x faster                                                  |
| unpack_sequence          | 60.0 ns                                                | 54.3 ns: 1.10x faster                                                  |
| regex_v8                 | 27.8 ms                                                | 25.2 ms: 1.10x faster                                                  |
| json_loads               | 31.2 us                                                | 28.4 us: 1.10x faster                                                  |
| regex_compile            | 188 ms                                                 | 172 ms: 1.10x faster                                                   |
| fannkuch                 | 532 ms                                                 | 485 ms: 1.10x faster                                                   |
| xml_etree_generate       | 99.4 ms                                                | 90.8 ms: 1.09x faster                                                  |
| create_gc_cycles         | 1.62 ms                                                | 1.49 ms: 1.09x faster                                                  |
| json                     | 5.69 ms                                                | 5.28 ms: 1.08x faster                                                  |
| mdp                      | 2.85 sec                                               | 2.66 sec: 1.07x faster                                                 |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 6.05 ms: 1.07x faster                                                  |
| nqueens                  | 106 ms                                                 | 99.0 ms: 1.07x faster                                                  |
| pathlib                  | 20.5 ms                                                | 19.1 ms: 1.07x faster                                                  |
| xml_etree_parse          | 168 ms                                                 | 158 ms: 1.07x faster                                                   |
| sqlite_synth             | 3.02 us                                                | 2.86 us: 1.06x faster                                                  |
| unpickle_list            | 5.20 us                                                | 4.93 us: 1.06x faster                                                  |
| gc_traversal             | 3.62 ms                                                | 3.52 ms: 1.03x faster                                                  |
| scimark_fft              | 466 ms                                                 | 452 ms: 1.03x faster                                                   |
| meteor_contest           | 120 ms                                                 | 116 ms: 1.03x faster                                                   |
| xml_etree_iterparse      | 115 ms                                                 | 112 ms: 1.03x faster                                                   |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                   |
| pidigits                 | 191 ms                                                 | 189 ms: 1.01x faster                                                   |
| regex_dna                | 227 ms                                                 | 227 ms: 1.00x slower                                                   |
| unpickle                 | 14.4 us                                                | 14.8 us: 1.03x slower                                                  |
| async_generators         | 444 ms                                                 | 458 ms: 1.03x slower                                                   |
| pickle_list              | 5.08 us                                                | 5.34 us: 1.05x slower                                                  |
| pickle                   | 10.7 us                                                | 11.4 us: 1.07x slower                                                  |
| telco                    | 7.27 ms                                                | 8.72 ms: 1.20x slower                                                  |
| coverage                 | 79.4 ms                                                | 95.4 ms: 1.20x slower                                                  |
| pickle_dict              | 29.6 us                                                | 37.0 us: 1.25x slower                                                  |
| python_startup_no_site   | 5.93 ms                                                | 8.74 ms: 1.47x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.22x faster                                                           |

Benchmark hidden because not significant (3): regex_effbot, bench_mp_pool, mypy2
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240116-3.13.0a2+-d73fe0a-PYTHON_UOPS/bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.15x
- 95% likely to have a speedup of 1.15x
- 99% likely to have a speedup of 1.14x


# Memory

- memory change: 1.06x