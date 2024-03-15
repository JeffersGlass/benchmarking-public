# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_relax_absolut
- machine: linux-x86_64
- commit hash: 78b2070
- commit date: 2024-03-14
- overall geometric mean: 1.29x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.21x faster
- Memory change: 1.33x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 284 ms: 1.23x faster                                                         |
| chameleon      | 9.68 ms                                                | 6.96 ms: 1.39x faster                                                        |
| docutils       | 3.30 sec                                               | 2.78 sec: 1.19x faster                                                       |
| html5lib       | 88.9 ms                                                | 68.2 ms: 1.30x faster                                                        |
| tornado_http   | 136 ms                                                 | 99.1 ms: 1.38x faster                                                        |
| Geometric mean | (ref)                                                  | 1.29x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 448 ms: 1.63x faster                                                         |
| async_tree_memoization  | 870 ms                                                 | 576 ms: 1.51x faster                                                         |
| async_tree_io           | 1.77 sec                                               | 1.21 sec: 1.46x faster                                                       |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 728 ms: 1.40x faster                                                         |
| Geometric mean          | (ref)                                                  | 1.50x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 92.6 ms: 1.66x faster                                                        |
| float          | 117 ms                                                 | 81.3 ms: 1.44x faster                                                        |
| pidigits       | 191 ms                                                 | 190 ms: 1.00x faster                                                         |
| Geometric mean | (ref)                                                  | 1.34x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 144 ms: 1.31x faster                                                         |
| regex_v8       | 27.8 ms                                                | 24.0 ms: 1.16x faster                                                        |
| regex_dna      | 227 ms                                                 | 225 ms: 1.01x faster                                                         |
| Geometric mean | (ref)                                                  | 1.11x faster                                                                 |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 301 us: 1.61x faster                                                         |
| tomli_loads          | 3.14 sec                                               | 2.05 sec: 1.53x faster                                                       |
| json_dumps           | 14.2 ms                                                | 10.5 ms: 1.35x faster                                                        |
| unpickle_pure_python | 331 us                                                 | 245 us: 1.35x faster                                                         |
| xml_etree_process    | 79.1 ms                                                | 60.6 ms: 1.31x faster                                                        |
| xml_etree_generate   | 99.4 ms                                                | 88.1 ms: 1.13x faster                                                        |
| json_loads           | 31.2 us                                                | 28.4 us: 1.10x faster                                                        |
| unpickle_list        | 5.20 us                                                | 4.81 us: 1.08x faster                                                        |
| xml_etree_iterparse  | 115 ms                                                 | 109 ms: 1.06x faster                                                         |
| pickle_list          | 5.08 us                                                | 4.81 us: 1.06x faster                                                        |
| xml_etree_parse      | 168 ms                                                 | 161 ms: 1.05x faster                                                         |
| unpickle             | 14.4 us                                                | 15.7 us: 1.09x slower                                                        |
| pickle               | 10.7 us                                                | 11.8 us: 1.11x slower                                                        |
| pickle_dict          | 29.6 us                                                | 34.9 us: 1.18x slower                                                        |
| Geometric mean       | (ref)                                                  | 1.14x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 12.6 ms: 1.15x faster                                                        |
| python_startup_no_site | 5.93 ms                                                | 11.2 ms: 1.89x slower                                                        |
| Geometric mean         | (ref)                                                  | 1.28x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako            | 16.3 ms                                                | 10.9 ms: 1.49x faster                                                        |
| django_template | 48.2 ms                                                | 34.2 ms: 1.41x faster                                                        |
| genshi_text     | 31.8 ms                                                | 24.1 ms: 1.32x faster                                                        |
| genshi_xml      | 66.0 ms                                                | 54.3 ms: 1.22x faster                                                        |
| Geometric mean  | (ref)                                                  | 1.36x faster                                                                 |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 112 us: 4.86x faster                                                         |
| generators               | 80.1 ms                                                | 29.7 ms: 2.69x faster                                                        |
| deltablue                | 7.91 ms                                                | 3.48 ms: 2.27x faster                                                        |
| logging_silent           | 190 ns                                                 | 100 ns: 1.89x faster                                                         |
| asyncio_tcp              | 922 ms                                                 | 495 ms: 1.86x faster                                                         |
| richards_super           | 94.7 ms                                                | 53.5 ms: 1.77x faster                                                        |
| chaos                    | 115 ms                                                 | 65.3 ms: 1.77x faster                                                        |
| pylint                   | 551 ms                                                 | 324 ms: 1.70x faster                                                         |
| scimark_sor              | 220 ms                                                 | 131 ms: 1.68x faster                                                         |
| raytrace                 | 507 ms                                                 | 302 ms: 1.68x faster                                                         |
| richards                 | 79.3 ms                                                | 47.7 ms: 1.66x faster                                                        |
| nbody                    | 154 ms                                                 | 92.6 ms: 1.66x faster                                                        |
| sqlglot_parse            | 2.17 ms                                                | 1.31 ms: 1.65x faster                                                        |
| crypto_pyaes             | 128 ms                                                 | 77.3 ms: 1.65x faster                                                        |
| async_tree_none          | 728 ms                                                 | 448 ms: 1.63x faster                                                         |
| scimark_monte_carlo      | 118 ms                                                 | 73.1 ms: 1.62x faster                                                        |
| comprehensions           | 28.8 us                                                | 17.9 us: 1.61x faster                                                        |
| pickle_pure_python       | 484 us                                                 | 301 us: 1.61x faster                                                         |
| sqlglot_transpile        | 2.57 ms                                                | 1.65 ms: 1.56x faster                                                        |
| coroutines               | 35.1 ms                                                | 22.8 ms: 1.54x faster                                                        |
| tomli_loads              | 3.14 sec                                               | 2.05 sec: 1.53x faster                                                       |
| go                       | 240 ms                                                 | 158 ms: 1.52x faster                                                         |
| async_tree_memoization   | 870 ms                                                 | 576 ms: 1.51x faster                                                         |
| mako                     | 16.3 ms                                                | 10.9 ms: 1.49x faster                                                        |
| deepcopy_memo            | 58.5 us                                                | 39.4 us: 1.48x faster                                                        |
| async_tree_io            | 1.77 sec                                               | 1.21 sec: 1.46x faster                                                       |
| spectral_norm            | 170 ms                                                 | 118 ms: 1.44x faster                                                         |
| float                    | 117 ms                                                 | 81.3 ms: 1.44x faster                                                        |
| hexiom                   | 10.4 ms                                                | 7.29 ms: 1.43x faster                                                        |
| logging_simple           | 8.30 us                                                | 5.83 us: 1.43x faster                                                        |
| pyflate                  | 716 ms                                                 | 503 ms: 1.42x faster                                                         |
| logging_format           | 9.09 us                                                | 6.40 us: 1.42x faster                                                        |
| django_template          | 48.2 ms                                                | 34.2 ms: 1.41x faster                                                        |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 728 ms: 1.40x faster                                                         |
| chameleon                | 9.68 ms                                                | 6.96 ms: 1.39x faster                                                        |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.85 sec: 1.39x faster                                                       |
| tornado_http             | 136 ms                                                 | 99.1 ms: 1.38x faster                                                        |
| deepcopy_reduce          | 4.17 us                                                | 3.04 us: 1.37x faster                                                        |
| pprint_safe_repr         | 1.02 sec                                               | 751 ms: 1.35x faster                                                         |
| json_dumps               | 14.2 ms                                                | 10.5 ms: 1.35x faster                                                        |
| deepcopy                 | 479 us                                                 | 355 us: 1.35x faster                                                         |
| unpickle_pure_python     | 331 us                                                 | 245 us: 1.35x faster                                                         |
| scimark_fft              | 466 ms                                                 | 346 ms: 1.35x faster                                                         |
| thrift                   | 1.07 ms                                                | 804 us: 1.33x faster                                                         |
| pprint_pformat           | 2.10 sec                                               | 1.58 sec: 1.33x faster                                                       |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.89 ms: 1.32x faster                                                        |
| genshi_text              | 31.8 ms                                                | 24.1 ms: 1.32x faster                                                        |
| fannkuch                 | 532 ms                                                 | 403 ms: 1.32x faster                                                         |
| scimark_lu               | 176 ms                                                 | 134 ms: 1.32x faster                                                         |
| sqlglot_normalize        | 143 ms                                                 | 109 ms: 1.31x faster                                                         |
| regex_compile            | 188 ms                                                 | 144 ms: 1.31x faster                                                         |
| xml_etree_process        | 79.1 ms                                                | 60.6 ms: 1.31x faster                                                        |
| html5lib                 | 88.9 ms                                                | 68.2 ms: 1.30x faster                                                        |
| pycparser                | 1.58 sec                                               | 1.22 sec: 1.29x faster                                                       |
| 2to3                     | 348 ms                                                 | 284 ms: 1.23x faster                                                         |
| djangocms                | 38.4 us                                                | 31.4 us: 1.22x faster                                                        |
| genshi_xml               | 66.0 ms                                                | 54.3 ms: 1.22x faster                                                        |
| sqlglot_optimize         | 69.2 ms                                                | 56.8 ms: 1.22x faster                                                        |
| sympy_integrate          | 25.8 ms                                                | 21.2 ms: 1.22x faster                                                        |
| sympy_sum                | 196 ms                                                 | 162 ms: 1.21x faster                                                         |
| dulwich_log              | 84.3 ms                                                | 69.9 ms: 1.21x faster                                                        |
| sympy_str                | 346 ms                                                 | 287 ms: 1.21x faster                                                         |
| aiohttp                  | 1.44 ms                                                | 1.20 ms: 1.20x faster                                                        |
| docutils                 | 3.30 sec                                               | 2.78 sec: 1.19x faster                                                       |
| dask                     | 441 ms                                                 | 373 ms: 1.18x faster                                                         |
| gunicorn                 | 1.53 ms                                                | 1.30 ms: 1.18x faster                                                        |
| nqueens                  | 106 ms                                                 | 90.8 ms: 1.17x faster                                                        |
| sympy_expand             | 566 ms                                                 | 487 ms: 1.16x faster                                                         |
| regex_v8                 | 27.8 ms                                                | 24.0 ms: 1.16x faster                                                        |
| python_startup           | 14.6 ms                                                | 12.6 ms: 1.15x faster                                                        |
| bench_thread_pool        | 986 us                                                 | 860 us: 1.15x faster                                                         |
| xml_etree_generate       | 99.4 ms                                                | 88.1 ms: 1.13x faster                                                        |
| pathlib                  | 20.5 ms                                                | 18.5 ms: 1.11x faster                                                        |
| json_loads               | 31.2 us                                                | 28.4 us: 1.10x faster                                                        |
| json                     | 5.69 ms                                                | 5.20 ms: 1.09x faster                                                        |
| unpickle_list            | 5.20 us                                                | 4.81 us: 1.08x faster                                                        |
| meteor_contest           | 120 ms                                                 | 111 ms: 1.08x faster                                                         |
| mdp                      | 2.85 sec                                               | 2.65 sec: 1.07x faster                                                       |
| sqlite_synth             | 3.02 us                                                | 2.84 us: 1.07x faster                                                        |
| xml_etree_iterparse      | 115 ms                                                 | 109 ms: 1.06x faster                                                         |
| pickle_list              | 5.08 us                                                | 4.81 us: 1.06x faster                                                        |
| xml_etree_parse          | 168 ms                                                 | 161 ms: 1.05x faster                                                         |
| create_gc_cycles         | 1.62 ms                                                | 1.55 ms: 1.05x faster                                                        |
| regex_dna                | 227 ms                                                 | 225 ms: 1.01x faster                                                         |
| pidigits                 | 191 ms                                                 | 190 ms: 1.00x faster                                                         |
| asyncio_websockets       | 559 ms                                                 | 562 ms: 1.01x slower                                                         |
| gc_traversal             | 3.62 ms                                                | 3.81 ms: 1.05x slower                                                        |
| async_generators         | 444 ms                                                 | 471 ms: 1.06x slower                                                         |
| unpickle                 | 14.4 us                                                | 15.7 us: 1.09x slower                                                        |
| bench_mp_pool            | 24.0 ms                                                | 26.4 ms: 1.10x slower                                                        |
| pickle                   | 10.7 us                                                | 11.8 us: 1.11x slower                                                        |
| telco                    | 7.27 ms                                                | 8.48 ms: 1.17x slower                                                        |
| pickle_dict              | 29.6 us                                                | 34.9 us: 1.18x slower                                                        |
| coverage                 | 79.4 ms                                                | 97.4 ms: 1.23x slower                                                        |
| unpack_sequence          | 60.0 ns                                                | 87.8 ns: 1.46x slower                                                        |
| python_startup_no_site   | 5.93 ms                                                | 11.2 ms: 1.89x slower                                                        |
| Geometric mean           | (ref)                                                  | 1.29x faster                                                                 |

Benchmark hidden because not significant (2): regex_effbot, mypy2
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240314-3.13.0a5+-78b2070-JIT/bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.26x
- 95% likely to have a speedup of 1.23x
- 99% likely to have a speedup of 1.21x


# Memory

- memory change: 1.33x