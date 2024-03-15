
# Results vs. 3.10.4

- fork: python
- ref: 4ee6bdfbaa792a3aa93c
- machine: linux-x86_64
- commit hash: 4ee6bdf
- commit date: 2024-02-22
- overall geometric mean: 1.26x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.19x faster
- Memory change: 1.22x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4+-4ee6bdf |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 288 ms: 1.21x faster                                                   |
| chameleon      | 9.68 ms                                                | 6.74 ms: 1.44x faster                                                  |
| docutils       | 3.30 sec                                               | 2.75 sec: 1.20x faster                                                 |
| tornado_http   | 136 ms                                                 | 97.3 ms: 1.40x faster                                                  |
| Geometric mean | (ref)                                                  | 1.31x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4+-4ee6bdf |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 437 ms: 1.67x faster                                                   |
| async_tree_memoization  | 870 ms                                                 | 565 ms: 1.54x faster                                                   |
| async_tree_io           | 1.77 sec                                               | 1.19 sec: 1.49x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 709 ms: 1.43x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.53x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4+-4ee6bdf |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 100 ms: 1.53x faster                                                   |
| float          | 117 ms                                                 | 83.7 ms: 1.40x faster                                                  |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                                   |
| Geometric mean | (ref)                                                  | 1.30x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4+-4ee6bdf |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_v8       | 27.8 ms                                                | 24.4 ms: 1.14x faster                                                  |
| regex_compile  | 188 ms                                                 | 169 ms: 1.12x faster                                                   |
| regex_dna      | 227 ms                                                 | 226 ms: 1.00x faster                                                   |
| Geometric mean | (ref)                                                  | 1.06x faster                                                           |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4+-4ee6bdf |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 295 us: 1.64x faster                                                   |
| tomli_loads          | 3.14 sec                                               | 2.30 sec: 1.37x faster                                                 |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.36x faster                                                  |
| xml_etree_process    | 79.1 ms                                                | 59.2 ms: 1.34x faster                                                  |
| unpickle_pure_python | 331 us                                                 | 254 us: 1.30x faster                                                   |
| xml_etree_generate   | 99.4 ms                                                | 87.2 ms: 1.14x faster                                                  |
| json_loads           | 31.2 us                                                | 27.4 us: 1.14x faster                                                  |
| xml_etree_parse      | 168 ms                                                 | 157 ms: 1.07x faster                                                   |
| xml_etree_iterparse  | 115 ms                                                 | 109 ms: 1.06x faster                                                   |
| unpickle_list        | 5.20 us                                                | 5.08 us: 1.02x faster                                                  |
| pickle_list          | 5.08 us                                                | 5.20 us: 1.02x slower                                                  |
| unpickle             | 14.4 us                                                | 14.8 us: 1.03x slower                                                  |
| pickle               | 10.7 us                                                | 11.5 us: 1.08x slower                                                  |
| pickle_dict          | 29.6 us                                                | 34.2 us: 1.16x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.14x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4+-4ee6bdf |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 11.7 ms: 1.25x faster                                                  |
| python_startup_no_site | 5.93 ms                                                | 10.3 ms: 1.74x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.18x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4+-4ee6bdf |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 12.1 ms: 1.35x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4+-4ee6bdf |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 111 us: 4.90x faster                                                   |
| generators               | 80.1 ms                                                | 29.6 ms: 2.70x faster                                                  |
| deltablue                | 7.91 ms                                                | 3.53 ms: 2.24x faster                                                  |
| logging_silent           | 190 ns                                                 | 97.3 ns: 1.95x faster                                                  |
| asyncio_tcp              | 922 ms                                                 | 489 ms: 1.89x faster                                                   |
| async_tree_none          | 728 ms                                                 | 437 ms: 1.67x faster                                                   |
| chaos                    | 115 ms                                                 | 69.4 ms: 1.66x faster                                                  |
| richards_super           | 94.7 ms                                                | 57.2 ms: 1.66x faster                                                  |
| scimark_sor              | 220 ms                                                 | 133 ms: 1.65x faster                                                   |
| crypto_pyaes             | 128 ms                                                 | 77.7 ms: 1.64x faster                                                  |
| pickle_pure_python       | 484 us                                                 | 295 us: 1.64x faster                                                   |
| raytrace                 | 507 ms                                                 | 316 ms: 1.60x faster                                                   |
| sqlglot_parse            | 2.17 ms                                                | 1.36 ms: 1.60x faster                                                  |
| coroutines               | 35.1 ms                                                | 22.1 ms: 1.59x faster                                                  |
| async_tree_memoization   | 870 ms                                                 | 565 ms: 1.54x faster                                                   |
| richards                 | 79.3 ms                                                | 51.6 ms: 1.54x faster                                                  |
| nbody                    | 154 ms                                                 | 100 ms: 1.53x faster                                                   |
| sqlglot_transpile        | 2.57 ms                                                | 1.68 ms: 1.53x faster                                                  |
| async_tree_io            | 1.77 sec                                               | 1.19 sec: 1.49x faster                                                 |
| comprehensions           | 28.8 us                                                | 19.4 us: 1.48x faster                                                  |
| deepcopy_memo            | 58.5 us                                                | 39.9 us: 1.47x faster                                                  |
| logging_simple           | 8.30 us                                                | 5.72 us: 1.45x faster                                                  |
| scimark_monte_carlo      | 118 ms                                                 | 81.4 ms: 1.45x faster                                                  |
| logging_format           | 9.09 us                                                | 6.31 us: 1.44x faster                                                  |
| chameleon                | 9.68 ms                                                | 6.74 ms: 1.44x faster                                                  |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 709 ms: 1.43x faster                                                   |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                                 |
| go                       | 240 ms                                                 | 171 ms: 1.41x faster                                                   |
| tornado_http             | 136 ms                                                 | 97.3 ms: 1.40x faster                                                  |
| float                    | 117 ms                                                 | 83.7 ms: 1.40x faster                                                  |
| deepcopy                 | 479 us                                                 | 348 us: 1.38x faster                                                   |
| deepcopy_reduce          | 4.17 us                                                | 3.04 us: 1.37x faster                                                  |
| tomli_loads              | 3.14 sec                                               | 2.30 sec: 1.37x faster                                                 |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.36x faster                                                  |
| mako                     | 16.3 ms                                                | 12.1 ms: 1.35x faster                                                  |
| spectral_norm            | 170 ms                                                 | 126 ms: 1.35x faster                                                   |
| xml_etree_process        | 79.1 ms                                                | 59.2 ms: 1.34x faster                                                  |
| pyflate                  | 716 ms                                                 | 543 ms: 1.32x faster                                                   |
| sqlglot_normalize        | 143 ms                                                 | 109 ms: 1.31x faster                                                   |
| scimark_lu               | 176 ms                                                 | 135 ms: 1.30x faster                                                   |
| unpickle_pure_python     | 331 us                                                 | 254 us: 1.30x faster                                                   |
| scimark_fft              | 466 ms                                                 | 363 ms: 1.28x faster                                                   |
| python_startup           | 14.6 ms                                                | 11.7 ms: 1.25x faster                                                  |
| pycparser                | 1.58 sec                                               | 1.27 sec: 1.24x faster                                                 |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.23 ms: 1.24x faster                                                  |
| sympy_integrate          | 25.8 ms                                                | 21.2 ms: 1.22x faster                                                  |
| 2to3                     | 348 ms                                                 | 288 ms: 1.21x faster                                                   |
| sympy_sum                | 196 ms                                                 | 162 ms: 1.21x faster                                                   |
| fannkuch                 | 532 ms                                                 | 442 ms: 1.20x faster                                                   |
| docutils                 | 3.30 sec                                               | 2.75 sec: 1.20x faster                                                 |
| sqlglot_optimize         | 69.2 ms                                                | 57.9 ms: 1.20x faster                                                  |
| sympy_str                | 346 ms                                                 | 291 ms: 1.19x faster                                                   |
| dulwich_log              | 84.3 ms                                                | 71.2 ms: 1.18x faster                                                  |
| hexiom                   | 10.4 ms                                                | 8.80 ms: 1.18x faster                                                  |
| bench_thread_pool        | 986 us                                                 | 851 us: 1.16x faster                                                   |
| pprint_safe_repr         | 1.02 sec                                               | 889 ms: 1.15x faster                                                   |
| json                     | 5.69 ms                                                | 4.97 ms: 1.14x faster                                                  |
| xml_etree_generate       | 99.4 ms                                                | 87.2 ms: 1.14x faster                                                  |
| sympy_expand             | 566 ms                                                 | 497 ms: 1.14x faster                                                   |
| json_loads               | 31.2 us                                                | 27.4 us: 1.14x faster                                                  |
| regex_v8                 | 27.8 ms                                                | 24.4 ms: 1.14x faster                                                  |
| regex_compile            | 188 ms                                                 | 169 ms: 1.12x faster                                                   |
| nqueens                  | 106 ms                                                 | 95.5 ms: 1.11x faster                                                  |
| pathlib                  | 20.5 ms                                                | 18.6 ms: 1.10x faster                                                  |
| pprint_pformat           | 2.10 sec                                               | 1.92 sec: 1.10x faster                                                 |
| create_gc_cycles         | 1.62 ms                                                | 1.50 ms: 1.08x faster                                                  |
| sqlite_synth             | 3.02 us                                                | 2.82 us: 1.07x faster                                                  |
| xml_etree_parse          | 168 ms                                                 | 157 ms: 1.07x faster                                                   |
| xml_etree_iterparse      | 115 ms                                                 | 109 ms: 1.06x faster                                                   |
| meteor_contest           | 120 ms                                                 | 113 ms: 1.06x faster                                                   |
| unpickle_list            | 5.20 us                                                | 5.08 us: 1.02x faster                                                  |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                                   |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                   |
| mdp                      | 2.85 sec                                               | 2.83 sec: 1.00x faster                                                 |
| regex_dna                | 227 ms                                                 | 226 ms: 1.00x faster                                                   |
| pickle_list              | 5.08 us                                                | 5.20 us: 1.02x slower                                                  |
| unpickle                 | 14.4 us                                                | 14.8 us: 1.03x slower                                                  |
| gc_traversal             | 3.62 ms                                                | 3.80 ms: 1.05x slower                                                  |
| async_generators         | 444 ms                                                 | 470 ms: 1.06x slower                                                   |
| pickle                   | 10.7 us                                                | 11.5 us: 1.08x slower                                                  |
| pickle_dict              | 29.6 us                                                | 34.2 us: 1.16x slower                                                  |
| telco                    | 7.27 ms                                                | 8.46 ms: 1.16x slower                                                  |
| bench_mp_pool            | 24.0 ms                                                | 28.2 ms: 1.17x slower                                                  |
| coverage                 | 79.4 ms                                                | 95.8 ms: 1.21x slower                                                  |
| python_startup_no_site   | 5.93 ms                                                | 10.3 ms: 1.74x slower                                                  |
| unpack_sequence          | 60.0 ns                                                | 159 ns: 2.66x slower                                                   |
| Geometric mean           | (ref)                                                  | 1.26x faster                                                           |

Benchmark hidden because not significant (2): regex_effbot, mypy2
Ignored benchmarks (13) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240222-3.13.0a4+-4ee6bdf-JIT/bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4+-4ee6bdf.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.20x
- 95% likely to have a speedup of 1.20x
- 99% likely to have a speedup of 1.19x


# Memory

- memory change: 1.22x