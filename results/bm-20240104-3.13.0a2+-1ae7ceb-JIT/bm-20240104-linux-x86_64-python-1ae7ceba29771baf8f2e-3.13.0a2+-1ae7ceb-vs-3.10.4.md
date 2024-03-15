
# Results vs. 3.10.4

- fork: python
- ref: 1ae7ceba29771baf8f2e
- machine: linux-x86_64
- commit hash: 1ae7ceb
- commit date: 2024-01-04
- overall geometric mean: 1.36x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.28x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 264 ms: 1.32x faster                                                   |
| chameleon      | 9.68 ms                                                | 6.90 ms: 1.40x faster                                                  |
| docutils       | 3.30 sec                                               | 2.59 sec: 1.27x faster                                                 |
| tornado_http   | 136 ms                                                 | 94.1 ms: 1.45x faster                                                  |
| Geometric mean | (ref)                                                  | 1.36x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 434 ms: 1.68x faster                                                   |
| async_tree_memoization  | 870 ms                                                 | 559 ms: 1.56x faster                                                   |
| async_tree_io           | 1.77 sec                                               | 1.17 sec: 1.51x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 706 ms: 1.44x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.54x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 87.4 ms: 1.76x faster                                                  |
| float          | 117 ms                                                 | 79.7 ms: 1.47x faster                                                  |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                                   |
| Geometric mean | (ref)                                                  | 1.38x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 130 ms: 1.45x faster                                                   |
| regex_v8       | 27.8 ms                                                | 25.0 ms: 1.11x faster                                                  |
| regex_dna      | 227 ms                                                 | 223 ms: 1.02x faster                                                   |
| Geometric mean | (ref)                                                  | 1.13x faster                                                           |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 302 us: 1.60x faster                                                   |
| unpickle_pure_python | 331 us                                                 | 216 us: 1.53x faster                                                   |
| tomli_loads          | 3.14 sec                                               | 2.13 sec: 1.48x faster                                                 |
| xml_etree_process    | 79.1 ms                                                | 58.6 ms: 1.35x faster                                                  |
| json_dumps           | 14.2 ms                                                | 10.5 ms: 1.34x faster                                                  |
| xml_etree_generate   | 99.4 ms                                                | 85.1 ms: 1.17x faster                                                  |
| json_loads           | 31.2 us                                                | 28.1 us: 1.11x faster                                                  |
| xml_etree_iterparse  | 115 ms                                                 | 105 ms: 1.10x faster                                                   |
| xml_etree_parse      | 168 ms                                                 | 157 ms: 1.07x faster                                                   |
| unpickle_list        | 5.20 us                                                | 5.05 us: 1.03x faster                                                  |
| pickle_list          | 5.08 us                                                | 5.20 us: 1.02x slower                                                  |
| unpickle             | 14.4 us                                                | 14.9 us: 1.04x slower                                                  |
| pickle               | 10.7 us                                                | 11.7 us: 1.10x slower                                                  |
| pickle_dict          | 29.6 us                                                | 35.5 us: 1.20x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.15x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.45x faster                                                  |
| python_startup_no_site | 5.93 ms                                                | 8.71 ms: 1.47x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.2 ms: 1.46x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 111 us: 4.92x faster                                                   |
| generators               | 80.1 ms                                                | 29.4 ms: 2.72x faster                                                  |
| deltablue                | 7.91 ms                                                | 3.26 ms: 2.43x faster                                                  |
| chaos                    | 115 ms                                                 | 58.9 ms: 1.96x faster                                                  |
| raytrace                 | 507 ms                                                 | 262 ms: 1.94x faster                                                   |
| asyncio_tcp              | 922 ms                                                 | 480 ms: 1.92x faster                                                   |
| logging_silent           | 190 ns                                                 | 102 ns: 1.87x faster                                                   |
| crypto_pyaes             | 128 ms                                                 | 70.0 ms: 1.82x faster                                                  |
| comprehensions           | 28.8 us                                                | 16.0 us: 1.80x faster                                                  |
| nbody                    | 154 ms                                                 | 87.4 ms: 1.76x faster                                                  |
| scimark_monte_carlo      | 118 ms                                                 | 67.6 ms: 1.75x faster                                                  |
| sqlglot_parse            | 2.17 ms                                                | 1.25 ms: 1.74x faster                                                  |
| go                       | 240 ms                                                 | 139 ms: 1.73x faster                                                   |
| richards_super           | 94.7 ms                                                | 55.0 ms: 1.72x faster                                                  |
| scimark_sor              | 220 ms                                                 | 128 ms: 1.71x faster                                                   |
| hexiom                   | 10.4 ms                                                | 6.07 ms: 1.71x faster                                                  |
| async_tree_none          | 728 ms                                                 | 434 ms: 1.68x faster                                                   |
| richards                 | 79.3 ms                                                | 48.3 ms: 1.64x faster                                                  |
| sqlglot_transpile        | 2.57 ms                                                | 1.57 ms: 1.64x faster                                                  |
| pickle_pure_python       | 484 us                                                 | 302 us: 1.60x faster                                                   |
| pyflate                  | 716 ms                                                 | 455 ms: 1.57x faster                                                   |
| scimark_lu               | 176 ms                                                 | 112 ms: 1.57x faster                                                   |
| coroutines               | 35.1 ms                                                | 22.4 ms: 1.57x faster                                                  |
| async_tree_memoization   | 870 ms                                                 | 559 ms: 1.56x faster                                                   |
| spectral_norm            | 170 ms                                                 | 109 ms: 1.56x faster                                                   |
| unpickle_pure_python     | 331 us                                                 | 216 us: 1.53x faster                                                   |
| deepcopy_memo            | 58.5 us                                                | 38.4 us: 1.52x faster                                                  |
| async_tree_io            | 1.77 sec                                               | 1.17 sec: 1.51x faster                                                 |
| logging_simple           | 8.30 us                                                | 5.62 us: 1.48x faster                                                  |
| tomli_loads              | 3.14 sec                                               | 2.13 sec: 1.48x faster                                                 |
| logging_format           | 9.09 us                                                | 6.18 us: 1.47x faster                                                  |
| float                    | 117 ms                                                 | 79.7 ms: 1.47x faster                                                  |
| mako                     | 16.3 ms                                                | 11.2 ms: 1.46x faster                                                  |
| regex_compile            | 188 ms                                                 | 130 ms: 1.45x faster                                                   |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.77 sec: 1.45x faster                                                 |
| tornado_http             | 136 ms                                                 | 94.1 ms: 1.45x faster                                                  |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.45x faster                                                  |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 706 ms: 1.44x faster                                                   |
| pprint_pformat           | 2.10 sec                                               | 1.48 sec: 1.42x faster                                                 |
| pprint_safe_repr         | 1.02 sec                                               | 724 ms: 1.41x faster                                                   |
| chameleon                | 9.68 ms                                                | 6.90 ms: 1.40x faster                                                  |
| deepcopy                 | 479 us                                                 | 344 us: 1.39x faster                                                   |
| deepcopy_reduce          | 4.17 us                                                | 3.02 us: 1.38x faster                                                  |
| unpack_sequence          | 60.0 ns                                                | 44.4 ns: 1.35x faster                                                  |
| xml_etree_process        | 79.1 ms                                                | 58.6 ms: 1.35x faster                                                  |
| json_dumps               | 14.2 ms                                                | 10.5 ms: 1.34x faster                                                  |
| fannkuch                 | 532 ms                                                 | 399 ms: 1.33x faster                                                   |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.87 ms: 1.33x faster                                                  |
| sqlglot_normalize        | 143 ms                                                 | 108 ms: 1.33x faster                                                   |
| sympy_integrate          | 25.8 ms                                                | 19.5 ms: 1.33x faster                                                  |
| sympy_sum                | 196 ms                                                 | 148 ms: 1.32x faster                                                   |
| pycparser                | 1.58 sec                                               | 1.19 sec: 1.32x faster                                                 |
| 2to3                     | 348 ms                                                 | 264 ms: 1.32x faster                                                   |
| nqueens                  | 106 ms                                                 | 80.6 ms: 1.31x faster                                                  |
| dulwich_log              | 84.3 ms                                                | 65.3 ms: 1.29x faster                                                  |
| scimark_fft              | 466 ms                                                 | 362 ms: 1.29x faster                                                   |
| sqlglot_optimize         | 69.2 ms                                                | 53.9 ms: 1.28x faster                                                  |
| docutils                 | 3.30 sec                                               | 2.59 sec: 1.27x faster                                                 |
| sympy_str                | 346 ms                                                 | 276 ms: 1.25x faster                                                   |
| dask                     | 441 ms                                                 | 359 ms: 1.23x faster                                                   |
| sympy_expand             | 566 ms                                                 | 465 ms: 1.22x faster                                                   |
| bench_thread_pool        | 986 us                                                 | 827 us: 1.19x faster                                                   |
| xml_etree_generate       | 99.4 ms                                                | 85.1 ms: 1.17x faster                                                  |
| mdp                      | 2.85 sec                                               | 2.53 sec: 1.13x faster                                                 |
| pathlib                  | 20.5 ms                                                | 18.3 ms: 1.12x faster                                                  |
| json_loads               | 31.2 us                                                | 28.1 us: 1.11x faster                                                  |
| regex_v8                 | 27.8 ms                                                | 25.0 ms: 1.11x faster                                                  |
| meteor_contest           | 120 ms                                                 | 108 ms: 1.11x faster                                                   |
| xml_etree_iterparse      | 115 ms                                                 | 105 ms: 1.10x faster                                                   |
| create_gc_cycles         | 1.62 ms                                                | 1.47 ms: 1.10x faster                                                  |
| json                     | 5.69 ms                                                | 5.18 ms: 1.10x faster                                                  |
| xml_etree_parse          | 168 ms                                                 | 157 ms: 1.07x faster                                                   |
| sqlite_synth             | 3.02 us                                                | 2.85 us: 1.06x faster                                                  |
| unpickle_list            | 5.20 us                                                | 5.05 us: 1.03x faster                                                  |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                                   |
| regex_dna                | 227 ms                                                 | 223 ms: 1.02x faster                                                   |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                   |
| async_generators         | 444 ms                                                 | 439 ms: 1.01x faster                                                   |
| gc_traversal             | 3.62 ms                                                | 3.69 ms: 1.02x slower                                                  |
| pickle_list              | 5.08 us                                                | 5.20 us: 1.02x slower                                                  |
| unpickle                 | 14.4 us                                                | 14.9 us: 1.04x slower                                                  |
| pickle                   | 10.7 us                                                | 11.7 us: 1.10x slower                                                  |
| telco                    | 7.27 ms                                                | 8.35 ms: 1.15x slower                                                  |
| coverage                 | 79.4 ms                                                | 95.0 ms: 1.20x slower                                                  |
| pickle_dict              | 29.6 us                                                | 35.5 us: 1.20x slower                                                  |
| python_startup_no_site   | 5.93 ms                                                | 8.71 ms: 1.47x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.36x faster                                                           |

Benchmark hidden because not significant (3): mypy2, bench_mp_pool, regex_effbot
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240104-3.13.0a2+-1ae7ceb-JIT/bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.31x
- 95% likely to have a speedup of 1.30x
- 99% likely to have a speedup of 1.28x


# Memory

- memory change: 1.06x