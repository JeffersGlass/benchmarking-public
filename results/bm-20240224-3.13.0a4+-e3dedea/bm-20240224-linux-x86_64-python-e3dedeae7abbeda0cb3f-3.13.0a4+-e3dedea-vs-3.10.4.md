
# Results vs. 3.10.4

- fork: python
- ref: e3dedeae7abbeda0cb3f
- machine: linux-x86_64
- commit hash: e3dedea
- commit date: 2024-02-24
- overall geometric mean: 1.37x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.30x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 263 ms: 1.33x faster                                                   |
| chameleon      | 9.68 ms                                                | 6.67 ms: 1.45x faster                                                  |
| docutils       | 3.30 sec                                               | 2.58 sec: 1.28x faster                                                 |
| tornado_http   | 136 ms                                                 | 94.5 ms: 1.44x faster                                                  |
| Geometric mean | (ref)                                                  | 1.37x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 433 ms: 1.68x faster                                                   |
| async_tree_memoization  | 870 ms                                                 | 556 ms: 1.56x faster                                                   |
| async_tree_io           | 1.77 sec                                               | 1.17 sec: 1.51x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 703 ms: 1.45x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.55x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 88.7 ms: 1.73x faster                                                  |
| float          | 117 ms                                                 | 80.1 ms: 1.46x faster                                                  |
| pidigits       | 191 ms                                                 | 188 ms: 1.02x faster                                                   |
| Geometric mean | (ref)                                                  | 1.37x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 130 ms: 1.45x faster                                                   |
| regex_v8       | 27.8 ms                                                | 24.6 ms: 1.13x faster                                                  |
| regex_dna      | 227 ms                                                 | 214 ms: 1.06x faster                                                   |
| regex_effbot   | 3.63 ms                                                | 3.49 ms: 1.04x faster                                                  |
| Geometric mean | (ref)                                                  | 1.16x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 289 us: 1.67x faster                                                   |
| unpickle_pure_python | 331 us                                                 | 211 us: 1.57x faster                                                   |
| tomli_loads          | 3.14 sec                                               | 2.14 sec: 1.47x faster                                                 |
| xml_etree_process    | 79.1 ms                                                | 57.9 ms: 1.37x faster                                                  |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.36x faster                                                  |
| xml_etree_generate   | 99.4 ms                                                | 84.3 ms: 1.18x faster                                                  |
| json_loads           | 31.2 us                                                | 27.4 us: 1.14x faster                                                  |
| xml_etree_iterparse  | 115 ms                                                 | 105 ms: 1.10x faster                                                   |
| xml_etree_parse      | 168 ms                                                 | 157 ms: 1.07x faster                                                   |
| unpickle_list        | 5.20 us                                                | 4.98 us: 1.04x faster                                                  |
| pickle_list          | 5.08 us                                                | 5.21 us: 1.03x slower                                                  |
| unpickle             | 14.4 us                                                | 14.9 us: 1.03x slower                                                  |
| pickle               | 10.7 us                                                | 12.1 us: 1.13x slower                                                  |
| pickle_dict          | 29.6 us                                                | 35.8 us: 1.21x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.16x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                  |
| python_startup_no_site | 5.93 ms                                                | 8.73 ms: 1.47x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 10.7 ms: 1.52x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 111 us: 4.91x faster                                                   |
| generators               | 80.1 ms                                                | 29.2 ms: 2.74x faster                                                  |
| deltablue                | 7.91 ms                                                | 3.13 ms: 2.53x faster                                                  |
| chaos                    | 115 ms                                                 | 58.5 ms: 1.97x faster                                                  |
| raytrace                 | 507 ms                                                 | 257 ms: 1.97x faster                                                   |
| logging_silent           | 190 ns                                                 | 97.0 ns: 1.96x faster                                                  |
| asyncio_tcp              | 922 ms                                                 | 484 ms: 1.90x faster                                                   |
| crypto_pyaes             | 128 ms                                                 | 70.5 ms: 1.81x faster                                                  |
| richards_super           | 94.7 ms                                                | 52.5 ms: 1.80x faster                                                  |
| scimark_sor              | 220 ms                                                 | 122 ms: 1.80x faster                                                   |
| scimark_monte_carlo      | 118 ms                                                 | 66.0 ms: 1.79x faster                                                  |
| comprehensions           | 28.8 us                                                | 16.2 us: 1.78x faster                                                  |
| go                       | 240 ms                                                 | 135 ms: 1.77x faster                                                   |
| sqlglot_parse            | 2.17 ms                                                | 1.24 ms: 1.75x faster                                                  |
| hexiom                   | 10.4 ms                                                | 5.99 ms: 1.74x faster                                                  |
| nbody                    | 154 ms                                                 | 88.7 ms: 1.73x faster                                                  |
| richards                 | 79.3 ms                                                | 46.3 ms: 1.71x faster                                                  |
| async_tree_none          | 728 ms                                                 | 433 ms: 1.68x faster                                                   |
| pickle_pure_python       | 484 us                                                 | 289 us: 1.67x faster                                                   |
| sqlglot_transpile        | 2.57 ms                                                | 1.56 ms: 1.65x faster                                                  |
| deepcopy_memo            | 58.5 us                                                | 36.2 us: 1.62x faster                                                  |
| coroutines               | 35.1 ms                                                | 22.0 ms: 1.59x faster                                                  |
| unpickle_pure_python     | 331 us                                                 | 211 us: 1.57x faster                                                   |
| scimark_lu               | 176 ms                                                 | 112 ms: 1.57x faster                                                   |
| async_tree_memoization   | 870 ms                                                 | 556 ms: 1.56x faster                                                   |
| pyflate                  | 716 ms                                                 | 458 ms: 1.56x faster                                                   |
| spectral_norm            | 170 ms                                                 | 109 ms: 1.56x faster                                                   |
| mako                     | 16.3 ms                                                | 10.7 ms: 1.52x faster                                                  |
| async_tree_io            | 1.77 sec                                               | 1.17 sec: 1.51x faster                                                 |
| logging_simple           | 8.30 us                                                | 5.61 us: 1.48x faster                                                  |
| logging_format           | 9.09 us                                                | 6.16 us: 1.48x faster                                                  |
| tomli_loads              | 3.14 sec                                               | 2.14 sec: 1.47x faster                                                 |
| float                    | 117 ms                                                 | 80.1 ms: 1.46x faster                                                  |
| chameleon                | 9.68 ms                                                | 6.67 ms: 1.45x faster                                                  |
| regex_compile            | 188 ms                                                 | 130 ms: 1.45x faster                                                   |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 703 ms: 1.45x faster                                                   |
| tornado_http             | 136 ms                                                 | 94.5 ms: 1.44x faster                                                  |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                  |
| pprint_pformat           | 2.10 sec                                               | 1.46 sec: 1.44x faster                                                 |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.79 sec: 1.44x faster                                                 |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.54 ms: 1.43x faster                                                  |
| deepcopy                 | 479 us                                                 | 337 us: 1.42x faster                                                   |
| pprint_safe_repr         | 1.02 sec                                               | 720 ms: 1.41x faster                                                   |
| deepcopy_reduce          | 4.17 us                                                | 2.98 us: 1.40x faster                                                  |
| fannkuch                 | 532 ms                                                 | 381 ms: 1.40x faster                                                   |
| pycparser                | 1.58 sec                                               | 1.15 sec: 1.37x faster                                                 |
| xml_etree_process        | 79.1 ms                                                | 57.9 ms: 1.37x faster                                                  |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.36x faster                                                  |
| sqlglot_normalize        | 143 ms                                                 | 105 ms: 1.36x faster                                                   |
| sympy_sum                | 196 ms                                                 | 147 ms: 1.33x faster                                                   |
| 2to3                     | 348 ms                                                 | 263 ms: 1.33x faster                                                   |
| sympy_integrate          | 25.8 ms                                                | 19.5 ms: 1.32x faster                                                  |
| scimark_fft              | 466 ms                                                 | 352 ms: 1.32x faster                                                   |
| nqueens                  | 106 ms                                                 | 80.0 ms: 1.32x faster                                                  |
| sqlglot_optimize         | 69.2 ms                                                | 53.0 ms: 1.30x faster                                                  |
| dulwich_log              | 84.3 ms                                                | 65.2 ms: 1.29x faster                                                  |
| sympy_str                | 346 ms                                                 | 268 ms: 1.29x faster                                                   |
| docutils                 | 3.30 sec                                               | 2.58 sec: 1.28x faster                                                 |
| sympy_expand             | 566 ms                                                 | 449 ms: 1.26x faster                                                   |
| bench_thread_pool        | 986 us                                                 | 813 us: 1.21x faster                                                   |
| xml_etree_generate       | 99.4 ms                                                | 84.3 ms: 1.18x faster                                                  |
| json                     | 5.69 ms                                                | 4.98 ms: 1.14x faster                                                  |
| json_loads               | 31.2 us                                                | 27.4 us: 1.14x faster                                                  |
| pathlib                  | 20.5 ms                                                | 18.1 ms: 1.13x faster                                                  |
| mdp                      | 2.85 sec                                               | 2.52 sec: 1.13x faster                                                 |
| regex_v8                 | 27.8 ms                                                | 24.6 ms: 1.13x faster                                                  |
| meteor_contest           | 120 ms                                                 | 107 ms: 1.12x faster                                                   |
| xml_etree_iterparse      | 115 ms                                                 | 105 ms: 1.10x faster                                                   |
| unpack_sequence          | 60.0 ns                                                | 55.0 ns: 1.09x faster                                                  |
| create_gc_cycles         | 1.62 ms                                                | 1.49 ms: 1.09x faster                                                  |
| sqlite_synth             | 3.02 us                                                | 2.81 us: 1.07x faster                                                  |
| xml_etree_parse          | 168 ms                                                 | 157 ms: 1.07x faster                                                   |
| regex_dna                | 227 ms                                                 | 214 ms: 1.06x faster                                                   |
| unpickle_list            | 5.20 us                                                | 4.98 us: 1.04x faster                                                  |
| regex_effbot             | 3.63 ms                                                | 3.49 ms: 1.04x faster                                                  |
| pidigits                 | 191 ms                                                 | 188 ms: 1.02x faster                                                   |
| asyncio_websockets       | 559 ms                                                 | 551 ms: 1.01x faster                                                   |
| async_generators         | 444 ms                                                 | 449 ms: 1.01x slower                                                   |
| pickle_list              | 5.08 us                                                | 5.21 us: 1.03x slower                                                  |
| unpickle                 | 14.4 us                                                | 14.9 us: 1.03x slower                                                  |
| gc_traversal             | 3.62 ms                                                | 3.83 ms: 1.06x slower                                                  |
| pickle                   | 10.7 us                                                | 12.1 us: 1.13x slower                                                  |
| telco                    | 7.27 ms                                                | 8.34 ms: 1.15x slower                                                  |
| coverage                 | 79.4 ms                                                | 94.4 ms: 1.19x slower                                                  |
| pickle_dict              | 29.6 us                                                | 35.8 us: 1.21x slower                                                  |
| python_startup_no_site   | 5.93 ms                                                | 8.73 ms: 1.47x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.37x faster                                                           |

Benchmark hidden because not significant (2): mypy2, bench_mp_pool
Ignored benchmarks (13) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240224-3.13.0a4+-e3dedea/bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.33x
- 95% likely to have a speedup of 1.32x
- 99% likely to have a speedup of 1.30x


# Memory

- memory change: 1.06x