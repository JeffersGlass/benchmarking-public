
# Results vs. 3.10.4

- fork: python
- ref: 2feec0fc7fd0b9caae7a
- machine: linux-x86_64
- commit hash: 2feec0f
- commit date: 2023-12-18
- overall geometric mean: 1.36x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.29x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 263 ms: 1.33x faster                                                   |
| chameleon      | 9.68 ms                                                | 6.94 ms: 1.40x faster                                                  |
| docutils       | 3.30 sec                                               | 2.64 sec: 1.25x faster                                                 |
| tornado_http   | 136 ms                                                 | 94.4 ms: 1.44x faster                                                  |
| Geometric mean | (ref)                                                  | 1.35x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 434 ms: 1.68x faster                                                   |
| async_tree_memoization  | 870 ms                                                 | 557 ms: 1.56x faster                                                   |
| async_tree_io           | 1.77 sec                                               | 1.17 sec: 1.51x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 703 ms: 1.45x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.55x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 88.9 ms: 1.73x faster                                                  |
| float          | 117 ms                                                 | 80.7 ms: 1.45x faster                                                  |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                                   |
| Geometric mean | (ref)                                                  | 1.37x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 129 ms: 1.46x faster                                                   |
| regex_v8       | 27.8 ms                                                | 23.5 ms: 1.18x faster                                                  |
| regex_dna      | 227 ms                                                 | 222 ms: 1.02x faster                                                   |
| Geometric mean | (ref)                                                  | 1.15x faster                                                           |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 297 us: 1.63x faster                                                   |
| unpickle_pure_python | 331 us                                                 | 216 us: 1.53x faster                                                   |
| tomli_loads          | 3.14 sec                                               | 2.14 sec: 1.47x faster                                                 |
| json_dumps           | 14.2 ms                                                | 10.3 ms: 1.38x faster                                                  |
| xml_etree_process    | 79.1 ms                                                | 59.7 ms: 1.32x faster                                                  |
| json_loads           | 31.2 us                                                | 27.5 us: 1.13x faster                                                  |
| xml_etree_generate   | 99.4 ms                                                | 88.2 ms: 1.13x faster                                                  |
| xml_etree_iterparse  | 115 ms                                                 | 104 ms: 1.11x faster                                                   |
| xml_etree_parse      | 168 ms                                                 | 158 ms: 1.07x faster                                                   |
| unpickle_list        | 5.20 us                                                | 5.02 us: 1.04x faster                                                  |
| pickle_list          | 5.08 us                                                | 5.01 us: 1.01x faster                                                  |
| unpickle             | 14.4 us                                                | 14.7 us: 1.02x slower                                                  |
| pickle               | 10.7 us                                                | 11.4 us: 1.07x slower                                                  |
| pickle_dict          | 29.6 us                                                | 33.9 us: 1.15x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.16x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.45x faster                                                  |
| python_startup_no_site | 5.93 ms                                                | 8.72 ms: 1.47x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.5 ms: 1.42x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 110 us: 4.95x faster                                                   |
| generators               | 80.1 ms                                                | 28.6 ms: 2.80x faster                                                  |
| deltablue                | 7.91 ms                                                | 3.19 ms: 2.48x faster                                                  |
| raytrace                 | 507 ms                                                 | 259 ms: 1.95x faster                                                   |
| chaos                    | 115 ms                                                 | 59.7 ms: 1.93x faster                                                  |
| asyncio_tcp              | 922 ms                                                 | 482 ms: 1.91x faster                                                   |
| logging_silent           | 190 ns                                                 | 102 ns: 1.86x faster                                                   |
| scimark_sor              | 220 ms                                                 | 120 ms: 1.84x faster                                                   |
| comprehensions           | 28.8 us                                                | 16.1 us: 1.79x faster                                                  |
| crypto_pyaes             | 128 ms                                                 | 71.7 ms: 1.78x faster                                                  |
| richards_super           | 94.7 ms                                                | 53.9 ms: 1.76x faster                                                  |
| go                       | 240 ms                                                 | 137 ms: 1.75x faster                                                   |
| scimark_monte_carlo      | 118 ms                                                 | 68.0 ms: 1.74x faster                                                  |
| sqlglot_parse            | 2.17 ms                                                | 1.25 ms: 1.74x faster                                                  |
| nbody                    | 154 ms                                                 | 88.9 ms: 1.73x faster                                                  |
| hexiom                   | 10.4 ms                                                | 6.05 ms: 1.72x faster                                                  |
| async_tree_none          | 728 ms                                                 | 434 ms: 1.68x faster                                                   |
| richards                 | 79.3 ms                                                | 47.4 ms: 1.67x faster                                                  |
| sqlglot_transpile        | 2.57 ms                                                | 1.57 ms: 1.64x faster                                                  |
| pickle_pure_python       | 484 us                                                 | 297 us: 1.63x faster                                                   |
| pyflate                  | 716 ms                                                 | 448 ms: 1.60x faster                                                   |
| async_tree_memoization   | 870 ms                                                 | 557 ms: 1.56x faster                                                   |
| deepcopy_memo            | 58.5 us                                                | 37.6 us: 1.56x faster                                                  |
| scimark_lu               | 176 ms                                                 | 113 ms: 1.55x faster                                                   |
| coroutines               | 35.1 ms                                                | 22.6 ms: 1.55x faster                                                  |
| spectral_norm            | 170 ms                                                 | 111 ms: 1.54x faster                                                   |
| unpickle_pure_python     | 331 us                                                 | 216 us: 1.53x faster                                                   |
| async_tree_io            | 1.77 sec                                               | 1.17 sec: 1.51x faster                                                 |
| tomli_loads              | 3.14 sec                                               | 2.14 sec: 1.47x faster                                                 |
| logging_simple           | 8.30 us                                                | 5.70 us: 1.46x faster                                                  |
| regex_compile            | 188 ms                                                 | 129 ms: 1.46x faster                                                   |
| float                    | 117 ms                                                 | 80.7 ms: 1.45x faster                                                  |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.45x faster                                                  |
| logging_format           | 9.09 us                                                | 6.28 us: 1.45x faster                                                  |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 703 ms: 1.45x faster                                                   |
| tornado_http             | 136 ms                                                 | 94.4 ms: 1.44x faster                                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.78 sec: 1.44x faster                                                 |
| mako                     | 16.3 ms                                                | 11.5 ms: 1.42x faster                                                  |
| pprint_pformat           | 2.10 sec                                               | 1.48 sec: 1.42x faster                                                 |
| pprint_safe_repr         | 1.02 sec                                               | 729 ms: 1.40x faster                                                   |
| chameleon                | 9.68 ms                                                | 6.94 ms: 1.40x faster                                                  |
| deepcopy                 | 479 us                                                 | 347 us: 1.38x faster                                                   |
| json_dumps               | 14.2 ms                                                | 10.3 ms: 1.38x faster                                                  |
| sqlglot_normalize        | 143 ms                                                 | 106 ms: 1.35x faster                                                   |
| deepcopy_reduce          | 4.17 us                                                | 3.11 us: 1.34x faster                                                  |
| 2to3                     | 348 ms                                                 | 263 ms: 1.33x faster                                                   |
| nqueens                  | 106 ms                                                 | 79.8 ms: 1.33x faster                                                  |
| xml_etree_process        | 79.1 ms                                                | 59.7 ms: 1.32x faster                                                  |
| fannkuch                 | 532 ms                                                 | 402 ms: 1.32x faster                                                   |
| sympy_integrate          | 25.8 ms                                                | 19.5 ms: 1.32x faster                                                  |
| sympy_sum                | 196 ms                                                 | 149 ms: 1.31x faster                                                   |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.92 ms: 1.31x faster                                                  |
| pycparser                | 1.58 sec                                               | 1.20 sec: 1.31x faster                                                 |
| sqlglot_optimize         | 69.2 ms                                                | 53.5 ms: 1.29x faster                                                  |
| dulwich_log              | 84.3 ms                                                | 65.5 ms: 1.29x faster                                                  |
| sympy_str                | 346 ms                                                 | 269 ms: 1.29x faster                                                   |
| unpack_sequence          | 60.0 ns                                                | 46.8 ns: 1.28x faster                                                  |
| scimark_fft              | 466 ms                                                 | 367 ms: 1.27x faster                                                   |
| docutils                 | 3.30 sec                                               | 2.64 sec: 1.25x faster                                                 |
| sympy_expand             | 566 ms                                                 | 457 ms: 1.24x faster                                                   |
| dask                     | 441 ms                                                 | 360 ms: 1.22x faster                                                   |
| bench_thread_pool        | 986 us                                                 | 828 us: 1.19x faster                                                   |
| regex_v8                 | 27.8 ms                                                | 23.5 ms: 1.18x faster                                                  |
| json_loads               | 31.2 us                                                | 27.5 us: 1.13x faster                                                  |
| pathlib                  | 20.5 ms                                                | 18.1 ms: 1.13x faster                                                  |
| json                     | 5.69 ms                                                | 5.05 ms: 1.13x faster                                                  |
| xml_etree_generate       | 99.4 ms                                                | 88.2 ms: 1.13x faster                                                  |
| mdp                      | 2.85 sec                                               | 2.53 sec: 1.13x faster                                                 |
| meteor_contest           | 120 ms                                                 | 108 ms: 1.11x faster                                                   |
| xml_etree_iterparse      | 115 ms                                                 | 104 ms: 1.11x faster                                                   |
| create_gc_cycles         | 1.62 ms                                                | 1.47 ms: 1.10x faster                                                  |
| sqlite_synth             | 3.02 us                                                | 2.83 us: 1.07x faster                                                  |
| xml_etree_parse          | 168 ms                                                 | 158 ms: 1.07x faster                                                   |
| unpickle_list            | 5.20 us                                                | 5.02 us: 1.04x faster                                                  |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                                   |
| regex_dna                | 227 ms                                                 | 222 ms: 1.02x faster                                                   |
| asyncio_websockets       | 559 ms                                                 | 551 ms: 1.01x faster                                                   |
| pickle_list              | 5.08 us                                                | 5.01 us: 1.01x faster                                                  |
| gc_traversal             | 3.62 ms                                                | 3.67 ms: 1.01x slower                                                  |
| unpickle                 | 14.4 us                                                | 14.7 us: 1.02x slower                                                  |
| pickle                   | 10.7 us                                                | 11.4 us: 1.07x slower                                                  |
| pickle_dict              | 29.6 us                                                | 33.9 us: 1.15x slower                                                  |
| telco                    | 7.27 ms                                                | 8.35 ms: 1.15x slower                                                  |
| coverage                 | 79.4 ms                                                | 96.8 ms: 1.22x slower                                                  |
| python_startup_no_site   | 5.93 ms                                                | 8.72 ms: 1.47x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.36x faster                                                           |

Benchmark hidden because not significant (4): mypy2, regex_effbot, bench_mp_pool, async_generators
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231218-3.13.0a2+-2feec0f-JIT/bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.31x
- 95% likely to have a speedup of 1.30x
- 99% likely to have a speedup of 1.29x


# Memory

- memory change: 1.06x