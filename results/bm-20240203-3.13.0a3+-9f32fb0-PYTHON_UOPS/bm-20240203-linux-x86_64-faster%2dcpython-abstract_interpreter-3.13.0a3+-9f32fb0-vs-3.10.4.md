
# Results vs. 3.10.4

- fork: faster-cpython
- ref: abstract_interpreter
- machine: linux-x86_64
- commit hash: 9f32fb0
- commit date: 2024-02-03
- overall geometric mean: 1.28x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.20x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 284 ms: 1.23x faster                                                             |
| chameleon      | 9.68 ms                                                | 7.28 ms: 1.33x faster                                                            |
| docutils       | 3.30 sec                                               | 2.70 sec: 1.22x faster                                                           |
| tornado_http   | 136 ms                                                 | 99.0 ms: 1.38x faster                                                            |
| Geometric mean | (ref)                                                  | 1.29x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 448 ms: 1.62x faster                                                             |
| async_tree_memoization  | 870 ms                                                 | 575 ms: 1.51x faster                                                             |
| async_tree_io           | 1.77 sec                                               | 1.19 sec: 1.48x faster                                                           |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 717 ms: 1.42x faster                                                             |
| Geometric mean          | (ref)                                                  | 1.51x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 109 ms: 1.41x faster                                                             |
| float          | 117 ms                                                 | 90.0 ms: 1.30x faster                                                            |
| pidigits       | 191 ms                                                 | 188 ms: 1.01x faster                                                             |
| Geometric mean | (ref)                                                  | 1.23x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 149 ms: 1.26x faster                                                             |
| regex_v8       | 27.8 ms                                                | 25.0 ms: 1.11x faster                                                            |
| regex_dna      | 227 ms                                                 | 220 ms: 1.03x faster                                                             |
| Geometric mean | (ref)                                                  | 1.09x faster                                                                     |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 301 us: 1.61x faster                                                             |
| unpickle_pure_python | 331 us                                                 | 234 us: 1.41x faster                                                             |
| json_dumps           | 14.2 ms                                                | 10.7 ms: 1.33x faster                                                            |
| xml_etree_process    | 79.1 ms                                                | 60.1 ms: 1.32x faster                                                            |
| tomli_loads          | 3.14 sec                                               | 2.55 sec: 1.23x faster                                                           |
| xml_etree_generate   | 99.4 ms                                                | 88.3 ms: 1.13x faster                                                            |
| json_loads           | 31.2 us                                                | 28.6 us: 1.09x faster                                                            |
| xml_etree_parse      | 168 ms                                                 | 157 ms: 1.07x faster                                                             |
| xml_etree_iterparse  | 115 ms                                                 | 108 ms: 1.07x faster                                                             |
| unpickle_list        | 5.20 us                                                | 5.02 us: 1.04x faster                                                            |
| pickle_list          | 5.08 us                                                | 5.26 us: 1.04x slower                                                            |
| pickle               | 10.7 us                                                | 11.7 us: 1.10x slower                                                            |
| unpickle             | 14.4 us                                                | 16.3 us: 1.13x slower                                                            |
| pickle_dict          | 29.6 us                                                | 34.6 us: 1.17x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.12x faster                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                            |
| python_startup_no_site | 5.93 ms                                                | 8.80 ms: 1.48x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.02x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 13.1 ms: 1.24x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 112 us: 4.88x faster                                                             |
| generators               | 80.1 ms                                                | 30.3 ms: 2.65x faster                                                            |
| deltablue                | 7.91 ms                                                | 3.54 ms: 2.24x faster                                                            |
| asyncio_tcp              | 922 ms                                                 | 491 ms: 1.88x faster                                                             |
| logging_silent           | 190 ns                                                 | 105 ns: 1.81x faster                                                             |
| scimark_sor              | 220 ms                                                 | 122 ms: 1.80x faster                                                             |
| richards_super           | 94.7 ms                                                | 54.5 ms: 1.74x faster                                                            |
| raytrace                 | 507 ms                                                 | 301 ms: 1.68x faster                                                             |
| sqlglot_parse            | 2.17 ms                                                | 1.33 ms: 1.64x faster                                                            |
| richards                 | 79.3 ms                                                | 48.8 ms: 1.63x faster                                                            |
| async_tree_none          | 728 ms                                                 | 448 ms: 1.62x faster                                                             |
| pickle_pure_python       | 484 us                                                 | 301 us: 1.61x faster                                                             |
| chaos                    | 115 ms                                                 | 72.2 ms: 1.60x faster                                                            |
| coroutines               | 35.1 ms                                                | 22.0 ms: 1.59x faster                                                            |
| crypto_pyaes             | 128 ms                                                 | 81.7 ms: 1.56x faster                                                            |
| sqlglot_transpile        | 2.57 ms                                                | 1.66 ms: 1.55x faster                                                            |
| async_tree_memoization   | 870 ms                                                 | 575 ms: 1.51x faster                                                             |
| scimark_lu               | 176 ms                                                 | 117 ms: 1.51x faster                                                             |
| async_tree_io            | 1.77 sec                                               | 1.19 sec: 1.48x faster                                                           |
| scimark_monte_carlo      | 118 ms                                                 | 79.9 ms: 1.48x faster                                                            |
| deepcopy_memo            | 58.5 us                                                | 39.6 us: 1.48x faster                                                            |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                            |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                                           |
| logging_simple           | 8.30 us                                                | 5.85 us: 1.42x faster                                                            |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 717 ms: 1.42x faster                                                             |
| unpickle_pure_python     | 331 us                                                 | 234 us: 1.41x faster                                                             |
| nbody                    | 154 ms                                                 | 109 ms: 1.41x faster                                                             |
| pyflate                  | 716 ms                                                 | 509 ms: 1.41x faster                                                             |
| comprehensions           | 28.8 us                                                | 20.8 us: 1.39x faster                                                            |
| tornado_http             | 136 ms                                                 | 99.0 ms: 1.38x faster                                                            |
| go                       | 240 ms                                                 | 175 ms: 1.37x faster                                                             |
| logging_format           | 9.09 us                                                | 6.63 us: 1.37x faster                                                            |
| deepcopy                 | 479 us                                                 | 358 us: 1.34x faster                                                             |
| chameleon                | 9.68 ms                                                | 7.28 ms: 1.33x faster                                                            |
| json_dumps               | 14.2 ms                                                | 10.7 ms: 1.33x faster                                                            |
| deepcopy_reduce          | 4.17 us                                                | 3.14 us: 1.33x faster                                                            |
| xml_etree_process        | 79.1 ms                                                | 60.1 ms: 1.32x faster                                                            |
| float                    | 117 ms                                                 | 90.0 ms: 1.30x faster                                                            |
| hexiom                   | 10.4 ms                                                | 8.11 ms: 1.28x faster                                                            |
| pprint_safe_repr         | 1.02 sec                                               | 795 ms: 1.28x faster                                                             |
| pprint_pformat           | 2.10 sec                                               | 1.65 sec: 1.28x faster                                                           |
| spectral_norm            | 170 ms                                                 | 134 ms: 1.27x faster                                                             |
| sqlglot_normalize        | 143 ms                                                 | 113 ms: 1.27x faster                                                             |
| regex_compile            | 188 ms                                                 | 149 ms: 1.26x faster                                                             |
| mako                     | 16.3 ms                                                | 13.1 ms: 1.24x faster                                                            |
| pycparser                | 1.58 sec                                               | 1.27 sec: 1.24x faster                                                           |
| sympy_integrate          | 25.8 ms                                                | 20.9 ms: 1.23x faster                                                            |
| tomli_loads              | 3.14 sec                                               | 2.55 sec: 1.23x faster                                                           |
| 2to3                     | 348 ms                                                 | 284 ms: 1.23x faster                                                             |
| sympy_sum                | 196 ms                                                 | 160 ms: 1.23x faster                                                             |
| docutils                 | 3.30 sec                                               | 2.70 sec: 1.22x faster                                                           |
| sqlglot_optimize         | 69.2 ms                                                | 57.1 ms: 1.21x faster                                                            |
| dulwich_log              | 84.3 ms                                                | 69.9 ms: 1.21x faster                                                            |
| fannkuch                 | 532 ms                                                 | 441 ms: 1.21x faster                                                             |
| dask                     | 441 ms                                                 | 370 ms: 1.19x faster                                                             |
| unpack_sequence          | 60.0 ns                                                | 50.7 ns: 1.18x faster                                                            |
| sympy_str                | 346 ms                                                 | 293 ms: 1.18x faster                                                             |
| bench_thread_pool        | 986 us                                                 | 848 us: 1.16x faster                                                             |
| nqueens                  | 106 ms                                                 | 92.3 ms: 1.15x faster                                                            |
| sympy_expand             | 566 ms                                                 | 496 ms: 1.14x faster                                                             |
| xml_etree_generate       | 99.4 ms                                                | 88.3 ms: 1.13x faster                                                            |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.75 ms: 1.12x faster                                                            |
| regex_v8                 | 27.8 ms                                                | 25.0 ms: 1.11x faster                                                            |
| pathlib                  | 20.5 ms                                                | 18.5 ms: 1.11x faster                                                            |
| create_gc_cycles         | 1.62 ms                                                | 1.47 ms: 1.10x faster                                                            |
| json_loads               | 31.2 us                                                | 28.6 us: 1.09x faster                                                            |
| scimark_fft              | 466 ms                                                 | 431 ms: 1.08x faster                                                             |
| json                     | 5.69 ms                                                | 5.26 ms: 1.08x faster                                                            |
| mdp                      | 2.85 sec                                               | 2.66 sec: 1.07x faster                                                           |
| xml_etree_parse          | 168 ms                                                 | 157 ms: 1.07x faster                                                             |
| xml_etree_iterparse      | 115 ms                                                 | 108 ms: 1.07x faster                                                             |
| meteor_contest           | 120 ms                                                 | 112 ms: 1.07x faster                                                             |
| sqlite_synth             | 3.02 us                                                | 2.85 us: 1.06x faster                                                            |
| unpickle_list            | 5.20 us                                                | 5.02 us: 1.04x faster                                                            |
| regex_dna                | 227 ms                                                 | 220 ms: 1.03x faster                                                             |
| pidigits                 | 191 ms                                                 | 188 ms: 1.01x faster                                                             |
| asyncio_websockets       | 559 ms                                                 | 551 ms: 1.01x faster                                                             |
| async_generators         | 444 ms                                                 | 457 ms: 1.03x slower                                                             |
| pickle_list              | 5.08 us                                                | 5.26 us: 1.04x slower                                                            |
| gc_traversal             | 3.62 ms                                                | 3.79 ms: 1.05x slower                                                            |
| pickle                   | 10.7 us                                                | 11.7 us: 1.10x slower                                                            |
| unpickle                 | 14.4 us                                                | 16.3 us: 1.13x slower                                                            |
| pickle_dict              | 29.6 us                                                | 34.6 us: 1.17x slower                                                            |
| coverage                 | 79.4 ms                                                | 95.8 ms: 1.21x slower                                                            |
| telco                    | 7.27 ms                                                | 8.79 ms: 1.21x slower                                                            |
| python_startup_no_site   | 5.93 ms                                                | 8.80 ms: 1.48x slower                                                            |
| Geometric mean           | (ref)                                                  | 1.28x faster                                                                     |

Benchmark hidden because not significant (2): bench_mp_pool, regex_effbot
Ignored benchmarks (13) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240203-3.13.0a3+-9f32fb0-PYTHON_UOPS/bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.22x
- 95% likely to have a speedup of 1.22x
- 99% likely to have a speedup of 1.20x


# Memory

- memory change: 1.06x