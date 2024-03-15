
# Results vs. 3.10.4

- fork: faster-cpython
- ref: abstract_interpreter
- machine: linux-x86_64
- commit hash: a932d36
- commit date: 2024-02-02
- overall geometric mean: 1.27x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.19x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 284 ms: 1.23x faster                                                             |
| chameleon      | 9.68 ms                                                | 7.32 ms: 1.32x faster                                                            |
| docutils       | 3.30 sec                                               | 2.72 sec: 1.21x faster                                                           |
| tornado_http   | 136 ms                                                 | 99.2 ms: 1.37x faster                                                            |
| Geometric mean | (ref)                                                  | 1.28x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 449 ms: 1.62x faster                                                             |
| async_tree_memoization  | 870 ms                                                 | 570 ms: 1.53x faster                                                             |
| async_tree_io           | 1.77 sec                                               | 1.19 sec: 1.49x faster                                                           |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 720 ms: 1.41x faster                                                             |
| Geometric mean          | (ref)                                                  | 1.51x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 117 ms: 1.31x faster                                                             |
| float          | 117 ms                                                 | 93.1 ms: 1.26x faster                                                            |
| pidigits       | 191 ms                                                 | 189 ms: 1.01x faster                                                             |
| Geometric mean | (ref)                                                  | 1.18x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 151 ms: 1.25x faster                                                             |
| regex_v8       | 27.8 ms                                                | 24.8 ms: 1.12x faster                                                            |
| regex_effbot   | 3.63 ms                                                | 3.74 ms: 1.03x slower                                                            |
| Geometric mean | (ref)                                                  | 1.08x faster                                                                     |

