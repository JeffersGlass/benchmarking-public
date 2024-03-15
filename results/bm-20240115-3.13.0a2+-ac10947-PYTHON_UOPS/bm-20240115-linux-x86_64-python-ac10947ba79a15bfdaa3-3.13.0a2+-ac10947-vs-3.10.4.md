
# Results vs. 3.10.4

- fork: python
- ref: ac10947ba79a15bfdaa3
- machine: linux-x86_64
- commit hash: ac10947
- commit date: 2024-01-15
- overall geometric mean: 1.24x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.17x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 284 ms: 1.23x faster                                                   |
| chameleon      | 9.68 ms                                                | 7.37 ms: 1.31x faster                                                  |
| docutils       | 3.30 sec                                               | 2.72 sec: 1.21x faster                                                 |
| tornado_http   | 136 ms                                                 | 97.7 ms: 1.40x faster                                                  |
| Geometric mean | (ref)                                                  | 1.28x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 450 ms: 1.62x faster                                                   |
| async_tree_memoization  | 870 ms                                                 | 577 ms: 1.51x faster                                                   |
| async_tree_io           | 1.77 sec                                               | 1.21 sec: 1.47x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 721 ms: 1.41x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.50x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 131 ms: 1.17x faster                                                   |
| float          | 117 ms                                                 | 100 ms: 1.17x faster                                                   |
| pidigits       | 191 ms                                                 | 197 ms: 1.03x slower                                                   |
| Geometric mean | (ref)                                                  | 1.10x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 156 ms: 1.21x faster                                                   |
| regex_v8       | 27.8 ms                                                | 24.9 ms: 1.12x faster                                                  |
| regex_dna      | 227 ms                                                 | 223 ms: 1.02x faster                                                   |
| Geometric mean | (ref)                                                  | 1.08x faster                                                           |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 302 us: 1.61x faster                                                   |
| unpickle_pure_python | 331 us                                                 | 240 us: 1.38x faster                                                   |
| json_dumps           | 14.2 ms                                                | 10.7 ms: 1.33x faster                                                  |
| xml_etree_process    | 79.1 ms                                                | 61.8 ms: 1.28x faster                                                  |
| tomli_loads          | 3.14 sec                                               | 2.54 sec: 1.23x faster                                                 |
| xml_etree_generate   | 99.4 ms                                                | 90.4 ms: 1.10x faster                                                  |
| json_loads           | 31.2 us                                                | 28.5 us: 1.10x faster                                                  |
| xml_etree_parse      | 168 ms                                                 | 157 ms: 1.07x faster                                                   |
| xml_etree_iterparse  | 115 ms                                                 | 113 ms: 1.02x faster                                                   |
| unpickle             | 14.4 us                                                | 14.9 us: 1.03x slower                                                  |
| pickle_list          | 5.08 us                                                | 5.32 us: 1.05x slower                                                  |
| unpickle_list        | 5.20 us                                                | 5.51 us: 1.06x slower                                                  |
| pickle               | 10.7 us                                                | 11.7 us: 1.10x slower                                                  |
| pickle_dict          | 29.6 us                                                | 34.9 us: 1.18x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.11x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.45x faster                                                  |
| python_startup_no_site | 5.93 ms                                                | 8.71 ms: 1.47x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 15.0 ms: 1.09x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 116 us: 4.70x faster                                                   |
| generators               | 80.1 ms                                                | 36.4 ms: 2.20x faster                                                  |
| asyncio_tcp              | 922 ms                                                 | 496 ms: 1.86x faster                                                   |
| logging_silent           | 190 ns                                                 | 106 ns: 1.79x faster                                                   |
| richards_super           | 94.7 ms                                                | 55.2 ms: 1.72x faster                                                  |
| scimark_sor              | 220 ms                                                 | 132 ms: 1.67x faster                                                   |
| raytrace                 | 507 ms                                                 | 308 ms: 1.64x faster                                                   |
| sqlglot_parse            | 2.17 ms                                                | 1.33 ms: 1.63x faster                                                  |
| richards                 | 79.3 ms                                                | 48.9 ms: 1.62x faster                                                  |
| async_tree_none          | 728 ms                                                 | 450 ms: 1.62x faster                                                   |
| pickle_pure_python       | 484 us                                                 | 302 us: 1.61x faster                                                   |
| coroutines               | 35.1 ms                                                | 22.0 ms: 1.60x faster                                                  |
| deltablue                | 7.91 ms                                                | 5.11 ms: 1.55x faster                                                  |
| sqlglot_transpile        | 2.57 ms                                                | 1.66 ms: 1.55x faster                                                  |
| async_tree_memoization   | 870 ms                                                 | 577 ms: 1.51x faster                                                   |
| go                       | 240 ms                                                 | 160 ms: 1.50x faster                                                   |
| scimark_lu               | 176 ms                                                 | 119 ms: 1.48x faster                                                   |
| chaos                    | 115 ms                                                 | 78.2 ms: 1.48x faster                                                  |
| async_tree_io            | 1.77 sec                                               | 1.21 sec: 1.47x faster                                                 |
| crypto_pyaes             | 128 ms                                                 | 87.7 ms: 1.46x faster                                                  |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.45x faster                                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                                 |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 721 ms: 1.41x faster                                                   |
| tornado_http             | 136 ms                                                 | 97.7 ms: 1.40x faster                                                  |
| deepcopy_memo            | 58.5 us                                                | 42.4 us: 1.38x faster                                                  |
| unpickle_pure_python     | 331 us                                                 | 240 us: 1.38x faster                                                   |
| logging_simple           | 8.30 us                                                | 6.05 us: 1.37x faster                                                  |
| scimark_monte_carlo      | 118 ms                                                 | 86.2 ms: 1.37x faster                                                  |
| logging_format           | 9.09 us                                                | 6.71 us: 1.35x faster                                                  |
| deepcopy                 | 479 us                                                 | 358 us: 1.34x faster                                                   |
| deepcopy_reduce          | 4.17 us                                                | 3.13 us: 1.33x faster                                                  |
| json_dumps               | 14.2 ms                                                | 10.7 ms: 1.33x faster                                                  |
| chameleon                | 9.68 ms                                                | 7.37 ms: 1.31x faster                                                  |
| xml_etree_process        | 79.1 ms                                                | 61.8 ms: 1.28x faster                                                  |
| pyflate                  | 716 ms                                                 | 562 ms: 1.27x faster                                                   |
| pycparser                | 1.58 sec                                               | 1.25 sec: 1.26x faster                                                 |
| comprehensions           | 28.8 us                                                | 22.9 us: 1.25x faster                                                  |
| sqlglot_normalize        | 143 ms                                                 | 115 ms: 1.24x faster                                                   |
| tomli_loads              | 3.14 sec                                               | 2.54 sec: 1.23x faster                                                 |
| 2to3                     | 348 ms                                                 | 284 ms: 1.23x faster                                                   |
| dulwich_log              | 84.3 ms                                                | 69.2 ms: 1.22x faster                                                  |
| sympy_sum                | 196 ms                                                 | 162 ms: 1.21x faster                                                   |
| regex_compile            | 188 ms                                                 | 156 ms: 1.21x faster                                                   |
| docutils                 | 3.30 sec                                               | 2.72 sec: 1.21x faster                                                 |
| sympy_integrate          | 25.8 ms                                                | 21.4 ms: 1.21x faster                                                  |
| pprint_safe_repr         | 1.02 sec                                               | 845 ms: 1.20x faster                                                   |
| dask                     | 441 ms                                                 | 368 ms: 1.20x faster                                                   |
| pprint_pformat           | 2.10 sec                                               | 1.77 sec: 1.19x faster                                                 |
| sqlglot_optimize         | 69.2 ms                                                | 58.6 ms: 1.18x faster                                                  |
| nbody                    | 154 ms                                                 | 131 ms: 1.17x faster                                                   |
| sympy_str                | 346 ms                                                 | 296 ms: 1.17x faster                                                   |
| float                    | 117 ms                                                 | 100 ms: 1.17x faster                                                   |
| bench_thread_pool        | 986 us                                                 | 851 us: 1.16x faster                                                   |
| sympy_expand             | 566 ms                                                 | 493 ms: 1.15x faster                                                   |
| hexiom                   | 10.4 ms                                                | 9.08 ms: 1.15x faster                                                  |
| regex_v8                 | 27.8 ms                                                | 24.9 ms: 1.12x faster                                                  |
| fannkuch                 | 532 ms                                                 | 479 ms: 1.11x faster                                                   |
| unpack_sequence          | 60.0 ns                                                | 54.0 ns: 1.11x faster                                                  |
| create_gc_cycles         | 1.62 ms                                                | 1.47 ms: 1.10x faster                                                  |
| xml_etree_generate       | 99.4 ms                                                | 90.4 ms: 1.10x faster                                                  |
| json_loads               | 31.2 us                                                | 28.5 us: 1.10x faster                                                  |
| pathlib                  | 20.5 ms                                                | 18.7 ms: 1.10x faster                                                  |
| mako                     | 16.3 ms                                                | 15.0 ms: 1.09x faster                                                  |
| json                     | 5.69 ms                                                | 5.28 ms: 1.08x faster                                                  |
| mdp                      | 2.85 sec                                               | 2.65 sec: 1.08x faster                                                 |
| xml_etree_parse          | 168 ms                                                 | 157 ms: 1.07x faster                                                   |
| nqueens                  | 106 ms                                                 | 99.2 ms: 1.07x faster                                                  |
| spectral_norm            | 170 ms                                                 | 161 ms: 1.06x faster                                                   |
| sqlite_synth             | 3.02 us                                                | 2.88 us: 1.05x faster                                                  |
| xml_etree_iterparse      | 115 ms                                                 | 113 ms: 1.02x faster                                                   |
| meteor_contest           | 120 ms                                                 | 117 ms: 1.02x faster                                                   |
| regex_dna                | 227 ms                                                 | 223 ms: 1.02x faster                                                   |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                   |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 6.40 ms: 1.01x faster                                                  |
| gc_traversal             | 3.62 ms                                                | 3.70 ms: 1.02x slower                                                  |
| async_generators         | 444 ms                                                 | 454 ms: 1.02x slower                                                   |
| scimark_fft              | 466 ms                                                 | 480 ms: 1.03x slower                                                   |
| pidigits                 | 191 ms                                                 | 197 ms: 1.03x slower                                                   |
| unpickle                 | 14.4 us                                                | 14.9 us: 1.03x slower                                                  |
| pickle_list              | 5.08 us                                                | 5.32 us: 1.05x slower                                                  |
| unpickle_list            | 5.20 us                                                | 5.51 us: 1.06x slower                                                  |
| pickle                   | 10.7 us                                                | 11.7 us: 1.10x slower                                                  |
| pickle_dict              | 29.6 us                                                | 34.9 us: 1.18x slower                                                  |
| telco                    | 7.27 ms                                                | 8.69 ms: 1.20x slower                                                  |
| coverage                 | 79.4 ms                                                | 95.7 ms: 1.20x slower                                                  |
| python_startup_no_site   | 5.93 ms                                                | 8.71 ms: 1.47x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.24x faster                                                           |

Benchmark hidden because not significant (3): mypy2, bench_mp_pool, regex_effbot
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240115-3.13.0a2+-ac10947-PYTHON_UOPS/bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.19x
- 95% likely to have a speedup of 1.18x
- 99% likely to have a speedup of 1.17x


# Memory

- memory change: 1.06x