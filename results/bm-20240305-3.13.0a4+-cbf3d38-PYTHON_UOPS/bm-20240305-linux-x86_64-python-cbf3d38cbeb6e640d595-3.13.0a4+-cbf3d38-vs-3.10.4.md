# Results vs. 3.10.4

- fork: python
- ref: cbf3d38cbeb6e640d595
- machine: linux-x86_64
- commit hash: cbf3d38
- commit date: 2024-03-05
- overall geometric mean: 1.24x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.15x faster
- Memory change: 1.08x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4+-cbf3d38 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 292 ms: 1.19x faster                                                   |
| chameleon      | 9.68 ms                                                | 6.84 ms: 1.42x faster                                                  |
| docutils       | 3.30 sec                                               | 2.82 sec: 1.17x faster                                                 |
| tornado_http   | 136 ms                                                 | 99.5 ms: 1.37x faster                                                  |
| Geometric mean | (ref)                                                  | 1.28x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4+-cbf3d38 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 444 ms: 1.64x faster                                                   |
| async_tree_memoization  | 870 ms                                                 | 572 ms: 1.52x faster                                                   |
| async_tree_io           | 1.77 sec                                               | 1.19 sec: 1.48x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 717 ms: 1.42x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.51x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4+-cbf3d38 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 117 ms: 1.32x faster                                                   |
| float          | 117 ms                                                 | 91.4 ms: 1.28x faster                                                  |
| pidigits       | 191 ms                                                 | 188 ms: 1.01x faster                                                   |
| Geometric mean | (ref)                                                  | 1.20x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4+-cbf3d38 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_v8       | 27.8 ms                                                | 25.3 ms: 1.10x faster                                                  |
| regex_compile  | 188 ms                                                 | 173 ms: 1.09x faster                                                   |
| regex_dna      | 227 ms                                                 | 221 ms: 1.03x faster                                                   |
| regex_effbot   | 3.63 ms                                                | 3.57 ms: 1.02x faster                                                  |
| Geometric mean | (ref)                                                  | 1.06x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4+-cbf3d38 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 304 us: 1.59x faster                                                   |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.36x faster                                                  |
| xml_etree_process    | 79.1 ms                                                | 60.8 ms: 1.30x faster                                                  |
| tomli_loads          | 3.14 sec                                               | 2.45 sec: 1.28x faster                                                 |
| unpickle_pure_python | 331 us                                                 | 278 us: 1.19x faster                                                   |
| json_loads           | 31.2 us                                                | 27.2 us: 1.15x faster                                                  |
| xml_etree_generate   | 99.4 ms                                                | 88.8 ms: 1.12x faster                                                  |
| xml_etree_parse      | 168 ms                                                 | 158 ms: 1.07x faster                                                   |
| unpickle_list        | 5.20 us                                                | 4.99 us: 1.04x faster                                                  |
| xml_etree_iterparse  | 115 ms                                                 | 111 ms: 1.04x faster                                                   |
| unpickle             | 14.4 us                                                | 15.3 us: 1.06x slower                                                  |
| pickle               | 10.7 us                                                | 11.7 us: 1.10x slower                                                  |
| pickle_dict          | 29.6 us                                                | 34.9 us: 1.18x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.12x faster                                                           |