Benchmark hidden because not significant (1): regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 300 us: 1.62x faster                                                             |
| unpickle_pure_python | 331 us                                                 | 235 us: 1.40x faster                                                             |
| json_dumps           | 14.2 ms                                                | 10.6 ms: 1.34x faster                                                            |
| xml_etree_process    | 79.1 ms                                                | 60.7 ms: 1.30x faster                                                            |
| tomli_loads          | 3.14 sec                                               | 2.59 sec: 1.21x faster                                                           |
| xml_etree_generate   | 99.4 ms                                                | 89.1 ms: 1.12x faster                                                            |
| json_loads           | 31.2 us                                                | 28.6 us: 1.09x faster                                                            |
| xml_etree_parse      | 168 ms                                                 | 158 ms: 1.06x faster                                                             |
| xml_etree_iterparse  | 115 ms                                                 | 109 ms: 1.06x faster                                                             |
| unpickle_list        | 5.20 us                                                | 4.96 us: 1.05x faster                                                            |
| pickle_list          | 5.08 us                                                | 5.37 us: 1.06x slower                                                            |
| pickle               | 10.7 us                                                | 11.8 us: 1.11x slower                                                            |
| unpickle             | 14.4 us                                                | 17.0 us: 1.18x slower                                                            |
| pickle_dict          | 29.6 us                                                | 36.6 us: 1.24x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.10x faster                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                            |
| python_startup_no_site | 5.93 ms                                                | 8.84 ms: 1.49x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.02x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 14.0 ms: 1.17x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 112 us: 4.88x faster                                                             |
| generators               | 80.1 ms                                                | 29.8 ms: 2.69x faster                                                            |
| deltablue                | 7.91 ms                                                | 3.57 ms: 2.22x faster                                                            |
| asyncio_tcp              | 922 ms                                                 | 492 ms: 1.87x faster                                                             |
| logging_silent           | 190 ns                                                 | 103 ns: 1.84x faster                                                             |
| scimark_sor              | 220 ms                                                 | 126 ms: 1.75x faster                                                             |
| richards_super           | 94.7 ms                                                | 54.2 ms: 1.75x faster                                                            |
| raytrace                 | 507 ms                                                 | 301 ms: 1.68x faster                                                             |
| richards                 | 79.3 ms                                                | 48.6 ms: 1.63x faster                                                            |
| sqlglot_parse            | 2.17 ms                                                | 1.34 ms: 1.62x faster                                                            |
| async_tree_none          | 728 ms                                                 | 449 ms: 1.62x faster                                                             |
| pickle_pure_python       | 484 us                                                 | 300 us: 1.62x faster                                                             |
| chaos                    | 115 ms                                                 | 72.4 ms: 1.59x faster                                                            |
| coroutines               | 35.1 ms                                                | 22.2 ms: 1.58x faster                                                            |
| sqlglot_transpile        | 2.57 ms                                                | 1.67 ms: 1.54x faster                                                            |
| async_tree_memoization   | 870 ms                                                 | 570 ms: 1.53x faster                                                             |
| crypto_pyaes             | 128 ms                                                 | 83.9 ms: 1.52x faster                                                            |
| unpack_sequence          | 60.0 ns                                                | 39.4 ns: 1.52x faster                                                            |
| scimark_lu               | 176 ms                                                 | 116 ms: 1.52x faster                                                             |
| async_tree_io            | 1.77 sec                                               | 1.19 sec: 1.49x faster                                                           |
| scimark_monte_carlo      | 118 ms                                                 | 81.0 ms: 1.46x faster                                                            |
| deepcopy_memo            | 58.5 us                                                | 40.3 us: 1.45x faster                                                            |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.79 sec: 1.43x faster                                                           |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                            |
| logging_simple           | 8.30 us                                                | 5.88 us: 1.41x faster                                                            |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 720 ms: 1.41x faster                                                             |
| unpickle_pure_python     | 331 us                                                 | 235 us: 1.40x faster                                                             |
| go                       | 240 ms                                                 | 173 ms: 1.39x faster                                                             |
| pyflate                  | 716 ms                                                 | 519 ms: 1.38x faster                                                             |
| tornado_http             | 136 ms                                                 | 99.2 ms: 1.37x faster                                                            |
| logging_format           | 9.09 us                                                | 6.68 us: 1.36x faster                                                            |
| comprehensions           | 28.8 us                                                | 21.3 us: 1.35x faster                                                            |
| json_dumps               | 14.2 ms                                                | 10.6 ms: 1.34x faster                                                            |
| deepcopy_reduce          | 4.17 us                                                | 3.14 us: 1.33x faster                                                            |
| chameleon                | 9.68 ms                                                | 7.32 ms: 1.32x faster                                                            |
| deepcopy                 | 479 us                                                 | 362 us: 1.32x faster                                                             |
| nbody                    | 154 ms                                                 | 117 ms: 1.31x faster                                                             |
| xml_etree_process        | 79.1 ms                                                | 60.7 ms: 1.30x faster                                                            |
| pycparser                | 1.58 sec                                               | 1.24 sec: 1.27x faster                                                           |
| sqlglot_normalize        | 143 ms                                                 | 113 ms: 1.27x faster                                                             |
| pprint_safe_repr         | 1.02 sec                                               | 804 ms: 1.27x faster                                                             |
| pprint_pformat           | 2.10 sec                                               | 1.67 sec: 1.26x faster                                                           |
| float                    | 117 ms                                                 | 93.1 ms: 1.26x faster                                                            |
| regex_compile            | 188 ms                                                 | 151 ms: 1.25x faster                                                             |
| hexiom                   | 10.4 ms                                                | 8.38 ms: 1.24x faster                                                            |
| 2to3                     | 348 ms                                                 | 284 ms: 1.23x faster                                                             |
| sympy_integrate          | 25.8 ms                                                | 21.1 ms: 1.22x faster                                                            |
| sympy_sum                | 196 ms                                                 | 161 ms: 1.22x faster                                                             |
| dulwich_log              | 84.3 ms                                                | 69.0 ms: 1.22x faster                                                            |
| docutils                 | 3.30 sec                                               | 2.72 sec: 1.21x faster                                                           |
| tomli_loads              | 3.14 sec                                               | 2.59 sec: 1.21x faster                                                           |
| sqlglot_optimize         | 69.2 ms                                                | 57.4 ms: 1.20x faster                                                            |
| dask                     | 441 ms                                                 | 369 ms: 1.20x faster                                                             |
| fannkuch                 | 532 ms                                                 | 445 ms: 1.19x faster                                                             |
| sympy_str                | 346 ms                                                 | 291 ms: 1.19x faster                                                             |
| mako                     | 16.3 ms                                                | 14.0 ms: 1.17x faster                                                            |
| bench_thread_pool        | 986 us                                                 | 848 us: 1.16x faster                                                             |
| sympy_expand             | 566 ms                                                 | 488 ms: 1.16x faster                                                             |
| spectral_norm            | 170 ms                                                 | 147 ms: 1.15x faster                                                             |
| regex_v8                 | 27.8 ms                                                | 24.8 ms: 1.12x faster                                                            |
| nqueens                  | 106 ms                                                 | 94.5 ms: 1.12x faster                                                            |
| xml_etree_generate       | 99.4 ms                                                | 89.1 ms: 1.12x faster                                                            |
| pathlib                  | 20.5 ms                                                | 18.4 ms: 1.11x faster                                                            |
| create_gc_cycles         | 1.62 ms                                                | 1.48 ms: 1.10x faster                                                            |
| json_loads               | 31.2 us                                                | 28.6 us: 1.09x faster                                                            |
| json                     | 5.69 ms                                                | 5.27 ms: 1.08x faster                                                            |
| scimark_fft              | 466 ms                                                 | 436 ms: 1.07x faster                                                             |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 6.06 ms: 1.07x faster                                                            |
| sqlite_synth             | 3.02 us                                                | 2.84 us: 1.06x faster                                                            |
| xml_etree_parse          | 168 ms                                                 | 158 ms: 1.06x faster                                                             |
| mdp                      | 2.85 sec                                               | 2.69 sec: 1.06x faster                                                           |
| xml_etree_iterparse      | 115 ms                                                 | 109 ms: 1.06x faster                                                             |
| unpickle_list            | 5.20 us                                                | 4.96 us: 1.05x faster                                                            |
| gc_traversal             | 3.62 ms                                                | 3.49 ms: 1.04x faster                                                            |
| meteor_contest           | 120 ms                                                 | 116 ms: 1.03x faster                                                             |
| asyncio_websockets       | 559 ms                                                 | 551 ms: 1.01x faster                                                             |
| pidigits                 | 191 ms                                                 | 189 ms: 1.01x faster                                                             |
| async_generators         | 444 ms                                                 | 450 ms: 1.01x slower                                                             |
| regex_effbot             | 3.63 ms                                                | 3.74 ms: 1.03x slower                                                            |
| pickle_list              | 5.08 us                                                | 5.37 us: 1.06x slower                                                            |
| pickle                   | 10.7 us                                                | 11.8 us: 1.11x slower                                                            |
| unpickle                 | 14.4 us                                                | 17.0 us: 1.18x slower                                                            |
| coverage                 | 79.4 ms                                                | 96.1 ms: 1.21x slower                                                            |
| telco                    | 7.27 ms                                                | 8.97 ms: 1.23x slower                                                            |
| pickle_dict              | 29.6 us                                                | 36.6 us: 1.24x slower                                                            |
| python_startup_no_site   | 5.93 ms                                                | 8.84 ms: 1.49x slower                                                            |
| Geometric mean           | (ref)                                                  | 1.27x faster                                                                     |

Benchmark hidden because not significant (3): mypy2, bench_mp_pool, regex_dna
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240202-3.13.0a3+-a932d36-PYTHON_UOPS/bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.21x
- 95% likely to have a speedup of 1.21x
- 99% likely to have a speedup of 1.19x


# Memory

- memory change: 1.06x