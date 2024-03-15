# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_relax_absolut
- machine: linux-x86_64
- commit hash: 89ade43
- commit date: 2024-03-14
- overall geometric mean: 1.29x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.21x faster
- Memory change: 1.22x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 282 ms: 1.23x faster                                                         |
| chameleon      | 9.68 ms                                                | 6.89 ms: 1.41x faster                                                        |
| docutils       | 3.30 sec                                               | 2.79 sec: 1.18x faster                                                       |
| html5lib       | 88.9 ms                                                | 68.3 ms: 1.30x faster                                                        |
| tornado_http   | 136 ms                                                 | 98.8 ms: 1.38x faster                                                        |
| Geometric mean | (ref)                                                  | 1.30x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 452 ms: 1.61x faster                                                         |
| async_tree_memoization  | 870 ms                                                 | 581 ms: 1.50x faster                                                         |
| async_tree_io           | 1.77 sec                                               | 1.22 sec: 1.44x faster                                                       |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 728 ms: 1.39x faster                                                         |
| Geometric mean          | (ref)                                                  | 1.48x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 92.3 ms: 1.66x faster                                                        |
| float          | 117 ms                                                 | 82.7 ms: 1.42x faster                                                        |
| pidigits       | 191 ms                                                 | 189 ms: 1.01x faster                                                         |
| Geometric mean | (ref)                                                  | 1.33x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 144 ms: 1.31x faster                                                         |
| regex_v8       | 27.8 ms                                                | 25.9 ms: 1.07x faster                                                        |
| regex_effbot   | 3.63 ms                                                | 3.74 ms: 1.03x slower                                                        |
| Geometric mean | (ref)                                                  | 1.08x faster                                                                 |

Benchmark hidden because not significant (1): regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 301 us: 1.61x faster                                                         |
| tomli_loads          | 3.14 sec                                               | 2.07 sec: 1.52x faster                                                       |
| unpickle_pure_python | 331 us                                                 | 244 us: 1.35x faster                                                         |
| json_dumps           | 14.2 ms                                                | 10.5 ms: 1.35x faster                                                        |
| xml_etree_process    | 79.1 ms                                                | 60.2 ms: 1.31x faster                                                        |
| xml_etree_generate   | 99.4 ms                                                | 88.3 ms: 1.13x faster                                                        |
| json_loads           | 31.2 us                                                | 28.4 us: 1.10x faster                                                        |
| unpickle_list        | 5.20 us                                                | 4.83 us: 1.08x faster                                                        |
| xml_etree_iterparse  | 115 ms                                                 | 109 ms: 1.06x faster                                                         |
| xml_etree_parse      | 168 ms                                                 | 162 ms: 1.04x faster                                                         |
| unpickle             | 14.4 us                                                | 15.5 us: 1.08x slower                                                        |
| pickle               | 10.7 us                                                | 11.6 us: 1.09x slower                                                        |
| pickle_dict          | 29.6 us                                                | 34.9 us: 1.18x slower                                                        |
| Geometric mean       | (ref)                                                  | 1.14x faster                                                                 |

