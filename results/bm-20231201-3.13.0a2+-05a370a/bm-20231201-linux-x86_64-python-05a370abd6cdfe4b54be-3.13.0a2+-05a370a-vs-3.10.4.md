
# Results vs. 3.10.4

- fork: python
- ref: 05a370abd6cdfe4b54be
- machine: linux-x86_64
- commit hash: 05a370a
- commit date: 2023-12-01
- overall geometric mean: 1.35x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.28x faster
- Memory change: 1.05x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 263 ms: 1.33x faster                                                   |
| chameleon      | 9.68 ms                                                | 7.00 ms: 1.38x faster                                                  |
| docutils       | 3.30 sec                                               | 2.61 sec: 1.26x faster                                                 |
| tornado_http   | 136 ms                                                 | 94.3 ms: 1.45x faster                                                  |
| Geometric mean | (ref)                                                  | 1.35x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 435 ms: 1.68x faster                                                   |
| async_tree_memoization  | 870 ms                                                 | 568 ms: 1.53x faster                                                   |
| async_tree_io           | 1.77 sec                                               | 1.18 sec: 1.50x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 710 ms: 1.43x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.53x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 92.4 ms: 1.66x faster                                                  |
| float          | 117 ms                                                 | 80.9 ms: 1.45x faster                                                  |
| pidigits       | 191 ms                                                 | 196 ms: 1.02x slower                                                   |
| Geometric mean | (ref)                                                  | 1.33x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 133 ms: 1.42x faster                                                   |
| regex_v8       | 27.8 ms                                                | 25.7 ms: 1.08x faster                                                  |
| regex_dna      | 227 ms                                                 | 219 ms: 1.03x faster                                                   |
| Geometric mean | (ref)                                                  | 1.12x faster                                                           |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 302 us: 1.61x faster                                                   |
| unpickle_pure_python | 331 us                                                 | 217 us: 1.52x faster                                                   |
| tomli_loads          | 3.14 sec                                               | 2.14 sec: 1.47x faster                                                 |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.37x faster                                                  |
| xml_etree_process    | 79.1 ms                                                | 59.4 ms: 1.33x faster                                                  |
| xml_etree_generate   | 99.4 ms                                                | 86.6 ms: 1.15x faster                                                  |
| json_loads           | 31.2 us                                                | 28.2 us: 1.10x faster                                                  |
| xml_etree_iterparse  | 115 ms                                                 | 106 ms: 1.09x faster                                                   |
| xml_etree_parse      | 168 ms                                                 | 157 ms: 1.07x faster                                                   |
| unpickle_list        | 5.20 us                                                | 5.04 us: 1.03x faster                                                  |
| unpickle             | 14.4 us                                                | 15.5 us: 1.08x slower                                                  |
| pickle               | 10.7 us                                                | 11.6 us: 1.09x slower                                                  |
| pickle_dict          | 29.6 us                                                | 34.3 us: 1.16x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.15x faster                                                           |

