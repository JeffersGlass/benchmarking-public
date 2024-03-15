
# Results vs. 3.10.4

- fork: python
- ref: v3.11.6
- machine: linux-x86_64
- commit hash: 8b6ee5b
- commit date: 2023-10-02
- overall geometric mean: 1.32x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.27x faster
- Memory change: 1.09x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231002-linux-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 257 ms: 1.36x faster                                   |
| chameleon      | 9.68 ms                                                | 6.61 ms: 1.47x faster                                  |
| docutils       | 3.30 sec                                               | 2.58 sec: 1.28x faster                                 |
| html5lib       | 88.9 ms                                                | 63.9 ms: 1.39x faster                                  |
| tornado_http   | 136 ms                                                 | 96.9 ms: 1.41x faster                                  |
| Geometric mean | (ref)                                                  | 1.38x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231002-linux-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 522 ms: 1.39x faster                                   |
| async_tree_memoization  | 870 ms                                                 | 632 ms: 1.38x faster                                   |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 742 ms: 1.37x faster                                   |
| async_tree_io           | 1.77 sec                                               | 1.30 sec: 1.36x faster                                 |
| Geometric mean          | (ref)                                                  | 1.37x faster                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231002-linux-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| nbody          | 154 ms                                                 | 92.6 ms: 1.66x faster                                  |
| float          | 117 ms                                                 | 75.7 ms: 1.55x faster                                  |
| pidigits       | 191 ms                                                 | 199 ms: 1.04x slower                                   |
| Geometric mean | (ref)                                                  | 1.35x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231002-linux-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 136 ms: 1.39x faster                                   |
| regex_v8       | 27.8 ms                                                | 21.9 ms: 1.27x faster                                  |
| regex_dna      | 227 ms                                                 | 199 ms: 1.14x faster                                   |
| regex_effbot   | 3.63 ms                                                | 3.47 ms: 1.05x faster                                  |
| Geometric mean | (ref)                                                  | 1.20x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231002-linux-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 306 us: 1.58x faster                                   |
| xml_etree_process    | 79.1 ms                                                | 53.7 ms: 1.47x faster                                  |
| unpickle_pure_python | 331 us                                                 | 230 us: 1.44x faster                                   |
| tomli_loads          | 3.14 sec                                               | 2.25 sec: 1.39x faster                                 |
| json_loads           | 31.2 us                                                | 23.9 us: 1.31x faster                                  |
| xml_etree_generate   | 99.4 ms                                                | 76.7 ms: 1.30x faster                                  |
| pickle_list          | 5.08 us                                                | 4.05 us: 1.25x faster                                  |
| xml_etree_iterparse  | 115 ms                                                 | 103 ms: 1.12x faster                                   |
| json_dumps           | 14.2 ms                                                | 12.7 ms: 1.12x faster                                  |
| pickle               | 10.7 us                                                | 9.82 us: 1.08x faster                                  |
| unpickle             | 14.4 us                                                | 13.3 us: 1.08x faster                                  |
| xml_etree_parse      | 168 ms                                                 | 158 ms: 1.06x faster                                   |
| unpickle_list        | 5.20 us                                                | 5.08 us: 1.02x faster                                  |
| pickle_dict          | 29.6 us                                                | 29.9 us: 1.01x slower                                  |
| Geometric mean       | (ref)                                                  | 1.22x faster                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231002-linux-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 8.50 ms: 1.72x faster                                  |
| python_startup_no_site | 5.93 ms                                                | 6.00 ms: 1.01x slower                                  |
| Geometric mean         | (ref)                                                  | 1.30x faster                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231002-linux-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako            | 16.3 ms                                                | 9.88 ms: 1.65x faster                                  |
| django_template | 48.2 ms                                                | 33.1 ms: 1.46x faster                                  |
| genshi_text     | 31.8 ms                                                | 21.9 ms: 1.45x faster                                  |
| genshi_xml      | 66.0 ms                                                | 51.5 ms: 1.28x faster                                  |
| Geometric mean  | (ref)                                                  | 1.45x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231002-linux-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| deltablue                | 7.91 ms                                                | 3.94 ms: 2.01x faster                                  |
| logging_silent           | 190 ns                                                 | 101 ns: 1.87x faster                                   |
| scimark_sor              | 220 ms                                                 | 118 ms: 1.87x faster                                   |
| pyflate                  | 716 ms                                                 | 412 ms: 1.74x faster                                   |
| raytrace                 | 507 ms                                                 | 293 ms: 1.73x faster                                   |
| scimark_monte_carlo      | 118 ms                                                 | 68.5 ms: 1.73x faster                                  |
| crypto_pyaes             | 128 ms                                                 | 74.4 ms: 1.72x faster                                  |
| go                       | 240 ms                                                 | 140 ms: 1.72x faster                                   |
| python_startup           | 14.6 ms                                                | 8.50 ms: 1.72x faster                                  |
| chaos                    | 115 ms                                                 | 68.8 ms: 1.68x faster                                  |
| nbody                    | 154 ms                                                 | 92.6 ms: 1.66x faster                                  |
| richards                 | 79.3 ms                                                | 47.9 ms: 1.65x faster                                  |
| mako                     | 16.3 ms                                                | 9.88 ms: 1.65x faster                                  |
| spectral_norm            | 170 ms                                                 | 103 ms: 1.64x faster                                   |
| deepcopy_memo            | 58.5 us                                                | 36.3 us: 1.61x faster                                  |
| scimark_lu               | 176 ms                                                 | 110 ms: 1.61x faster                                   |
| richards_super           | 94.7 ms                                                | 59.0 ms: 1.60x faster                                  |
| hexiom                   | 10.4 ms                                                | 6.49 ms: 1.60x faster                                  |
| pickle_pure_python       | 484 us                                                 | 306 us: 1.58x faster                                   |
| sqlglot_parse            | 2.17 ms                                                | 1.37 ms: 1.58x faster                                  |
| float                    | 117 ms                                                 | 75.7 ms: 1.55x faster                                  |
| sqlglot_transpile        | 2.57 ms                                                | 1.68 ms: 1.53x faster                                  |
| xml_etree_process        | 79.1 ms                                                | 53.7 ms: 1.47x faster                                  |
| chameleon                | 9.68 ms                                                | 6.61 ms: 1.47x faster                                  |
| django_template          | 48.2 ms                                                | 33.1 ms: 1.46x faster                                  |
| genshi_text              | 31.8 ms                                                | 21.9 ms: 1.45x faster                                  |
| pprint_pformat           | 2.10 sec                                               | 1.45 sec: 1.45x faster                                 |
| pprint_safe_repr         | 1.02 sec                                               | 703 ms: 1.45x faster                                   |
| unpickle_pure_python     | 331 us                                                 | 230 us: 1.44x faster                                   |
| thrift                   | 1.07 ms                                                | 757 us: 1.42x faster                                   |
| pycparser                | 1.58 sec                                               | 1.12 sec: 1.41x faster                                 |
| tornado_http             | 136 ms                                                 | 96.9 ms: 1.41x faster                                  |
| scimark_fft              | 466 ms                                                 | 332 ms: 1.40x faster                                   |
| logging_simple           | 8.30 us                                                | 5.93 us: 1.40x faster                                  |
| deepcopy                 | 479 us                                                 | 342 us: 1.40x faster                                   |
| deepcopy_reduce          | 4.17 us                                                | 2.98 us: 1.40x faster                                  |
| unpack_sequence          | 60.0 ns                                                | 42.9 ns: 1.40x faster                                  |
| tomli_loads              | 3.14 sec                                               | 2.25 sec: 1.39x faster                                 |
| async_tree_none          | 728 ms                                                 | 522 ms: 1.39x faster                                   |
| logging_format           | 9.09 us                                                | 6.52 us: 1.39x faster                                  |
| html5lib                 | 88.9 ms                                                | 63.9 ms: 1.39x faster                                  |
| regex_compile            | 188 ms                                                 | 136 ms: 1.39x faster                                   |
| async_tree_memoization   | 870 ms                                                 | 632 ms: 1.38x faster                                   |
| fannkuch                 | 532 ms                                                 | 387 ms: 1.37x faster                                   |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 742 ms: 1.37x faster                                   |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.76 ms: 1.36x faster                                  |
| async_tree_io            | 1.77 sec                                               | 1.30 sec: 1.36x faster                                 |
| 2to3                     | 348 ms                                                 | 257 ms: 1.36x faster                                   |
| coroutines               | 35.1 ms                                                | 25.9 ms: 1.35x faster                                  |
| sqlglot_normalize        | 143 ms                                                 | 108 ms: 1.32x faster                                   |
| sqlalchemy_imperative    | 23.3 ms                                                | 17.7 ms: 1.32x faster                                  |
| aiohttp                  | 1.44 ms                                                | 1.10 ms: 1.31x faster                                  |
| dulwich_log              | 84.3 ms                                                | 64.5 ms: 1.31x faster                                  |
| json_loads               | 31.2 us                                                | 23.9 us: 1.31x faster                                  |
| sqlglot_optimize         | 69.2 ms                                                | 53.0 ms: 1.31x faster                                  |
| gunicorn                 | 1.53 ms                                                | 1.17 ms: 1.31x faster                                  |
| comprehensions           | 28.8 us                                                | 22.2 us: 1.30x faster                                  |
| xml_etree_generate       | 99.4 ms                                                | 76.7 ms: 1.30x faster                                  |
| genshi_xml               | 66.0 ms                                                | 51.5 ms: 1.28x faster                                  |
| docutils                 | 3.30 sec                                               | 2.58 sec: 1.28x faster                                 |
| regex_v8                 | 27.8 ms                                                | 21.9 ms: 1.27x faster                                  |
| nqueens                  | 106 ms                                                 | 83.7 ms: 1.26x faster                                  |
| pickle_list              | 5.08 us                                                | 4.05 us: 1.25x faster                                  |
| async_generators         | 444 ms                                                 | 356 ms: 1.25x faster                                   |
| sqlalchemy_declarative   | 172 ms                                                 | 139 ms: 1.24x faster                                   |
| sympy_integrate          | 25.8 ms                                                | 20.8 ms: 1.24x faster                                  |
| json                     | 5.69 ms                                                | 4.59 ms: 1.24x faster                                  |
| dask                     | 441 ms                                                 | 358 ms: 1.23x faster                                   |
| flaskblogging            | 8.58 ms                                                | 7.04 ms: 1.22x faster                                  |
| sqlite_synth             | 3.02 us                                                | 2.50 us: 1.21x faster                                  |
| sympy_str                | 346 ms                                                 | 287 ms: 1.20x faster                                   |
| bench_thread_pool        | 986 us                                                 | 821 us: 1.20x faster                                   |
| sympy_expand             | 566 ms                                                 | 471 ms: 1.20x faster                                   |
| sympy_sum                | 196 ms                                                 | 165 ms: 1.19x faster                                   |
| djangocms                | 38.4 us                                                | 32.6 us: 1.18x faster                                  |
| pylint                   | 551 ms                                                 | 473 ms: 1.17x faster                                   |
| regex_dna                | 227 ms                                                 | 199 ms: 1.14x faster                                   |
| meteor_contest           | 120 ms                                                 | 105 ms: 1.14x faster                                   |
| pathlib                  | 20.5 ms                                                | 18.2 ms: 1.12x faster                                  |
| xml_etree_iterparse      | 115 ms                                                 | 103 ms: 1.12x faster                                   |
| json_dumps               | 14.2 ms                                                | 12.7 ms: 1.12x faster                                  |
| generators               | 80.1 ms                                                | 72.2 ms: 1.11x faster                                  |
| typing_runtime_protocols | 544 us                                                 | 493 us: 1.10x faster                                   |
| create_gc_cycles         | 1.62 ms                                                | 1.47 ms: 1.10x faster                                  |
| telco                    | 7.27 ms                                                | 6.66 ms: 1.09x faster                                  |
| pickle                   | 10.7 us                                                | 9.82 us: 1.08x faster                                  |
| unpickle                 | 14.4 us                                                | 13.3 us: 1.08x faster                                  |
| xml_etree_parse          | 168 ms                                                 | 158 ms: 1.06x faster                                   |
| regex_effbot             | 3.63 ms                                                | 3.47 ms: 1.05x faster                                  |
| unpickle_list            | 5.20 us                                                | 5.08 us: 1.02x faster                                  |
| mdp                      | 2.85 sec                                               | 2.81 sec: 1.01x faster                                 |
| pickle_dict              | 29.6 us                                                | 29.9 us: 1.01x slower                                  |
| python_startup_no_site   | 5.93 ms                                                | 6.00 ms: 1.01x slower                                  |
| asyncio_tcp              | 922 ms                                                 | 934 ms: 1.01x slower                                   |
| pidigits                 | 191 ms                                                 | 199 ms: 1.04x slower                                   |
| gc_traversal             | 3.62 ms                                                | 4.25 ms: 1.17x slower                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 3.14 sec: 1.22x slower                                 |
| Geometric mean           | (ref)                                                  | 1.32x faster                                           |

Benchmark hidden because not significant (1): bench_mp_pool
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: asyncio_websockets, coverage, mypy2


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.30x
- 95% likely to have a speedup of 1.29x
- 99% likely to have a speedup of 1.27x


# Memory

- memory change: 1.09x