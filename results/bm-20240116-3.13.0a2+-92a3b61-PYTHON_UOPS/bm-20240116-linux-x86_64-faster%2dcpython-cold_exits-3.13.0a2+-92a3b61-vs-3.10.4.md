
# Results vs. 3.10.4

- fork: faster-cpython
- ref: cold_exits
- machine: linux-x86_64
- commit hash: 92a3b61
- commit date: 2024-01-16
- overall geometric mean: 1.25x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.16x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 288 ms: 1.21x faster                                                   |
| chameleon      | 9.68 ms                                                | 7.11 ms: 1.36x faster                                                  |
| docutils       | 3.30 sec                                               | 2.71 sec: 1.22x faster                                                 |
| tornado_http   | 136 ms                                                 | 98.2 ms: 1.39x faster                                                  |
| Geometric mean | (ref)                                                  | 1.29x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 445 ms: 1.64x faster                                                   |
| async_tree_memoization  | 870 ms                                                 | 574 ms: 1.52x faster                                                   |
| async_tree_io           | 1.77 sec                                               | 1.20 sec: 1.47x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 717 ms: 1.42x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.51x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 120 ms: 1.28x faster                                                   |
| float          | 117 ms                                                 | 94.2 ms: 1.24x faster                                                  |
| pidigits       | 191 ms                                                 | 189 ms: 1.01x faster                                                   |
| Geometric mean | (ref)                                                  | 1.17x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 164 ms: 1.15x faster                                                   |
| regex_v8       | 27.8 ms                                                | 24.7 ms: 1.13x faster                                                  |
| regex_dna      | 227 ms                                                 | 223 ms: 1.02x faster                                                   |
| Geometric mean | (ref)                                                  | 1.07x faster                                                           |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 301 us: 1.61x faster                                                   |
| unpickle_pure_python | 331 us                                                 | 233 us: 1.42x faster                                                   |
| json_dumps           | 14.2 ms                                                | 10.8 ms: 1.32x faster                                                  |
| xml_etree_process    | 79.1 ms                                                | 60.9 ms: 1.30x faster                                                  |
| tomli_loads          | 3.14 sec                                               | 2.49 sec: 1.26x faster                                                 |
| xml_etree_generate   | 99.4 ms                                                | 89.4 ms: 1.11x faster                                                  |
| json_loads           | 31.2 us                                                | 28.5 us: 1.09x faster                                                  |
| xml_etree_parse      | 168 ms                                                 | 157 ms: 1.07x faster                                                   |
| xml_etree_iterparse  | 115 ms                                                 | 111 ms: 1.04x faster                                                   |
| pickle_list          | 5.08 us                                                | 5.13 us: 1.01x slower                                                  |
| unpickle_list        | 5.20 us                                                | 5.32 us: 1.02x slower                                                  |
| unpickle             | 14.4 us                                                | 14.8 us: 1.03x slower                                                  |
| pickle               | 10.7 us                                                | 11.7 us: 1.09x slower                                                  |
| pickle_dict          | 29.6 us                                                | 33.9 us: 1.14x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.12x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.45x faster                                                  |
| python_startup_no_site | 5.93 ms                                                | 8.70 ms: 1.47x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 14.2 ms: 1.15x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 117 us: 4.67x faster                                                   |
| generators               | 80.1 ms                                                | 29.1 ms: 2.75x faster                                                  |
| asyncio_tcp              | 922 ms                                                 | 493 ms: 1.87x faster                                                   |
| logging_silent           | 190 ns                                                 | 106 ns: 1.79x faster                                                   |
| richards_super           | 94.7 ms                                                | 55.0 ms: 1.72x faster                                                  |
| scimark_sor              | 220 ms                                                 | 131 ms: 1.68x faster                                                   |
| raytrace                 | 507 ms                                                 | 304 ms: 1.67x faster                                                   |
| richards                 | 79.3 ms                                                | 48.3 ms: 1.64x faster                                                  |
| deltablue                | 7.91 ms                                                | 4.84 ms: 1.64x faster                                                  |
| async_tree_none          | 728 ms                                                 | 445 ms: 1.64x faster                                                   |
| sqlglot_parse            | 2.17 ms                                                | 1.33 ms: 1.63x faster                                                  |
| pickle_pure_python       | 484 us                                                 | 301 us: 1.61x faster                                                   |
| chaos                    | 115 ms                                                 | 74.0 ms: 1.56x faster                                                  |
| coroutines               | 35.1 ms                                                | 22.6 ms: 1.56x faster                                                  |
| sqlglot_transpile        | 2.57 ms                                                | 1.67 ms: 1.54x faster                                                  |
| async_tree_memoization   | 870 ms                                                 | 574 ms: 1.52x faster                                                   |
| crypto_pyaes             | 128 ms                                                 | 84.5 ms: 1.51x faster                                                  |
| scimark_lu               | 176 ms                                                 | 119 ms: 1.48x faster                                                   |
| async_tree_io            | 1.77 sec                                               | 1.20 sec: 1.47x faster                                                 |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.45x faster                                                  |
| deepcopy_memo            | 58.5 us                                                | 40.4 us: 1.45x faster                                                  |
| go                       | 240 ms                                                 | 168 ms: 1.43x faster                                                   |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.42x faster                                                 |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 717 ms: 1.42x faster                                                   |
| unpickle_pure_python     | 331 us                                                 | 233 us: 1.42x faster                                                   |
| tornado_http             | 136 ms                                                 | 98.2 ms: 1.39x faster                                                  |
| chameleon                | 9.68 ms                                                | 7.11 ms: 1.36x faster                                                  |
| deepcopy                 | 479 us                                                 | 358 us: 1.34x faster                                                   |
| comprehensions           | 28.8 us                                                | 21.5 us: 1.34x faster                                                  |
| deepcopy_reduce          | 4.17 us                                                | 3.15 us: 1.32x faster                                                  |
| logging_simple           | 8.30 us                                                | 6.29 us: 1.32x faster                                                  |
| json_dumps               | 14.2 ms                                                | 10.8 ms: 1.32x faster                                                  |
| scimark_monte_carlo      | 118 ms                                                 | 90.2 ms: 1.31x faster                                                  |
| xml_etree_process        | 79.1 ms                                                | 60.9 ms: 1.30x faster                                                  |
| logging_format           | 9.09 us                                                | 7.02 us: 1.29x faster                                                  |
| nbody                    | 154 ms                                                 | 120 ms: 1.28x faster                                                   |
| tomli_loads              | 3.14 sec                                               | 2.49 sec: 1.26x faster                                                 |
| pycparser                | 1.58 sec                                               | 1.26 sec: 1.26x faster                                                 |
| float                    | 117 ms                                                 | 94.2 ms: 1.24x faster                                                  |
| sqlglot_normalize        | 143 ms                                                 | 115 ms: 1.24x faster                                                   |
| docutils                 | 3.30 sec                                               | 2.71 sec: 1.22x faster                                                 |
| dulwich_log              | 84.3 ms                                                | 69.3 ms: 1.22x faster                                                  |
| pyflate                  | 716 ms                                                 | 589 ms: 1.22x faster                                                   |
| 2to3                     | 348 ms                                                 | 288 ms: 1.21x faster                                                   |
| sympy_integrate          | 25.8 ms                                                | 21.4 ms: 1.21x faster                                                  |
| sympy_sum                | 196 ms                                                 | 163 ms: 1.21x faster                                                   |
| dask                     | 441 ms                                                 | 368 ms: 1.20x faster                                                   |
| hexiom                   | 10.4 ms                                                | 8.74 ms: 1.19x faster                                                  |
| unpack_sequence          | 60.0 ns                                                | 50.9 ns: 1.18x faster                                                  |
| sympy_str                | 346 ms                                                 | 295 ms: 1.17x faster                                                   |
| pprint_safe_repr         | 1.02 sec                                               | 870 ms: 1.17x faster                                                   |
| sqlglot_optimize         | 69.2 ms                                                | 59.3 ms: 1.17x faster                                                  |
| pprint_pformat           | 2.10 sec                                               | 1.80 sec: 1.17x faster                                                 |
| spectral_norm            | 170 ms                                                 | 146 ms: 1.16x faster                                                   |
| bench_thread_pool        | 986 us                                                 | 848 us: 1.16x faster                                                   |
| sympy_expand             | 566 ms                                                 | 492 ms: 1.15x faster                                                   |
| regex_compile            | 188 ms                                                 | 164 ms: 1.15x faster                                                   |
| mako                     | 16.3 ms                                                | 14.2 ms: 1.15x faster                                                  |
| regex_v8                 | 27.8 ms                                                | 24.7 ms: 1.13x faster                                                  |
| xml_etree_generate       | 99.4 ms                                                | 89.4 ms: 1.11x faster                                                  |
| pathlib                  | 20.5 ms                                                | 18.6 ms: 1.10x faster                                                  |
| create_gc_cycles         | 1.62 ms                                                | 1.48 ms: 1.10x faster                                                  |
| fannkuch                 | 532 ms                                                 | 485 ms: 1.10x faster                                                   |
| json_loads               | 31.2 us                                                | 28.5 us: 1.09x faster                                                  |
| nqueens                  | 106 ms                                                 | 97.0 ms: 1.09x faster                                                  |
| json                     | 5.69 ms                                                | 5.22 ms: 1.09x faster                                                  |
| mdp                      | 2.85 sec                                               | 2.63 sec: 1.08x faster                                                 |
| xml_etree_parse          | 168 ms                                                 | 157 ms: 1.07x faster                                                   |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 6.12 ms: 1.06x faster                                                  |
| xml_etree_iterparse      | 115 ms                                                 | 111 ms: 1.04x faster                                                   |
| sqlite_synth             | 3.02 us                                                | 2.91 us: 1.04x faster                                                  |
| meteor_contest           | 120 ms                                                 | 117 ms: 1.02x faster                                                   |
| scimark_fft              | 466 ms                                                 | 458 ms: 1.02x faster                                                   |
| regex_dna                | 227 ms                                                 | 223 ms: 1.02x faster                                                   |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                   |
| pidigits                 | 191 ms                                                 | 189 ms: 1.01x faster                                                   |
| pickle_list              | 5.08 us                                                | 5.13 us: 1.01x slower                                                  |
| async_generators         | 444 ms                                                 | 452 ms: 1.02x slower                                                   |
| unpickle_list            | 5.20 us                                                | 5.32 us: 1.02x slower                                                  |
| unpickle                 | 14.4 us                                                | 14.8 us: 1.03x slower                                                  |
| pickle                   | 10.7 us                                                | 11.7 us: 1.09x slower                                                  |
| gc_traversal             | 3.62 ms                                                | 4.00 ms: 1.10x slower                                                  |
| pickle_dict              | 29.6 us                                                | 33.9 us: 1.14x slower                                                  |
| telco                    | 7.27 ms                                                | 8.67 ms: 1.19x slower                                                  |
| coverage                 | 79.4 ms                                                | 96.1 ms: 1.21x slower                                                  |
| python_startup_no_site   | 5.93 ms                                                | 8.70 ms: 1.47x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.25x faster                                                           |

Benchmark hidden because not significant (3): mypy2, bench_mp_pool, regex_effbot
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240116-3.13.0a2+-92a3b61-PYTHON_UOPS/bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.19x
- 95% likely to have a speedup of 1.18x
- 99% likely to have a speedup of 1.16x


# Memory

- memory change: 1.06x