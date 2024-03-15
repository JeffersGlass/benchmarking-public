
# Results vs. 3.10.4

- fork: faster-cpython
- ref: tier_2_inline_consts
- machine: linux-x86_64
- commit hash: 9d22a48
- commit date: 2024-01-17
- overall geometric mean: 1.28x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.21x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240117-linux-x86_64-faster%2dcpython-tier_2_inline_consts-3.13.0a3+-9d22a48 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 281 ms: 1.24x faster                                                             |
| chameleon      | 9.68 ms                                                | 7.35 ms: 1.32x faster                                                            |
| docutils       | 3.30 sec                                               | 2.70 sec: 1.22x faster                                                           |
| tornado_http   | 136 ms                                                 | 99.7 ms: 1.37x faster                                                            |
| Geometric mean | (ref)                                                  | 1.28x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240117-linux-x86_64-faster%2dcpython-tier_2_inline_consts-3.13.0a3+-9d22a48 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 447 ms: 1.63x faster                                                             |
| async_tree_memoization  | 870 ms                                                 | 572 ms: 1.52x faster                                                             |
| async_tree_io           | 1.77 sec                                               | 1.20 sec: 1.48x faster                                                           |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 716 ms: 1.42x faster                                                             |
| Geometric mean          | (ref)                                                  | 1.51x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240117-linux-x86_64-faster%2dcpython-tier_2_inline_consts-3.13.0a3+-9d22a48 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 114 ms: 1.35x faster                                                             |
| float          | 117 ms                                                 | 89.9 ms: 1.30x faster                                                            |
| pidigits       | 191 ms                                                 | 189 ms: 1.01x faster                                                             |
| Geometric mean | (ref)                                                  | 1.21x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240117-linux-x86_64-faster%2dcpython-tier_2_inline_consts-3.13.0a3+-9d22a48 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 149 ms: 1.27x faster                                                             |
| regex_v8       | 27.8 ms                                                | 27.0 ms: 1.03x faster                                                            |
| regex_dna      | 227 ms                                                 | 226 ms: 1.00x faster                                                             |
| Geometric mean | (ref)                                                  | 1.07x faster                                                                     |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240117-linux-x86_64-faster%2dcpython-tier_2_inline_consts-3.13.0a3+-9d22a48 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 301 us: 1.61x faster                                                             |
| unpickle_pure_python | 331 us                                                 | 234 us: 1.41x faster                                                             |
| tomli_loads          | 3.14 sec                                               | 2.34 sec: 1.34x faster                                                           |
| json_dumps           | 14.2 ms                                                | 10.6 ms: 1.34x faster                                                            |
| xml_etree_process    | 79.1 ms                                                | 60.5 ms: 1.31x faster                                                            |
| xml_etree_generate   | 99.4 ms                                                | 89.0 ms: 1.12x faster                                                            |
| json_loads           | 31.2 us                                                | 28.1 us: 1.11x faster                                                            |
| xml_etree_parse      | 168 ms                                                 | 159 ms: 1.06x faster                                                             |
| xml_etree_iterparse  | 115 ms                                                 | 110 ms: 1.05x faster                                                             |
| pickle_list          | 5.08 us                                                | 5.14 us: 1.01x slower                                                            |
| unpickle             | 14.4 us                                                | 15.0 us: 1.04x slower                                                            |
| pickle               | 10.7 us                                                | 11.5 us: 1.08x slower                                                            |
| pickle_dict          | 29.6 us                                                | 34.1 us: 1.15x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.13x faster                                                                     |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240117-linux-x86_64-faster%2dcpython-tier_2_inline_consts-3.13.0a3+-9d22a48 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                            |
| python_startup_no_site | 5.93 ms                                                | 8.75 ms: 1.48x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240117-linux-x86_64-faster%2dcpython-tier_2_inline_consts-3.13.0a3+-9d22a48 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 13.3 ms: 1.22x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240117-linux-x86_64-faster%2dcpython-tier_2_inline_consts-3.13.0a3+-9d22a48 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 116 us: 4.71x faster                                                             |
| generators               | 80.1 ms                                                | 29.1 ms: 2.75x faster                                                            |
| asyncio_tcp              | 922 ms                                                 | 497 ms: 1.85x faster                                                             |
| logging_silent           | 190 ns                                                 | 106 ns: 1.80x faster                                                             |
| deltablue                | 7.91 ms                                                | 4.49 ms: 1.76x faster                                                            |
| richards_super           | 94.7 ms                                                | 54.2 ms: 1.75x faster                                                            |
| raytrace                 | 507 ms                                                 | 296 ms: 1.72x faster                                                             |
| scimark_sor              | 220 ms                                                 | 132 ms: 1.67x faster                                                             |
| richards                 | 79.3 ms                                                | 47.9 ms: 1.66x faster                                                            |
| sqlglot_parse            | 2.17 ms                                                | 1.32 ms: 1.65x faster                                                            |
| async_tree_none          | 728 ms                                                 | 447 ms: 1.63x faster                                                             |
| pickle_pure_python       | 484 us                                                 | 301 us: 1.61x faster                                                             |
| chaos                    | 115 ms                                                 | 71.9 ms: 1.61x faster                                                            |
| coroutines               | 35.1 ms                                                | 22.2 ms: 1.58x faster                                                            |
| crypto_pyaes             | 128 ms                                                 | 81.5 ms: 1.57x faster                                                            |
| sqlglot_transpile        | 2.57 ms                                                | 1.65 ms: 1.56x faster                                                            |
| go                       | 240 ms                                                 | 154 ms: 1.55x faster                                                             |
| async_tree_memoization   | 870 ms                                                 | 572 ms: 1.52x faster                                                             |
| unpack_sequence          | 60.0 ns                                                | 39.7 ns: 1.51x faster                                                            |
| scimark_lu               | 176 ms                                                 | 117 ms: 1.51x faster                                                             |
| scimark_monte_carlo      | 118 ms                                                 | 78.9 ms: 1.50x faster                                                            |
| async_tree_io            | 1.77 sec                                               | 1.20 sec: 1.48x faster                                                           |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                            |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                                           |
| deepcopy_memo            | 58.5 us                                                | 41.2 us: 1.42x faster                                                            |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 716 ms: 1.42x faster                                                             |
| comprehensions           | 28.8 us                                                | 20.4 us: 1.41x faster                                                            |
| unpickle_pure_python     | 331 us                                                 | 234 us: 1.41x faster                                                             |
| pyflate                  | 716 ms                                                 | 509 ms: 1.41x faster                                                             |
| tornado_http             | 136 ms                                                 | 99.7 ms: 1.37x faster                                                            |
| logging_simple           | 8.30 us                                                | 6.09 us: 1.36x faster                                                            |
| nbody                    | 154 ms                                                 | 114 ms: 1.35x faster                                                             |
| tomli_loads              | 3.14 sec                                               | 2.34 sec: 1.34x faster                                                           |
| json_dumps               | 14.2 ms                                                | 10.6 ms: 1.34x faster                                                            |
| pycparser                | 1.58 sec                                               | 1.19 sec: 1.33x faster                                                           |
| logging_format           | 9.09 us                                                | 6.86 us: 1.32x faster                                                            |
| deepcopy                 | 479 us                                                 | 364 us: 1.32x faster                                                             |
| chameleon                | 9.68 ms                                                | 7.35 ms: 1.32x faster                                                            |
| xml_etree_process        | 79.1 ms                                                | 60.5 ms: 1.31x faster                                                            |
| deepcopy_reduce          | 4.17 us                                                | 3.20 us: 1.30x faster                                                            |
| float                    | 117 ms                                                 | 89.9 ms: 1.30x faster                                                            |
| hexiom                   | 10.4 ms                                                | 8.04 ms: 1.29x faster                                                            |
| regex_compile            | 188 ms                                                 | 149 ms: 1.27x faster                                                             |
| sqlglot_normalize        | 143 ms                                                 | 114 ms: 1.26x faster                                                             |
| 2to3                     | 348 ms                                                 | 281 ms: 1.24x faster                                                             |
| pprint_safe_repr         | 1.02 sec                                               | 824 ms: 1.23x faster                                                             |
| pprint_pformat           | 2.10 sec                                               | 1.71 sec: 1.23x faster                                                           |
| mako                     | 16.3 ms                                                | 13.3 ms: 1.22x faster                                                            |
| spectral_norm            | 170 ms                                                 | 139 ms: 1.22x faster                                                             |
| docutils                 | 3.30 sec                                               | 2.70 sec: 1.22x faster                                                           |
| sympy_integrate          | 25.8 ms                                                | 21.2 ms: 1.22x faster                                                            |
| dulwich_log              | 84.3 ms                                                | 69.5 ms: 1.21x faster                                                            |
| fannkuch                 | 532 ms                                                 | 439 ms: 1.21x faster                                                             |
| sympy_sum                | 196 ms                                                 | 163 ms: 1.21x faster                                                             |
| sqlglot_optimize         | 69.2 ms                                                | 57.6 ms: 1.20x faster                                                            |
| dask                     | 441 ms                                                 | 370 ms: 1.19x faster                                                             |
| sympy_str                | 346 ms                                                 | 291 ms: 1.19x faster                                                             |
| nqueens                  | 106 ms                                                 | 91.0 ms: 1.16x faster                                                            |
| sympy_expand             | 566 ms                                                 | 487 ms: 1.16x faster                                                             |
| bench_thread_pool        | 986 us                                                 | 850 us: 1.16x faster                                                             |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.75 ms: 1.13x faster                                                            |
| xml_etree_generate       | 99.4 ms                                                | 89.0 ms: 1.12x faster                                                            |
| json_loads               | 31.2 us                                                | 28.1 us: 1.11x faster                                                            |
| json                     | 5.69 ms                                                | 5.16 ms: 1.10x faster                                                            |
| pathlib                  | 20.5 ms                                                | 18.7 ms: 1.09x faster                                                            |
| create_gc_cycles         | 1.62 ms                                                | 1.50 ms: 1.08x faster                                                            |
| mdp                      | 2.85 sec                                               | 2.68 sec: 1.06x faster                                                           |
| xml_etree_parse          | 168 ms                                                 | 159 ms: 1.06x faster                                                             |
| sqlite_synth             | 3.02 us                                                | 2.86 us: 1.06x faster                                                            |
| meteor_contest           | 120 ms                                                 | 113 ms: 1.06x faster                                                             |
| scimark_fft              | 466 ms                                                 | 442 ms: 1.05x faster                                                             |
| xml_etree_iterparse      | 115 ms                                                 | 110 ms: 1.05x faster                                                             |
| regex_v8                 | 27.8 ms                                                | 27.0 ms: 1.03x faster                                                            |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                             |
| pidigits                 | 191 ms                                                 | 189 ms: 1.01x faster                                                             |
| regex_dna                | 227 ms                                                 | 226 ms: 1.00x faster                                                             |
| pickle_list              | 5.08 us                                                | 5.14 us: 1.01x slower                                                            |
| gc_traversal             | 3.62 ms                                                | 3.70 ms: 1.02x slower                                                            |
| async_generators         | 444 ms                                                 | 454 ms: 1.02x slower                                                             |
| unpickle                 | 14.4 us                                                | 15.0 us: 1.04x slower                                                            |
| pickle                   | 10.7 us                                                | 11.5 us: 1.08x slower                                                            |
| pickle_dict              | 29.6 us                                                | 34.1 us: 1.15x slower                                                            |
| coverage                 | 79.4 ms                                                | 94.8 ms: 1.19x slower                                                            |
| telco                    | 7.27 ms                                                | 8.68 ms: 1.19x slower                                                            |
| python_startup_no_site   | 5.93 ms                                                | 8.75 ms: 1.48x slower                                                            |
| Geometric mean           | (ref)                                                  | 1.28x faster                                                                     |

Benchmark hidden because not significant (4): mypy2, unpickle_list, bench_mp_pool, regex_effbot
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240117-3.13.0a3+-9d22a48-PYTHON_UOPS/bm-20240117-linux-x86_64-faster%2dcpython-tier_2_inline_consts-3.13.0a3+-9d22a48.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.22x
- 95% likely to have a speedup of 1.21x
- 99% likely to have a speedup of 1.21x


# Memory

- memory change: 1.06x