# Results vs. 3.10.4

- fork: python
- ref: ffed8d985b57a97def2e
- machine: linux-x86_64
- commit hash: ffed8d9
- commit date: 2024-03-04
- overall geometric mean: 1.31x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.23x faster
- Memory change: 1.33x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 276 ms: 1.26x faster                                                   |
| chameleon      | 9.68 ms                                                | 6.76 ms: 1.43x faster                                                  |
| docutils       | 3.30 sec                                               | 2.70 sec: 1.22x faster                                                 |
| tornado_http   | 136 ms                                                 | 97.0 ms: 1.41x faster                                                  |
| Geometric mean | (ref)                                                  | 1.33x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 437 ms: 1.67x faster                                                   |
| async_tree_memoization  | 870 ms                                                 | 561 ms: 1.55x faster                                                   |
| async_tree_io           | 1.77 sec                                               | 1.18 sec: 1.50x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 709 ms: 1.43x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.54x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 95.4 ms: 1.61x faster                                                  |
| float          | 117 ms                                                 | 79.2 ms: 1.48x faster                                                  |
| pidigits       | 191 ms                                                 | 188 ms: 1.02x faster                                                   |
| Geometric mean | (ref)                                                  | 1.34x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 143 ms: 1.32x faster                                                   |
| regex_v8       | 27.8 ms                                                | 25.2 ms: 1.10x faster                                                  |
| regex_dna      | 227 ms                                                 | 226 ms: 1.00x faster                                                   |
| Geometric mean | (ref)                                                  | 1.10x faster                                                           |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 305 us: 1.59x faster                                                   |
| tomli_loads          | 3.14 sec                                               | 2.02 sec: 1.56x faster                                                 |
| unpickle_pure_python | 331 us                                                 | 233 us: 1.42x faster                                                   |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.37x faster                                                  |
| xml_etree_process    | 79.1 ms                                                | 58.7 ms: 1.35x faster                                                  |
| xml_etree_generate   | 99.4 ms                                                | 86.2 ms: 1.15x faster                                                  |
| json_loads           | 31.2 us                                                | 27.4 us: 1.14x faster                                                  |
| xml_etree_iterparse  | 115 ms                                                 | 106 ms: 1.09x faster                                                   |
| xml_etree_parse      | 168 ms                                                 | 156 ms: 1.08x faster                                                   |
| unpickle_list        | 5.20 us                                                | 4.90 us: 1.06x faster                                                  |
| pickle_list          | 5.08 us                                                | 5.16 us: 1.02x slower                                                  |
| unpickle             | 14.4 us                                                | 14.9 us: 1.04x slower                                                  |
| pickle               | 10.7 us                                                | 11.8 us: 1.11x slower                                                  |
| pickle_dict          | 29.6 us                                                | 34.9 us: 1.18x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.16x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 12.3 ms: 1.19x faster                                                  |
| python_startup_no_site | 5.93 ms                                                | 10.9 ms: 1.84x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.25x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 10.8 ms: 1.51x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 110 us: 4.93x faster                                                   |
| generators               | 80.1 ms                                                | 29.4 ms: 2.72x faster                                                  |
| deltablue                | 7.91 ms                                                | 3.38 ms: 2.34x faster                                                  |
| asyncio_tcp              | 922 ms                                                 | 479 ms: 1.92x faster                                                   |
| logging_silent           | 190 ns                                                 | 101 ns: 1.89x faster                                                   |
| chaos                    | 115 ms                                                 | 62.4 ms: 1.85x faster                                                  |
| richards_super           | 94.7 ms                                                | 52.2 ms: 1.82x faster                                                  |
| raytrace                 | 507 ms                                                 | 288 ms: 1.76x faster                                                   |
| scimark_sor              | 220 ms                                                 | 127 ms: 1.73x faster                                                   |
| richards                 | 79.3 ms                                                | 45.8 ms: 1.73x faster                                                  |
| crypto_pyaes             | 128 ms                                                 | 73.9 ms: 1.73x faster                                                  |
| comprehensions           | 28.8 us                                                | 17.0 us: 1.69x faster                                                  |
| sqlglot_parse            | 2.17 ms                                                | 1.29 ms: 1.68x faster                                                  |
| scimark_monte_carlo      | 118 ms                                                 | 70.6 ms: 1.67x faster                                                  |
| async_tree_none          | 728 ms                                                 | 437 ms: 1.67x faster                                                   |
| nbody                    | 154 ms                                                 | 95.4 ms: 1.61x faster                                                  |
| pickle_pure_python       | 484 us                                                 | 305 us: 1.59x faster                                                   |
| sqlglot_transpile        | 2.57 ms                                                | 1.63 ms: 1.58x faster                                                  |
| tomli_loads              | 3.14 sec                                               | 2.02 sec: 1.56x faster                                                 |
| async_tree_memoization   | 870 ms                                                 | 561 ms: 1.55x faster                                                   |
| coroutines               | 35.1 ms                                                | 22.7 ms: 1.55x faster                                                  |
| go                       | 240 ms                                                 | 156 ms: 1.54x faster                                                   |
| pyflate                  | 716 ms                                                 | 469 ms: 1.53x faster                                                   |
| spectral_norm            | 170 ms                                                 | 112 ms: 1.51x faster                                                   |
| mako                     | 16.3 ms                                                | 10.8 ms: 1.51x faster                                                  |
| deepcopy_memo            | 58.5 us                                                | 38.9 us: 1.50x faster                                                  |
| async_tree_io            | 1.77 sec                                               | 1.18 sec: 1.50x faster                                                 |
| hexiom                   | 10.4 ms                                                | 6.95 ms: 1.50x faster                                                  |
| float                    | 117 ms                                                 | 79.2 ms: 1.48x faster                                                  |
| logging_simple           | 8.30 us                                                | 5.67 us: 1.47x faster                                                  |
| logging_format           | 9.09 us                                                | 6.23 us: 1.46x faster                                                  |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 709 ms: 1.43x faster                                                   |
| chameleon                | 9.68 ms                                                | 6.76 ms: 1.43x faster                                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                                 |
| unpickle_pure_python     | 331 us                                                 | 233 us: 1.42x faster                                                   |
| tornado_http             | 136 ms                                                 | 97.0 ms: 1.41x faster                                                  |
| deepcopy                 | 479 us                                                 | 350 us: 1.37x faster                                                   |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.37x faster                                                  |
| pprint_safe_repr         | 1.02 sec                                               | 745 ms: 1.37x faster                                                   |
| pprint_pformat           | 2.10 sec                                               | 1.54 sec: 1.37x faster                                                 |
| scimark_fft              | 466 ms                                                 | 341 ms: 1.36x faster                                                   |
| deepcopy_reduce          | 4.17 us                                                | 3.06 us: 1.36x faster                                                  |
| fannkuch                 | 532 ms                                                 | 392 ms: 1.36x faster                                                   |
| scimark_lu               | 176 ms                                                 | 130 ms: 1.35x faster                                                   |
| xml_etree_process        | 79.1 ms                                                | 58.7 ms: 1.35x faster                                                  |
| sqlglot_normalize        | 143 ms                                                 | 106 ms: 1.35x faster                                                   |
| regex_compile            | 188 ms                                                 | 143 ms: 1.32x faster                                                   |
| pycparser                | 1.58 sec                                               | 1.20 sec: 1.31x faster                                                 |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.01 ms: 1.29x faster                                                  |
| 2to3                     | 348 ms                                                 | 276 ms: 1.26x faster                                                   |
| sympy_sum                | 196 ms                                                 | 157 ms: 1.25x faster                                                   |
| sqlglot_optimize         | 69.2 ms                                                | 55.6 ms: 1.24x faster                                                  |
| dulwich_log              | 84.3 ms                                                | 68.1 ms: 1.24x faster                                                  |
| sympy_integrate          | 25.8 ms                                                | 20.9 ms: 1.24x faster                                                  |
| sympy_str                | 346 ms                                                 | 280 ms: 1.24x faster                                                   |
| docutils                 | 3.30 sec                                               | 2.70 sec: 1.22x faster                                                 |
| sympy_expand             | 566 ms                                                 | 475 ms: 1.19x faster                                                   |
| python_startup           | 14.6 ms                                                | 12.3 ms: 1.19x faster                                                  |
| nqueens                  | 106 ms                                                 | 90.2 ms: 1.17x faster                                                  |
| bench_thread_pool        | 986 us                                                 | 846 us: 1.17x faster                                                   |
| xml_etree_generate       | 99.4 ms                                                | 86.2 ms: 1.15x faster                                                  |
| json_loads               | 31.2 us                                                | 27.4 us: 1.14x faster                                                  |
| json                     | 5.69 ms                                                | 5.03 ms: 1.13x faster                                                  |
| pathlib                  | 20.5 ms                                                | 18.3 ms: 1.12x faster                                                  |
| meteor_contest           | 120 ms                                                 | 107 ms: 1.11x faster                                                   |
| regex_v8                 | 27.8 ms                                                | 25.2 ms: 1.10x faster                                                  |
| mdp                      | 2.85 sec                                               | 2.61 sec: 1.09x faster                                                 |
| xml_etree_iterparse      | 115 ms                                                 | 106 ms: 1.09x faster                                                   |
| sqlite_synth             | 3.02 us                                                | 2.79 us: 1.08x faster                                                  |
| create_gc_cycles         | 1.62 ms                                                | 1.50 ms: 1.08x faster                                                  |
| xml_etree_parse          | 168 ms                                                 | 156 ms: 1.08x faster                                                   |
| unpickle_list            | 5.20 us                                                | 4.90 us: 1.06x faster                                                  |
| pidigits                 | 191 ms                                                 | 188 ms: 1.02x faster                                                   |
| asyncio_websockets       | 559 ms                                                 | 554 ms: 1.01x faster                                                   |
| regex_dna                | 227 ms                                                 | 226 ms: 1.00x faster                                                   |
| pickle_list              | 5.08 us                                                | 5.16 us: 1.02x slower                                                  |
| unpickle                 | 14.4 us                                                | 14.9 us: 1.04x slower                                                  |
| async_generators         | 444 ms                                                 | 462 ms: 1.04x slower                                                   |
| pickle                   | 10.7 us                                                | 11.8 us: 1.11x slower                                                  |
| gc_traversal             | 3.62 ms                                                | 4.03 ms: 1.11x slower                                                  |
| telco                    | 7.27 ms                                                | 8.45 ms: 1.16x slower                                                  |
| bench_mp_pool            | 24.0 ms                                                | 28.0 ms: 1.16x slower                                                  |
| pickle_dict              | 29.6 us                                                | 34.9 us: 1.18x slower                                                  |
| dask                     | 441 ms                                                 | 532 ms: 1.21x slower                                                   |
| coverage                 | 79.4 ms                                                | 97.0 ms: 1.22x slower                                                  |
| unpack_sequence          | 60.0 ns                                                | 85.0 ns: 1.42x slower                                                  |
| python_startup_no_site   | 5.93 ms                                                | 10.9 ms: 1.84x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.31x faster                                                           |

Benchmark hidden because not significant (2): mypy2, regex_effbot
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240304-3.13.0a4+-ffed8d9-JIT/bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.26x
- 95% likely to have a speedup of 1.25x
- 99% likely to have a speedup of 1.23x


# Memory

- memory change: 1.33x