Benchmark hidden because not significant (1): pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.4 ms: 1.41x faster                                                  |
| python_startup_no_site | 5.93 ms                                                | 9.01 ms: 1.52x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.04x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.4 ms: 1.44x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 117 us: 4.64x faster                                                   |
| generators               | 80.1 ms                                                | 28.6 ms: 2.80x faster                                                  |
| deltablue                | 7.91 ms                                                | 3.25 ms: 2.43x faster                                                  |
| asyncio_tcp              | 922 ms                                                 | 483 ms: 1.91x faster                                                   |
| chaos                    | 115 ms                                                 | 60.9 ms: 1.90x faster                                                  |
| raytrace                 | 507 ms                                                 | 272 ms: 1.86x faster                                                   |
| logging_silent           | 190 ns                                                 | 104 ns: 1.82x faster                                                   |
| crypto_pyaes             | 128 ms                                                 | 70.9 ms: 1.80x faster                                                  |
| scimark_sor              | 220 ms                                                 | 123 ms: 1.78x faster                                                   |
| richards_super           | 94.7 ms                                                | 53.3 ms: 1.78x faster                                                  |
| comprehensions           | 28.8 us                                                | 16.3 us: 1.77x faster                                                  |
| sqlglot_parse            | 2.17 ms                                                | 1.26 ms: 1.72x faster                                                  |
| hexiom                   | 10.4 ms                                                | 6.09 ms: 1.71x faster                                                  |
| scimark_monte_carlo      | 118 ms                                                 | 69.3 ms: 1.71x faster                                                  |
| go                       | 240 ms                                                 | 142 ms: 1.68x faster                                                   |
| async_tree_none          | 728 ms                                                 | 435 ms: 1.68x faster                                                   |
| nbody                    | 154 ms                                                 | 92.4 ms: 1.66x faster                                                  |
| richards                 | 79.3 ms                                                | 47.9 ms: 1.66x faster                                                  |
| sqlglot_transpile        | 2.57 ms                                                | 1.57 ms: 1.63x faster                                                  |
| coroutines               | 35.1 ms                                                | 21.7 ms: 1.62x faster                                                  |
| pickle_pure_python       | 484 us                                                 | 302 us: 1.61x faster                                                   |
| pyflate                  | 716 ms                                                 | 459 ms: 1.56x faster                                                   |
| scimark_lu               | 176 ms                                                 | 115 ms: 1.53x faster                                                   |
| async_tree_memoization   | 870 ms                                                 | 568 ms: 1.53x faster                                                   |
| unpickle_pure_python     | 331 us                                                 | 217 us: 1.52x faster                                                   |
| spectral_norm            | 170 ms                                                 | 112 ms: 1.52x faster                                                   |
| async_tree_io            | 1.77 sec                                               | 1.18 sec: 1.50x faster                                                 |
| deepcopy_memo            | 58.5 us                                                | 39.0 us: 1.50x faster                                                  |
| tomli_loads              | 3.14 sec                                               | 2.14 sec: 1.47x faster                                                 |
| float                    | 117 ms                                                 | 80.9 ms: 1.45x faster                                                  |
| tornado_http             | 136 ms                                                 | 94.3 ms: 1.45x faster                                                  |
| logging_simple           | 8.30 us                                                | 5.74 us: 1.45x faster                                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.78 sec: 1.44x faster                                                 |
| logging_format           | 9.09 us                                                | 6.32 us: 1.44x faster                                                  |
| mako                     | 16.3 ms                                                | 11.4 ms: 1.44x faster                                                  |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 710 ms: 1.43x faster                                                   |
| regex_compile            | 188 ms                                                 | 133 ms: 1.42x faster                                                   |
| python_startup           | 14.6 ms                                                | 10.4 ms: 1.41x faster                                                  |
| pprint_pformat           | 2.10 sec                                               | 1.51 sec: 1.39x faster                                                 |
| chameleon                | 9.68 ms                                                | 7.00 ms: 1.38x faster                                                  |
| pprint_safe_repr         | 1.02 sec                                               | 739 ms: 1.38x faster                                                   |
| deepcopy                 | 479 us                                                 | 349 us: 1.37x faster                                                   |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.37x faster                                                  |
| sqlglot_normalize        | 143 ms                                                 | 105 ms: 1.36x faster                                                   |
| fannkuch                 | 532 ms                                                 | 394 ms: 1.35x faster                                                   |
| deepcopy_reduce          | 4.17 us                                                | 3.09 us: 1.35x faster                                                  |
| sympy_sum                | 196 ms                                                 | 147 ms: 1.33x faster                                                   |
| xml_etree_process        | 79.1 ms                                                | 59.4 ms: 1.33x faster                                                  |
| sympy_integrate          | 25.8 ms                                                | 19.5 ms: 1.33x faster                                                  |
| 2to3                     | 348 ms                                                 | 263 ms: 1.33x faster                                                   |
| nqueens                  | 106 ms                                                 | 80.0 ms: 1.32x faster                                                  |
| pycparser                | 1.58 sec                                               | 1.20 sec: 1.31x faster                                                 |
| sympy_str                | 346 ms                                                 | 267 ms: 1.30x faster                                                   |
| sqlglot_optimize         | 69.2 ms                                                | 53.5 ms: 1.29x faster                                                  |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.02 ms: 1.29x faster                                                  |
| unpack_sequence          | 60.0 ns                                                | 46.6 ns: 1.29x faster                                                  |
| dulwich_log              | 84.3 ms                                                | 65.5 ms: 1.29x faster                                                  |
| scimark_fft              | 466 ms                                                 | 366 ms: 1.27x faster                                                   |
| docutils                 | 3.30 sec                                               | 2.61 sec: 1.26x faster                                                 |
| sympy_expand             | 566 ms                                                 | 451 ms: 1.25x faster                                                   |
| dask                     | 441 ms                                                 | 360 ms: 1.22x faster                                                   |
| bench_thread_pool        | 986 us                                                 | 828 us: 1.19x faster                                                   |
| xml_etree_generate       | 99.4 ms                                                | 86.6 ms: 1.15x faster                                                  |
| pathlib                  | 20.5 ms                                                | 18.1 ms: 1.13x faster                                                  |
| mdp                      | 2.85 sec                                               | 2.56 sec: 1.11x faster                                                 |
| create_gc_cycles         | 1.62 ms                                                | 1.46 ms: 1.11x faster                                                  |
| json_loads               | 31.2 us                                                | 28.2 us: 1.10x faster                                                  |
| json                     | 5.69 ms                                                | 5.19 ms: 1.10x faster                                                  |
| meteor_contest           | 120 ms                                                 | 109 ms: 1.09x faster                                                   |
| xml_etree_iterparse      | 115 ms                                                 | 106 ms: 1.09x faster                                                   |
| regex_v8                 | 27.8 ms                                                | 25.7 ms: 1.08x faster                                                  |
| sqlite_synth             | 3.02 us                                                | 2.81 us: 1.08x faster                                                  |
| xml_etree_parse          | 168 ms                                                 | 157 ms: 1.07x faster                                                   |
| regex_dna                | 227 ms                                                 | 219 ms: 1.03x faster                                                   |
| unpickle_list            | 5.20 us                                                | 5.04 us: 1.03x faster                                                  |
| asyncio_websockets       | 559 ms                                                 | 551 ms: 1.01x faster                                                   |
| pidigits                 | 191 ms                                                 | 196 ms: 1.02x slower                                                   |
| unpickle                 | 14.4 us                                                | 15.5 us: 1.08x slower                                                  |
| pickle                   | 10.7 us                                                | 11.6 us: 1.09x slower                                                  |
| telco                    | 7.27 ms                                                | 8.34 ms: 1.15x slower                                                  |
| gc_traversal             | 3.62 ms                                                | 4.16 ms: 1.15x slower                                                  |
| pickle_dict              | 29.6 us                                                | 34.3 us: 1.16x slower                                                  |
| coverage                 | 79.4 ms                                                | 95.4 ms: 1.20x slower                                                  |
| python_startup_no_site   | 5.93 ms                                                | 9.01 ms: 1.52x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.35x faster                                                           |

Benchmark hidden because not significant (5): mypy2, async_generators, bench_mp_pool, pickle_list, regex_effbot
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231201-3.13.0a2+-05a370a/bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.31x
- 95% likely to have a speedup of 1.30x
- 99% likely to have a speedup of 1.28x


# Memory

- memory change: 1.05x