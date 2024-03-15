
# Results vs. 3.10.4

- fork: python
- ref: 35ef8cb25917bfd6cbbd
- machine: linux-x86_64
- commit hash: 35ef8cb
- commit date: 2024-01-04
- overall geometric mean: 1.25x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.17x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 285 ms: 1.22x faster                                                   |
| chameleon      | 9.68 ms                                                | 7.27 ms: 1.33x faster                                                  |
| docutils       | 3.30 sec                                               | 2.72 sec: 1.21x faster                                                 |
| tornado_http   | 136 ms                                                 | 98.2 ms: 1.39x faster                                                  |
| Geometric mean | (ref)                                                  | 1.29x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 456 ms: 1.60x faster                                                   |
| async_tree_memoization  | 870 ms                                                 | 583 ms: 1.49x faster                                                   |
| async_tree_io           | 1.77 sec                                               | 1.21 sec: 1.46x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 724 ms: 1.40x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.49x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| float          | 117 ms                                                 | 94.0 ms: 1.25x faster                                                  |
| nbody          | 154 ms                                                 | 126 ms: 1.21x faster                                                   |
| pidigits       | 191 ms                                                 | 190 ms: 1.01x faster                                                   |
| Geometric mean | (ref)                                                  | 1.15x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 156 ms: 1.21x faster                                                   |
| regex_v8       | 27.8 ms                                                | 24.6 ms: 1.13x faster                                                  |
| Geometric mean | (ref)                                                  | 1.08x faster                                                           |

