# Results vs. 3.10.4

- fork: python
- ref: 61e54bfcee9f08a8e09a
- machine: linux-x86_64
- commit hash: 61e54bf
- commit date: 2024-03-14
- overall geometric mean: 1.29x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.21x faster
- Memory change: 1.33x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 282 ms: 1.24x faster                                                   |
| chameleon      | 9.68 ms                                                | 6.96 ms: 1.39x faster                                                  |
| docutils       | 3.30 sec                                               | 2.78 sec: 1.19x faster                                                 |
| html5lib       | 88.9 ms                                                | 66.8 ms: 1.33x faster                                                  |
| tornado_http   | 136 ms                                                 | 99.0 ms: 1.38x faster                                                  |
| Geometric mean | (ref)                                                  | 1.30x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 447 ms: 1.63x faster                                                   |
| async_tree_memoization  | 870 ms                                                 | 576 ms: 1.51x faster                                                   |
| async_tree_io           | 1.77 sec                                               | 1.22 sec: 1.46x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 731 ms: 1.39x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.49x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 92.7 ms: 1.66x faster                                                  |
| float          | 117 ms                                                 | 80.0 ms: 1.46x faster                                                  |
| pidigits       | 191 ms                                                 | 189 ms: 1.01x faster                                                   |
| Geometric mean | (ref)                                                  | 1.35x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 143 ms: 1.32x faster                                                   |
| regex_v8       | 27.8 ms                                                | 25.9 ms: 1.07x faster                                                  |
| regex_dna      | 227 ms                                                 | 234 ms: 1.03x slower                                                   |
| regex_effbot   | 3.63 ms                                                | 3.79 ms: 1.05x slower                                                  |
| Geometric mean | (ref)                                                  | 1.07x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 308 us: 1.57x faster                                                   |
| tomli_loads          | 3.14 sec                                               | 2.07 sec: 1.51x faster                                                 |
| unpickle_pure_python | 331 us                                                 | 239 us: 1.39x faster                                                   |
| json_dumps           | 14.2 ms                                                | 10.6 ms: 1.34x faster                                                  |
| xml_etree_process    | 79.1 ms                                                | 60.6 ms: 1.31x faster                                                  |
| xml_etree_generate   | 99.4 ms                                                | 88.6 ms: 1.12x faster                                                  |
| json_loads           | 31.2 us                                                | 28.1 us: 1.11x faster                                                  |
| xml_etree_iterparse  | 115 ms                                                 | 108 ms: 1.06x faster                                                   |
| unpickle_list        | 5.20 us                                                | 4.93 us: 1.05x faster                                                  |
| xml_etree_parse      | 168 ms                                                 | 160 ms: 1.05x faster                                                   |
| pickle_list          | 5.08 us                                                | 5.29 us: 1.04x slower                                                  |
| unpickle             | 14.4 us                                                | 15.4 us: 1.07x slower                                                  |
| pickle               | 10.7 us                                                | 11.9 us: 1.12x slower                                                  |
| pickle_dict          | 29.6 us                                                | 35.4 us: 1.20x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.13x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 12.6 ms: 1.16x faster                                                  |
| python_startup_no_site | 5.93 ms                                                | 11.2 ms: 1.88x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.27x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako            | 16.3 ms                                                | 11.1 ms: 1.47x faster                                                  |
| django_template | 48.2 ms                                                | 34.7 ms: 1.39x faster                                                  |
| genshi_text     | 31.8 ms                                                | 24.2 ms: 1.31x faster                                                  |
| genshi_xml      | 66.0 ms                                                | 54.6 ms: 1.21x faster                                                  |
| Geometric mean  | (ref)                                                  | 1.34x faster                                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 111 us: 4.91x faster                                                   |
| generators               | 80.1 ms                                                | 29.5 ms: 2.71x faster                                                  |
| deltablue                | 7.91 ms                                                | 3.42 ms: 2.32x faster                                                  |
| logging_silent           | 190 ns                                                 | 102 ns: 1.85x faster                                                   |
| asyncio_tcp              | 922 ms                                                 | 505 ms: 1.82x faster                                                   |
| chaos                    | 115 ms                                                 | 64.0 ms: 1.80x faster                                                  |
| richards_super           | 94.7 ms                                                | 53.1 ms: 1.79x faster                                                  |
| scimark_sor              | 220 ms                                                 | 127 ms: 1.72x faster                                                   |
| raytrace                 | 507 ms                                                 | 297 ms: 1.71x faster                                                   |
| richards                 | 79.3 ms                                                | 46.5 ms: 1.70x faster                                                  |
| pylint                   | 551 ms                                                 | 325 ms: 1.70x faster                                                   |
| scimark_monte_carlo      | 118 ms                                                 | 70.9 ms: 1.67x faster                                                  |
| crypto_pyaes             | 128 ms                                                 | 77.0 ms: 1.66x faster                                                  |
| nbody                    | 154 ms                                                 | 92.7 ms: 1.66x faster                                                  |
| comprehensions           | 28.8 us                                                | 17.5 us: 1.64x faster                                                  |
| sqlglot_parse            | 2.17 ms                                                | 1.32 ms: 1.64x faster                                                  |
| async_tree_none          | 728 ms                                                 | 447 ms: 1.63x faster                                                   |
| pickle_pure_python       | 484 us                                                 | 308 us: 1.57x faster                                                   |
| coroutines               | 35.1 ms                                                | 22.4 ms: 1.56x faster                                                  |
| sqlglot_transpile        | 2.57 ms                                                | 1.66 ms: 1.55x faster                                                  |
| go                       | 240 ms                                                 | 157 ms: 1.53x faster                                                   |
| tomli_loads              | 3.14 sec                                               | 2.07 sec: 1.51x faster                                                 |
| async_tree_memoization   | 870 ms                                                 | 576 ms: 1.51x faster                                                   |
| deepcopy_memo            | 58.5 us                                                | 38.9 us: 1.50x faster                                                  |
| spectral_norm            | 170 ms                                                 | 115 ms: 1.48x faster                                                   |
| hexiom                   | 10.4 ms                                                | 7.06 ms: 1.47x faster                                                  |
| mako                     | 16.3 ms                                                | 11.1 ms: 1.47x faster                                                  |
| float                    | 117 ms                                                 | 80.0 ms: 1.46x faster                                                  |
| async_tree_io            | 1.77 sec                                               | 1.22 sec: 1.46x faster                                                 |
| pyflate                  | 716 ms                                                 | 493 ms: 1.45x faster                                                   |
| logging_simple           | 8.30 us                                                | 5.77 us: 1.44x faster                                                  |
| logging_format           | 9.09 us                                                | 6.42 us: 1.42x faster                                                  |
| chameleon                | 9.68 ms                                                | 6.96 ms: 1.39x faster                                                  |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 731 ms: 1.39x faster                                                   |
| django_template          | 48.2 ms                                                | 34.7 ms: 1.39x faster                                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.85 sec: 1.39x faster                                                 |
| unpickle_pure_python     | 331 us                                                 | 239 us: 1.39x faster                                                   |
| tornado_http             | 136 ms                                                 | 99.0 ms: 1.38x faster                                                  |
| deepcopy                 | 479 us                                                 | 351 us: 1.37x faster                                                   |
| deepcopy_reduce          | 4.17 us                                                | 3.06 us: 1.36x faster                                                  |
| scimark_lu               | 176 ms                                                 | 129 ms: 1.36x faster                                                   |
| scimark_fft              | 466 ms                                                 | 345 ms: 1.35x faster                                                   |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.82 ms: 1.34x faster                                                  |
| json_dumps               | 14.2 ms                                                | 10.6 ms: 1.34x faster                                                  |
| thrift                   | 1.07 ms                                                | 804 us: 1.33x faster                                                   |
| fannkuch                 | 532 ms                                                 | 399 ms: 1.33x faster                                                   |
| html5lib                 | 88.9 ms                                                | 66.8 ms: 1.33x faster                                                  |
| pprint_pformat           | 2.10 sec                                               | 1.58 sec: 1.33x faster                                                 |
| sqlglot_normalize        | 143 ms                                                 | 108 ms: 1.32x faster                                                   |
| pprint_safe_repr         | 1.02 sec                                               | 770 ms: 1.32x faster                                                   |
| regex_compile            | 188 ms                                                 | 143 ms: 1.32x faster                                                   |
| genshi_text              | 31.8 ms                                                | 24.2 ms: 1.31x faster                                                  |
| xml_etree_process        | 79.1 ms                                                | 60.6 ms: 1.31x faster                                                  |
| pycparser                | 1.58 sec                                               | 1.26 sec: 1.25x faster                                                 |
| 2to3                     | 348 ms                                                 | 282 ms: 1.24x faster                                                   |
| sqlglot_optimize         | 69.2 ms                                                | 56.8 ms: 1.22x faster                                                  |
| sympy_sum                | 196 ms                                                 | 162 ms: 1.22x faster                                                   |
| sympy_integrate          | 25.8 ms                                                | 21.3 ms: 1.21x faster                                                  |
| genshi_xml               | 66.0 ms                                                | 54.6 ms: 1.21x faster                                                  |
| sympy_str                | 346 ms                                                 | 287 ms: 1.21x faster                                                   |
| dulwich_log              | 84.3 ms                                                | 70.0 ms: 1.20x faster                                                  |
| aiohttp                  | 1.44 ms                                                | 1.20 ms: 1.20x faster                                                  |
| djangocms                | 38.4 us                                                | 32.3 us: 1.19x faster                                                  |
| docutils                 | 3.30 sec                                               | 2.78 sec: 1.19x faster                                                 |
| dask                     | 441 ms                                                 | 373 ms: 1.18x faster                                                   |
| gunicorn                 | 1.53 ms                                                | 1.30 ms: 1.18x faster                                                  |
| nqueens                  | 106 ms                                                 | 90.0 ms: 1.18x faster                                                  |
| sympy_expand             | 566 ms                                                 | 486 ms: 1.17x faster                                                   |
| python_startup           | 14.6 ms                                                | 12.6 ms: 1.16x faster                                                  |
| bench_thread_pool        | 986 us                                                 | 864 us: 1.14x faster                                                   |
| xml_etree_generate       | 99.4 ms                                                | 88.6 ms: 1.12x faster                                                  |
| json_loads               | 31.2 us                                                | 28.1 us: 1.11x faster                                                  |
| mdp                      | 2.85 sec                                               | 2.61 sec: 1.09x faster                                                 |
| json                     | 5.69 ms                                                | 5.21 ms: 1.09x faster                                                  |
| pathlib                  | 20.5 ms                                                | 18.7 ms: 1.09x faster                                                  |
| meteor_contest           | 120 ms                                                 | 111 ms: 1.08x faster                                                   |
| create_gc_cycles         | 1.62 ms                                                | 1.51 ms: 1.07x faster                                                  |
| regex_v8                 | 27.8 ms                                                | 25.9 ms: 1.07x faster                                                  |
| xml_etree_iterparse      | 115 ms                                                 | 108 ms: 1.06x faster                                                   |
| unpickle_list            | 5.20 us                                                | 4.93 us: 1.05x faster                                                  |
| sqlite_synth             | 3.02 us                                                | 2.87 us: 1.05x faster                                                  |
| xml_etree_parse          | 168 ms                                                 | 160 ms: 1.05x faster                                                   |
| pidigits                 | 191 ms                                                 | 189 ms: 1.01x faster                                                   |
| asyncio_websockets       | 559 ms                                                 | 564 ms: 1.01x slower                                                   |
| regex_dna                | 227 ms                                                 | 234 ms: 1.03x slower                                                   |
| pickle_list              | 5.08 us                                                | 5.29 us: 1.04x slower                                                  |
| regex_effbot             | 3.63 ms                                                | 3.79 ms: 1.05x slower                                                  |
| async_generators         | 444 ms                                                 | 469 ms: 1.06x slower                                                   |
| unpickle                 | 14.4 us                                                | 15.4 us: 1.07x slower                                                  |
| bench_mp_pool            | 24.0 ms                                                | 26.8 ms: 1.11x slower                                                  |
| pickle                   | 10.7 us                                                | 11.9 us: 1.12x slower                                                  |
| gc_traversal             | 3.62 ms                                                | 4.07 ms: 1.12x slower                                                  |
| telco                    | 7.27 ms                                                | 8.43 ms: 1.16x slower                                                  |
| pickle_dict              | 29.6 us                                                | 35.4 us: 1.20x slower                                                  |
| coverage                 | 79.4 ms                                                | 98.5 ms: 1.24x slower                                                  |
| unpack_sequence          | 60.0 ns                                                | 87.8 ns: 1.46x slower                                                  |
| python_startup_no_site   | 5.93 ms                                                | 11.2 ms: 1.88x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.29x faster                                                           |

Benchmark hidden because not significant (1): mypy2
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240314-3.13.0a5+-61e54bf-JIT/bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.24x
- 95% likely to have a speedup of 1.23x
- 99% likely to have a speedup of 1.21x


# Memory

- memory change: 1.33x