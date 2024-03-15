# Results vs. 3.10.4

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: f58f8ce
- commit date: 2024-02-29
- overall geometric mean: 1.37x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.29x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 264 ms: 1.32x faster                                   |
| chameleon      | 9.68 ms                                                | 6.91 ms: 1.40x faster                                  |
| docutils       | 3.30 sec                                               | 2.59 sec: 1.27x faster                                 |
| tornado_http   | 136 ms                                                 | 94.8 ms: 1.44x faster                                  |
| Geometric mean | (ref)                                                  | 1.36x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 432 ms: 1.69x faster                                   |
| async_tree_memoization  | 870 ms                                                 | 556 ms: 1.57x faster                                   |
| async_tree_io           | 1.77 sec                                               | 1.17 sec: 1.51x faster                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 704 ms: 1.44x faster                                   |
| Geometric mean          | (ref)                                                  | 1.55x faster                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| nbody          | 154 ms                                                 | 88.0 ms: 1.74x faster                                  |
| float          | 117 ms                                                 | 80.4 ms: 1.46x faster                                  |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                   |
| Geometric mean | (ref)                                                  | 1.37x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 132 ms: 1.43x faster                                   |
| regex_v8       | 27.8 ms                                                | 24.6 ms: 1.13x faster                                  |
| regex_dna      | 227 ms                                                 | 216 ms: 1.05x faster                                   |
| regex_effbot   | 3.63 ms                                                | 3.56 ms: 1.02x faster                                  |
| Geometric mean | (ref)                                                  | 1.14x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 295 us: 1.64x faster                                   |
| unpickle_pure_python | 331 us                                                 | 214 us: 1.55x faster                                   |
| tomli_loads          | 3.14 sec                                               | 2.14 sec: 1.47x faster                                 |
| json_dumps           | 14.2 ms                                                | 10.3 ms: 1.37x faster                                  |
| xml_etree_process    | 79.1 ms                                                | 58.3 ms: 1.36x faster                                  |
| xml_etree_generate   | 99.4 ms                                                | 85.0 ms: 1.17x faster                                  |
| json_loads           | 31.2 us                                                | 27.6 us: 1.13x faster                                  |
| xml_etree_iterparse  | 115 ms                                                 | 106 ms: 1.09x faster                                   |
| xml_etree_parse      | 168 ms                                                 | 157 ms: 1.07x faster                                   |
| unpickle_list        | 5.20 us                                                | 4.95 us: 1.05x faster                                  |
| pickle_list          | 5.08 us                                                | 4.91 us: 1.04x faster                                  |
| pickle               | 10.7 us                                                | 11.4 us: 1.07x slower                                  |
| pickle_dict          | 29.6 us                                                | 33.1 us: 1.12x slower                                  |
| Geometric mean       | (ref)                                                  | 1.18x faster                                           |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.44x faster                                  |
| python_startup_no_site | 5.93 ms                                                | 8.75 ms: 1.48x slower                                  |
| Geometric mean         | (ref)                                                  | 1.01x slower                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|-----------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.4 ms: 1.43x faster                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 110 us: 4.93x faster                                   |
| generators               | 80.1 ms                                                | 29.3 ms: 2.73x faster                                  |
| deltablue                | 7.91 ms                                                | 3.16 ms: 2.50x faster                                  |
| chaos                    | 115 ms                                                 | 59.8 ms: 1.93x faster                                  |
| raytrace                 | 507 ms                                                 | 263 ms: 1.93x faster                                   |
| asyncio_tcp              | 922 ms                                                 | 483 ms: 1.91x faster                                   |
| logging_silent           | 190 ns                                                 | 102 ns: 1.85x faster                                   |
| crypto_pyaes             | 128 ms                                                 | 69.6 ms: 1.84x faster                                  |
| comprehensions           | 28.8 us                                                | 16.0 us: 1.79x faster                                  |
| richards_super           | 94.7 ms                                                | 52.9 ms: 1.79x faster                                  |
| scimark_sor              | 220 ms                                                 | 124 ms: 1.77x faster                                   |
| scimark_monte_carlo      | 118 ms                                                 | 66.9 ms: 1.77x faster                                  |
| nbody                    | 154 ms                                                 | 88.0 ms: 1.74x faster                                  |
| hexiom                   | 10.4 ms                                                | 5.97 ms: 1.74x faster                                  |
| go                       | 240 ms                                                 | 138 ms: 1.73x faster                                   |
| sqlglot_parse            | 2.17 ms                                                | 1.25 ms: 1.73x faster                                  |
| async_tree_none          | 728 ms                                                 | 432 ms: 1.69x faster                                   |
| richards                 | 79.3 ms                                                | 47.4 ms: 1.67x faster                                  |
| pickle_pure_python       | 484 us                                                 | 295 us: 1.64x faster                                   |
| sqlglot_transpile        | 2.57 ms                                                | 1.57 ms: 1.64x faster                                  |
| scimark_lu               | 176 ms                                                 | 110 ms: 1.60x faster                                   |
| coroutines               | 35.1 ms                                                | 22.1 ms: 1.59x faster                                  |
| deepcopy_memo            | 58.5 us                                                | 37.2 us: 1.57x faster                                  |
| async_tree_memoization   | 870 ms                                                 | 556 ms: 1.57x faster                                   |
| spectral_norm            | 170 ms                                                 | 110 ms: 1.55x faster                                   |
| unpickle_pure_python     | 331 us                                                 | 214 us: 1.55x faster                                   |
| pyflate                  | 716 ms                                                 | 466 ms: 1.54x faster                                   |
| async_tree_io            | 1.77 sec                                               | 1.17 sec: 1.51x faster                                 |
| logging_simple           | 8.30 us                                                | 5.60 us: 1.48x faster                                  |
| logging_format           | 9.09 us                                                | 6.14 us: 1.48x faster                                  |
| tomli_loads              | 3.14 sec                                               | 2.14 sec: 1.47x faster                                 |
| float                    | 117 ms                                                 | 80.4 ms: 1.46x faster                                  |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 704 ms: 1.44x faster                                   |
| tornado_http             | 136 ms                                                 | 94.8 ms: 1.44x faster                                  |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.44x faster                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.79 sec: 1.44x faster                                 |
| mako                     | 16.3 ms                                                | 11.4 ms: 1.43x faster                                  |
| regex_compile            | 188 ms                                                 | 132 ms: 1.43x faster                                   |
| pprint_pformat           | 2.10 sec                                               | 1.49 sec: 1.41x faster                                 |
| pprint_safe_repr         | 1.02 sec                                               | 724 ms: 1.41x faster                                   |
| chameleon                | 9.68 ms                                                | 6.91 ms: 1.40x faster                                  |
| deepcopy                 | 479 us                                                 | 344 us: 1.39x faster                                   |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.69 ms: 1.38x faster                                  |
| json_dumps               | 14.2 ms                                                | 10.3 ms: 1.37x faster                                  |
| fannkuch                 | 532 ms                                                 | 388 ms: 1.37x faster                                   |
| deepcopy_reduce          | 4.17 us                                                | 3.05 us: 1.37x faster                                  |
| xml_etree_process        | 79.1 ms                                                | 58.3 ms: 1.36x faster                                  |
| sqlglot_normalize        | 143 ms                                                 | 105 ms: 1.35x faster                                   |
| nqueens                  | 106 ms                                                 | 78.9 ms: 1.34x faster                                  |
| sympy_sum                | 196 ms                                                 | 148 ms: 1.33x faster                                   |
| 2to3                     | 348 ms                                                 | 264 ms: 1.32x faster                                   |
| sympy_integrate          | 25.8 ms                                                | 19.6 ms: 1.32x faster                                  |
| pycparser                | 1.58 sec                                               | 1.21 sec: 1.31x faster                                 |
| sqlglot_optimize         | 69.2 ms                                                | 53.4 ms: 1.30x faster                                  |
| scimark_fft              | 466 ms                                                 | 360 ms: 1.29x faster                                   |
| sympy_str                | 346 ms                                                 | 268 ms: 1.29x faster                                   |
| dulwich_log              | 84.3 ms                                                | 65.6 ms: 1.29x faster                                  |
| docutils                 | 3.30 sec                                               | 2.59 sec: 1.27x faster                                 |
| unpack_sequence          | 60.0 ns                                                | 47.4 ns: 1.27x faster                                  |
| sympy_expand             | 566 ms                                                 | 454 ms: 1.24x faster                                   |
| bench_thread_pool        | 986 us                                                 | 816 us: 1.21x faster                                   |
| xml_etree_generate       | 99.4 ms                                                | 85.0 ms: 1.17x faster                                  |
| pathlib                  | 20.5 ms                                                | 18.0 ms: 1.13x faster                                  |
| json_loads               | 31.2 us                                                | 27.6 us: 1.13x faster                                  |
| regex_v8                 | 27.8 ms                                                | 24.6 ms: 1.13x faster                                  |
| json                     | 5.69 ms                                                | 5.05 ms: 1.13x faster                                  |
| meteor_contest           | 120 ms                                                 | 107 ms: 1.12x faster                                   |
| xml_etree_iterparse      | 115 ms                                                 | 106 ms: 1.09x faster                                   |
| create_gc_cycles         | 1.62 ms                                                | 1.50 ms: 1.08x faster                                  |
| xml_etree_parse          | 168 ms                                                 | 157 ms: 1.07x faster                                   |
| mdp                      | 2.85 sec                                               | 2.68 sec: 1.06x faster                                 |
| sqlite_synth             | 3.02 us                                                | 2.88 us: 1.05x faster                                  |
| unpickle_list            | 5.20 us                                                | 4.95 us: 1.05x faster                                  |
| regex_dna                | 227 ms                                                 | 216 ms: 1.05x faster                                   |
| pickle_list              | 5.08 us                                                | 4.91 us: 1.04x faster                                  |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                   |
| regex_effbot             | 3.63 ms                                                | 3.56 ms: 1.02x faster                                  |
| async_generators         | 444 ms                                                 | 448 ms: 1.01x slower                                   |
| gc_traversal             | 3.62 ms                                                | 3.75 ms: 1.03x slower                                  |
| pickle                   | 10.7 us                                                | 11.4 us: 1.07x slower                                  |
| pickle_dict              | 29.6 us                                                | 33.1 us: 1.12x slower                                  |
| telco                    | 7.27 ms                                                | 8.20 ms: 1.13x slower                                  |
| coverage                 | 79.4 ms                                                | 93.0 ms: 1.17x slower                                  |
| python_startup_no_site   | 5.93 ms                                                | 8.75 ms: 1.48x slower                                  |
| Geometric mean           | (ref)                                                  | 1.37x faster                                           |

Benchmark hidden because not significant (4): mypy2, bench_mp_pool, asyncio_websockets, unpickle
Ignored benchmarks (13) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240229-3.13.0a4+-f58f8ce/bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.32x
- 95% likely to have a speedup of 1.31x
- 99% likely to have a speedup of 1.29x


# Memory

- memory change: 1.06x