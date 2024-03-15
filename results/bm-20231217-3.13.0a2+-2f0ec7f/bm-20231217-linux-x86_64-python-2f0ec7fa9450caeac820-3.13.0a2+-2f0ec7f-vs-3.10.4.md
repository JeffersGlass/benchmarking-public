
# Results vs. 3.10.4

- fork: python
- ref: 2f0ec7fa9450caeac820
- machine: linux-x86_64
- commit hash: 2f0ec7f
- commit date: 2023-12-17
- overall geometric mean: 1.36x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.29x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 262 ms: 1.33x faster                                                   |
| chameleon      | 9.68 ms                                                | 6.96 ms: 1.39x faster                                                  |
| docutils       | 3.30 sec                                               | 2.61 sec: 1.26x faster                                                 |
| tornado_http   | 136 ms                                                 | 93.8 ms: 1.45x faster                                                  |
| Geometric mean | (ref)                                                  | 1.36x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 438 ms: 1.66x faster                                                   |
| async_tree_memoization  | 870 ms                                                 | 564 ms: 1.54x faster                                                   |
| async_tree_io           | 1.77 sec                                               | 1.19 sec: 1.49x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 710 ms: 1.43x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.53x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 88.8 ms: 1.73x faster                                                  |
| float          | 117 ms                                                 | 80.8 ms: 1.45x faster                                                  |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                                   |
| Geometric mean | (ref)                                                  | 1.37x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 129 ms: 1.46x faster                                                   |
| regex_v8       | 27.8 ms                                                | 23.8 ms: 1.17x faster                                                  |
| regex_dna      | 227 ms                                                 | 229 ms: 1.01x slower                                                   |
| regex_effbot   | 3.63 ms                                                | 3.72 ms: 1.03x slower                                                  |
| Geometric mean | (ref)                                                  | 1.13x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 295 us: 1.64x faster                                                   |
| unpickle_pure_python | 331 us                                                 | 215 us: 1.53x faster                                                   |
| tomli_loads          | 3.14 sec                                               | 2.13 sec: 1.47x faster                                                 |
| json_dumps           | 14.2 ms                                                | 10.3 ms: 1.37x faster                                                  |
| xml_etree_process    | 79.1 ms                                                | 58.3 ms: 1.36x faster                                                  |
| xml_etree_generate   | 99.4 ms                                                | 85.2 ms: 1.17x faster                                                  |
| json_loads           | 31.2 us                                                | 28.1 us: 1.11x faster                                                  |
| xml_etree_iterparse  | 115 ms                                                 | 104 ms: 1.11x faster                                                   |
| xml_etree_parse      | 168 ms                                                 | 157 ms: 1.07x faster                                                   |
| unpickle_list        | 5.20 us                                                | 5.06 us: 1.03x faster                                                  |
| pickle_list          | 5.08 us                                                | 4.96 us: 1.02x faster                                                  |
| unpickle             | 14.4 us                                                | 14.6 us: 1.01x slower                                                  |
| pickle               | 10.7 us                                                | 11.2 us: 1.05x slower                                                  |
| pickle_dict          | 29.6 us                                                | 33.7 us: 1.14x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.17x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.45x faster                                                  |
| python_startup_no_site | 5.93 ms                                                | 8.70 ms: 1.47x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.4 ms: 1.44x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 111 us: 4.90x faster                                                   |
| generators               | 80.1 ms                                                | 28.3 ms: 2.83x faster                                                  |
| deltablue                | 7.91 ms                                                | 3.19 ms: 2.48x faster                                                  |
| raytrace                 | 507 ms                                                 | 260 ms: 1.95x faster                                                   |
| chaos                    | 115 ms                                                 | 59.7 ms: 1.93x faster                                                  |
| asyncio_tcp              | 922 ms                                                 | 478 ms: 1.93x faster                                                   |
| logging_silent           | 190 ns                                                 | 103 ns: 1.85x faster                                                   |
| scimark_sor              | 220 ms                                                 | 121 ms: 1.81x faster                                                   |
| comprehensions           | 28.8 us                                                | 16.0 us: 1.80x faster                                                  |
| richards_super           | 94.7 ms                                                | 53.2 ms: 1.78x faster                                                  |
| crypto_pyaes             | 128 ms                                                 | 71.9 ms: 1.78x faster                                                  |
| scimark_monte_carlo      | 118 ms                                                 | 66.5 ms: 1.78x faster                                                  |
| sqlglot_parse            | 2.17 ms                                                | 1.24 ms: 1.74x faster                                                  |
| hexiom                   | 10.4 ms                                                | 6.00 ms: 1.73x faster                                                  |
| nbody                    | 154 ms                                                 | 88.8 ms: 1.73x faster                                                  |
| go                       | 240 ms                                                 | 139 ms: 1.73x faster                                                   |
| richards                 | 79.3 ms                                                | 47.0 ms: 1.69x faster                                                  |
| async_tree_none          | 728 ms                                                 | 438 ms: 1.66x faster                                                   |
| pickle_pure_python       | 484 us                                                 | 295 us: 1.64x faster                                                   |
| sqlglot_transpile        | 2.57 ms                                                | 1.57 ms: 1.64x faster                                                  |
| coroutines               | 35.1 ms                                                | 21.8 ms: 1.61x faster                                                  |
| scimark_lu               | 176 ms                                                 | 112 ms: 1.57x faster                                                   |
| pyflate                  | 716 ms                                                 | 458 ms: 1.56x faster                                                   |
| async_tree_memoization   | 870 ms                                                 | 564 ms: 1.54x faster                                                   |
| unpickle_pure_python     | 331 us                                                 | 215 us: 1.53x faster                                                   |
| spectral_norm            | 170 ms                                                 | 111 ms: 1.53x faster                                                   |
| deepcopy_memo            | 58.5 us                                                | 38.4 us: 1.52x faster                                                  |
| async_tree_io            | 1.77 sec                                               | 1.19 sec: 1.49x faster                                                 |
| logging_simple           | 8.30 us                                                | 5.63 us: 1.47x faster                                                  |
| tomli_loads              | 3.14 sec                                               | 2.13 sec: 1.47x faster                                                 |
| logging_format           | 9.09 us                                                | 6.20 us: 1.47x faster                                                  |
| regex_compile            | 188 ms                                                 | 129 ms: 1.46x faster                                                   |
| tornado_http             | 136 ms                                                 | 93.8 ms: 1.45x faster                                                  |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.45x faster                                                  |
| float                    | 117 ms                                                 | 80.8 ms: 1.45x faster                                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.78 sec: 1.44x faster                                                 |
| mako                     | 16.3 ms                                                | 11.4 ms: 1.44x faster                                                  |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 710 ms: 1.43x faster                                                   |
| pprint_pformat           | 2.10 sec                                               | 1.51 sec: 1.40x faster                                                 |
| chameleon                | 9.68 ms                                                | 6.96 ms: 1.39x faster                                                  |
| json_dumps               | 14.2 ms                                                | 10.3 ms: 1.37x faster                                                  |
| pprint_safe_repr         | 1.02 sec                                               | 744 ms: 1.37x faster                                                   |
| deepcopy                 | 479 us                                                 | 351 us: 1.37x faster                                                   |
| xml_etree_process        | 79.1 ms                                                | 58.3 ms: 1.36x faster                                                  |
| sqlglot_normalize        | 143 ms                                                 | 106 ms: 1.35x faster                                                   |
| fannkuch                 | 532 ms                                                 | 397 ms: 1.34x faster                                                   |
| pycparser                | 1.58 sec                                               | 1.18 sec: 1.33x faster                                                 |
| 2to3                     | 348 ms                                                 | 262 ms: 1.33x faster                                                   |
| deepcopy_reduce          | 4.17 us                                                | 3.15 us: 1.33x faster                                                  |
| nqueens                  | 106 ms                                                 | 79.8 ms: 1.33x faster                                                  |
| sympy_integrate          | 25.8 ms                                                | 19.5 ms: 1.32x faster                                                  |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.89 ms: 1.32x faster                                                  |
| sympy_sum                | 196 ms                                                 | 149 ms: 1.32x faster                                                   |
| sqlglot_optimize         | 69.2 ms                                                | 53.2 ms: 1.30x faster                                                  |
| dulwich_log              | 84.3 ms                                                | 65.5 ms: 1.29x faster                                                  |
| sympy_str                | 346 ms                                                 | 269 ms: 1.28x faster                                                   |
| docutils                 | 3.30 sec                                               | 2.61 sec: 1.26x faster                                                 |
| scimark_fft              | 466 ms                                                 | 371 ms: 1.25x faster                                                   |
| sympy_expand             | 566 ms                                                 | 455 ms: 1.24x faster                                                   |
| dask                     | 441 ms                                                 | 361 ms: 1.22x faster                                                   |
| bench_thread_pool        | 986 us                                                 | 824 us: 1.20x faster                                                   |
| regex_v8                 | 27.8 ms                                                | 23.8 ms: 1.17x faster                                                  |
| xml_etree_generate       | 99.4 ms                                                | 85.2 ms: 1.17x faster                                                  |
| unpack_sequence          | 60.0 ns                                                | 53.1 ns: 1.13x faster                                                  |
| mdp                      | 2.85 sec                                               | 2.53 sec: 1.12x faster                                                 |
| meteor_contest           | 120 ms                                                 | 107 ms: 1.11x faster                                                   |
| json_loads               | 31.2 us                                                | 28.1 us: 1.11x faster                                                  |
| xml_etree_iterparse      | 115 ms                                                 | 104 ms: 1.11x faster                                                   |
| pathlib                  | 20.5 ms                                                | 18.5 ms: 1.10x faster                                                  |
| json                     | 5.69 ms                                                | 5.18 ms: 1.10x faster                                                  |
| create_gc_cycles         | 1.62 ms                                                | 1.48 ms: 1.10x faster                                                  |
| sqlite_synth             | 3.02 us                                                | 2.80 us: 1.08x faster                                                  |
| xml_etree_parse          | 168 ms                                                 | 157 ms: 1.07x faster                                                   |
| unpickle_list            | 5.20 us                                                | 5.06 us: 1.03x faster                                                  |
| gc_traversal             | 3.62 ms                                                | 3.54 ms: 1.02x faster                                                  |
| pickle_list              | 5.08 us                                                | 4.96 us: 1.02x faster                                                  |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                                   |
| asyncio_websockets       | 559 ms                                                 | 551 ms: 1.01x faster                                                   |
| async_generators         | 444 ms                                                 | 440 ms: 1.01x faster                                                   |
| regex_dna                | 227 ms                                                 | 229 ms: 1.01x slower                                                   |
| unpickle                 | 14.4 us                                                | 14.6 us: 1.01x slower                                                  |
| regex_effbot             | 3.63 ms                                                | 3.72 ms: 1.03x slower                                                  |
| pickle                   | 10.7 us                                                | 11.2 us: 1.05x slower                                                  |
| telco                    | 7.27 ms                                                | 8.20 ms: 1.13x slower                                                  |
| pickle_dict              | 29.6 us                                                | 33.7 us: 1.14x slower                                                  |
| coverage                 | 79.4 ms                                                | 95.2 ms: 1.20x slower                                                  |
| python_startup_no_site   | 5.93 ms                                                | 8.70 ms: 1.47x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.36x faster                                                           |

Benchmark hidden because not significant (2): mypy2, bench_mp_pool
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231217-3.13.0a2+-2f0ec7f/bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.32x
- 95% likely to have a speedup of 1.31x
- 99% likely to have a speedup of 1.29x


# Memory

- memory change: 1.06x