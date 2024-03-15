
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin
- machine: linux-x86_64
- commit hash: b63610e
- commit date: 2023-12-19
- overall geometric mean: 1.30x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.21x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 277 ms: 1.26x faster                                           |
| chameleon      | 9.68 ms                                                | 7.09 ms: 1.37x faster                                          |
| docutils       | 3.30 sec                                               | 2.68 sec: 1.23x faster                                         |
| tornado_http   | 136 ms                                                 | 97.7 ms: 1.40x faster                                          |
| Geometric mean | (ref)                                                  | 1.31x faster                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 446 ms: 1.63x faster                                           |
| async_tree_memoization  | 870 ms                                                 | 569 ms: 1.53x faster                                           |
| async_tree_io           | 1.77 sec                                               | 1.19 sec: 1.48x faster                                         |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 717 ms: 1.42x faster                                           |
| Geometric mean          | (ref)                                                  | 1.51x faster                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 106 ms: 1.44x faster                                           |
| float          | 117 ms                                                 | 88.1 ms: 1.33x faster                                          |
| pidigits       | 191 ms                                                 | 188 ms: 1.02x faster                                           |
| Geometric mean | (ref)                                                  | 1.25x faster                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 142 ms: 1.32x faster                                           |
| regex_dna      | 227 ms                                                 | 213 ms: 1.07x faster                                           |
| regex_v8       | 27.8 ms                                                | 26.1 ms: 1.07x faster                                          |
| regex_effbot   | 3.63 ms                                                | 3.69 ms: 1.02x slower                                          |
| Geometric mean | (ref)                                                  | 1.10x faster                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 301 us: 1.61x faster                                           |
| unpickle_pure_python | 331 us                                                 | 228 us: 1.45x faster                                           |
| tomli_loads          | 3.14 sec                                               | 2.25 sec: 1.39x faster                                         |
| json_dumps           | 14.2 ms                                                | 10.3 ms: 1.38x faster                                          |
| xml_etree_process    | 79.1 ms                                                | 59.0 ms: 1.34x faster                                          |
| xml_etree_generate   | 99.4 ms                                                | 86.8 ms: 1.15x faster                                          |
| json_loads           | 31.2 us                                                | 27.5 us: 1.13x faster                                          |
| xml_etree_parse      | 168 ms                                                 | 158 ms: 1.06x faster                                           |
| xml_etree_iterparse  | 115 ms                                                 | 109 ms: 1.06x faster                                           |
| unpickle_list        | 5.20 us                                                | 5.13 us: 1.01x faster                                          |
| pickle_list          | 5.08 us                                                | 5.02 us: 1.01x faster                                          |
| unpickle             | 14.4 us                                                | 14.6 us: 1.01x slower                                          |
| pickle               | 10.7 us                                                | 11.6 us: 1.09x slower                                          |
| pickle_dict          | 29.6 us                                                | 35.4 us: 1.20x slower                                          |
| Geometric mean       | (ref)                                                  | 1.15x faster                                                   |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.43x faster                                          |
| python_startup_no_site | 5.93 ms                                                | 8.87 ms: 1.50x slower                                          |
| Geometric mean         | (ref)                                                  | 1.02x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 12.7 ms: 1.28x faster                                          |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 113 us: 4.82x faster                                           |
| generators               | 80.1 ms                                                | 28.8 ms: 2.78x faster                                          |
| deltablue                | 7.91 ms                                                | 4.07 ms: 1.95x faster                                          |
| asyncio_tcp              | 922 ms                                                 | 496 ms: 1.86x faster                                           |
| logging_silent           | 190 ns                                                 | 103 ns: 1.83x faster                                           |
| richards_super           | 94.7 ms                                                | 52.7 ms: 1.80x faster                                          |
| raytrace                 | 507 ms                                                 | 282 ms: 1.80x faster                                           |
| richards                 | 79.3 ms                                                | 46.3 ms: 1.71x faster                                          |
| scimark_sor              | 220 ms                                                 | 131 ms: 1.68x faster                                           |
| sqlglot_parse            | 2.17 ms                                                | 1.29 ms: 1.68x faster                                          |
| chaos                    | 115 ms                                                 | 70.6 ms: 1.64x faster                                          |
| async_tree_none          | 728 ms                                                 | 446 ms: 1.63x faster                                           |
| pickle_pure_python       | 484 us                                                 | 301 us: 1.61x faster                                           |
| sqlglot_transpile        | 2.57 ms                                                | 1.62 ms: 1.59x faster                                          |
| go                       | 240 ms                                                 | 152 ms: 1.58x faster                                           |
| scimark_monte_carlo      | 118 ms                                                 | 75.1 ms: 1.57x faster                                          |
| crypto_pyaes             | 128 ms                                                 | 81.4 ms: 1.57x faster                                          |
| coroutines               | 35.1 ms                                                | 22.5 ms: 1.56x faster                                          |
| scimark_lu               | 176 ms                                                 | 115 ms: 1.54x faster                                           |
| deepcopy_memo            | 58.5 us                                                | 38.1 us: 1.53x faster                                          |
| async_tree_memoization   | 870 ms                                                 | 569 ms: 1.53x faster                                           |
| async_tree_io            | 1.77 sec                                               | 1.19 sec: 1.48x faster                                         |
| unpickle_pure_python     | 331 us                                                 | 228 us: 1.45x faster                                           |
| comprehensions           | 28.8 us                                                | 19.8 us: 1.45x faster                                          |
| nbody                    | 154 ms                                                 | 106 ms: 1.44x faster                                           |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.43x faster                                          |
| logging_simple           | 8.30 us                                                | 5.83 us: 1.42x faster                                          |
| pyflate                  | 716 ms                                                 | 504 ms: 1.42x faster                                           |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.81 sec: 1.42x faster                                         |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 717 ms: 1.42x faster                                           |
| logging_format           | 9.09 us                                                | 6.45 us: 1.41x faster                                          |
| tornado_http             | 136 ms                                                 | 97.7 ms: 1.40x faster                                          |
| tomli_loads              | 3.14 sec                                               | 2.25 sec: 1.39x faster                                         |
| json_dumps               | 14.2 ms                                                | 10.3 ms: 1.38x faster                                          |
| deepcopy                 | 479 us                                                 | 349 us: 1.37x faster                                           |
| deepcopy_reduce          | 4.17 us                                                | 3.04 us: 1.37x faster                                          |
| chameleon                | 9.68 ms                                                | 7.09 ms: 1.37x faster                                          |
| pycparser                | 1.58 sec                                               | 1.17 sec: 1.34x faster                                         |
| xml_etree_process        | 79.1 ms                                                | 59.0 ms: 1.34x faster                                          |
| float                    | 117 ms                                                 | 88.1 ms: 1.33x faster                                          |
| regex_compile            | 188 ms                                                 | 142 ms: 1.32x faster                                           |
| sqlglot_normalize        | 143 ms                                                 | 111 ms: 1.29x faster                                           |
| hexiom                   | 10.4 ms                                                | 8.11 ms: 1.28x faster                                          |
| mako                     | 16.3 ms                                                | 12.7 ms: 1.28x faster                                          |
| pprint_safe_repr         | 1.02 sec                                               | 807 ms: 1.26x faster                                           |
| 2to3                     | 348 ms                                                 | 277 ms: 1.26x faster                                           |
| pprint_pformat           | 2.10 sec                                               | 1.68 sec: 1.25x faster                                         |
| dulwich_log              | 84.3 ms                                                | 68.0 ms: 1.24x faster                                          |
| unpack_sequence          | 60.0 ns                                                | 48.5 ns: 1.24x faster                                          |
| docutils                 | 3.30 sec                                               | 2.68 sec: 1.23x faster                                         |
| sqlglot_optimize         | 69.2 ms                                                | 56.2 ms: 1.23x faster                                          |
| sympy_integrate          | 25.8 ms                                                | 21.2 ms: 1.22x faster                                          |
| sympy_sum                | 196 ms                                                 | 162 ms: 1.22x faster                                           |
| fannkuch                 | 532 ms                                                 | 438 ms: 1.21x faster                                           |
| spectral_norm            | 170 ms                                                 | 141 ms: 1.21x faster                                           |
| dask                     | 441 ms                                                 | 366 ms: 1.20x faster                                           |
| scimark_fft              | 466 ms                                                 | 391 ms: 1.19x faster                                           |
| sympy_str                | 346 ms                                                 | 290 ms: 1.19x faster                                           |
| sympy_expand             | 566 ms                                                 | 483 ms: 1.17x faster                                           |
| bench_thread_pool        | 986 us                                                 | 843 us: 1.17x faster                                           |
| nqueens                  | 106 ms                                                 | 91.2 ms: 1.16x faster                                          |
| xml_etree_generate       | 99.4 ms                                                | 86.8 ms: 1.15x faster                                          |
| json_loads               | 31.2 us                                                | 27.5 us: 1.13x faster                                          |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.72 ms: 1.13x faster                                          |
| pathlib                  | 20.5 ms                                                | 18.4 ms: 1.11x faster                                          |
| json                     | 5.69 ms                                                | 5.17 ms: 1.10x faster                                          |
| create_gc_cycles         | 1.62 ms                                                | 1.48 ms: 1.09x faster                                          |
| mdp                      | 2.85 sec                                               | 2.61 sec: 1.09x faster                                         |
| meteor_contest           | 120 ms                                                 | 110 ms: 1.09x faster                                           |
| regex_dna                | 227 ms                                                 | 213 ms: 1.07x faster                                           |
| regex_v8                 | 27.8 ms                                                | 26.1 ms: 1.07x faster                                          |
| xml_etree_parse          | 168 ms                                                 | 158 ms: 1.06x faster                                           |
| sqlite_synth             | 3.02 us                                                | 2.85 us: 1.06x faster                                          |
| xml_etree_iterparse      | 115 ms                                                 | 109 ms: 1.06x faster                                           |
| pidigits                 | 191 ms                                                 | 188 ms: 1.02x faster                                           |
| unpickle_list            | 5.20 us                                                | 5.13 us: 1.01x faster                                          |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                           |
| pickle_list              | 5.08 us                                                | 5.02 us: 1.01x faster                                          |
| unpickle                 | 14.4 us                                                | 14.6 us: 1.01x slower                                          |
| regex_effbot             | 3.63 ms                                                | 3.69 ms: 1.02x slower                                          |
| async_generators         | 444 ms                                                 | 460 ms: 1.04x slower                                           |
| gc_traversal             | 3.62 ms                                                | 3.77 ms: 1.04x slower                                          |
| pickle                   | 10.7 us                                                | 11.6 us: 1.09x slower                                          |
| telco                    | 7.27 ms                                                | 8.50 ms: 1.17x slower                                          |
| pickle_dict              | 29.6 us                                                | 35.4 us: 1.20x slower                                          |
| coverage                 | 79.4 ms                                                | 95.4 ms: 1.20x slower                                          |
| python_startup_no_site   | 5.93 ms                                                | 8.87 ms: 1.50x slower                                          |
| Geometric mean           | (ref)                                                  | 1.30x faster                                                   |

Benchmark hidden because not significant (2): mypy2, bench_mp_pool
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231219-3.13.0a2+-b63610e-JIT/bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.24x
- 95% likely to have a speedup of 1.23x
- 99% likely to have a speedup of 1.21x


# Memory

- memory change: 1.10x