
# Results vs. 3.10.4

- fork: python
- ref: f19b93fce04fb0bc9b59
- machine: linux-x86_64
- commit hash: f19b93f
- commit date: 2024-01-06
- overall geometric mean: 1.36x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.29x faster
- Memory change: 1.05x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 263 ms: 1.33x faster                                                   |
| chameleon      | 9.68 ms                                                | 6.94 ms: 1.39x faster                                                  |
| docutils       | 3.30 sec                                               | 2.58 sec: 1.28x faster                                                 |
| tornado_http   | 136 ms                                                 | 94.2 ms: 1.45x faster                                                  |
| Geometric mean | (ref)                                                  | 1.36x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 431 ms: 1.69x faster                                                   |
| async_tree_memoization  | 870 ms                                                 | 557 ms: 1.56x faster                                                   |
| async_tree_io           | 1.77 sec                                               | 1.18 sec: 1.50x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 703 ms: 1.45x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.55x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 86.9 ms: 1.77x faster                                                  |
| float          | 117 ms                                                 | 80.0 ms: 1.46x faster                                                  |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                                   |
| Geometric mean | (ref)                                                  | 1.38x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 130 ms: 1.45x faster                                                   |
| regex_v8       | 27.8 ms                                                | 24.9 ms: 1.12x faster                                                  |
| regex_dna      | 227 ms                                                 | 218 ms: 1.04x faster                                                   |
| Geometric mean | (ref)                                                  | 1.14x faster                                                           |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 299 us: 1.62x faster                                                   |
| unpickle_pure_python | 331 us                                                 | 214 us: 1.54x faster                                                   |
| tomli_loads          | 3.14 sec                                               | 2.12 sec: 1.48x faster                                                 |
| json_dumps           | 14.2 ms                                                | 10.5 ms: 1.35x faster                                                  |
| xml_etree_process    | 79.1 ms                                                | 59.2 ms: 1.34x faster                                                  |
| xml_etree_generate   | 99.4 ms                                                | 85.6 ms: 1.16x faster                                                  |
| json_loads           | 31.2 us                                                | 28.4 us: 1.10x faster                                                  |
| xml_etree_iterparse  | 115 ms                                                 | 105 ms: 1.10x faster                                                   |
| xml_etree_parse      | 168 ms                                                 | 157 ms: 1.07x faster                                                   |
| unpickle_list        | 5.20 us                                                | 5.45 us: 1.05x slower                                                  |
| pickle               | 10.7 us                                                | 11.5 us: 1.08x slower                                                  |
| unpickle             | 14.4 us                                                | 15.5 us: 1.08x slower                                                  |
| pickle_dict          | 29.6 us                                                | 34.9 us: 1.18x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.15x faster                                                           |

