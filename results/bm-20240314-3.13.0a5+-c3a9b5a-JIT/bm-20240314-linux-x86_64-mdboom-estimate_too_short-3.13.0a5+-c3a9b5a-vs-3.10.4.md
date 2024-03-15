# Results vs. 3.10.4

- fork: mdboom
- ref: estimate_too_short
- machine: linux-x86_64
- commit hash: c3a9b5a
- commit date: 2024-03-14
- overall geometric mean: 1.30x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.23x faster
- Memory change: 1.33x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 280 ms: 1.25x faster                                                 |
| chameleon      | 9.68 ms                                                | 7.00 ms: 1.38x faster                                                |
| docutils       | 3.30 sec                                               | 2.72 sec: 1.21x faster                                               |
| html5lib       | 88.9 ms                                                | 67.6 ms: 1.31x faster                                                |
| tornado_http   | 136 ms                                                 | 98.6 ms: 1.38x faster                                                |
| Geometric mean | (ref)                                                  | 1.31x faster                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 445 ms: 1.64x faster                                                 |
| async_tree_memoization  | 870 ms                                                 | 574 ms: 1.52x faster                                                 |
| async_tree_io           | 1.77 sec                                               | 1.20 sec: 1.47x faster                                               |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 724 ms: 1.40x faster                                                 |
| Geometric mean          | (ref)                                                  | 1.50x faster                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 93.1 ms: 1.65x faster                                                |
| float          | 117 ms                                                 | 81.3 ms: 1.44x faster                                                |
| pidigits       | 191 ms                                                 | 189 ms: 1.01x faster                                                 |
| Geometric mean | (ref)                                                  | 1.34x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 142 ms: 1.32x faster                                                 |
| regex_v8       | 27.8 ms                                                | 25.7 ms: 1.08x faster                                                |
| regex_dna      | 227 ms                                                 | 224 ms: 1.01x faster                                                 |
| regex_effbot   | 3.63 ms                                                | 3.83 ms: 1.06x slower                                                |
| Geometric mean | (ref)                                                  | 1.08x faster                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 304 us: 1.60x faster                                                 |
| tomli_loads          | 3.14 sec                                               | 2.05 sec: 1.53x faster                                               |
| unpickle_pure_python | 331 us                                                 | 237 us: 1.40x faster                                                 |
| json_dumps           | 14.2 ms                                                | 10.5 ms: 1.35x faster                                                |
| xml_etree_process    | 79.1 ms                                                | 59.7 ms: 1.32x faster                                                |
| xml_etree_generate   | 99.4 ms                                                | 86.9 ms: 1.14x faster                                                |
| json_loads           | 31.2 us                                                | 28.1 us: 1.11x faster                                                |
| xml_etree_iterparse  | 115 ms                                                 | 107 ms: 1.08x faster                                                 |
| unpickle_list        | 5.20 us                                                | 4.88 us: 1.06x faster                                                |
| xml_etree_parse      | 168 ms                                                 | 159 ms: 1.06x faster                                                 |
| pickle_list          | 5.08 us                                                | 5.10 us: 1.01x slower                                                |
| unpickle             | 14.4 us                                                | 15.0 us: 1.04x slower                                                |
| pickle               | 10.7 us                                                | 11.6 us: 1.09x slower                                                |
| pickle_dict          | 29.6 us                                                | 34.6 us: 1.17x slower                                                |
| Geometric mean       | (ref)                                                  | 1.15x faster                                                         |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 12.6 ms: 1.16x faster                                                |
| python_startup_no_site | 5.93 ms                                                | 11.2 ms: 1.88x slower                                                |
| Geometric mean         | (ref)                                                  | 1.28x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|-----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako            | 16.3 ms                                                | 10.9 ms: 1.50x faster                                                |
| django_template | 48.2 ms                                                | 33.9 ms: 1.42x faster                                                |
| genshi_text     | 31.8 ms                                                | 23.7 ms: 1.34x faster                                                |
| genshi_xml      | 66.0 ms                                                | 53.5 ms: 1.23x faster                                                |
| Geometric mean  | (ref)                                                  | 1.37x faster                                                         |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 109 us: 4.99x faster                                                 |
| generators               | 80.1 ms                                                | 29.6 ms: 2.70x faster                                                |
| deltablue                | 7.91 ms                                                | 3.75 ms: 2.11x faster                                                |
| logging_silent           | 190 ns                                                 | 102 ns: 1.87x faster                                                 |
| richards_super           | 94.7 ms                                                | 52.0 ms: 1.82x faster                                                |
| chaos                    | 115 ms                                                 | 63.6 ms: 1.82x faster                                                |
| asyncio_tcp              | 922 ms                                                 | 510 ms: 1.81x faster                                                 |
| raytrace                 | 507 ms                                                 | 286 ms: 1.77x faster                                                 |
| richards                 | 79.3 ms                                                | 45.9 ms: 1.73x faster                                                |
| pylint                   | 551 ms                                                 | 321 ms: 1.72x faster                                                 |
| crypto_pyaes             | 128 ms                                                 | 75.5 ms: 1.69x faster                                                |
| comprehensions           | 28.8 us                                                | 17.2 us: 1.68x faster                                                |
| scimark_monte_carlo      | 118 ms                                                 | 70.7 ms: 1.67x faster                                                |
| sqlglot_parse            | 2.17 ms                                                | 1.31 ms: 1.66x faster                                                |
| nbody                    | 154 ms                                                 | 93.1 ms: 1.65x faster                                                |
| async_tree_none          | 728 ms                                                 | 445 ms: 1.64x faster                                                 |
| scimark_sor              | 220 ms                                                 | 138 ms: 1.60x faster                                                 |
| pickle_pure_python       | 484 us                                                 | 304 us: 1.60x faster                                                 |
| coroutines               | 35.1 ms                                                | 22.0 ms: 1.59x faster                                                |
| sqlglot_transpile        | 2.57 ms                                                | 1.64 ms: 1.57x faster                                                |
| deepcopy_memo            | 58.5 us                                                | 37.5 us: 1.56x faster                                                |
| hexiom                   | 10.4 ms                                                | 6.74 ms: 1.54x faster                                                |
| go                       | 240 ms                                                 | 156 ms: 1.54x faster                                                 |
| tomli_loads              | 3.14 sec                                               | 2.05 sec: 1.53x faster                                               |
| spectral_norm            | 170 ms                                                 | 111 ms: 1.52x faster                                                 |
| async_tree_memoization   | 870 ms                                                 | 574 ms: 1.52x faster                                                 |
| mako                     | 16.3 ms                                                | 10.9 ms: 1.50x faster                                                |
| async_tree_io            | 1.77 sec                                               | 1.20 sec: 1.47x faster                                               |
| pyflate                  | 716 ms                                                 | 492 ms: 1.46x faster                                                 |
| float                    | 117 ms                                                 | 81.3 ms: 1.44x faster                                                |
| django_template          | 48.2 ms                                                | 33.9 ms: 1.42x faster                                                |
| logging_simple           | 8.30 us                                                | 5.86 us: 1.42x faster                                                |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 724 ms: 1.40x faster                                                 |
| deepcopy                 | 479 us                                                 | 342 us: 1.40x faster                                                 |
| unpickle_pure_python     | 331 us                                                 | 237 us: 1.40x faster                                                 |
| logging_format           | 9.09 us                                                | 6.53 us: 1.39x faster                                                |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.85 sec: 1.39x faster                                               |
| deepcopy_reduce          | 4.17 us                                                | 3.01 us: 1.39x faster                                                |
| tornado_http             | 136 ms                                                 | 98.6 ms: 1.38x faster                                                |
| chameleon                | 9.68 ms                                                | 7.00 ms: 1.38x faster                                                |
| pprint_pformat           | 2.10 sec                                               | 1.53 sec: 1.37x faster                                               |
| pprint_safe_repr         | 1.02 sec                                               | 748 ms: 1.36x faster                                                 |
| scimark_lu               | 176 ms                                                 | 130 ms: 1.35x faster                                                 |
| json_dumps               | 14.2 ms                                                | 10.5 ms: 1.35x faster                                                |
| thrift                   | 1.07 ms                                                | 798 us: 1.34x faster                                                 |
| scimark_fft              | 466 ms                                                 | 347 ms: 1.34x faster                                                 |
| genshi_text              | 31.8 ms                                                | 23.7 ms: 1.34x faster                                                |
| sqlglot_normalize        | 143 ms                                                 | 107 ms: 1.33x faster                                                 |
| xml_etree_process        | 79.1 ms                                                | 59.7 ms: 1.32x faster                                                |
| fannkuch                 | 532 ms                                                 | 401 ms: 1.32x faster                                                 |
| regex_compile            | 188 ms                                                 | 142 ms: 1.32x faster                                                 |
| html5lib                 | 88.9 ms                                                | 67.6 ms: 1.31x faster                                                |
| pycparser                | 1.58 sec                                               | 1.21 sec: 1.30x faster                                               |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.99 ms: 1.30x faster                                                |
| nqueens                  | 106 ms                                                 | 81.8 ms: 1.29x faster                                                |
| 2to3                     | 348 ms                                                 | 280 ms: 1.25x faster                                                 |
| sympy_integrate          | 25.8 ms                                                | 20.8 ms: 1.24x faster                                                |
| genshi_xml               | 66.0 ms                                                | 53.5 ms: 1.23x faster                                                |
| sqlglot_optimize         | 69.2 ms                                                | 56.2 ms: 1.23x faster                                                |
| djangocms                | 38.4 us                                                | 31.3 us: 1.23x faster                                                |
| sympy_sum                | 196 ms                                                 | 160 ms: 1.22x faster                                                 |
| sympy_str                | 346 ms                                                 | 283 ms: 1.22x faster                                                 |
| dulwich_log              | 84.3 ms                                                | 69.4 ms: 1.22x faster                                                |
| docutils                 | 3.30 sec                                               | 2.72 sec: 1.21x faster                                               |
| aiohttp                  | 1.44 ms                                                | 1.20 ms: 1.20x faster                                                |
| gunicorn                 | 1.53 ms                                                | 1.29 ms: 1.19x faster                                                |
| dask                     | 441 ms                                                 | 373 ms: 1.18x faster                                                 |
| sympy_expand             | 566 ms                                                 | 484 ms: 1.17x faster                                                 |
| python_startup           | 14.6 ms                                                | 12.6 ms: 1.16x faster                                                |
| bench_thread_pool        | 986 us                                                 | 857 us: 1.15x faster                                                 |
| xml_etree_generate       | 99.4 ms                                                | 86.9 ms: 1.14x faster                                                |
| pathlib                  | 20.5 ms                                                | 18.4 ms: 1.11x faster                                                |
| json_loads               | 31.2 us                                                | 28.1 us: 1.11x faster                                                |
| json                     | 5.69 ms                                                | 5.14 ms: 1.11x faster                                                |
| meteor_contest           | 120 ms                                                 | 110 ms: 1.08x faster                                                 |
| xml_etree_iterparse      | 115 ms                                                 | 107 ms: 1.08x faster                                                 |
| regex_v8                 | 27.8 ms                                                | 25.7 ms: 1.08x faster                                                |
| unpickle_list            | 5.20 us                                                | 4.88 us: 1.06x faster                                                |
| create_gc_cycles         | 1.62 ms                                                | 1.52 ms: 1.06x faster                                                |
| xml_etree_parse          | 168 ms                                                 | 159 ms: 1.06x faster                                                 |
| sqlite_synth             | 3.02 us                                                | 2.89 us: 1.05x faster                                                |
| mdp                      | 2.85 sec                                               | 2.74 sec: 1.04x faster                                               |
| regex_dna                | 227 ms                                                 | 224 ms: 1.01x faster                                                 |
| pidigits                 | 191 ms                                                 | 189 ms: 1.01x faster                                                 |
| gc_traversal             | 3.62 ms                                                | 3.59 ms: 1.01x faster                                                |
| pickle_list              | 5.08 us                                                | 5.10 us: 1.01x slower                                                |
| asyncio_websockets       | 559 ms                                                 | 563 ms: 1.01x slower                                                 |
| unpickle                 | 14.4 us                                                | 15.0 us: 1.04x slower                                                |
| regex_effbot             | 3.63 ms                                                | 3.83 ms: 1.06x slower                                                |
| async_generators         | 444 ms                                                 | 469 ms: 1.06x slower                                                 |
| pickle                   | 10.7 us                                                | 11.6 us: 1.09x slower                                                |
| bench_mp_pool            | 24.0 ms                                                | 26.4 ms: 1.10x slower                                                |
| telco                    | 7.27 ms                                                | 8.33 ms: 1.15x slower                                                |
| pickle_dict              | 29.6 us                                                | 34.6 us: 1.17x slower                                                |
| coverage                 | 79.4 ms                                                | 96.0 ms: 1.21x slower                                                |
| unpack_sequence          | 60.0 ns                                                | 92.9 ns: 1.55x slower                                                |
| python_startup_no_site   | 5.93 ms                                                | 11.2 ms: 1.88x slower                                                |
| Geometric mean           | (ref)                                                  | 1.30x faster                                                         |

Benchmark hidden because not significant (1): mypy2
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240314-3.13.0a5+-c3a9b5a-JIT/bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.28x
- 95% likely to have a speedup of 1.25x
- 99% likely to have a speedup of 1.23x


# Memory

- memory change: 1.33x