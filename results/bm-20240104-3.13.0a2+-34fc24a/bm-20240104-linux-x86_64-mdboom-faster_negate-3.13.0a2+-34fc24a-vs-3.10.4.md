
# Results vs. 3.10.4

- fork: mdboom
- ref: faster_negate
- machine: linux-x86_64
- commit hash: 34fc24a
- commit date: 2024-01-04
- overall geometric mean: 1.35x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.28x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 265 ms: 1.32x faster                                            |
| chameleon      | 9.68 ms                                                | 6.87 ms: 1.41x faster                                           |
| docutils       | 3.30 sec                                               | 2.59 sec: 1.27x faster                                          |
| tornado_http   | 136 ms                                                 | 94.2 ms: 1.45x faster                                           |
| Geometric mean | (ref)                                                  | 1.36x faster                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 434 ms: 1.68x faster                                            |
| async_tree_memoization  | 870 ms                                                 | 558 ms: 1.56x faster                                            |
| async_tree_io           | 1.77 sec                                               | 1.17 sec: 1.51x faster                                          |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 703 ms: 1.45x faster                                            |
| Geometric mean          | (ref)                                                  | 1.54x faster                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 90.1 ms: 1.70x faster                                           |
| float          | 117 ms                                                 | 80.3 ms: 1.46x faster                                           |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                            |
| Geometric mean | (ref)                                                  | 1.36x faster                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 130 ms: 1.44x faster                                            |
| regex_v8       | 27.8 ms                                                | 25.0 ms: 1.11x faster                                           |
| regex_dna      | 227 ms                                                 | 225 ms: 1.01x faster                                            |
| Geometric mean | (ref)                                                  | 1.13x faster                                                    |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 305 us: 1.59x faster                                            |
| unpickle_pure_python | 331 us                                                 | 219 us: 1.51x faster                                            |
| tomli_loads          | 3.14 sec                                               | 2.18 sec: 1.44x faster                                          |
| json_dumps           | 14.2 ms                                                | 10.5 ms: 1.34x faster                                           |
| xml_etree_process    | 79.1 ms                                                | 58.9 ms: 1.34x faster                                           |
| xml_etree_generate   | 99.4 ms                                                | 85.8 ms: 1.16x faster                                           |
| json_loads           | 31.2 us                                                | 28.3 us: 1.10x faster                                           |
| xml_etree_iterparse  | 115 ms                                                 | 105 ms: 1.10x faster                                            |
| xml_etree_parse      | 168 ms                                                 | 160 ms: 1.05x faster                                            |
| pickle_list          | 5.08 us                                                | 4.90 us: 1.04x faster                                           |
| unpickle_list        | 5.20 us                                                | 5.10 us: 1.02x faster                                           |
| pickle               | 10.7 us                                                | 11.4 us: 1.07x slower                                           |
| unpickle             | 14.4 us                                                | 15.7 us: 1.09x slower                                           |
| pickle_dict          | 29.6 us                                                | 34.2 us: 1.16x slower                                           |
| Geometric mean       | (ref)                                                  | 1.15x faster                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.44x faster                                           |
| python_startup_no_site | 5.93 ms                                                | 8.73 ms: 1.47x slower                                           |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|-----------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.2 ms: 1.45x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|--------------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 109 us: 5.01x faster                                            |
| generators               | 80.1 ms                                                | 29.5 ms: 2.71x faster                                           |
| deltablue                | 7.91 ms                                                | 3.25 ms: 2.43x faster                                           |
| raytrace                 | 507 ms                                                 | 261 ms: 1.94x faster                                            |
| chaos                    | 115 ms                                                 | 60.1 ms: 1.92x faster                                           |
| asyncio_tcp              | 922 ms                                                 | 484 ms: 1.90x faster                                            |
| logging_silent           | 190 ns                                                 | 103 ns: 1.84x faster                                            |
| crypto_pyaes             | 128 ms                                                 | 71.8 ms: 1.78x faster                                           |
| richards_super           | 94.7 ms                                                | 53.7 ms: 1.76x faster                                           |
| comprehensions           | 28.8 us                                                | 16.4 us: 1.75x faster                                           |
| sqlglot_parse            | 2.17 ms                                                | 1.24 ms: 1.74x faster                                           |
| scimark_monte_carlo      | 118 ms                                                 | 68.4 ms: 1.73x faster                                           |
| go                       | 240 ms                                                 | 141 ms: 1.71x faster                                            |
| nbody                    | 154 ms                                                 | 90.1 ms: 1.70x faster                                           |
| scimark_sor              | 220 ms                                                 | 130 ms: 1.68x faster                                            |
| richards                 | 79.3 ms                                                | 47.2 ms: 1.68x faster                                           |
| async_tree_none          | 728 ms                                                 | 434 ms: 1.68x faster                                            |
| hexiom                   | 10.4 ms                                                | 6.29 ms: 1.65x faster                                           |
| sqlglot_transpile        | 2.57 ms                                                | 1.56 ms: 1.65x faster                                           |
| pickle_pure_python       | 484 us                                                 | 305 us: 1.59x faster                                            |
| coroutines               | 35.1 ms                                                | 22.1 ms: 1.59x faster                                           |
| pyflate                  | 716 ms                                                 | 456 ms: 1.57x faster                                            |
| scimark_lu               | 176 ms                                                 | 112 ms: 1.57x faster                                            |
| async_tree_memoization   | 870 ms                                                 | 558 ms: 1.56x faster                                            |
| deepcopy_memo            | 58.5 us                                                | 38.6 us: 1.52x faster                                           |
| unpickle_pure_python     | 331 us                                                 | 219 us: 1.51x faster                                            |
| async_tree_io            | 1.77 sec                                               | 1.17 sec: 1.51x faster                                          |
| logging_simple           | 8.30 us                                                | 5.58 us: 1.49x faster                                           |
| spectral_norm            | 170 ms                                                 | 115 ms: 1.47x faster                                            |
| logging_format           | 9.09 us                                                | 6.19 us: 1.47x faster                                           |
| float                    | 117 ms                                                 | 80.3 ms: 1.46x faster                                           |
| mako                     | 16.3 ms                                                | 11.2 ms: 1.45x faster                                           |
| tornado_http             | 136 ms                                                 | 94.2 ms: 1.45x faster                                           |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 703 ms: 1.45x faster                                            |
| regex_compile            | 188 ms                                                 | 130 ms: 1.44x faster                                            |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.78 sec: 1.44x faster                                          |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.44x faster                                           |
| tomli_loads              | 3.14 sec                                               | 2.18 sec: 1.44x faster                                          |
| chameleon                | 9.68 ms                                                | 6.87 ms: 1.41x faster                                           |
| pprint_pformat           | 2.10 sec                                               | 1.50 sec: 1.40x faster                                          |
| deepcopy                 | 479 us                                                 | 346 us: 1.39x faster                                            |
| pprint_safe_repr         | 1.02 sec                                               | 737 ms: 1.38x faster                                            |
| unpack_sequence          | 60.0 ns                                                | 44.1 ns: 1.36x faster                                           |
| deepcopy_reduce          | 4.17 us                                                | 3.08 us: 1.35x faster                                           |
| sqlglot_normalize        | 143 ms                                                 | 106 ms: 1.35x faster                                            |
| pycparser                | 1.58 sec                                               | 1.17 sec: 1.35x faster                                          |
| json_dumps               | 14.2 ms                                                | 10.5 ms: 1.34x faster                                           |
| xml_etree_process        | 79.1 ms                                                | 58.9 ms: 1.34x faster                                           |
| sympy_sum                | 196 ms                                                 | 148 ms: 1.33x faster                                            |
| sympy_integrate          | 25.8 ms                                                | 19.5 ms: 1.32x faster                                           |
| fannkuch                 | 532 ms                                                 | 403 ms: 1.32x faster                                            |
| 2to3                     | 348 ms                                                 | 265 ms: 1.32x faster                                            |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.00 ms: 1.29x faster                                           |
| dulwich_log              | 84.3 ms                                                | 65.1 ms: 1.29x faster                                           |
| sqlglot_optimize         | 69.2 ms                                                | 53.5 ms: 1.29x faster                                           |
| sympy_str                | 346 ms                                                 | 268 ms: 1.29x faster                                            |
| scimark_fft              | 466 ms                                                 | 364 ms: 1.28x faster                                            |
| docutils                 | 3.30 sec                                               | 2.59 sec: 1.27x faster                                          |
| nqueens                  | 106 ms                                                 | 83.9 ms: 1.26x faster                                           |
| sympy_expand             | 566 ms                                                 | 457 ms: 1.24x faster                                            |
| dask                     | 441 ms                                                 | 360 ms: 1.22x faster                                            |
| bench_thread_pool        | 986 us                                                 | 830 us: 1.19x faster                                            |
| xml_etree_generate       | 99.4 ms                                                | 85.8 ms: 1.16x faster                                           |
| pathlib                  | 20.5 ms                                                | 18.2 ms: 1.12x faster                                           |
| meteor_contest           | 120 ms                                                 | 107 ms: 1.12x faster                                            |
| regex_v8                 | 27.8 ms                                                | 25.0 ms: 1.11x faster                                           |
| mdp                      | 2.85 sec                                               | 2.57 sec: 1.11x faster                                          |
| json_loads               | 31.2 us                                                | 28.3 us: 1.10x faster                                           |
| xml_etree_iterparse      | 115 ms                                                 | 105 ms: 1.10x faster                                            |
| create_gc_cycles         | 1.62 ms                                                | 1.48 ms: 1.09x faster                                           |
| json                     | 5.69 ms                                                | 5.27 ms: 1.08x faster                                           |
| sqlite_synth             | 3.02 us                                                | 2.86 us: 1.06x faster                                           |
| xml_etree_parse          | 168 ms                                                 | 160 ms: 1.05x faster                                            |
| pickle_list              | 5.08 us                                                | 4.90 us: 1.04x faster                                           |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                            |
| unpickle_list            | 5.20 us                                                | 5.10 us: 1.02x faster                                           |
| asyncio_websockets       | 559 ms                                                 | 551 ms: 1.01x faster                                            |
| regex_dna                | 227 ms                                                 | 225 ms: 1.01x faster                                            |
| gc_traversal             | 3.62 ms                                                | 3.70 ms: 1.02x slower                                           |
| pickle                   | 10.7 us                                                | 11.4 us: 1.07x slower                                           |
| unpickle                 | 14.4 us                                                | 15.7 us: 1.09x slower                                           |
| pickle_dict              | 29.6 us                                                | 34.2 us: 1.16x slower                                           |
| telco                    | 7.27 ms                                                | 8.42 ms: 1.16x slower                                           |
| coverage                 | 79.4 ms                                                | 97.0 ms: 1.22x slower                                           |
| python_startup_no_site   | 5.93 ms                                                | 8.73 ms: 1.47x slower                                           |
| Geometric mean           | (ref)                                                  | 1.35x faster                                                    |

Benchmark hidden because not significant (4): mypy2, bench_mp_pool, regex_effbot, async_generators
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240104-3.13.0a2+-34fc24a/bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.31x
- 95% likely to have a speedup of 1.30x
- 99% likely to have a speedup of 1.28x


# Memory

- memory change: 1.06x