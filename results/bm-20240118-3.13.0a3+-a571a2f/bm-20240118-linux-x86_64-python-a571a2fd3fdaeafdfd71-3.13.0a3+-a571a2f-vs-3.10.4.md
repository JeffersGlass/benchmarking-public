
# Results vs. 3.10.4

- fork: python
- ref: a571a2fd3fdaeafdfd71
- machine: linux-x86_64
- commit hash: a571a2f
- commit date: 2024-01-18
- overall geometric mean: 1.36x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.29x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 264 ms: 1.32x faster                                                   |
| chameleon      | 9.68 ms                                                | 6.86 ms: 1.41x faster                                                  |
| docutils       | 3.30 sec                                               | 2.60 sec: 1.27x faster                                                 |
| tornado_http   | 136 ms                                                 | 94.5 ms: 1.44x faster                                                  |
| Geometric mean | (ref)                                                  | 1.36x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 432 ms: 1.69x faster                                                   |
| async_tree_memoization  | 870 ms                                                 | 560 ms: 1.55x faster                                                   |
| async_tree_io           | 1.77 sec                                               | 1.17 sec: 1.51x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 703 ms: 1.45x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.55x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 86.2 ms: 1.78x faster                                                  |
| float          | 117 ms                                                 | 80.3 ms: 1.46x faster                                                  |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                                   |
| Geometric mean | (ref)                                                  | 1.38x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 129 ms: 1.46x faster                                                   |
| regex_v8       | 27.8 ms                                                | 25.1 ms: 1.11x faster                                                  |
| regex_dna      | 227 ms                                                 | 219 ms: 1.03x faster                                                   |
| Geometric mean | (ref)                                                  | 1.14x faster                                                           |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 296 us: 1.63x faster                                                   |
| unpickle_pure_python | 331 us                                                 | 213 us: 1.55x faster                                                   |
| tomli_loads          | 3.14 sec                                               | 2.10 sec: 1.50x faster                                                 |
| json_dumps           | 14.2 ms                                                | 10.3 ms: 1.37x faster                                                  |
| xml_etree_process    | 79.1 ms                                                | 58.8 ms: 1.35x faster                                                  |
| xml_etree_generate   | 99.4 ms                                                | 85.6 ms: 1.16x faster                                                  |
| xml_etree_iterparse  | 115 ms                                                 | 104 ms: 1.10x faster                                                   |
| json_loads           | 31.2 us                                                | 28.3 us: 1.10x faster                                                  |
| xml_etree_parse      | 168 ms                                                 | 158 ms: 1.07x faster                                                   |
| unpickle_list        | 5.20 us                                                | 5.04 us: 1.03x faster                                                  |
| pickle_list          | 5.08 us                                                | 5.17 us: 1.02x slower                                                  |
| unpickle             | 14.4 us                                                | 15.0 us: 1.05x slower                                                  |
| pickle               | 10.7 us                                                | 11.7 us: 1.09x slower                                                  |
| pickle_dict          | 29.6 us                                                | 34.8 us: 1.18x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.16x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                  |
| python_startup_no_site | 5.93 ms                                                | 8.73 ms: 1.47x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.1 ms: 1.48x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 109 us: 5.00x faster                                                   |
| generators               | 80.1 ms                                                | 29.6 ms: 2.71x faster                                                  |
| deltablue                | 7.91 ms                                                | 3.21 ms: 2.46x faster                                                  |
| chaos                    | 115 ms                                                 | 58.5 ms: 1.97x faster                                                  |
| raytrace                 | 507 ms                                                 | 260 ms: 1.95x faster                                                   |
| asyncio_tcp              | 922 ms                                                 | 481 ms: 1.92x faster                                                   |
| logging_silent           | 190 ns                                                 | 100 ns: 1.89x faster                                                   |
| crypto_pyaes             | 128 ms                                                 | 71.1 ms: 1.80x faster                                                  |
| scimark_monte_carlo      | 118 ms                                                 | 66.1 ms: 1.79x faster                                                  |
| comprehensions           | 28.8 us                                                | 16.1 us: 1.78x faster                                                  |
| nbody                    | 154 ms                                                 | 86.2 ms: 1.78x faster                                                  |
| richards_super           | 94.7 ms                                                | 53.7 ms: 1.76x faster                                                  |
| go                       | 240 ms                                                 | 138 ms: 1.74x faster                                                   |
| sqlglot_parse            | 2.17 ms                                                | 1.25 ms: 1.73x faster                                                  |
| scimark_sor              | 220 ms                                                 | 127 ms: 1.73x faster                                                   |
| hexiom                   | 10.4 ms                                                | 6.09 ms: 1.71x faster                                                  |
| async_tree_none          | 728 ms                                                 | 432 ms: 1.69x faster                                                   |
| richards                 | 79.3 ms                                                | 47.7 ms: 1.66x faster                                                  |
| sqlglot_transpile        | 2.57 ms                                                | 1.57 ms: 1.64x faster                                                  |
| pickle_pure_python       | 484 us                                                 | 296 us: 1.63x faster                                                   |
| scimark_lu               | 176 ms                                                 | 110 ms: 1.59x faster                                                   |
| spectral_norm            | 170 ms                                                 | 108 ms: 1.58x faster                                                   |
| pyflate                  | 716 ms                                                 | 457 ms: 1.57x faster                                                   |
| deepcopy_memo            | 58.5 us                                                | 37.4 us: 1.56x faster                                                  |
| async_tree_memoization   | 870 ms                                                 | 560 ms: 1.55x faster                                                   |
| unpickle_pure_python     | 331 us                                                 | 213 us: 1.55x faster                                                   |
| coroutines               | 35.1 ms                                                | 22.7 ms: 1.54x faster                                                  |
| async_tree_io            | 1.77 sec                                               | 1.17 sec: 1.51x faster                                                 |
| tomli_loads              | 3.14 sec                                               | 2.10 sec: 1.50x faster                                                 |
| mako                     | 16.3 ms                                                | 11.1 ms: 1.48x faster                                                  |
| float                    | 117 ms                                                 | 80.3 ms: 1.46x faster                                                  |
| logging_simple           | 8.30 us                                                | 5.70 us: 1.46x faster                                                  |
| regex_compile            | 188 ms                                                 | 129 ms: 1.46x faster                                                   |
| logging_format           | 9.09 us                                                | 6.27 us: 1.45x faster                                                  |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 703 ms: 1.45x faster                                                   |
| tornado_http             | 136 ms                                                 | 94.5 ms: 1.44x faster                                                  |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.79 sec: 1.44x faster                                                 |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.51 ms: 1.43x faster                                                  |
| chameleon                | 9.68 ms                                                | 6.86 ms: 1.41x faster                                                  |
| pprint_pformat           | 2.10 sec                                               | 1.49 sec: 1.41x faster                                                 |
| deepcopy                 | 479 us                                                 | 342 us: 1.40x faster                                                   |
| pprint_safe_repr         | 1.02 sec                                               | 728 ms: 1.40x faster                                                   |
| deepcopy_reduce          | 4.17 us                                                | 3.04 us: 1.37x faster                                                  |
| json_dumps               | 14.2 ms                                                | 10.3 ms: 1.37x faster                                                  |
| xml_etree_process        | 79.1 ms                                                | 58.8 ms: 1.35x faster                                                  |
| unpack_sequence          | 60.0 ns                                                | 44.9 ns: 1.34x faster                                                  |
| scimark_fft              | 466 ms                                                 | 350 ms: 1.33x faster                                                   |
| sympy_sum                | 196 ms                                                 | 148 ms: 1.33x faster                                                   |
| nqueens                  | 106 ms                                                 | 79.6 ms: 1.33x faster                                                  |
| fannkuch                 | 532 ms                                                 | 400 ms: 1.33x faster                                                   |
| sqlglot_normalize        | 143 ms                                                 | 108 ms: 1.33x faster                                                   |
| sympy_integrate          | 25.8 ms                                                | 19.5 ms: 1.33x faster                                                  |
| 2to3                     | 348 ms                                                 | 264 ms: 1.32x faster                                                   |
| pycparser                | 1.58 sec                                               | 1.20 sec: 1.31x faster                                                 |
| dulwich_log              | 84.3 ms                                                | 65.5 ms: 1.29x faster                                                  |
| sqlglot_optimize         | 69.2 ms                                                | 54.1 ms: 1.28x faster                                                  |
| sympy_str                | 346 ms                                                 | 270 ms: 1.28x faster                                                   |
| docutils                 | 3.30 sec                                               | 2.60 sec: 1.27x faster                                                 |
| sympy_expand             | 566 ms                                                 | 458 ms: 1.24x faster                                                   |
| dask                     | 441 ms                                                 | 360 ms: 1.22x faster                                                   |
| bench_thread_pool        | 986 us                                                 | 828 us: 1.19x faster                                                   |
| xml_etree_generate       | 99.4 ms                                                | 85.6 ms: 1.16x faster                                                  |
| mdp                      | 2.85 sec                                               | 2.52 sec: 1.13x faster                                                 |
| pathlib                  | 20.5 ms                                                | 18.2 ms: 1.12x faster                                                  |
| meteor_contest           | 120 ms                                                 | 107 ms: 1.11x faster                                                   |
| regex_v8                 | 27.8 ms                                                | 25.1 ms: 1.11x faster                                                  |
| xml_etree_iterparse      | 115 ms                                                 | 104 ms: 1.10x faster                                                   |
| json_loads               | 31.2 us                                                | 28.3 us: 1.10x faster                                                  |
| json                     | 5.69 ms                                                | 5.16 ms: 1.10x faster                                                  |
| create_gc_cycles         | 1.62 ms                                                | 1.49 ms: 1.09x faster                                                  |
| sqlite_synth             | 3.02 us                                                | 2.82 us: 1.07x faster                                                  |
| xml_etree_parse          | 168 ms                                                 | 158 ms: 1.07x faster                                                   |
| regex_dna                | 227 ms                                                 | 219 ms: 1.03x faster                                                   |
| unpickle_list            | 5.20 us                                                | 5.04 us: 1.03x faster                                                  |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                                   |
| asyncio_websockets       | 559 ms                                                 | 551 ms: 1.01x faster                                                   |
| async_generators         | 444 ms                                                 | 446 ms: 1.00x slower                                                   |
| pickle_list              | 5.08 us                                                | 5.17 us: 1.02x slower                                                  |
| unpickle                 | 14.4 us                                                | 15.0 us: 1.05x slower                                                  |
| gc_traversal             | 3.62 ms                                                | 3.86 ms: 1.06x slower                                                  |
| pickle                   | 10.7 us                                                | 11.7 us: 1.09x slower                                                  |
| telco                    | 7.27 ms                                                | 8.24 ms: 1.13x slower                                                  |
| pickle_dict              | 29.6 us                                                | 34.8 us: 1.18x slower                                                  |
| coverage                 | 79.4 ms                                                | 94.9 ms: 1.19x slower                                                  |
| python_startup_no_site   | 5.93 ms                                                | 8.73 ms: 1.47x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.36x faster                                                           |

Benchmark hidden because not significant (3): mypy2, regex_effbot, bench_mp_pool
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240118-3.13.0a3+-a571a2f/bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.32x
- 95% likely to have a speedup of 1.31x
- 99% likely to have a speedup of 1.29x


# Memory

- memory change: 1.06x