
# Results vs. 3.10.4

- fork: faster-cpython
- ref: remove_pep_523_check
- machine: linux-x86_64
- commit hash: 42374f4
- commit date: 2024-01-17
- overall geometric mean: 1.28x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.22x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240117-linux-x86_64-faster%2dcpython-remove_pep_523_check-3.13.0a3+-42374f4 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 282 ms: 1.24x faster                                                             |
| chameleon      | 9.68 ms                                                | 7.31 ms: 1.32x faster                                                            |
| docutils       | 3.30 sec                                               | 2.70 sec: 1.22x faster                                                           |
| tornado_http   | 136 ms                                                 | 97.8 ms: 1.39x faster                                                            |
| Geometric mean | (ref)                                                  | 1.29x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240117-linux-x86_64-faster%2dcpython-remove_pep_523_check-3.13.0a3+-42374f4 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 449 ms: 1.62x faster                                                             |
| async_tree_memoization  | 870 ms                                                 | 576 ms: 1.51x faster                                                             |
| async_tree_io           | 1.77 sec                                               | 1.20 sec: 1.48x faster                                                           |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 721 ms: 1.41x faster                                                             |
| Geometric mean          | (ref)                                                  | 1.50x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240117-linux-x86_64-faster%2dcpython-remove_pep_523_check-3.13.0a3+-42374f4 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 114 ms: 1.34x faster                                                             |
| float          | 117 ms                                                 | 90.3 ms: 1.30x faster                                                            |
| pidigits       | 191 ms                                                 | 189 ms: 1.01x faster                                                             |
| Geometric mean | (ref)                                                  | 1.21x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240117-linux-x86_64-faster%2dcpython-remove_pep_523_check-3.13.0a3+-42374f4 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 149 ms: 1.26x faster                                                             |
| regex_v8       | 27.8 ms                                                | 24.9 ms: 1.12x faster                                                            |
| regex_effbot   | 3.63 ms                                                | 3.52 ms: 1.03x faster                                                            |
| regex_dna      | 227 ms                                                 | 223 ms: 1.02x faster                                                             |
| Geometric mean | (ref)                                                  | 1.10x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240117-linux-x86_64-faster%2dcpython-remove_pep_523_check-3.13.0a3+-42374f4 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 300 us: 1.61x faster                                                             |
| unpickle_pure_python | 331 us                                                 | 234 us: 1.41x faster                                                             |
| tomli_loads          | 3.14 sec                                               | 2.34 sec: 1.34x faster                                                           |
| json_dumps           | 14.2 ms                                                | 10.7 ms: 1.33x faster                                                            |
| xml_etree_process    | 79.1 ms                                                | 60.3 ms: 1.31x faster                                                            |
| xml_etree_generate   | 99.4 ms                                                | 88.2 ms: 1.13x faster                                                            |
| json_loads           | 31.2 us                                                | 28.3 us: 1.10x faster                                                            |
| xml_etree_parse      | 168 ms                                                 | 158 ms: 1.06x faster                                                             |
| xml_etree_iterparse  | 115 ms                                                 | 110 ms: 1.05x faster                                                             |
| unpickle_list        | 5.20 us                                                | 5.06 us: 1.03x faster                                                            |
| pickle_list          | 5.08 us                                                | 5.27 us: 1.04x slower                                                            |
| pickle               | 10.7 us                                                | 11.6 us: 1.08x slower                                                            |
| unpickle             | 14.4 us                                                | 16.4 us: 1.14x slower                                                            |
| pickle_dict          | 29.6 us                                                | 35.0 us: 1.18x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.12x faster                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240117-linux-x86_64-faster%2dcpython-remove_pep_523_check-3.13.0a3+-42374f4 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                            |
| python_startup_no_site | 5.93 ms                                                | 8.78 ms: 1.48x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240117-linux-x86_64-faster%2dcpython-remove_pep_523_check-3.13.0a3+-42374f4 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 13.2 ms: 1.24x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240117-linux-x86_64-faster%2dcpython-remove_pep_523_check-3.13.0a3+-42374f4 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 114 us: 4.77x faster                                                             |
| generators               | 80.1 ms                                                | 29.5 ms: 2.71x faster                                                            |
| asyncio_tcp              | 922 ms                                                 | 487 ms: 1.89x faster                                                             |
| logging_silent           | 190 ns                                                 | 103 ns: 1.84x faster                                                             |
| deltablue                | 7.91 ms                                                | 4.47 ms: 1.77x faster                                                            |
| richards_super           | 94.7 ms                                                | 53.9 ms: 1.76x faster                                                            |
| raytrace                 | 507 ms                                                 | 295 ms: 1.72x faster                                                             |
| richards                 | 79.3 ms                                                | 47.5 ms: 1.67x faster                                                            |
| scimark_sor              | 220 ms                                                 | 132 ms: 1.67x faster                                                             |
| sqlglot_parse            | 2.17 ms                                                | 1.32 ms: 1.65x faster                                                            |
| async_tree_none          | 728 ms                                                 | 449 ms: 1.62x faster                                                             |
| chaos                    | 115 ms                                                 | 71.5 ms: 1.62x faster                                                            |
| pickle_pure_python       | 484 us                                                 | 300 us: 1.61x faster                                                             |
| coroutines               | 35.1 ms                                                | 21.8 ms: 1.61x faster                                                            |
| crypto_pyaes             | 128 ms                                                 | 81.6 ms: 1.57x faster                                                            |
| go                       | 240 ms                                                 | 153 ms: 1.56x faster                                                             |
| sqlglot_transpile        | 2.57 ms                                                | 1.65 ms: 1.56x faster                                                            |
| async_tree_memoization   | 870 ms                                                 | 576 ms: 1.51x faster                                                             |
| scimark_monte_carlo      | 118 ms                                                 | 78.9 ms: 1.50x faster                                                            |
| scimark_lu               | 176 ms                                                 | 118 ms: 1.49x faster                                                             |
| async_tree_io            | 1.77 sec                                               | 1.20 sec: 1.48x faster                                                           |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                            |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                                           |
| deepcopy_memo            | 58.5 us                                                | 41.0 us: 1.42x faster                                                            |
| pyflate                  | 716 ms                                                 | 504 ms: 1.42x faster                                                             |
| unpickle_pure_python     | 331 us                                                 | 234 us: 1.41x faster                                                             |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 721 ms: 1.41x faster                                                             |
| comprehensions           | 28.8 us                                                | 20.4 us: 1.41x faster                                                            |
| tornado_http             | 136 ms                                                 | 97.8 ms: 1.39x faster                                                            |
| unpack_sequence          | 60.0 ns                                                | 43.1 ns: 1.39x faster                                                            |
| logging_simple           | 8.30 us                                                | 6.05 us: 1.37x faster                                                            |
| logging_format           | 9.09 us                                                | 6.74 us: 1.35x faster                                                            |
| tomli_loads              | 3.14 sec                                               | 2.34 sec: 1.34x faster                                                           |
| nbody                    | 154 ms                                                 | 114 ms: 1.34x faster                                                             |
| deepcopy                 | 479 us                                                 | 358 us: 1.34x faster                                                             |
| json_dumps               | 14.2 ms                                                | 10.7 ms: 1.33x faster                                                            |
| chameleon                | 9.68 ms                                                | 7.31 ms: 1.32x faster                                                            |
| deepcopy_reduce          | 4.17 us                                                | 3.16 us: 1.32x faster                                                            |
| pycparser                | 1.58 sec                                               | 1.20 sec: 1.31x faster                                                           |
| xml_etree_process        | 79.1 ms                                                | 60.3 ms: 1.31x faster                                                            |
| float                    | 117 ms                                                 | 90.3 ms: 1.30x faster                                                            |
| hexiom                   | 10.4 ms                                                | 8.05 ms: 1.29x faster                                                            |
| pprint_safe_repr         | 1.02 sec                                               | 805 ms: 1.26x faster                                                             |
| regex_compile            | 188 ms                                                 | 149 ms: 1.26x faster                                                             |
| sqlglot_normalize        | 143 ms                                                 | 113 ms: 1.26x faster                                                             |
| pprint_pformat           | 2.10 sec                                               | 1.68 sec: 1.25x faster                                                           |
| mako                     | 16.3 ms                                                | 13.2 ms: 1.24x faster                                                            |
| sympy_sum                | 196 ms                                                 | 159 ms: 1.24x faster                                                             |
| 2to3                     | 348 ms                                                 | 282 ms: 1.24x faster                                                             |
| fannkuch                 | 532 ms                                                 | 431 ms: 1.23x faster                                                             |
| sympy_integrate          | 25.8 ms                                                | 21.0 ms: 1.23x faster                                                            |
| docutils                 | 3.30 sec                                               | 2.70 sec: 1.22x faster                                                           |
| dulwich_log              | 84.3 ms                                                | 69.2 ms: 1.22x faster                                                            |
| spectral_norm            | 170 ms                                                 | 140 ms: 1.21x faster                                                             |
| sqlglot_optimize         | 69.2 ms                                                | 57.4 ms: 1.21x faster                                                            |
| sympy_str                | 346 ms                                                 | 289 ms: 1.20x faster                                                             |
| dask                     | 441 ms                                                 | 369 ms: 1.19x faster                                                             |
| bench_thread_pool        | 986 us                                                 | 846 us: 1.17x faster                                                             |
| nqueens                  | 106 ms                                                 | 91.1 ms: 1.16x faster                                                            |
| sympy_expand             | 566 ms                                                 | 487 ms: 1.16x faster                                                             |
| xml_etree_generate       | 99.4 ms                                                | 88.2 ms: 1.13x faster                                                            |
| regex_v8                 | 27.8 ms                                                | 24.9 ms: 1.12x faster                                                            |
| json_loads               | 31.2 us                                                | 28.3 us: 1.10x faster                                                            |
| json                     | 5.69 ms                                                | 5.17 ms: 1.10x faster                                                            |
| pathlib                  | 20.5 ms                                                | 18.6 ms: 1.10x faster                                                            |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.93 ms: 1.09x faster                                                            |
| create_gc_cycles         | 1.62 ms                                                | 1.49 ms: 1.09x faster                                                            |
| meteor_contest           | 120 ms                                                 | 112 ms: 1.06x faster                                                             |
| xml_etree_parse          | 168 ms                                                 | 158 ms: 1.06x faster                                                             |
| xml_etree_iterparse      | 115 ms                                                 | 110 ms: 1.05x faster                                                             |
| sqlite_synth             | 3.02 us                                                | 2.88 us: 1.05x faster                                                            |
| scimark_fft              | 466 ms                                                 | 450 ms: 1.04x faster                                                             |
| mdp                      | 2.85 sec                                               | 2.75 sec: 1.03x faster                                                           |
| regex_effbot             | 3.63 ms                                                | 3.52 ms: 1.03x faster                                                            |
| unpickle_list            | 5.20 us                                                | 5.06 us: 1.03x faster                                                            |
| regex_dna                | 227 ms                                                 | 223 ms: 1.02x faster                                                             |
| asyncio_websockets       | 559 ms                                                 | 551 ms: 1.01x faster                                                             |
| pidigits                 | 191 ms                                                 | 189 ms: 1.01x faster                                                             |
| async_generators         | 444 ms                                                 | 458 ms: 1.03x slower                                                             |
| gc_traversal             | 3.62 ms                                                | 3.76 ms: 1.04x slower                                                            |
| pickle_list              | 5.08 us                                                | 5.27 us: 1.04x slower                                                            |
| pickle                   | 10.7 us                                                | 11.6 us: 1.08x slower                                                            |
| unpickle                 | 14.4 us                                                | 16.4 us: 1.14x slower                                                            |
| pickle_dict              | 29.6 us                                                | 35.0 us: 1.18x slower                                                            |
| telco                    | 7.27 ms                                                | 8.69 ms: 1.20x slower                                                            |
| coverage                 | 79.4 ms                                                | 96.4 ms: 1.21x slower                                                            |
| python_startup_no_site   | 5.93 ms                                                | 8.78 ms: 1.48x slower                                                            |
| Geometric mean           | (ref)                                                  | 1.28x faster                                                                     |

Benchmark hidden because not significant (2): mypy2, bench_mp_pool
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240117-3.13.0a3+-42374f4-PYTHON_UOPS/bm-20240117-linux-x86_64-faster%2dcpython-remove_pep_523_check-3.13.0a3+-42374f4.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.23x
- 95% likely to have a speedup of 1.23x
- 99% likely to have a speedup of 1.22x


# Memory

- memory change: 1.06x