Benchmark hidden because not significant (1): pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.45x faster                                                  |
| python_startup_no_site | 5.93 ms                                                | 8.68 ms: 1.46x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.00x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.0 ms: 1.49x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 111 us: 4.90x faster                                                   |
| generators               | 80.1 ms                                                | 29.4 ms: 2.72x faster                                                  |
| deltablue                | 7.91 ms                                                | 3.20 ms: 2.47x faster                                                  |
| chaos                    | 115 ms                                                 | 59.0 ms: 1.96x faster                                                  |
| raytrace                 | 507 ms                                                 | 261 ms: 1.94x faster                                                   |
| asyncio_tcp              | 922 ms                                                 | 475 ms: 1.94x faster                                                   |
| logging_silent           | 190 ns                                                 | 104 ns: 1.83x faster                                                   |
| crypto_pyaes             | 128 ms                                                 | 70.7 ms: 1.81x faster                                                  |
| comprehensions           | 28.8 us                                                | 16.3 us: 1.77x faster                                                  |
| richards_super           | 94.7 ms                                                | 53.6 ms: 1.77x faster                                                  |
| nbody                    | 154 ms                                                 | 86.9 ms: 1.77x faster                                                  |
| sqlglot_parse            | 2.17 ms                                                | 1.24 ms: 1.75x faster                                                  |
| scimark_monte_carlo      | 118 ms                                                 | 67.9 ms: 1.74x faster                                                  |
| go                       | 240 ms                                                 | 139 ms: 1.72x faster                                                   |
| scimark_sor              | 220 ms                                                 | 128 ms: 1.72x faster                                                   |
| hexiom                   | 10.4 ms                                                | 6.07 ms: 1.71x faster                                                  |
| richards                 | 79.3 ms                                                | 46.9 ms: 1.69x faster                                                  |
| async_tree_none          | 728 ms                                                 | 431 ms: 1.69x faster                                                   |
| sqlglot_transpile        | 2.57 ms                                                | 1.56 ms: 1.65x faster                                                  |
| pickle_pure_python       | 484 us                                                 | 299 us: 1.62x faster                                                   |
| coroutines               | 35.1 ms                                                | 22.0 ms: 1.60x faster                                                  |
| async_tree_memoization   | 870 ms                                                 | 557 ms: 1.56x faster                                                   |
| spectral_norm            | 170 ms                                                 | 109 ms: 1.56x faster                                                   |
| scimark_lu               | 176 ms                                                 | 114 ms: 1.55x faster                                                   |
| deepcopy_memo            | 58.5 us                                                | 37.9 us: 1.54x faster                                                  |
| unpickle_pure_python     | 331 us                                                 | 214 us: 1.54x faster                                                   |
| pyflate                  | 716 ms                                                 | 468 ms: 1.53x faster                                                   |
| async_tree_io            | 1.77 sec                                               | 1.18 sec: 1.50x faster                                                 |
| mako                     | 16.3 ms                                                | 11.0 ms: 1.49x faster                                                  |
| tomli_loads              | 3.14 sec                                               | 2.12 sec: 1.48x faster                                                 |
| logging_simple           | 8.30 us                                                | 5.63 us: 1.48x faster                                                  |
| logging_format           | 9.09 us                                                | 6.19 us: 1.47x faster                                                  |
| float                    | 117 ms                                                 | 80.0 ms: 1.46x faster                                                  |
| regex_compile            | 188 ms                                                 | 130 ms: 1.45x faster                                                   |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.45x faster                                                  |
| tornado_http             | 136 ms                                                 | 94.2 ms: 1.45x faster                                                  |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 703 ms: 1.45x faster                                                   |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.78 sec: 1.44x faster                                                 |
| pprint_pformat           | 2.10 sec                                               | 1.49 sec: 1.41x faster                                                 |
| pprint_safe_repr         | 1.02 sec                                               | 728 ms: 1.40x faster                                                   |
| chameleon                | 9.68 ms                                                | 6.94 ms: 1.39x faster                                                  |
| deepcopy                 | 479 us                                                 | 348 us: 1.38x faster                                                   |
| deepcopy_reduce          | 4.17 us                                                | 3.07 us: 1.36x faster                                                  |
| json_dumps               | 14.2 ms                                                | 10.5 ms: 1.35x faster                                                  |
| sympy_sum                | 196 ms                                                 | 147 ms: 1.34x faster                                                   |
| sqlglot_normalize        | 143 ms                                                 | 107 ms: 1.34x faster                                                   |
| sympy_integrate          | 25.8 ms                                                | 19.3 ms: 1.34x faster                                                  |
| xml_etree_process        | 79.1 ms                                                | 59.2 ms: 1.34x faster                                                  |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.85 ms: 1.33x faster                                                  |
| fannkuch                 | 532 ms                                                 | 400 ms: 1.33x faster                                                   |
| 2to3                     | 348 ms                                                 | 263 ms: 1.33x faster                                                   |
| pycparser                | 1.58 sec                                               | 1.20 sec: 1.31x faster                                                 |
| sympy_str                | 346 ms                                                 | 267 ms: 1.30x faster                                                   |
| unpack_sequence          | 60.0 ns                                                | 46.5 ns: 1.29x faster                                                  |
| scimark_fft              | 466 ms                                                 | 361 ms: 1.29x faster                                                   |
| sqlglot_optimize         | 69.2 ms                                                | 53.7 ms: 1.29x faster                                                  |
| dulwich_log              | 84.3 ms                                                | 65.8 ms: 1.28x faster                                                  |
| docutils                 | 3.30 sec                                               | 2.58 sec: 1.28x faster                                                 |
| nqueens                  | 106 ms                                                 | 83.1 ms: 1.27x faster                                                  |
| sympy_expand             | 566 ms                                                 | 454 ms: 1.25x faster                                                   |
| dask                     | 441 ms                                                 | 360 ms: 1.22x faster                                                   |
| bench_thread_pool        | 986 us                                                 | 826 us: 1.19x faster                                                   |
| xml_etree_generate       | 99.4 ms                                                | 85.6 ms: 1.16x faster                                                  |
| pathlib                  | 20.5 ms                                                | 18.1 ms: 1.13x faster                                                  |
| mdp                      | 2.85 sec                                               | 2.55 sec: 1.12x faster                                                 |
| regex_v8                 | 27.8 ms                                                | 24.9 ms: 1.12x faster                                                  |
| meteor_contest           | 120 ms                                                 | 107 ms: 1.11x faster                                                   |
| create_gc_cycles         | 1.62 ms                                                | 1.47 ms: 1.10x faster                                                  |
| json_loads               | 31.2 us                                                | 28.4 us: 1.10x faster                                                  |
| xml_etree_iterparse      | 115 ms                                                 | 105 ms: 1.10x faster                                                   |
| json                     | 5.69 ms                                                | 5.24 ms: 1.09x faster                                                  |
| sqlite_synth             | 3.02 us                                                | 2.82 us: 1.07x faster                                                  |
| xml_etree_parse          | 168 ms                                                 | 157 ms: 1.07x faster                                                   |
| regex_dna                | 227 ms                                                 | 218 ms: 1.04x faster                                                   |
| gc_traversal             | 3.62 ms                                                | 3.53 ms: 1.03x faster                                                  |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                                   |
| asyncio_websockets       | 559 ms                                                 | 551 ms: 1.01x faster                                                   |
| unpickle_list            | 5.20 us                                                | 5.45 us: 1.05x slower                                                  |
| pickle                   | 10.7 us                                                | 11.5 us: 1.08x slower                                                  |
| unpickle                 | 14.4 us                                                | 15.5 us: 1.08x slower                                                  |
| telco                    | 7.27 ms                                                | 8.26 ms: 1.14x slower                                                  |
| pickle_dict              | 29.6 us                                                | 34.9 us: 1.18x slower                                                  |
| coverage                 | 79.4 ms                                                | 96.4 ms: 1.21x slower                                                  |
| python_startup_no_site   | 5.93 ms                                                | 8.68 ms: 1.46x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.36x faster                                                           |

Benchmark hidden because not significant (5): mypy2, async_generators, regex_effbot, bench_mp_pool, pickle_list
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240106-3.13.0a2+-f19b93f/bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.31x
- 95% likely to have a speedup of 1.30x
- 99% likely to have a speedup of 1.29x


# Memory

- memory change: 1.05x