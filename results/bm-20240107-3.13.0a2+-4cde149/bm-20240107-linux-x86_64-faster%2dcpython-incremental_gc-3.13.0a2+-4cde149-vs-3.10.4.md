
# Results vs. 3.10.4

- fork: faster-cpython
- ref: incremental_gc
- machine: linux-x86_64
- commit hash: 4cde149
- commit date: 2024-01-07
- overall geometric mean: 1.35x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.28x faster
- Memory change: 1.08x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-4cde149 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 270 ms: 1.29x faster                                                       |
| chameleon      | 9.68 ms                                                | 7.02 ms: 1.38x faster                                                      |
| docutils       | 3.30 sec                                               | 2.53 sec: 1.31x faster                                                     |
| tornado_http   | 136 ms                                                 | 93.6 ms: 1.46x faster                                                      |
| Geometric mean | (ref)                                                  | 1.36x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-4cde149 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_io           | 1.77 sec                                               | 806 ms: 2.19x faster                                                       |
| async_tree_none         | 728 ms                                                 | 358 ms: 2.04x faster                                                       |
| async_tree_memoization  | 870 ms                                                 | 463 ms: 1.88x faster                                                       |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 631 ms: 1.61x faster                                                       |
| Geometric mean          | (ref)                                                  | 1.92x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-4cde149 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 91.9 ms: 1.67x faster                                                      |
| float          | 117 ms                                                 | 86.6 ms: 1.35x faster                                                      |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                                       |
| Geometric mean | (ref)                                                  | 1.32x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-4cde149 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 133 ms: 1.42x faster                                                       |
| regex_v8       | 27.8 ms                                                | 26.0 ms: 1.07x faster                                                      |
| regex_dna      | 227 ms                                                 | 223 ms: 1.02x faster                                                       |
| regex_effbot   | 3.63 ms                                                | 3.78 ms: 1.04x slower                                                      |
| Geometric mean | (ref)                                                  | 1.10x faster                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-4cde149 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 299 us: 1.62x faster                                                       |
| unpickle_pure_python | 331 us                                                 | 216 us: 1.53x faster                                                       |
| tomli_loads          | 3.14 sec                                               | 2.15 sec: 1.46x faster                                                     |
| json_dumps           | 14.2 ms                                                | 10.6 ms: 1.34x faster                                                      |
| xml_etree_process    | 79.1 ms                                                | 61.1 ms: 1.29x faster                                                      |
| json_loads           | 31.2 us                                                | 28.2 us: 1.11x faster                                                      |
| xml_etree_generate   | 99.4 ms                                                | 90.5 ms: 1.10x faster                                                      |
| pickle_list          | 5.08 us                                                | 4.97 us: 1.02x faster                                                      |
| unpickle             | 14.4 us                                                | 15.1 us: 1.05x slower                                                      |
| unpickle_list        | 5.20 us                                                | 5.49 us: 1.06x slower                                                      |
| pickle               | 10.7 us                                                | 11.5 us: 1.08x slower                                                      |
| xml_etree_iterparse  | 115 ms                                                 | 132 ms: 1.14x slower                                                       |
| pickle_dict          | 29.6 us                                                | 34.5 us: 1.16x slower                                                      |
| xml_etree_parse      | 168 ms                                                 | 207 ms: 1.23x slower                                                       |
| Geometric mean       | (ref)                                                  | 1.10x faster                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-4cde149 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                      |
| python_startup_no_site | 5.93 ms                                                | 8.56 ms: 1.44x slower                                                      |
| Geometric mean         | (ref)                                                  | 1.00x slower                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-4cde149 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.4 ms: 1.43x faster                                                      |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-4cde149 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 115 us: 4.74x faster                                                       |
| generators               | 80.1 ms                                                | 29.6 ms: 2.71x faster                                                      |
| deltablue                | 7.91 ms                                                | 3.23 ms: 2.45x faster                                                      |
| async_tree_io            | 1.77 sec                                               | 806 ms: 2.19x faster                                                       |
| async_tree_none          | 728 ms                                                 | 358 ms: 2.04x faster                                                       |
| chaos                    | 115 ms                                                 | 58.8 ms: 1.96x faster                                                      |
| raytrace                 | 507 ms                                                 | 261 ms: 1.94x faster                                                       |
| asyncio_tcp              | 922 ms                                                 | 483 ms: 1.91x faster                                                       |
| async_tree_memoization   | 870 ms                                                 | 463 ms: 1.88x faster                                                       |
| logging_silent           | 190 ns                                                 | 103 ns: 1.85x faster                                                       |
| scimark_sor              | 220 ms                                                 | 120 ms: 1.83x faster                                                       |
| crypto_pyaes             | 128 ms                                                 | 72.3 ms: 1.77x faster                                                      |
| comprehensions           | 28.8 us                                                | 16.3 us: 1.76x faster                                                      |
| richards_super           | 94.7 ms                                                | 54.0 ms: 1.75x faster                                                      |
| sqlglot_parse            | 2.17 ms                                                | 1.25 ms: 1.74x faster                                                      |
| go                       | 240 ms                                                 | 138 ms: 1.73x faster                                                       |
| scimark_monte_carlo      | 118 ms                                                 | 68.4 ms: 1.73x faster                                                      |
| hexiom                   | 10.4 ms                                                | 6.15 ms: 1.69x faster                                                      |
| nbody                    | 154 ms                                                 | 91.9 ms: 1.67x faster                                                      |
| richards                 | 79.3 ms                                                | 47.7 ms: 1.66x faster                                                      |
| sqlglot_transpile        | 2.57 ms                                                | 1.56 ms: 1.65x faster                                                      |
| pickle_pure_python       | 484 us                                                 | 299 us: 1.62x faster                                                       |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 631 ms: 1.61x faster                                                       |
| scimark_lu               | 176 ms                                                 | 113 ms: 1.56x faster                                                       |
| coroutines               | 35.1 ms                                                | 22.7 ms: 1.55x faster                                                      |
| pyflate                  | 716 ms                                                 | 466 ms: 1.54x faster                                                       |
| unpickle_pure_python     | 331 us                                                 | 216 us: 1.53x faster                                                       |
| deepcopy_memo            | 58.5 us                                                | 38.3 us: 1.53x faster                                                      |
| spectral_norm            | 170 ms                                                 | 113 ms: 1.50x faster                                                       |
| tomli_loads              | 3.14 sec                                               | 2.15 sec: 1.46x faster                                                     |
| tornado_http             | 136 ms                                                 | 93.6 ms: 1.46x faster                                                      |
| logging_simple           | 8.30 us                                                | 5.71 us: 1.46x faster                                                      |
| logging_format           | 9.09 us                                                | 6.29 us: 1.45x faster                                                      |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.78 sec: 1.44x faster                                                     |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                      |
| mako                     | 16.3 ms                                                | 11.4 ms: 1.43x faster                                                      |
| regex_compile            | 188 ms                                                 | 133 ms: 1.42x faster                                                       |
| pprint_pformat           | 2.10 sec                                               | 1.49 sec: 1.41x faster                                                     |
| pprint_safe_repr         | 1.02 sec                                               | 727 ms: 1.40x faster                                                       |
| chameleon                | 9.68 ms                                                | 7.02 ms: 1.38x faster                                                      |
| deepcopy                 | 479 us                                                 | 349 us: 1.37x faster                                                       |
| float                    | 117 ms                                                 | 86.6 ms: 1.35x faster                                                      |
| sqlglot_normalize        | 143 ms                                                 | 106 ms: 1.34x faster                                                       |
| json_dumps               | 14.2 ms                                                | 10.6 ms: 1.34x faster                                                      |
| deepcopy_reduce          | 4.17 us                                                | 3.11 us: 1.34x faster                                                      |
| pycparser                | 1.58 sec                                               | 1.19 sec: 1.33x faster                                                     |
| sympy_sum                | 196 ms                                                 | 148 ms: 1.33x faster                                                       |
| sympy_integrate          | 25.8 ms                                                | 19.6 ms: 1.32x faster                                                      |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.93 ms: 1.31x faster                                                      |
| docutils                 | 3.30 sec                                               | 2.53 sec: 1.31x faster                                                     |
| nqueens                  | 106 ms                                                 | 81.1 ms: 1.30x faster                                                      |
| xml_etree_process        | 79.1 ms                                                | 61.1 ms: 1.29x faster                                                      |
| sqlglot_optimize         | 69.2 ms                                                | 53.6 ms: 1.29x faster                                                      |
| 2to3                     | 348 ms                                                 | 270 ms: 1.29x faster                                                       |
| sympy_str                | 346 ms                                                 | 270 ms: 1.28x faster                                                       |
| dulwich_log              | 84.3 ms                                                | 66.5 ms: 1.27x faster                                                      |
| fannkuch                 | 532 ms                                                 | 420 ms: 1.27x faster                                                       |
| scimark_fft              | 466 ms                                                 | 370 ms: 1.26x faster                                                       |
| sympy_expand             | 566 ms                                                 | 456 ms: 1.24x faster                                                       |
| dask                     | 441 ms                                                 | 356 ms: 1.24x faster                                                       |
| mypy2                    | 894 ms                                                 | 748 ms: 1.20x faster                                                       |
| unpack_sequence          | 60.0 ns                                                | 50.4 ns: 1.19x faster                                                      |
| bench_thread_pool        | 986 us                                                 | 837 us: 1.18x faster                                                       |
| create_gc_cycles         | 1.62 ms                                                | 1.44 ms: 1.12x faster                                                      |
| pathlib                  | 20.5 ms                                                | 18.3 ms: 1.12x faster                                                      |
| mdp                      | 2.85 sec                                               | 2.55 sec: 1.12x faster                                                     |
| json_loads               | 31.2 us                                                | 28.2 us: 1.11x faster                                                      |
| json                     | 5.69 ms                                                | 5.18 ms: 1.10x faster                                                      |
| xml_etree_generate       | 99.4 ms                                                | 90.5 ms: 1.10x faster                                                      |
| meteor_contest           | 120 ms                                                 | 110 ms: 1.09x faster                                                       |
| regex_v8                 | 27.8 ms                                                | 26.0 ms: 1.07x faster                                                      |
| sqlite_synth             | 3.02 us                                                | 2.86 us: 1.06x faster                                                      |
| pickle_list              | 5.08 us                                                | 4.97 us: 1.02x faster                                                      |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                                       |
| async_generators         | 444 ms                                                 | 436 ms: 1.02x faster                                                       |
| regex_dna                | 227 ms                                                 | 223 ms: 1.02x faster                                                       |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                       |
| regex_effbot             | 3.63 ms                                                | 3.78 ms: 1.04x slower                                                      |
| unpickle                 | 14.4 us                                                | 15.1 us: 1.05x slower                                                      |
| gc_traversal             | 3.62 ms                                                | 3.82 ms: 1.06x slower                                                      |
| unpickle_list            | 5.20 us                                                | 5.49 us: 1.06x slower                                                      |
| pickle                   | 10.7 us                                                | 11.5 us: 1.08x slower                                                      |
| xml_etree_iterparse      | 115 ms                                                 | 132 ms: 1.14x slower                                                       |
| telco                    | 7.27 ms                                                | 8.44 ms: 1.16x slower                                                      |
| pickle_dict              | 29.6 us                                                | 34.5 us: 1.16x slower                                                      |
| coverage                 | 79.4 ms                                                | 95.9 ms: 1.21x slower                                                      |
| xml_etree_parse          | 168 ms                                                 | 207 ms: 1.23x slower                                                       |
| python_startup_no_site   | 5.93 ms                                                | 8.56 ms: 1.44x slower                                                      |
| Geometric mean           | (ref)                                                  | 1.35x faster                                                               |

Benchmark hidden because not significant (1): bench_mp_pool
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240107-3.13.0a2+-4cde149/bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-4cde149.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.30x
- 95% likely to have a speedup of 1.29x
- 99% likely to have a speedup of 1.28x


# Memory

- memory change: 1.08x