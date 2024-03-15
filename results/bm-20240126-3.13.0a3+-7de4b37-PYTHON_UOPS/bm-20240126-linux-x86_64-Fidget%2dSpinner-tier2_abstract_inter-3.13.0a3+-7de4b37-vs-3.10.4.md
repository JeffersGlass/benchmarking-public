
# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: 7de4b37
- commit date: 2024-01-26
- overall geometric mean: 1.26x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.19x faster
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 285 ms: 1.22x faster                                                             |
| chameleon      | 9.68 ms                                                | 7.39 ms: 1.31x faster                                                            |
| docutils       | 3.30 sec                                               | 2.70 sec: 1.22x faster                                                           |
| tornado_http   | 136 ms                                                 | 98.8 ms: 1.38x faster                                                            |
| Geometric mean | (ref)                                                  | 1.28x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 451 ms: 1.61x faster                                                             |
| async_tree_memoization  | 870 ms                                                 | 579 ms: 1.50x faster                                                             |
| async_tree_io           | 1.77 sec                                               | 1.21 sec: 1.47x faster                                                           |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 725 ms: 1.40x faster                                                             |
| Geometric mean          | (ref)                                                  | 1.49x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| float          | 117 ms                                                 | 92.9 ms: 1.26x faster                                                            |
| nbody          | 154 ms                                                 | 125 ms: 1.23x faster                                                             |
| pidigits       | 191 ms                                                 | 189 ms: 1.01x faster                                                             |
| Geometric mean | (ref)                                                  | 1.16x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 152 ms: 1.24x faster                                                             |
| regex_v8       | 27.8 ms                                                | 25.9 ms: 1.07x faster                                                            |
| regex_dna      | 227 ms                                                 | 228 ms: 1.01x slower                                                             |
| Geometric mean | (ref)                                                  | 1.07x faster                                                                     |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 303 us: 1.60x faster                                                             |
| unpickle_pure_python | 331 us                                                 | 236 us: 1.40x faster                                                             |
| json_dumps           | 14.2 ms                                                | 10.5 ms: 1.35x faster                                                            |
| xml_etree_process    | 79.1 ms                                                | 61.4 ms: 1.29x faster                                                            |
| tomli_loads          | 3.14 sec                                               | 2.56 sec: 1.23x faster                                                           |
| xml_etree_generate   | 99.4 ms                                                | 89.7 ms: 1.11x faster                                                            |
| json_loads           | 31.2 us                                                | 28.2 us: 1.11x faster                                                            |
| xml_etree_parse      | 168 ms                                                 | 159 ms: 1.06x faster                                                             |
| xml_etree_iterparse  | 115 ms                                                 | 112 ms: 1.03x faster                                                             |
| pickle_list          | 5.08 us                                                | 5.19 us: 1.02x slower                                                            |
| unpickle             | 14.4 us                                                | 15.2 us: 1.06x slower                                                            |
| unpickle_list        | 5.20 us                                                | 5.52 us: 1.06x slower                                                            |
| pickle               | 10.7 us                                                | 11.5 us: 1.08x slower                                                            |
| pickle_dict          | 29.6 us                                                | 35.2 us: 1.19x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.11x faster                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                            |
| python_startup_no_site | 5.93 ms                                                | 8.82 ms: 1.49x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.02x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 13.9 ms: 1.17x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 117 us: 4.64x faster                                                             |
| generators               | 80.1 ms                                                | 30.0 ms: 2.67x faster                                                            |
| asyncio_tcp              | 922 ms                                                 | 491 ms: 1.88x faster                                                             |
| logging_silent           | 190 ns                                                 | 107 ns: 1.76x faster                                                             |
| richards_super           | 94.7 ms                                                | 54.7 ms: 1.73x faster                                                            |
| deltablue                | 7.91 ms                                                | 4.65 ms: 1.70x faster                                                            |
| raytrace                 | 507 ms                                                 | 299 ms: 1.69x faster                                                             |
| scimark_sor              | 220 ms                                                 | 130 ms: 1.69x faster                                                             |
| richards                 | 79.3 ms                                                | 48.4 ms: 1.64x faster                                                            |
| sqlglot_parse            | 2.17 ms                                                | 1.33 ms: 1.63x faster                                                            |
| async_tree_none          | 728 ms                                                 | 451 ms: 1.61x faster                                                             |
| pickle_pure_python       | 484 us                                                 | 303 us: 1.60x faster                                                             |
| chaos                    | 115 ms                                                 | 72.7 ms: 1.59x faster                                                            |
| coroutines               | 35.1 ms                                                | 22.1 ms: 1.58x faster                                                            |
| sqlglot_transpile        | 2.57 ms                                                | 1.66 ms: 1.55x faster                                                            |
| go                       | 240 ms                                                 | 156 ms: 1.54x faster                                                             |
| scimark_lu               | 176 ms                                                 | 115 ms: 1.53x faster                                                             |
| crypto_pyaes             | 128 ms                                                 | 84.9 ms: 1.50x faster                                                            |
| async_tree_memoization   | 870 ms                                                 | 579 ms: 1.50x faster                                                             |
| scimark_monte_carlo      | 118 ms                                                 | 79.0 ms: 1.50x faster                                                            |
| unpack_sequence          | 60.0 ns                                                | 40.6 ns: 1.48x faster                                                            |
| async_tree_io            | 1.77 sec                                               | 1.21 sec: 1.47x faster                                                           |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                            |
| deepcopy_memo            | 58.5 us                                                | 40.9 us: 1.43x faster                                                            |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                                           |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 725 ms: 1.40x faster                                                             |
| unpickle_pure_python     | 331 us                                                 | 236 us: 1.40x faster                                                             |
| tornado_http             | 136 ms                                                 | 98.8 ms: 1.38x faster                                                            |
| logging_simple           | 8.30 us                                                | 6.08 us: 1.37x faster                                                            |
| json_dumps               | 14.2 ms                                                | 10.5 ms: 1.35x faster                                                            |
| deepcopy_reduce          | 4.17 us                                                | 3.10 us: 1.34x faster                                                            |
| comprehensions           | 28.8 us                                                | 21.5 us: 1.34x faster                                                            |
| deepcopy                 | 479 us                                                 | 359 us: 1.33x faster                                                             |
| logging_format           | 9.09 us                                                | 6.84 us: 1.33x faster                                                            |
| pyflate                  | 716 ms                                                 | 546 ms: 1.31x faster                                                             |
| chameleon                | 9.68 ms                                                | 7.39 ms: 1.31x faster                                                            |
| pycparser                | 1.58 sec                                               | 1.21 sec: 1.30x faster                                                           |
| xml_etree_process        | 79.1 ms                                                | 61.4 ms: 1.29x faster                                                            |
| float                    | 117 ms                                                 | 92.9 ms: 1.26x faster                                                            |
| sqlglot_normalize        | 143 ms                                                 | 113 ms: 1.26x faster                                                             |
| pprint_safe_repr         | 1.02 sec                                               | 814 ms: 1.25x faster                                                             |
| pprint_pformat           | 2.10 sec                                               | 1.70 sec: 1.24x faster                                                           |
| regex_compile            | 188 ms                                                 | 152 ms: 1.24x faster                                                             |
| nbody                    | 154 ms                                                 | 125 ms: 1.23x faster                                                             |
| sympy_sum                | 196 ms                                                 | 160 ms: 1.23x faster                                                             |
| tomli_loads              | 3.14 sec                                               | 2.56 sec: 1.23x faster                                                           |
| hexiom                   | 10.4 ms                                                | 8.49 ms: 1.22x faster                                                            |
| 2to3                     | 348 ms                                                 | 285 ms: 1.22x faster                                                             |
| dulwich_log              | 84.3 ms                                                | 69.1 ms: 1.22x faster                                                            |
| docutils                 | 3.30 sec                                               | 2.70 sec: 1.22x faster                                                           |
| sympy_integrate          | 25.8 ms                                                | 21.2 ms: 1.22x faster                                                            |
| dask                     | 441 ms                                                 | 368 ms: 1.20x faster                                                             |
| sqlglot_optimize         | 69.2 ms                                                | 57.9 ms: 1.19x faster                                                            |
| spectral_norm            | 170 ms                                                 | 143 ms: 1.19x faster                                                             |
| sympy_str                | 346 ms                                                 | 292 ms: 1.18x faster                                                             |
| fannkuch                 | 532 ms                                                 | 451 ms: 1.18x faster                                                             |
| mako                     | 16.3 ms                                                | 13.9 ms: 1.17x faster                                                            |
| bench_thread_pool        | 986 us                                                 | 847 us: 1.16x faster                                                             |
| sympy_expand             | 566 ms                                                 | 487 ms: 1.16x faster                                                             |
| nqueens                  | 106 ms                                                 | 94.1 ms: 1.12x faster                                                            |
| xml_etree_generate       | 99.4 ms                                                | 89.7 ms: 1.11x faster                                                            |
| json_loads               | 31.2 us                                                | 28.2 us: 1.11x faster                                                            |
| pathlib                  | 20.5 ms                                                | 18.7 ms: 1.10x faster                                                            |
| create_gc_cycles         | 1.62 ms                                                | 1.49 ms: 1.09x faster                                                            |
| json                     | 5.69 ms                                                | 5.23 ms: 1.09x faster                                                            |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.98 ms: 1.08x faster                                                            |
| mdp                      | 2.85 sec                                               | 2.63 sec: 1.08x faster                                                           |
| scimark_fft              | 466 ms                                                 | 432 ms: 1.08x faster                                                             |
| regex_v8                 | 27.8 ms                                                | 25.9 ms: 1.07x faster                                                            |
| sqlite_synth             | 3.02 us                                                | 2.85 us: 1.06x faster                                                            |
| xml_etree_parse          | 168 ms                                                 | 159 ms: 1.06x faster                                                             |
| meteor_contest           | 120 ms                                                 | 115 ms: 1.04x faster                                                             |
| xml_etree_iterparse      | 115 ms                                                 | 112 ms: 1.03x faster                                                             |
| asyncio_websockets       | 559 ms                                                 | 554 ms: 1.01x faster                                                             |
| pidigits                 | 191 ms                                                 | 189 ms: 1.01x faster                                                             |
| regex_dna                | 227 ms                                                 | 228 ms: 1.01x slower                                                             |
| pickle_list              | 5.08 us                                                | 5.19 us: 1.02x slower                                                            |
| async_generators         | 444 ms                                                 | 460 ms: 1.04x slower                                                             |
| gc_traversal             | 3.62 ms                                                | 3.82 ms: 1.05x slower                                                            |
| unpickle                 | 14.4 us                                                | 15.2 us: 1.06x slower                                                            |
| unpickle_list            | 5.20 us                                                | 5.52 us: 1.06x slower                                                            |
| pickle                   | 10.7 us                                                | 11.5 us: 1.08x slower                                                            |
| telco                    | 7.27 ms                                                | 8.56 ms: 1.18x slower                                                            |
| pickle_dict              | 29.6 us                                                | 35.2 us: 1.19x slower                                                            |
| coverage                 | 79.4 ms                                                | 95.0 ms: 1.20x slower                                                            |
| python_startup_no_site   | 5.93 ms                                                | 8.82 ms: 1.49x slower                                                            |
| Geometric mean           | (ref)                                                  | 1.26x faster                                                                     |

Benchmark hidden because not significant (3): mypy2, bench_mp_pool, regex_effbot
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240126-3.13.0a3+-7de4b37-PYTHON_UOPS/bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.22x
- 95% likely to have a speedup of 1.21x
- 99% likely to have a speedup of 1.19x


# Memory

- memory change: 1.07x