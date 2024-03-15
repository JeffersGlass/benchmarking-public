
# Results vs. 3.10.4

- fork: faster-cpython
- ref: cold_exits
- machine: linux-x86_64
- commit hash: 2172d68
- commit date: 2024-01-16
- overall geometric mean: 1.24x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.16x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 288 ms: 1.21x faster                                                   |
| chameleon      | 9.68 ms                                                | 7.27 ms: 1.33x faster                                                  |
| docutils       | 3.30 sec                                               | 2.75 sec: 1.20x faster                                                 |
| tornado_http   | 136 ms                                                 | 97.9 ms: 1.39x faster                                                  |
| Geometric mean | (ref)                                                  | 1.28x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 451 ms: 1.62x faster                                                   |
| async_tree_memoization  | 870 ms                                                 | 570 ms: 1.53x faster                                                   |
| async_tree_io           | 1.77 sec                                               | 1.21 sec: 1.46x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 724 ms: 1.40x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.50x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 115 ms: 1.33x faster                                                   |
| float          | 117 ms                                                 | 92.1 ms: 1.27x faster                                                  |
| pidigits       | 191 ms                                                 | 197 ms: 1.03x slower                                                   |
| Geometric mean | (ref)                                                  | 1.18x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 170 ms: 1.11x faster                                                   |
| regex_v8       | 27.8 ms                                                | 25.2 ms: 1.10x faster                                                  |
| regex_dna      | 227 ms                                                 | 226 ms: 1.00x faster                                                   |
| regex_effbot   | 3.63 ms                                                | 3.72 ms: 1.02x slower                                                  |
| Geometric mean | (ref)                                                  | 1.05x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 300 us: 1.61x faster                                                   |
| unpickle_pure_python | 331 us                                                 | 233 us: 1.42x faster                                                   |
| json_dumps           | 14.2 ms                                                | 10.7 ms: 1.33x faster                                                  |
| xml_etree_process    | 79.1 ms                                                | 61.8 ms: 1.28x faster                                                  |
| tomli_loads          | 3.14 sec                                               | 2.71 sec: 1.16x faster                                                 |
| xml_etree_generate   | 99.4 ms                                                | 89.9 ms: 1.11x faster                                                  |
| json_loads           | 31.2 us                                                | 28.4 us: 1.10x faster                                                  |
| xml_etree_parse      | 168 ms                                                 | 158 ms: 1.06x faster                                                   |
| pickle_list          | 5.08 us                                                | 4.88 us: 1.04x faster                                                  |
| xml_etree_iterparse  | 115 ms                                                 | 112 ms: 1.03x faster                                                   |
| unpickle_list        | 5.20 us                                                | 5.36 us: 1.03x slower                                                  |
| unpickle             | 14.4 us                                                | 14.9 us: 1.04x slower                                                  |
| pickle               | 10.7 us                                                | 11.4 us: 1.07x slower                                                  |
| pickle_dict          | 29.6 us                                                | 34.4 us: 1.16x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.12x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                  |
| python_startup_no_site | 5.93 ms                                                | 8.78 ms: 1.48x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 13.6 ms: 1.20x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 119 us: 4.57x faster                                                   |
| generators               | 80.1 ms                                                | 29.1 ms: 2.75x faster                                                  |
| asyncio_tcp              | 922 ms                                                 | 493 ms: 1.87x faster                                                   |
| logging_silent           | 190 ns                                                 | 107 ns: 1.77x faster                                                   |
| raytrace                 | 507 ms                                                 | 302 ms: 1.68x faster                                                   |
| richards_super           | 94.7 ms                                                | 56.5 ms: 1.68x faster                                                  |
| deltablue                | 7.91 ms                                                | 4.82 ms: 1.64x faster                                                  |
| async_tree_none          | 728 ms                                                 | 451 ms: 1.62x faster                                                   |
| pickle_pure_python       | 484 us                                                 | 300 us: 1.61x faster                                                   |
| coroutines               | 35.1 ms                                                | 22.1 ms: 1.59x faster                                                  |
| scimark_sor              | 220 ms                                                 | 139 ms: 1.58x faster                                                   |
| richards                 | 79.3 ms                                                | 50.0 ms: 1.58x faster                                                  |
| sqlglot_parse            | 2.17 ms                                                | 1.38 ms: 1.57x faster                                                  |
| chaos                    | 115 ms                                                 | 74.4 ms: 1.55x faster                                                  |
| crypto_pyaes             | 128 ms                                                 | 83.5 ms: 1.53x faster                                                  |
| async_tree_memoization   | 870 ms                                                 | 570 ms: 1.53x faster                                                   |
| sqlglot_transpile        | 2.57 ms                                                | 1.71 ms: 1.50x faster                                                  |
| async_tree_io            | 1.77 sec                                               | 1.21 sec: 1.46x faster                                                 |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                                 |
| unpickle_pure_python     | 331 us                                                 | 233 us: 1.42x faster                                                   |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 724 ms: 1.40x faster                                                   |
| deepcopy_memo            | 58.5 us                                                | 41.7 us: 1.40x faster                                                  |
| tornado_http             | 136 ms                                                 | 97.9 ms: 1.39x faster                                                  |
| go                       | 240 ms                                                 | 175 ms: 1.37x faster                                                   |
| comprehensions           | 28.8 us                                                | 21.2 us: 1.36x faster                                                  |
| chameleon                | 9.68 ms                                                | 7.27 ms: 1.33x faster                                                  |
| nbody                    | 154 ms                                                 | 115 ms: 1.33x faster                                                   |
| json_dumps               | 14.2 ms                                                | 10.7 ms: 1.33x faster                                                  |
| deepcopy                 | 479 us                                                 | 361 us: 1.33x faster                                                   |
| scimark_monte_carlo      | 118 ms                                                 | 89.5 ms: 1.32x faster                                                  |
| deepcopy_reduce          | 4.17 us                                                | 3.19 us: 1.31x faster                                                  |
| pycparser                | 1.58 sec                                               | 1.21 sec: 1.30x faster                                                 |
| logging_simple           | 8.30 us                                                | 6.39 us: 1.30x faster                                                  |
| xml_etree_process        | 79.1 ms                                                | 61.8 ms: 1.28x faster                                                  |
| float                    | 117 ms                                                 | 92.1 ms: 1.27x faster                                                  |
| logging_format           | 9.09 us                                                | 7.24 us: 1.26x faster                                                  |
| sqlglot_normalize        | 143 ms                                                 | 116 ms: 1.23x faster                                                   |
| pyflate                  | 716 ms                                                 | 582 ms: 1.23x faster                                                   |
| 2to3                     | 348 ms                                                 | 288 ms: 1.21x faster                                                   |
| mako                     | 16.3 ms                                                | 13.6 ms: 1.20x faster                                                  |
| sympy_sum                | 196 ms                                                 | 163 ms: 1.20x faster                                                   |
| docutils                 | 3.30 sec                                               | 2.75 sec: 1.20x faster                                                 |
| dask                     | 441 ms                                                 | 369 ms: 1.20x faster                                                   |
| sympy_integrate          | 25.8 ms                                                | 21.7 ms: 1.19x faster                                                  |
| pprint_safe_repr         | 1.02 sec                                               | 856 ms: 1.19x faster                                                   |
| pprint_pformat           | 2.10 sec                                               | 1.78 sec: 1.18x faster                                                 |
| scimark_lu               | 176 ms                                                 | 149 ms: 1.18x faster                                                   |
| dulwich_log              | 84.3 ms                                                | 71.8 ms: 1.17x faster                                                  |
| spectral_norm            | 170 ms                                                 | 145 ms: 1.17x faster                                                   |
| tomli_loads              | 3.14 sec                                               | 2.71 sec: 1.16x faster                                                 |
| sympy_str                | 346 ms                                                 | 299 ms: 1.16x faster                                                   |
| sqlglot_optimize         | 69.2 ms                                                | 59.9 ms: 1.15x faster                                                  |
| bench_thread_pool        | 986 us                                                 | 855 us: 1.15x faster                                                   |
| hexiom                   | 10.4 ms                                                | 9.05 ms: 1.15x faster                                                  |
| sympy_expand             | 566 ms                                                 | 500 ms: 1.13x faster                                                   |
| regex_compile            | 188 ms                                                 | 170 ms: 1.11x faster                                                   |
| xml_etree_generate       | 99.4 ms                                                | 89.9 ms: 1.11x faster                                                  |
| regex_v8                 | 27.8 ms                                                | 25.2 ms: 1.10x faster                                                  |
| json_loads               | 31.2 us                                                | 28.4 us: 1.10x faster                                                  |
| fannkuch                 | 532 ms                                                 | 487 ms: 1.09x faster                                                   |
| json                     | 5.69 ms                                                | 5.26 ms: 1.08x faster                                                  |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.98 ms: 1.08x faster                                                  |
| create_gc_cycles         | 1.62 ms                                                | 1.51 ms: 1.07x faster                                                  |
| pathlib                  | 20.5 ms                                                | 19.1 ms: 1.07x faster                                                  |
| nqueens                  | 106 ms                                                 | 98.8 ms: 1.07x faster                                                  |
| xml_etree_parse          | 168 ms                                                 | 158 ms: 1.06x faster                                                   |
| sqlite_synth             | 3.02 us                                                | 2.85 us: 1.06x faster                                                  |
| unpack_sequence          | 60.0 ns                                                | 57.5 ns: 1.04x faster                                                  |
| pickle_list              | 5.08 us                                                | 4.88 us: 1.04x faster                                                  |
| scimark_fft              | 466 ms                                                 | 449 ms: 1.04x faster                                                   |
| meteor_contest           | 120 ms                                                 | 116 ms: 1.03x faster                                                   |
| xml_etree_iterparse      | 115 ms                                                 | 112 ms: 1.03x faster                                                   |
| mdp                      | 2.85 sec                                               | 2.78 sec: 1.02x faster                                                 |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                   |
| regex_dna                | 227 ms                                                 | 226 ms: 1.00x faster                                                   |
| regex_effbot             | 3.63 ms                                                | 3.72 ms: 1.02x slower                                                  |
| pidigits                 | 191 ms                                                 | 197 ms: 1.03x slower                                                   |
| unpickle_list            | 5.20 us                                                | 5.36 us: 1.03x slower                                                  |
| async_generators         | 444 ms                                                 | 459 ms: 1.03x slower                                                   |
| unpickle                 | 14.4 us                                                | 14.9 us: 1.04x slower                                                  |
| gc_traversal             | 3.62 ms                                                | 3.76 ms: 1.04x slower                                                  |
| pickle                   | 10.7 us                                                | 11.4 us: 1.07x slower                                                  |
| pickle_dict              | 29.6 us                                                | 34.4 us: 1.16x slower                                                  |
| telco                    | 7.27 ms                                                | 8.69 ms: 1.20x slower                                                  |
| coverage                 | 79.4 ms                                                | 95.8 ms: 1.21x slower                                                  |
| python_startup_no_site   | 5.93 ms                                                | 8.78 ms: 1.48x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.24x faster                                                           |

Benchmark hidden because not significant (2): mypy2, bench_mp_pool
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240116-3.13.0a2+-2172d68-PYTHON_UOPS/bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.18x
- 95% likely to have a speedup of 1.17x
- 99% likely to have a speedup of 1.16x


# Memory

- memory change: 1.06x