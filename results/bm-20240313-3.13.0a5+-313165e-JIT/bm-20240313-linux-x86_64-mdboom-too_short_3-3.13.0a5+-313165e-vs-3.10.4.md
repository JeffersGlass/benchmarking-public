# Results vs. 3.10.4

- fork: mdboom
- ref: too_short_3
- machine: linux-x86_64
- commit hash: 313165e
- commit date: 2024-03-13
- overall geometric mean: 1.30x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.21x faster
- Memory change: 1.33x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 282 ms: 1.24x faster                                          |
| chameleon      | 9.68 ms                                                | 6.86 ms: 1.41x faster                                         |
| docutils       | 3.30 sec                                               | 2.79 sec: 1.18x faster                                        |
| html5lib       | 88.9 ms                                                | 67.1 ms: 1.32x faster                                         |
| tornado_http   | 136 ms                                                 | 101 ms: 1.34x faster                                          |
| Geometric mean | (ref)                                                  | 1.30x faster                                                  |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|-------------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 451 ms: 1.61x faster                                          |
| async_tree_memoization  | 870 ms                                                 | 573 ms: 1.52x faster                                          |
| async_tree_io           | 1.77 sec                                               | 1.20 sec: 1.48x faster                                        |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 733 ms: 1.39x faster                                          |
| Geometric mean          | (ref)                                                  | 1.50x faster                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 94.0 ms: 1.63x faster                                         |
| float          | 117 ms                                                 | 79.9 ms: 1.47x faster                                         |
| pidigits       | 191 ms                                                 | 190 ms: 1.00x faster                                          |
| Geometric mean | (ref)                                                  | 1.34x faster                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 142 ms: 1.32x faster                                          |
| regex_v8       | 27.8 ms                                                | 24.1 ms: 1.15x faster                                         |
| regex_dna      | 227 ms                                                 | 220 ms: 1.03x faster                                          |
| Geometric mean | (ref)                                                  | 1.12x faster                                                  |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 302 us: 1.60x faster                                          |
| tomli_loads          | 3.14 sec                                               | 2.12 sec: 1.48x faster                                        |
| unpickle_pure_python | 331 us                                                 | 243 us: 1.36x faster                                          |
| json_dumps           | 14.2 ms                                                | 10.5 ms: 1.35x faster                                         |
| xml_etree_process    | 79.1 ms                                                | 59.8 ms: 1.32x faster                                         |
| xml_etree_generate   | 99.4 ms                                                | 87.8 ms: 1.13x faster                                         |
| json_loads           | 31.2 us                                                | 28.0 us: 1.12x faster                                         |
| xml_etree_iterparse  | 115 ms                                                 | 108 ms: 1.06x faster                                          |
| unpickle_list        | 5.20 us                                                | 4.91 us: 1.06x faster                                         |
| xml_etree_parse      | 168 ms                                                 | 161 ms: 1.05x faster                                          |
| pickle_list          | 5.08 us                                                | 4.99 us: 1.02x faster                                         |
| unpickle             | 14.4 us                                                | 14.7 us: 1.02x slower                                         |
| pickle               | 10.7 us                                                | 11.6 us: 1.08x slower                                         |
| pickle_dict          | 29.6 us                                                | 33.9 us: 1.15x slower                                         |
| Geometric mean       | (ref)                                                  | 1.15x faster                                                  |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 12.6 ms: 1.16x faster                                         |
| python_startup_no_site | 5.93 ms                                                | 11.1 ms: 1.88x slower                                         |
| Geometric mean         | (ref)                                                  | 1.27x slower                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|-----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| mako            | 16.3 ms                                                | 10.7 ms: 1.52x faster                                         |
| django_template | 48.2 ms                                                | 34.5 ms: 1.40x faster                                         |
| genshi_text     | 31.8 ms                                                | 24.2 ms: 1.31x faster                                         |
| genshi_xml      | 66.0 ms                                                | 54.6 ms: 1.21x faster                                         |
| Geometric mean  | (ref)                                                  | 1.36x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|--------------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 112 us: 4.85x faster                                          |
| generators               | 80.1 ms                                                | 29.6 ms: 2.70x faster                                         |
| deltablue                | 7.91 ms                                                | 3.47 ms: 2.28x faster                                         |
| logging_silent           | 190 ns                                                 | 103 ns: 1.84x faster                                          |
| asyncio_tcp              | 922 ms                                                 | 503 ms: 1.83x faster                                          |
| richards_super           | 94.7 ms                                                | 53.3 ms: 1.78x faster                                         |
| chaos                    | 115 ms                                                 | 65.1 ms: 1.77x faster                                         |
| raytrace                 | 507 ms                                                 | 290 ms: 1.75x faster                                          |
| scimark_sor              | 220 ms                                                 | 129 ms: 1.70x faster                                          |
| pylint                   | 551 ms                                                 | 325 ms: 1.70x faster                                          |
| crypto_pyaes             | 128 ms                                                 | 75.7 ms: 1.69x faster                                         |
| comprehensions           | 28.8 us                                                | 17.4 us: 1.66x faster                                         |
| richards                 | 79.3 ms                                                | 48.0 ms: 1.65x faster                                         |
| sqlglot_parse            | 2.17 ms                                                | 1.32 ms: 1.65x faster                                         |
| scimark_monte_carlo      | 118 ms                                                 | 71.8 ms: 1.65x faster                                         |
| nbody                    | 154 ms                                                 | 94.0 ms: 1.63x faster                                         |
| async_tree_none          | 728 ms                                                 | 451 ms: 1.61x faster                                          |
| pickle_pure_python       | 484 us                                                 | 302 us: 1.60x faster                                          |
| sqlglot_transpile        | 2.57 ms                                                | 1.66 ms: 1.55x faster                                         |
| coroutines               | 35.1 ms                                                | 22.7 ms: 1.55x faster                                         |
| go                       | 240 ms                                                 | 157 ms: 1.52x faster                                          |
| mako                     | 16.3 ms                                                | 10.7 ms: 1.52x faster                                         |
| async_tree_memoization   | 870 ms                                                 | 573 ms: 1.52x faster                                          |
| deepcopy_memo            | 58.5 us                                                | 39.1 us: 1.49x faster                                         |
| spectral_norm            | 170 ms                                                 | 114 ms: 1.49x faster                                          |
| tomli_loads              | 3.14 sec                                               | 2.12 sec: 1.48x faster                                        |
| async_tree_io            | 1.77 sec                                               | 1.20 sec: 1.48x faster                                        |
| pyflate                  | 716 ms                                                 | 486 ms: 1.48x faster                                          |
| hexiom                   | 10.4 ms                                                | 7.06 ms: 1.47x faster                                         |
| float                    | 117 ms                                                 | 79.9 ms: 1.47x faster                                         |
| logging_format           | 9.09 us                                                | 6.40 us: 1.42x faster                                         |
| logging_simple           | 8.30 us                                                | 5.86 us: 1.42x faster                                         |
| chameleon                | 9.68 ms                                                | 6.86 ms: 1.41x faster                                         |
| django_template          | 48.2 ms                                                | 34.5 ms: 1.40x faster                                         |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.85 sec: 1.39x faster                                        |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 733 ms: 1.39x faster                                          |
| scimark_fft              | 466 ms                                                 | 342 ms: 1.36x faster                                          |
| unpickle_pure_python     | 331 us                                                 | 243 us: 1.36x faster                                          |
| deepcopy                 | 479 us                                                 | 352 us: 1.36x faster                                          |
| thrift                   | 1.07 ms                                                | 794 us: 1.35x faster                                          |
| pprint_pformat           | 2.10 sec                                               | 1.56 sec: 1.35x faster                                        |
| json_dumps               | 14.2 ms                                                | 10.5 ms: 1.35x faster                                         |
| tornado_http             | 136 ms                                                 | 101 ms: 1.34x faster                                          |
| fannkuch                 | 532 ms                                                 | 396 ms: 1.34x faster                                          |
| scimark_lu               | 176 ms                                                 | 131 ms: 1.34x faster                                          |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.83 ms: 1.34x faster                                         |
| deepcopy_reduce          | 4.17 us                                                | 3.12 us: 1.34x faster                                         |
| regex_compile            | 188 ms                                                 | 142 ms: 1.32x faster                                          |
| html5lib                 | 88.9 ms                                                | 67.1 ms: 1.32x faster                                         |
| xml_etree_process        | 79.1 ms                                                | 59.8 ms: 1.32x faster                                         |
| pprint_safe_repr         | 1.02 sec                                               | 774 ms: 1.31x faster                                          |
| genshi_text              | 31.8 ms                                                | 24.2 ms: 1.31x faster                                         |
| sqlglot_normalize        | 143 ms                                                 | 110 ms: 1.30x faster                                          |
| pycparser                | 1.58 sec                                               | 1.22 sec: 1.29x faster                                        |
| 2to3                     | 348 ms                                                 | 282 ms: 1.24x faster                                          |
| sqlglot_optimize         | 69.2 ms                                                | 56.9 ms: 1.22x faster                                         |
| djangocms                | 38.4 us                                                | 31.6 us: 1.21x faster                                         |
| genshi_xml               | 66.0 ms                                                | 54.6 ms: 1.21x faster                                         |
| sympy_sum                | 196 ms                                                 | 163 ms: 1.21x faster                                          |
| dulwich_log              | 84.3 ms                                                | 70.2 ms: 1.20x faster                                         |
| sympy_str                | 346 ms                                                 | 288 ms: 1.20x faster                                          |
| sympy_integrate          | 25.8 ms                                                | 21.6 ms: 1.19x faster                                         |
| aiohttp                  | 1.44 ms                                                | 1.21 ms: 1.19x faster                                         |
| docutils                 | 3.30 sec                                               | 2.79 sec: 1.18x faster                                        |
| dask                     | 441 ms                                                 | 373 ms: 1.18x faster                                          |
| nqueens                  | 106 ms                                                 | 89.7 ms: 1.18x faster                                         |
| gunicorn                 | 1.53 ms                                                | 1.30 ms: 1.18x faster                                         |
| sympy_expand             | 566 ms                                                 | 487 ms: 1.16x faster                                          |
| python_startup           | 14.6 ms                                                | 12.6 ms: 1.16x faster                                         |
| regex_v8                 | 27.8 ms                                                | 24.1 ms: 1.15x faster                                         |
| bench_thread_pool        | 986 us                                                 | 866 us: 1.14x faster                                          |
| xml_etree_generate       | 99.4 ms                                                | 87.8 ms: 1.13x faster                                         |
| json_loads               | 31.2 us                                                | 28.0 us: 1.12x faster                                         |
| json                     | 5.69 ms                                                | 5.21 ms: 1.09x faster                                         |
| mdp                      | 2.85 sec                                               | 2.62 sec: 1.09x faster                                        |
| pathlib                  | 20.5 ms                                                | 18.8 ms: 1.09x faster                                         |
| meteor_contest           | 120 ms                                                 | 111 ms: 1.08x faster                                          |
| create_gc_cycles         | 1.62 ms                                                | 1.51 ms: 1.07x faster                                         |
| sqlite_synth             | 3.02 us                                                | 2.84 us: 1.07x faster                                         |
| xml_etree_iterparse      | 115 ms                                                 | 108 ms: 1.06x faster                                          |
| unpickle_list            | 5.20 us                                                | 4.91 us: 1.06x faster                                         |
| xml_etree_parse          | 168 ms                                                 | 161 ms: 1.05x faster                                          |
| regex_dna                | 227 ms                                                 | 220 ms: 1.03x faster                                          |
| pickle_list              | 5.08 us                                                | 4.99 us: 1.02x faster                                         |
| pidigits                 | 191 ms                                                 | 190 ms: 1.00x faster                                          |
| asyncio_websockets       | 559 ms                                                 | 562 ms: 1.01x slower                                          |
| gc_traversal             | 3.62 ms                                                | 3.69 ms: 1.02x slower                                         |
| unpickle                 | 14.4 us                                                | 14.7 us: 1.02x slower                                         |
| async_generators         | 444 ms                                                 | 472 ms: 1.06x slower                                          |
| pickle                   | 10.7 us                                                | 11.6 us: 1.08x slower                                         |
| bench_mp_pool            | 24.0 ms                                                | 26.3 ms: 1.09x slower                                         |
| pickle_dict              | 29.6 us                                                | 33.9 us: 1.15x slower                                         |
| telco                    | 7.27 ms                                                | 8.41 ms: 1.16x slower                                         |
| coverage                 | 79.4 ms                                                | 97.4 ms: 1.23x slower                                         |
| unpack_sequence          | 60.0 ns                                                | 87.5 ns: 1.46x slower                                         |
| python_startup_no_site   | 5.93 ms                                                | 11.1 ms: 1.88x slower                                         |
| Geometric mean           | (ref)                                                  | 1.30x faster                                                  |

Benchmark hidden because not significant (2): regex_effbot, mypy2
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240313-3.13.0a5+-313165e-JIT/bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.26x
- 95% likely to have a speedup of 1.23x
- 99% likely to have a speedup of 1.21x


# Memory

- memory change: 1.33x