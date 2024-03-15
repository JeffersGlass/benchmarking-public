
# Results vs. 3.10.4

- fork: python
- ref: 2feec0fc7fd0b9caae7a
- machine: linux-x86_64
- commit hash: 2feec0f
- commit date: 2023-12-18
- overall geometric mean: 1.28x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.21x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 281 ms: 1.24x faster                                                   |
| chameleon      | 9.68 ms                                                | 7.32 ms: 1.32x faster                                                  |
| docutils       | 3.30 sec                                               | 2.71 sec: 1.22x faster                                                 |
| tornado_http   | 136 ms                                                 | 98.2 ms: 1.39x faster                                                  |
| Geometric mean | (ref)                                                  | 1.29x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 451 ms: 1.61x faster                                                   |
| async_tree_memoization  | 870 ms                                                 | 578 ms: 1.51x faster                                                   |
| async_tree_io           | 1.77 sec                                               | 1.21 sec: 1.46x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 723 ms: 1.41x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.49x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 113 ms: 1.36x faster                                                   |
| float          | 117 ms                                                 | 88.3 ms: 1.33x faster                                                  |
| pidigits       | 191 ms                                                 | 196 ms: 1.02x slower                                                   |
| Geometric mean | (ref)                                                  | 1.21x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 151 ms: 1.25x faster                                                   |
| regex_v8       | 27.8 ms                                                | 26.1 ms: 1.07x faster                                                  |
| regex_dna      | 227 ms                                                 | 216 ms: 1.05x faster                                                   |
| Geometric mean | (ref)                                                  | 1.09x faster                                                           |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 303 us: 1.60x faster                                                   |
| unpickle_pure_python | 331 us                                                 | 233 us: 1.42x faster                                                   |
| json_dumps           | 14.2 ms                                                | 10.5 ms: 1.36x faster                                                  |
| tomli_loads          | 3.14 sec                                               | 2.32 sec: 1.35x faster                                                 |
| xml_etree_process    | 79.1 ms                                                | 61.2 ms: 1.29x faster                                                  |
| json_loads           | 31.2 us                                                | 27.7 us: 1.13x faster                                                  |
| xml_etree_generate   | 99.4 ms                                                | 89.3 ms: 1.11x faster                                                  |
| xml_etree_parse      | 168 ms                                                 | 157 ms: 1.07x faster                                                   |
| xml_etree_iterparse  | 115 ms                                                 | 109 ms: 1.06x faster                                                   |
| pickle_list          | 5.08 us                                                | 5.03 us: 1.01x faster                                                  |
| unpickle_list        | 5.20 us                                                | 5.28 us: 1.02x slower                                                  |
| unpickle             | 14.4 us                                                | 14.9 us: 1.04x slower                                                  |
| pickle               | 10.7 us                                                | 11.3 us: 1.06x slower                                                  |
| pickle_dict          | 29.6 us                                                | 34.0 us: 1.15x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.14x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                  |
| python_startup_no_site | 5.93 ms                                                | 8.74 ms: 1.47x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 13.5 ms: 1.21x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 115 us: 4.72x faster                                                   |
| generators               | 80.1 ms                                                | 29.8 ms: 2.69x faster                                                  |
| asyncio_tcp              | 922 ms                                                 | 495 ms: 1.86x faster                                                   |
| scimark_sor              | 220 ms                                                 | 124 ms: 1.77x faster                                                   |
| logging_silent           | 190 ns                                                 | 108 ns: 1.76x faster                                                   |
| deltablue                | 7.91 ms                                                | 4.57 ms: 1.73x faster                                                  |
| richards_super           | 94.7 ms                                                | 54.8 ms: 1.73x faster                                                  |
| raytrace                 | 507 ms                                                 | 297 ms: 1.71x faster                                                   |
| richards                 | 79.3 ms                                                | 48.4 ms: 1.64x faster                                                  |
| sqlglot_parse            | 2.17 ms                                                | 1.33 ms: 1.63x faster                                                  |
| async_tree_none          | 728 ms                                                 | 451 ms: 1.61x faster                                                   |
| chaos                    | 115 ms                                                 | 71.7 ms: 1.61x faster                                                  |
| pickle_pure_python       | 484 us                                                 | 303 us: 1.60x faster                                                   |
| sqlglot_transpile        | 2.57 ms                                                | 1.66 ms: 1.55x faster                                                  |
| coroutines               | 35.1 ms                                                | 22.6 ms: 1.55x faster                                                  |
| go                       | 240 ms                                                 | 155 ms: 1.55x faster                                                   |
| crypto_pyaes             | 128 ms                                                 | 82.5 ms: 1.55x faster                                                  |
| scimark_lu               | 176 ms                                                 | 115 ms: 1.53x faster                                                   |
| async_tree_memoization   | 870 ms                                                 | 578 ms: 1.51x faster                                                   |
| scimark_monte_carlo      | 118 ms                                                 | 79.7 ms: 1.48x faster                                                  |
| async_tree_io            | 1.77 sec                                               | 1.21 sec: 1.46x faster                                                 |
| deepcopy_memo            | 58.5 us                                                | 40.1 us: 1.46x faster                                                  |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                                 |
| unpickle_pure_python     | 331 us                                                 | 233 us: 1.42x faster                                                   |
| pyflate                  | 716 ms                                                 | 508 ms: 1.41x faster                                                   |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 723 ms: 1.41x faster                                                   |
| comprehensions           | 28.8 us                                                | 20.7 us: 1.39x faster                                                  |
| tornado_http             | 136 ms                                                 | 98.2 ms: 1.39x faster                                                  |
| logging_simple           | 8.30 us                                                | 6.02 us: 1.38x faster                                                  |
| nbody                    | 154 ms                                                 | 113 ms: 1.36x faster                                                   |
| unpack_sequence          | 60.0 ns                                                | 44.3 ns: 1.36x faster                                                  |
| json_dumps               | 14.2 ms                                                | 10.5 ms: 1.36x faster                                                  |
| deepcopy                 | 479 us                                                 | 354 us: 1.35x faster                                                   |
| tomli_loads              | 3.14 sec                                               | 2.32 sec: 1.35x faster                                                 |
| logging_format           | 9.09 us                                                | 6.81 us: 1.33x faster                                                  |
| float                    | 117 ms                                                 | 88.3 ms: 1.33x faster                                                  |
| chameleon                | 9.68 ms                                                | 7.32 ms: 1.32x faster                                                  |
| deepcopy_reduce          | 4.17 us                                                | 3.15 us: 1.32x faster                                                  |
| xml_etree_process        | 79.1 ms                                                | 61.2 ms: 1.29x faster                                                  |
| pprint_safe_repr         | 1.02 sec                                               | 798 ms: 1.28x faster                                                   |
| hexiom                   | 10.4 ms                                                | 8.15 ms: 1.27x faster                                                  |
| sqlglot_normalize        | 143 ms                                                 | 113 ms: 1.27x faster                                                   |
| pycparser                | 1.58 sec                                               | 1.25 sec: 1.26x faster                                                 |
| pprint_pformat           | 2.10 sec                                               | 1.67 sec: 1.26x faster                                                 |
| fannkuch                 | 532 ms                                                 | 426 ms: 1.25x faster                                                   |
| regex_compile            | 188 ms                                                 | 151 ms: 1.25x faster                                                   |
| 2to3                     | 348 ms                                                 | 281 ms: 1.24x faster                                                   |
| sympy_sum                | 196 ms                                                 | 160 ms: 1.23x faster                                                   |
| dulwich_log              | 84.3 ms                                                | 69.1 ms: 1.22x faster                                                  |
| sympy_integrate          | 25.8 ms                                                | 21.2 ms: 1.22x faster                                                  |
| docutils                 | 3.30 sec                                               | 2.71 sec: 1.22x faster                                                 |
| spectral_norm            | 170 ms                                                 | 140 ms: 1.21x faster                                                   |
| mako                     | 16.3 ms                                                | 13.5 ms: 1.21x faster                                                  |
| sqlglot_optimize         | 69.2 ms                                                | 57.4 ms: 1.21x faster                                                  |
| dask                     | 441 ms                                                 | 368 ms: 1.20x faster                                                   |
| sympy_str                | 346 ms                                                 | 290 ms: 1.19x faster                                                   |
| bench_thread_pool        | 986 us                                                 | 843 us: 1.17x faster                                                   |
| nqueens                  | 106 ms                                                 | 91.3 ms: 1.16x faster                                                  |
| sympy_expand             | 566 ms                                                 | 490 ms: 1.15x faster                                                   |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.72 ms: 1.13x faster                                                  |
| json_loads               | 31.2 us                                                | 27.7 us: 1.13x faster                                                  |
| create_gc_cycles         | 1.62 ms                                                | 1.45 ms: 1.11x faster                                                  |
| xml_etree_generate       | 99.4 ms                                                | 89.3 ms: 1.11x faster                                                  |
| json                     | 5.69 ms                                                | 5.17 ms: 1.10x faster                                                  |
| pathlib                  | 20.5 ms                                                | 18.7 ms: 1.09x faster                                                  |
| xml_etree_parse          | 168 ms                                                 | 157 ms: 1.07x faster                                                   |
| mdp                      | 2.85 sec                                               | 2.67 sec: 1.07x faster                                                 |
| meteor_contest           | 120 ms                                                 | 112 ms: 1.07x faster                                                   |
| regex_v8                 | 27.8 ms                                                | 26.1 ms: 1.07x faster                                                  |
| xml_etree_iterparse      | 115 ms                                                 | 109 ms: 1.06x faster                                                   |
| sqlite_synth             | 3.02 us                                                | 2.87 us: 1.05x faster                                                  |
| scimark_fft              | 466 ms                                                 | 443 ms: 1.05x faster                                                   |
| regex_dna                | 227 ms                                                 | 216 ms: 1.05x faster                                                   |
| asyncio_websockets       | 559 ms                                                 | 553 ms: 1.01x faster                                                   |
| pickle_list              | 5.08 us                                                | 5.03 us: 1.01x faster                                                  |
| unpickle_list            | 5.20 us                                                | 5.28 us: 1.02x slower                                                  |
| pidigits                 | 191 ms                                                 | 196 ms: 1.02x slower                                                   |
| async_generators         | 444 ms                                                 | 458 ms: 1.03x slower                                                   |
| unpickle                 | 14.4 us                                                | 14.9 us: 1.04x slower                                                  |
| pickle                   | 10.7 us                                                | 11.3 us: 1.06x slower                                                  |
| gc_traversal             | 3.62 ms                                                | 3.97 ms: 1.10x slower                                                  |
| pickle_dict              | 29.6 us                                                | 34.0 us: 1.15x slower                                                  |
| coverage                 | 79.4 ms                                                | 95.6 ms: 1.20x slower                                                  |
| telco                    | 7.27 ms                                                | 8.78 ms: 1.21x slower                                                  |
| python_startup_no_site   | 5.93 ms                                                | 8.74 ms: 1.47x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.28x faster                                                           |

Benchmark hidden because not significant (3): mypy2, regex_effbot, bench_mp_pool
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231218-3.13.0a2+-2feec0f-PYTHON_UOPS/bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.23x
- 95% likely to have a speedup of 1.22x
- 99% likely to have a speedup of 1.21x


# Memory

- memory change: 1.06x