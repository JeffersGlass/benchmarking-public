# Results vs. 3.10.4

- fork: python
- ref: ffed8d985b57a97def2e
- machine: linux-x86_64
- commit hash: ffed8d9
- commit date: 2024-03-04
- overall geometric mean: 1.23x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.14x faster
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 293 ms: 1.19x faster                                                   |
| chameleon      | 9.68 ms                                                | 6.90 ms: 1.40x faster                                                  |
| docutils       | 3.30 sec                                               | 2.82 sec: 1.17x faster                                                 |
| tornado_http   | 136 ms                                                 | 99.7 ms: 1.37x faster                                                  |
| Geometric mean | (ref)                                                  | 1.28x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 450 ms: 1.62x faster                                                   |
| async_tree_memoization  | 870 ms                                                 | 577 ms: 1.51x faster                                                   |
| async_tree_io           | 1.77 sec                                               | 1.21 sec: 1.47x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 723 ms: 1.41x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.50x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 121 ms: 1.27x faster                                                   |
| float          | 117 ms                                                 | 95.3 ms: 1.23x faster                                                  |
| pidigits       | 191 ms                                                 | 188 ms: 1.01x faster                                                   |
| Geometric mean | (ref)                                                  | 1.16x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_v8       | 27.8 ms                                                | 24.0 ms: 1.16x faster                                                  |
| regex_compile  | 188 ms                                                 | 176 ms: 1.07x faster                                                   |
| regex_effbot   | 3.63 ms                                                | 3.45 ms: 1.05x faster                                                  |
| regex_dna      | 227 ms                                                 | 216 ms: 1.05x faster                                                   |
| Geometric mean | (ref)                                                  | 1.08x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 305 us: 1.59x faster                                                   |
| json_dumps           | 14.2 ms                                                | 10.5 ms: 1.35x faster                                                  |
| xml_etree_process    | 79.1 ms                                                | 61.5 ms: 1.29x faster                                                  |
| tomli_loads          | 3.14 sec                                               | 2.56 sec: 1.22x faster                                                 |
| unpickle_pure_python | 331 us                                                 | 282 us: 1.17x faster                                                   |
| json_loads           | 31.2 us                                                | 27.5 us: 1.13x faster                                                  |
| xml_etree_generate   | 99.4 ms                                                | 89.8 ms: 1.11x faster                                                  |
| unpickle_list        | 5.20 us                                                | 4.74 us: 1.10x faster                                                  |
| xml_etree_parse      | 168 ms                                                 | 158 ms: 1.07x faster                                                   |
| xml_etree_iterparse  | 115 ms                                                 | 111 ms: 1.04x faster                                                   |
| pickle_list          | 5.08 us                                                | 5.18 us: 1.02x slower                                                  |
| unpickle             | 14.4 us                                                | 15.7 us: 1.09x slower                                                  |
| pickle               | 10.7 us                                                | 11.8 us: 1.11x slower                                                  |
| pickle_dict          | 29.6 us                                                | 34.8 us: 1.18x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.11x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.44x faster                                                  |
| python_startup_no_site | 5.93 ms                                                | 8.81 ms: 1.48x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.02x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 13.4 ms: 1.21x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 115 us: 4.75x faster                                                   |
| generators               | 80.1 ms                                                | 29.8 ms: 2.68x faster                                                  |
| deltablue                | 7.91 ms                                                | 3.83 ms: 2.07x faster                                                  |
| asyncio_tcp              | 922 ms                                                 | 478 ms: 1.93x faster                                                   |
| logging_silent           | 190 ns                                                 | 102 ns: 1.86x faster                                                   |
| async_tree_none          | 728 ms                                                 | 450 ms: 1.62x faster                                                   |
| pickle_pure_python       | 484 us                                                 | 305 us: 1.59x faster                                                   |
| coroutines               | 35.1 ms                                                | 22.1 ms: 1.59x faster                                                  |
| chaos                    | 115 ms                                                 | 74.4 ms: 1.55x faster                                                  |
| richards_super           | 94.7 ms                                                | 61.9 ms: 1.53x faster                                                  |
| scimark_sor              | 220 ms                                                 | 144 ms: 1.52x faster                                                   |
| sqlglot_parse            | 2.17 ms                                                | 1.43 ms: 1.51x faster                                                  |
| async_tree_memoization   | 870 ms                                                 | 577 ms: 1.51x faster                                                   |
| crypto_pyaes             | 128 ms                                                 | 85.5 ms: 1.50x faster                                                  |
| raytrace                 | 507 ms                                                 | 340 ms: 1.49x faster                                                   |
| async_tree_io            | 1.77 sec                                               | 1.21 sec: 1.47x faster                                                 |
| sqlglot_transpile        | 2.57 ms                                                | 1.78 ms: 1.44x faster                                                  |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.44x faster                                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                                 |
| deepcopy_memo            | 58.5 us                                                | 41.4 us: 1.41x faster                                                  |
| richards                 | 79.3 ms                                                | 56.2 ms: 1.41x faster                                                  |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 723 ms: 1.41x faster                                                   |
| chameleon                | 9.68 ms                                                | 6.90 ms: 1.40x faster                                                  |
| tornado_http             | 136 ms                                                 | 99.7 ms: 1.37x faster                                                  |
| go                       | 240 ms                                                 | 177 ms: 1.36x faster                                                   |
| logging_simple           | 8.30 us                                                | 6.15 us: 1.35x faster                                                  |
| json_dumps               | 14.2 ms                                                | 10.5 ms: 1.35x faster                                                  |
| deepcopy                 | 479 us                                                 | 357 us: 1.34x faster                                                   |
| deepcopy_reduce          | 4.17 us                                                | 3.14 us: 1.33x faster                                                  |
| comprehensions           | 28.8 us                                                | 21.7 us: 1.32x faster                                                  |
| logging_format           | 9.09 us                                                | 6.91 us: 1.32x faster                                                  |
| xml_etree_process        | 79.1 ms                                                | 61.5 ms: 1.29x faster                                                  |
| scimark_monte_carlo      | 118 ms                                                 | 92.0 ms: 1.28x faster                                                  |
| sqlglot_normalize        | 143 ms                                                 | 112 ms: 1.28x faster                                                   |
| nbody                    | 154 ms                                                 | 121 ms: 1.27x faster                                                   |
| pycparser                | 1.58 sec                                               | 1.27 sec: 1.24x faster                                                 |
| float                    | 117 ms                                                 | 95.3 ms: 1.23x faster                                                  |
| tomli_loads              | 3.14 sec                                               | 2.56 sec: 1.22x faster                                                 |
| pyflate                  | 716 ms                                                 | 589 ms: 1.22x faster                                                   |
| sympy_integrate          | 25.8 ms                                                | 21.3 ms: 1.21x faster                                                  |
| spectral_norm            | 170 ms                                                 | 140 ms: 1.21x faster                                                   |
| mako                     | 16.3 ms                                                | 13.4 ms: 1.21x faster                                                  |
| sympy_sum                | 196 ms                                                 | 164 ms: 1.20x faster                                                   |
| 2to3                     | 348 ms                                                 | 293 ms: 1.19x faster                                                   |
| unpickle_pure_python     | 331 us                                                 | 282 us: 1.17x faster                                                   |
| docutils                 | 3.30 sec                                               | 2.82 sec: 1.17x faster                                                 |
| dulwich_log              | 84.3 ms                                                | 72.6 ms: 1.16x faster                                                  |
| pprint_safe_repr         | 1.02 sec                                               | 877 ms: 1.16x faster                                                   |
| regex_v8                 | 27.8 ms                                                | 24.0 ms: 1.16x faster                                                  |
| sympy_str                | 346 ms                                                 | 299 ms: 1.15x faster                                                   |
| bench_thread_pool        | 986 us                                                 | 858 us: 1.15x faster                                                   |
| pprint_pformat           | 2.10 sec                                               | 1.83 sec: 1.15x faster                                                 |
| sqlglot_optimize         | 69.2 ms                                                | 60.5 ms: 1.14x faster                                                  |
| json_loads               | 31.2 us                                                | 27.5 us: 1.13x faster                                                  |
| sympy_expand             | 566 ms                                                 | 504 ms: 1.12x faster                                                   |
| json                     | 5.69 ms                                                | 5.13 ms: 1.11x faster                                                  |
| xml_etree_generate       | 99.4 ms                                                | 89.8 ms: 1.11x faster                                                  |
| unpickle_list            | 5.20 us                                                | 4.74 us: 1.10x faster                                                  |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.94 ms: 1.09x faster                                                  |
| hexiom                   | 10.4 ms                                                | 9.55 ms: 1.09x faster                                                  |
| scimark_lu               | 176 ms                                                 | 162 ms: 1.09x faster                                                   |
| unpack_sequence          | 60.0 ns                                                | 55.4 ns: 1.08x faster                                                  |
| scimark_fft              | 466 ms                                                 | 430 ms: 1.08x faster                                                   |
| pathlib                  | 20.5 ms                                                | 19.0 ms: 1.08x faster                                                  |
| create_gc_cycles         | 1.62 ms                                                | 1.51 ms: 1.07x faster                                                  |
| regex_compile            | 188 ms                                                 | 176 ms: 1.07x faster                                                   |
| xml_etree_parse          | 168 ms                                                 | 158 ms: 1.07x faster                                                   |
| fannkuch                 | 532 ms                                                 | 502 ms: 1.06x faster                                                   |
| regex_effbot             | 3.63 ms                                                | 3.45 ms: 1.05x faster                                                  |
| mdp                      | 2.85 sec                                               | 2.71 sec: 1.05x faster                                                 |
| regex_dna                | 227 ms                                                 | 216 ms: 1.05x faster                                                   |
| xml_etree_iterparse      | 115 ms                                                 | 111 ms: 1.04x faster                                                   |
| nqueens                  | 106 ms                                                 | 102 ms: 1.04x faster                                                   |
| sqlite_synth             | 3.02 us                                                | 2.92 us: 1.04x faster                                                  |
| pidigits                 | 191 ms                                                 | 188 ms: 1.01x faster                                                   |
| meteor_contest           | 120 ms                                                 | 118 ms: 1.01x faster                                                   |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                   |
| pickle_list              | 5.08 us                                                | 5.18 us: 1.02x slower                                                  |
| async_generators         | 444 ms                                                 | 466 ms: 1.05x slower                                                   |
| gc_traversal             | 3.62 ms                                                | 3.87 ms: 1.07x slower                                                  |
| unpickle                 | 14.4 us                                                | 15.7 us: 1.09x slower                                                  |
| pickle                   | 10.7 us                                                | 11.8 us: 1.11x slower                                                  |
| pickle_dict              | 29.6 us                                                | 34.8 us: 1.18x slower                                                  |
| telco                    | 7.27 ms                                                | 8.64 ms: 1.19x slower                                                  |
| coverage                 | 79.4 ms                                                | 95.6 ms: 1.20x slower                                                  |
| dask                     | 441 ms                                                 | 537 ms: 1.22x slower                                                   |
| python_startup_no_site   | 5.93 ms                                                | 8.81 ms: 1.48x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.23x faster                                                           |

Benchmark hidden because not significant (2): bench_mp_pool, mypy2
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240304-3.13.0a4+-ffed8d9-PYTHON_UOPS/bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.16x
- 95% likely to have a speedup of 1.15x
- 99% likely to have a speedup of 1.14x


# Memory

- memory change: 1.07x