Benchmark hidden because not significant (1): pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4+-cbf3d38 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                  |
| python_startup_no_site | 5.93 ms                                                | 8.83 ms: 1.49x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.02x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4+-cbf3d38 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 13.0 ms: 1.26x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4+-cbf3d38 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 115 us: 4.72x faster                                                   |
| generators               | 80.1 ms                                                | 29.6 ms: 2.70x faster                                                  |
| deltablue                | 7.91 ms                                                | 3.68 ms: 2.15x faster                                                  |
| asyncio_tcp              | 922 ms                                                 | 482 ms: 1.91x faster                                                   |
| logging_silent           | 190 ns                                                 | 100 ns: 1.89x faster                                                   |
| async_tree_none          | 728 ms                                                 | 444 ms: 1.64x faster                                                   |
| pickle_pure_python       | 484 us                                                 | 304 us: 1.59x faster                                                   |
| coroutines               | 35.1 ms                                                | 22.1 ms: 1.59x faster                                                  |
| chaos                    | 115 ms                                                 | 73.6 ms: 1.57x faster                                                  |
| richards_super           | 94.7 ms                                                | 61.2 ms: 1.55x faster                                                  |
| scimark_sor              | 220 ms                                                 | 142 ms: 1.54x faster                                                   |
| sqlglot_parse            | 2.17 ms                                                | 1.42 ms: 1.53x faster                                                  |
| async_tree_memoization   | 870 ms                                                 | 572 ms: 1.52x faster                                                   |
| crypto_pyaes             | 128 ms                                                 | 84.2 ms: 1.52x faster                                                  |
| raytrace                 | 507 ms                                                 | 340 ms: 1.49x faster                                                   |
| async_tree_io            | 1.77 sec                                               | 1.19 sec: 1.48x faster                                                 |
| sqlglot_transpile        | 2.57 ms                                                | 1.75 ms: 1.47x faster                                                  |
| richards                 | 79.3 ms                                                | 55.1 ms: 1.44x faster                                                  |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                  |
| deepcopy_memo            | 58.5 us                                                | 40.8 us: 1.43x faster                                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                                 |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 717 ms: 1.42x faster                                                   |
| chameleon                | 9.68 ms                                                | 6.84 ms: 1.42x faster                                                  |
| comprehensions           | 28.8 us                                                | 20.8 us: 1.38x faster                                                  |
| scimark_monte_carlo      | 118 ms                                                 | 85.5 ms: 1.38x faster                                                  |
| logging_simple           | 8.30 us                                                | 6.04 us: 1.38x faster                                                  |
| go                       | 240 ms                                                 | 175 ms: 1.37x faster                                                   |
| tornado_http             | 136 ms                                                 | 99.5 ms: 1.37x faster                                                  |
| deepcopy_reduce          | 4.17 us                                                | 3.05 us: 1.37x faster                                                  |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.36x faster                                                  |
| deepcopy                 | 479 us                                                 | 358 us: 1.34x faster                                                   |
| logging_format           | 9.09 us                                                | 6.79 us: 1.34x faster                                                  |
| nbody                    | 154 ms                                                 | 117 ms: 1.32x faster                                                   |
| xml_etree_process        | 79.1 ms                                                | 60.8 ms: 1.30x faster                                                  |
| sqlglot_normalize        | 143 ms                                                 | 111 ms: 1.28x faster                                                   |
| tomli_loads              | 3.14 sec                                               | 2.45 sec: 1.28x faster                                                 |
| float                    | 117 ms                                                 | 91.4 ms: 1.28x faster                                                  |
| mako                     | 16.3 ms                                                | 13.0 ms: 1.26x faster                                                  |
| spectral_norm            | 170 ms                                                 | 136 ms: 1.25x faster                                                   |
| sympy_integrate          | 25.8 ms                                                | 21.1 ms: 1.22x faster                                                  |
| pyflate                  | 716 ms                                                 | 586 ms: 1.22x faster                                                   |
| pprint_safe_repr         | 1.02 sec                                               | 843 ms: 1.21x faster                                                   |
| pprint_pformat           | 2.10 sec                                               | 1.75 sec: 1.20x faster                                                 |
| pycparser                | 1.58 sec                                               | 1.31 sec: 1.20x faster                                                 |
| sympy_sum                | 196 ms                                                 | 164 ms: 1.20x faster                                                   |
| 2to3                     | 348 ms                                                 | 292 ms: 1.19x faster                                                   |
| unpickle_pure_python     | 331 us                                                 | 278 us: 1.19x faster                                                   |
| dulwich_log              | 84.3 ms                                                | 71.1 ms: 1.19x faster                                                  |
| docutils                 | 3.30 sec                                               | 2.82 sec: 1.17x faster                                                 |
| bench_thread_pool        | 986 us                                                 | 853 us: 1.16x faster                                                   |
| sympy_str                | 346 ms                                                 | 299 ms: 1.15x faster                                                   |
| hexiom                   | 10.4 ms                                                | 9.02 ms: 1.15x faster                                                  |
| sqlglot_optimize         | 69.2 ms                                                | 60.2 ms: 1.15x faster                                                  |
| json_loads               | 31.2 us                                                | 27.2 us: 1.15x faster                                                  |
| sympy_expand             | 566 ms                                                 | 502 ms: 1.13x faster                                                   |
| fannkuch                 | 532 ms                                                 | 473 ms: 1.12x faster                                                   |
| scimark_lu               | 176 ms                                                 | 157 ms: 1.12x faster                                                   |
| xml_etree_generate       | 99.4 ms                                                | 88.8 ms: 1.12x faster                                                  |
| json                     | 5.69 ms                                                | 5.10 ms: 1.12x faster                                                  |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.85 ms: 1.11x faster                                                  |
| regex_v8                 | 27.8 ms                                                | 25.3 ms: 1.10x faster                                                  |
| regex_compile            | 188 ms                                                 | 173 ms: 1.09x faster                                                   |
| nqueens                  | 106 ms                                                 | 97.8 ms: 1.08x faster                                                  |
| pathlib                  | 20.5 ms                                                | 19.0 ms: 1.08x faster                                                  |
| scimark_fft              | 466 ms                                                 | 433 ms: 1.08x faster                                                   |
| create_gc_cycles         | 1.62 ms                                                | 1.51 ms: 1.07x faster                                                  |
| mdp                      | 2.85 sec                                               | 2.67 sec: 1.07x faster                                                 |
| xml_etree_parse          | 168 ms                                                 | 158 ms: 1.07x faster                                                   |
| meteor_contest           | 120 ms                                                 | 115 ms: 1.04x faster                                                   |
| unpickle_list            | 5.20 us                                                | 4.99 us: 1.04x faster                                                  |
| xml_etree_iterparse      | 115 ms                                                 | 111 ms: 1.04x faster                                                   |
| sqlite_synth             | 3.02 us                                                | 2.91 us: 1.04x faster                                                  |
| regex_dna                | 227 ms                                                 | 221 ms: 1.03x faster                                                   |
| unpack_sequence          | 60.0 ns                                                | 58.9 ns: 1.02x faster                                                  |
| regex_effbot             | 3.63 ms                                                | 3.57 ms: 1.02x faster                                                  |
| pidigits                 | 191 ms                                                 | 188 ms: 1.01x faster                                                   |
| asyncio_websockets       | 559 ms                                                 | 553 ms: 1.01x faster                                                   |
| async_generators         | 444 ms                                                 | 463 ms: 1.04x slower                                                   |
| unpickle                 | 14.4 us                                                | 15.3 us: 1.06x slower                                                  |
| pickle                   | 10.7 us                                                | 11.7 us: 1.10x slower                                                  |
| gc_traversal             | 3.62 ms                                                | 4.03 ms: 1.11x slower                                                  |
| pickle_dict              | 29.6 us                                                | 34.9 us: 1.18x slower                                                  |
| telco                    | 7.27 ms                                                | 8.62 ms: 1.19x slower                                                  |
| dask                     | 441 ms                                                 | 536 ms: 1.22x slower                                                   |
| coverage                 | 79.4 ms                                                | 96.9 ms: 1.22x slower                                                  |
| python_startup_no_site   | 5.93 ms                                                | 8.83 ms: 1.49x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.24x faster                                                           |

Benchmark hidden because not significant (3): mypy2, bench_mp_pool, pickle_list
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240305-3.13.0a4+-cbf3d38-PYTHON_UOPS/bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4+-cbf3d38.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.18x
- 95% likely to have a speedup of 1.17x
- 99% likely to have a speedup of 1.15x


# Memory

- memory change: 1.08x