Benchmark hidden because not significant (1): pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 11.5 ms: 1.27x faster                                                        |
| python_startup_no_site | 5.93 ms                                                | 10.1 ms: 1.70x slower                                                        |
| Geometric mean         | (ref)                                                  | 1.16x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako            | 16.3 ms                                                | 10.8 ms: 1.51x faster                                                        |
| django_template | 48.2 ms                                                | 34.3 ms: 1.41x faster                                                        |
| genshi_text     | 31.8 ms                                                | 24.5 ms: 1.30x faster                                                        |
| genshi_xml      | 66.0 ms                                                | 54.7 ms: 1.21x faster                                                        |
| Geometric mean  | (ref)                                                  | 1.35x faster                                                                 |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 110 us: 4.94x faster                                                         |
| generators               | 80.1 ms                                                | 29.6 ms: 2.71x faster                                                        |
| deltablue                | 7.91 ms                                                | 3.49 ms: 2.27x faster                                                        |
| logging_silent           | 190 ns                                                 | 101 ns: 1.88x faster                                                         |
| asyncio_tcp              | 922 ms                                                 | 505 ms: 1.82x faster                                                         |
| richards_super           | 94.7 ms                                                | 52.5 ms: 1.81x faster                                                        |
| chaos                    | 115 ms                                                 | 66.8 ms: 1.73x faster                                                        |
| pylint                   | 551 ms                                                 | 323 ms: 1.71x faster                                                         |
| richards                 | 79.3 ms                                                | 46.7 ms: 1.70x faster                                                        |
| raytrace                 | 507 ms                                                 | 302 ms: 1.68x faster                                                         |
| scimark_sor              | 220 ms                                                 | 131 ms: 1.68x faster                                                         |
| nbody                    | 154 ms                                                 | 92.3 ms: 1.66x faster                                                        |
| crypto_pyaes             | 128 ms                                                 | 77.2 ms: 1.65x faster                                                        |
| sqlglot_parse            | 2.17 ms                                                | 1.33 ms: 1.64x faster                                                        |
| async_tree_none          | 728 ms                                                 | 452 ms: 1.61x faster                                                         |
| pickle_pure_python       | 484 us                                                 | 301 us: 1.61x faster                                                         |
| scimark_monte_carlo      | 118 ms                                                 | 73.4 ms: 1.61x faster                                                        |
| comprehensions           | 28.8 us                                                | 17.9 us: 1.61x faster                                                        |
| sqlglot_transpile        | 2.57 ms                                                | 1.67 ms: 1.54x faster                                                        |
| coroutines               | 35.1 ms                                                | 23.0 ms: 1.53x faster                                                        |
| tomli_loads              | 3.14 sec                                               | 2.07 sec: 1.52x faster                                                       |
| mako                     | 16.3 ms                                                | 10.8 ms: 1.51x faster                                                        |
| go                       | 240 ms                                                 | 160 ms: 1.50x faster                                                         |
| async_tree_memoization   | 870 ms                                                 | 581 ms: 1.50x faster                                                         |
| deepcopy_memo            | 58.5 us                                                | 39.6 us: 1.48x faster                                                        |
| async_tree_io            | 1.77 sec                                               | 1.22 sec: 1.44x faster                                                       |
| pyflate                  | 716 ms                                                 | 497 ms: 1.44x faster                                                         |
| logging_simple           | 8.30 us                                                | 5.82 us: 1.43x faster                                                        |
| float                    | 117 ms                                                 | 82.7 ms: 1.42x faster                                                        |
| logging_format           | 9.09 us                                                | 6.43 us: 1.41x faster                                                        |
| hexiom                   | 10.4 ms                                                | 7.37 ms: 1.41x faster                                                        |
| spectral_norm            | 170 ms                                                 | 120 ms: 1.41x faster                                                         |
| django_template          | 48.2 ms                                                | 34.3 ms: 1.41x faster                                                        |
| chameleon                | 9.68 ms                                                | 6.89 ms: 1.41x faster                                                        |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 728 ms: 1.39x faster                                                         |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.85 sec: 1.39x faster                                                       |
| tornado_http             | 136 ms                                                 | 98.8 ms: 1.38x faster                                                        |
| pprint_pformat           | 2.10 sec                                               | 1.55 sec: 1.36x faster                                                       |
| deepcopy                 | 479 us                                                 | 353 us: 1.36x faster                                                         |
| unpickle_pure_python     | 331 us                                                 | 244 us: 1.35x faster                                                         |
| json_dumps               | 14.2 ms                                                | 10.5 ms: 1.35x faster                                                        |
| pprint_safe_repr         | 1.02 sec                                               | 756 ms: 1.35x faster                                                         |
| thrift                   | 1.07 ms                                                | 799 us: 1.34x faster                                                         |
| fannkuch                 | 532 ms                                                 | 397 ms: 1.34x faster                                                         |
| deepcopy_reduce          | 4.17 us                                                | 3.13 us: 1.33x faster                                                        |
| scimark_fft              | 466 ms                                                 | 351 ms: 1.33x faster                                                         |
| xml_etree_process        | 79.1 ms                                                | 60.2 ms: 1.31x faster                                                        |
| scimark_lu               | 176 ms                                                 | 134 ms: 1.31x faster                                                         |
| sqlglot_normalize        | 143 ms                                                 | 109 ms: 1.31x faster                                                         |
| regex_compile            | 188 ms                                                 | 144 ms: 1.31x faster                                                         |
| html5lib                 | 88.9 ms                                                | 68.3 ms: 1.30x faster                                                        |
| genshi_text              | 31.8 ms                                                | 24.5 ms: 1.30x faster                                                        |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.07 ms: 1.28x faster                                                        |
| python_startup           | 14.6 ms                                                | 11.5 ms: 1.27x faster                                                        |
| pycparser                | 1.58 sec                                               | 1.26 sec: 1.25x faster                                                       |
| 2to3                     | 348 ms                                                 | 282 ms: 1.23x faster                                                         |
| sympy_integrate          | 25.8 ms                                                | 21.2 ms: 1.22x faster                                                        |
| sympy_sum                | 196 ms                                                 | 162 ms: 1.21x faster                                                         |
| sqlglot_optimize         | 69.2 ms                                                | 57.0 ms: 1.21x faster                                                        |
| genshi_xml               | 66.0 ms                                                | 54.7 ms: 1.21x faster                                                        |
| dulwich_log              | 84.3 ms                                                | 70.0 ms: 1.20x faster                                                        |
| sympy_str                | 346 ms                                                 | 288 ms: 1.20x faster                                                         |
| djangocms                | 38.4 us                                                | 32.0 us: 1.20x faster                                                        |
| aiohttp                  | 1.44 ms                                                | 1.20 ms: 1.19x faster                                                        |
| docutils                 | 3.30 sec                                               | 2.79 sec: 1.18x faster                                                       |
| dask                     | 441 ms                                                 | 373 ms: 1.18x faster                                                         |
| gunicorn                 | 1.53 ms                                                | 1.30 ms: 1.18x faster                                                        |
| sympy_expand             | 566 ms                                                 | 487 ms: 1.16x faster                                                         |
| nqueens                  | 106 ms                                                 | 91.6 ms: 1.16x faster                                                        |
| bench_thread_pool        | 986 us                                                 | 858 us: 1.15x faster                                                         |
| xml_etree_generate       | 99.4 ms                                                | 88.3 ms: 1.13x faster                                                        |
| json                     | 5.69 ms                                                | 5.16 ms: 1.10x faster                                                        |
| json_loads               | 31.2 us                                                | 28.4 us: 1.10x faster                                                        |
| pathlib                  | 20.5 ms                                                | 18.8 ms: 1.09x faster                                                        |
| mdp                      | 2.85 sec                                               | 2.64 sec: 1.08x faster                                                       |
| unpickle_list            | 5.20 us                                                | 4.83 us: 1.08x faster                                                        |
| regex_v8                 | 27.8 ms                                                | 25.9 ms: 1.07x faster                                                        |
| meteor_contest           | 120 ms                                                 | 112 ms: 1.07x faster                                                         |
| sqlite_synth             | 3.02 us                                                | 2.84 us: 1.06x faster                                                        |
| xml_etree_iterparse      | 115 ms                                                 | 109 ms: 1.06x faster                                                         |
| create_gc_cycles         | 1.62 ms                                                | 1.54 ms: 1.05x faster                                                        |
| xml_etree_parse          | 168 ms                                                 | 162 ms: 1.04x faster                                                         |
| pidigits                 | 191 ms                                                 | 189 ms: 1.01x faster                                                         |
| asyncio_websockets       | 559 ms                                                 | 562 ms: 1.01x slower                                                         |
| regex_effbot             | 3.63 ms                                                | 3.74 ms: 1.03x slower                                                        |
| async_generators         | 444 ms                                                 | 470 ms: 1.06x slower                                                         |
| unpickle                 | 14.4 us                                                | 15.5 us: 1.08x slower                                                        |
| gc_traversal             | 3.62 ms                                                | 3.93 ms: 1.08x slower                                                        |
| pickle                   | 10.7 us                                                | 11.6 us: 1.09x slower                                                        |
| telco                    | 7.27 ms                                                | 8.39 ms: 1.16x slower                                                        |
| pickle_dict              | 29.6 us                                                | 34.9 us: 1.18x slower                                                        |
| coverage                 | 79.4 ms                                                | 96.6 ms: 1.22x slower                                                        |
| unpack_sequence          | 60.0 ns                                                | 87.5 ns: 1.46x slower                                                        |
| python_startup_no_site   | 5.93 ms                                                | 10.1 ms: 1.70x slower                                                        |
| Geometric mean           | (ref)                                                  | 1.29x faster                                                                 |

Benchmark hidden because not significant (4): bench_mp_pool, regex_dna, pickle_list, mypy2
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240314-3.13.0a5+-89ade43-JIT/bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.24x
- 95% likely to have a speedup of 1.23x
- 99% likely to have a speedup of 1.21x


# Memory

- memory change: 1.22x