Benchmark hidden because not significant (2): regex_effbot, regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 304 us: 1.59x faster                                                   |
| unpickle_pure_python | 331 us                                                 | 239 us: 1.39x faster                                                   |
| json_dumps           | 14.2 ms                                                | 10.6 ms: 1.34x faster                                                  |
| xml_etree_process    | 79.1 ms                                                | 62.0 ms: 1.28x faster                                                  |
| tomli_loads          | 3.14 sec                                               | 2.53 sec: 1.24x faster                                                 |
| json_loads           | 31.2 us                                                | 28.2 us: 1.11x faster                                                  |
| xml_etree_generate   | 99.4 ms                                                | 90.9 ms: 1.09x faster                                                  |
| xml_etree_parse      | 168 ms                                                 | 157 ms: 1.07x faster                                                   |
| xml_etree_iterparse  | 115 ms                                                 | 113 ms: 1.02x faster                                                   |
| pickle_list          | 5.08 us                                                | 5.13 us: 1.01x slower                                                  |
| unpickle             | 14.4 us                                                | 14.7 us: 1.02x slower                                                  |
| unpickle_list        | 5.20 us                                                | 5.39 us: 1.04x slower                                                  |
| pickle               | 10.7 us                                                | 11.6 us: 1.08x slower                                                  |
| pickle_dict          | 29.6 us                                                | 35.1 us: 1.19x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.11x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                  |
| python_startup_no_site | 5.93 ms                                                | 8.77 ms: 1.48x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 14.7 ms: 1.11x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 117 us: 4.66x faster                                                   |
| generators               | 80.1 ms                                                | 29.1 ms: 2.75x faster                                                  |
| asyncio_tcp              | 922 ms                                                 | 494 ms: 1.87x faster                                                   |
| logging_silent           | 190 ns                                                 | 108 ns: 1.76x faster                                                   |
| richards_super           | 94.7 ms                                                | 56.0 ms: 1.69x faster                                                  |
| raytrace                 | 507 ms                                                 | 304 ms: 1.67x faster                                                   |
| scimark_sor              | 220 ms                                                 | 132 ms: 1.67x faster                                                   |
| deltablue                | 7.91 ms                                                | 4.87 ms: 1.62x faster                                                  |
| sqlglot_parse            | 2.17 ms                                                | 1.34 ms: 1.62x faster                                                  |
| async_tree_none          | 728 ms                                                 | 456 ms: 1.60x faster                                                   |
| richards                 | 79.3 ms                                                | 49.7 ms: 1.59x faster                                                  |
| pickle_pure_python       | 484 us                                                 | 304 us: 1.59x faster                                                   |
| coroutines               | 35.1 ms                                                | 22.5 ms: 1.56x faster                                                  |
| sqlglot_transpile        | 2.57 ms                                                | 1.68 ms: 1.53x faster                                                  |
| chaos                    | 115 ms                                                 | 76.0 ms: 1.52x faster                                                  |
| go                       | 240 ms                                                 | 161 ms: 1.49x faster                                                   |
| async_tree_memoization   | 870 ms                                                 | 583 ms: 1.49x faster                                                   |
| scimark_lu               | 176 ms                                                 | 119 ms: 1.48x faster                                                   |
| crypto_pyaes             | 128 ms                                                 | 87.4 ms: 1.46x faster                                                  |
| async_tree_io            | 1.77 sec                                               | 1.21 sec: 1.46x faster                                                 |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                  |
| unpack_sequence          | 60.0 ns                                                | 41.7 ns: 1.44x faster                                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.81 sec: 1.42x faster                                                 |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 724 ms: 1.40x faster                                                   |
| deepcopy_memo            | 58.5 us                                                | 41.9 us: 1.39x faster                                                  |
| scimark_monte_carlo      | 118 ms                                                 | 84.8 ms: 1.39x faster                                                  |
| tornado_http             | 136 ms                                                 | 98.2 ms: 1.39x faster                                                  |
| unpickle_pure_python     | 331 us                                                 | 239 us: 1.39x faster                                                   |
| logging_simple           | 8.30 us                                                | 6.08 us: 1.36x faster                                                  |
| json_dumps               | 14.2 ms                                                | 10.6 ms: 1.34x faster                                                  |
| logging_format           | 9.09 us                                                | 6.80 us: 1.34x faster                                                  |
| chameleon                | 9.68 ms                                                | 7.27 ms: 1.33x faster                                                  |
| deepcopy                 | 479 us                                                 | 360 us: 1.33x faster                                                   |
| pycparser                | 1.58 sec                                               | 1.19 sec: 1.32x faster                                                 |
| deepcopy_reduce          | 4.17 us                                                | 3.16 us: 1.32x faster                                                  |
| pyflate                  | 716 ms                                                 | 554 ms: 1.29x faster                                                   |
| comprehensions           | 28.8 us                                                | 22.5 us: 1.28x faster                                                  |
| xml_etree_process        | 79.1 ms                                                | 62.0 ms: 1.28x faster                                                  |
| float                    | 117 ms                                                 | 94.0 ms: 1.25x faster                                                  |
| tomli_loads              | 3.14 sec                                               | 2.53 sec: 1.24x faster                                                 |
| sqlglot_normalize        | 143 ms                                                 | 116 ms: 1.23x faster                                                   |
| 2to3                     | 348 ms                                                 | 285 ms: 1.22x faster                                                   |
| dulwich_log              | 84.3 ms                                                | 68.9 ms: 1.22x faster                                                  |
| pprint_safe_repr         | 1.02 sec                                               | 836 ms: 1.22x faster                                                   |
| nbody                    | 154 ms                                                 | 126 ms: 1.21x faster                                                   |
| docutils                 | 3.30 sec                                               | 2.72 sec: 1.21x faster                                                 |
| pprint_pformat           | 2.10 sec                                               | 1.74 sec: 1.21x faster                                                 |
| regex_compile            | 188 ms                                                 | 156 ms: 1.21x faster                                                   |
| sympy_sum                | 196 ms                                                 | 163 ms: 1.20x faster                                                   |
| dask                     | 441 ms                                                 | 367 ms: 1.20x faster                                                   |
| sympy_integrate          | 25.8 ms                                                | 21.6 ms: 1.19x faster                                                  |
| sqlglot_optimize         | 69.2 ms                                                | 58.9 ms: 1.17x faster                                                  |
| sympy_str                | 346 ms                                                 | 298 ms: 1.16x faster                                                   |
| bench_thread_pool        | 986 us                                                 | 854 us: 1.16x faster                                                   |
| hexiom                   | 10.4 ms                                                | 9.02 ms: 1.15x faster                                                  |
| regex_v8                 | 27.8 ms                                                | 24.6 ms: 1.13x faster                                                  |
| sympy_expand             | 566 ms                                                 | 505 ms: 1.12x faster                                                   |
| mako                     | 16.3 ms                                                | 14.7 ms: 1.11x faster                                                  |
| fannkuch                 | 532 ms                                                 | 477 ms: 1.11x faster                                                   |
| json_loads               | 31.2 us                                                | 28.2 us: 1.11x faster                                                  |
| create_gc_cycles         | 1.62 ms                                                | 1.47 ms: 1.10x faster                                                  |
| xml_etree_generate       | 99.4 ms                                                | 90.9 ms: 1.09x faster                                                  |
| spectral_norm            | 170 ms                                                 | 157 ms: 1.08x faster                                                   |
| json                     | 5.69 ms                                                | 5.25 ms: 1.08x faster                                                  |
| pathlib                  | 20.5 ms                                                | 18.9 ms: 1.08x faster                                                  |
| xml_etree_parse          | 168 ms                                                 | 157 ms: 1.07x faster                                                   |
| mdp                      | 2.85 sec                                               | 2.66 sec: 1.07x faster                                                 |
| nqueens                  | 106 ms                                                 | 101 ms: 1.05x faster                                                   |
| sqlite_synth             | 3.02 us                                                | 2.92 us: 1.04x faster                                                  |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 6.30 ms: 1.03x faster                                                  |
| xml_etree_iterparse      | 115 ms                                                 | 113 ms: 1.02x faster                                                   |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                   |
| pidigits                 | 191 ms                                                 | 190 ms: 1.01x faster                                                   |
| meteor_contest           | 120 ms                                                 | 119 ms: 1.00x faster                                                   |
| pickle_list              | 5.08 us                                                | 5.13 us: 1.01x slower                                                  |
| scimark_fft              | 466 ms                                                 | 472 ms: 1.01x slower                                                   |
| unpickle                 | 14.4 us                                                | 14.7 us: 1.02x slower                                                  |
| async_generators         | 444 ms                                                 | 453 ms: 1.02x slower                                                   |
| unpickle_list            | 5.20 us                                                | 5.39 us: 1.04x slower                                                  |
| gc_traversal             | 3.62 ms                                                | 3.83 ms: 1.06x slower                                                  |
| pickle                   | 10.7 us                                                | 11.6 us: 1.08x slower                                                  |
| pickle_dict              | 29.6 us                                                | 35.1 us: 1.19x slower                                                  |
| coverage                 | 79.4 ms                                                | 94.7 ms: 1.19x slower                                                  |
| telco                    | 7.27 ms                                                | 8.88 ms: 1.22x slower                                                  |
| python_startup_no_site   | 5.93 ms                                                | 8.77 ms: 1.48x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.25x faster                                                           |

Benchmark hidden because not significant (4): mypy2, regex_effbot, bench_mp_pool, regex_dna
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240104-3.13.0a2+-35ef8cb-PYTHON_UOPS/bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.20x
- 95% likely to have a speedup of 1.20x
- 99% likely to have a speedup of 1.17x


# Memory

- memory change: 1.06x