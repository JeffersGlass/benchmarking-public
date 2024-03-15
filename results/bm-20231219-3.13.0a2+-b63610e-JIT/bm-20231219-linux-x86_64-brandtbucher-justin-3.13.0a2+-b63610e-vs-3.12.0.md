
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin
- machine: linux-x86_64
- commit hash: b63610e
- commit date: 2023-12-19
- overall geometric mean: 1.00x slower
- HPT reliability: 88.74%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.96x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 277 ms: 1.01x slower                                           |
| chameleon      | 7.41 ms                                                | 7.09 ms: 1.04x faster                                          |
| docutils       | 2.77 sec                                               | 2.68 sec: 1.03x faster                                         |
| tornado_http   | 103 ms                                                 | 97.7 ms: 1.05x faster                                          |
| Geometric mean | (ref)                                                  | 1.03x faster                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_none         | 472 ms                                                 | 446 ms: 1.06x faster                                           |
| async_tree_memoization  | 578 ms                                                 | 569 ms: 1.01x faster                                           |
| async_tree_cpu_io_mixed | 726 ms                                                 | 717 ms: 1.01x faster                                           |
| async_tree_io_tg        | 1.18 sec                                               | 1.20 sec: 1.01x slower                                         |
| async_tree_io           | 1.16 sec                                               | 1.19 sec: 1.03x slower                                         |
| Geometric mean          | (ref)                                                  | 1.00x faster                                                   |

Benchmark hidden because not significant (3): async_tree_none_tg, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 188 ms: 1.00x slower                                           |
| float          | 84.7 ms                                                | 88.1 ms: 1.04x slower                                          |
| nbody          | 97.0 ms                                                | 106 ms: 1.10x slower                                           |
| Geometric mean | (ref)                                                  | 1.05x slower                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 142 ms: 1.04x faster                                           |
| regex_dna      | 212 ms                                                 | 213 ms: 1.00x slower                                           |
| regex_effbot   | 3.61 ms                                                | 3.69 ms: 1.02x slower                                          |
| regex_v8       | 23.1 ms                                                | 26.1 ms: 1.13x slower                                          |
| Geometric mean | (ref)                                                  | 1.03x slower                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| unpickle             | 15.9 us                                                | 14.6 us: 1.09x faster                                          |
| pickle_pure_python   | 324 us                                                 | 301 us: 1.08x faster                                           |
| xml_etree_process    | 61.7 ms                                                | 59.0 ms: 1.05x faster                                          |
| json_loads           | 28.5 us                                                | 27.5 us: 1.04x faster                                          |
| tomli_loads          | 2.33 sec                                               | 2.25 sec: 1.03x faster                                         |
| unpickle_list        | 5.29 us                                                | 5.13 us: 1.03x faster                                          |
| xml_etree_generate   | 89.2 ms                                                | 86.8 ms: 1.03x faster                                          |
| pickle_list          | 5.08 us                                                | 5.02 us: 1.01x faster                                          |
| json_dumps           | 10.4 ms                                                | 10.3 ms: 1.01x faster                                          |
| xml_etree_parse      | 159 ms                                                 | 158 ms: 1.01x faster                                           |
| unpickle_pure_python | 230 us                                                 | 228 us: 1.01x faster                                           |
| pickle_dict          | 35.5 us                                                | 35.4 us: 1.00x faster                                          |
| xml_etree_iterparse  | 107 ms                                                 | 109 ms: 1.02x slower                                           |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                   |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.2 ms: 1.07x slower                                          |
| python_startup_no_site | 6.94 ms                                                | 8.87 ms: 1.28x slower                                          |
| Geometric mean         | (ref)                                                  | 1.17x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 12.7 ms: 1.07x slower                                          |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| typing_runtime_protocols | 158 us                                                 | 113 us: 1.40x faster                                           |
| logging_format           | 7.23 us                                                | 6.45 us: 1.12x faster                                          |
| unpack_sequence          | 54.0 ns                                                | 48.5 ns: 1.11x faster                                          |
| logging_simple           | 6.46 us                                                | 5.83 us: 1.11x faster                                          |
| raytrace                 | 312 ms                                                 | 282 ms: 1.11x faster                                           |
| deepcopy_reduce          | 3.35 us                                                | 3.04 us: 1.10x faster                                          |
| comprehensions           | 21.8 us                                                | 19.8 us: 1.10x faster                                          |
| unpickle                 | 15.9 us                                                | 14.6 us: 1.09x faster                                          |
| generators               | 31.2 ms                                                | 28.8 ms: 1.08x faster                                          |
| pickle_pure_python       | 324 us                                                 | 301 us: 1.08x faster                                           |
| deepcopy_memo            | 40.7 us                                                | 38.1 us: 1.07x faster                                          |
| deepcopy                 | 371 us                                                 | 349 us: 1.06x faster                                           |
| async_tree_none          | 472 ms                                                 | 446 ms: 1.06x faster                                           |
| sqlglot_parse            | 1.36 ms                                                | 1.29 ms: 1.05x faster                                          |
| tornado_http             | 103 ms                                                 | 97.7 ms: 1.05x faster                                          |
| pathlib                  | 19.3 ms                                                | 18.4 ms: 1.05x faster                                          |
| sympy_sum                | 169 ms                                                 | 162 ms: 1.05x faster                                           |
| xml_etree_process        | 61.7 ms                                                | 59.0 ms: 1.05x faster                                          |
| chameleon                | 7.41 ms                                                | 7.09 ms: 1.04x faster                                          |
| regex_compile            | 148 ms                                                 | 142 ms: 1.04x faster                                           |
| sqlglot_transpile        | 1.68 ms                                                | 1.62 ms: 1.04x faster                                          |
| json_loads               | 28.5 us                                                | 27.5 us: 1.04x faster                                          |
| docutils                 | 2.77 sec                                               | 2.68 sec: 1.03x faster                                         |
| tomli_loads              | 2.33 sec                                               | 2.25 sec: 1.03x faster                                         |
| sympy_str                | 300 ms                                                 | 290 ms: 1.03x faster                                           |
| coroutines               | 23.2 ms                                                | 22.5 ms: 1.03x faster                                          |
| scimark_lu               | 118 ms                                                 | 115 ms: 1.03x faster                                           |
| unpickle_list            | 5.29 us                                                | 5.13 us: 1.03x faster                                          |
| xml_etree_generate       | 89.2 ms                                                | 86.8 ms: 1.03x faster                                          |
| meteor_contest           | 112 ms                                                 | 110 ms: 1.02x faster                                           |
| json                     | 5.26 ms                                                | 5.17 ms: 1.02x faster                                          |
| dask                     | 372 ms                                                 | 366 ms: 1.01x faster                                           |
| async_tree_memoization   | 578 ms                                                 | 569 ms: 1.01x faster                                           |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 717 ms: 1.01x faster                                           |
| pickle_list              | 5.08 us                                                | 5.02 us: 1.01x faster                                          |
| logging_silent           | 104 ns                                                 | 103 ns: 1.01x faster                                           |
| sympy_integrate          | 21.4 ms                                                | 21.2 ms: 1.01x faster                                          |
| json_dumps               | 10.4 ms                                                | 10.3 ms: 1.01x faster                                          |
| xml_etree_parse          | 159 ms                                                 | 158 ms: 1.01x faster                                           |
| unpickle_pure_python     | 230 us                                                 | 228 us: 1.01x faster                                           |
| gc_traversal             | 3.79 ms                                                | 3.77 ms: 1.01x faster                                          |
| dulwich_log              | 68.5 ms                                                | 68.0 ms: 1.01x faster                                          |
| mdp                      | 2.63 sec                                               | 2.61 sec: 1.01x faster                                         |
| async_generators         | 463 ms                                                 | 460 ms: 1.01x faster                                           |
| pickle_dict              | 35.5 us                                                | 35.4 us: 1.00x faster                                          |
| bench_thread_pool        | 842 us                                                 | 843 us: 1.00x slower                                           |
| regex_dna                | 212 ms                                                 | 213 ms: 1.00x slower                                           |
| pidigits                 | 187 ms                                                 | 188 ms: 1.00x slower                                           |
| create_gc_cycles         | 1.48 ms                                                | 1.48 ms: 1.00x slower                                          |
| sqlglot_normalize        | 110 ms                                                 | 111 ms: 1.00x slower                                           |
| sqlite_synth             | 2.83 us                                                | 2.85 us: 1.00x slower                                          |
| 2to3                     | 274 ms                                                 | 277 ms: 1.01x slower                                           |
| richards                 | 45.8 ms                                                | 46.3 ms: 1.01x slower                                          |
| asyncio_tcp              | 491 ms                                                 | 496 ms: 1.01x slower                                           |
| scimark_sor              | 129 ms                                                 | 131 ms: 1.01x slower                                           |
| sympy_expand             | 478 ms                                                 | 483 ms: 1.01x slower                                           |
| async_tree_io_tg         | 1.18 sec                                               | 1.20 sec: 1.01x slower                                         |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.81 sec: 1.01x slower                                         |
| xml_etree_iterparse      | 107 ms                                                 | 109 ms: 1.02x slower                                           |
| regex_effbot             | 3.61 ms                                                | 3.69 ms: 1.02x slower                                          |
| richards_super           | 51.5 ms                                                | 52.7 ms: 1.02x slower                                          |
| scimark_fft              | 382 ms                                                 | 391 ms: 1.02x slower                                           |
| sqlglot_optimize         | 54.8 ms                                                | 56.2 ms: 1.03x slower                                          |
| async_tree_io            | 1.16 sec                                               | 1.19 sec: 1.03x slower                                         |
| pprint_safe_repr         | 776 ms                                                 | 807 ms: 1.04x slower                                           |
| float                    | 84.7 ms                                                | 88.1 ms: 1.04x slower                                          |
| pyflate                  | 482 ms                                                 | 504 ms: 1.05x slower                                           |
| fannkuch                 | 417 ms                                                 | 438 ms: 1.05x slower                                           |
| chaos                    | 67.0 ms                                                | 70.6 ms: 1.05x slower                                          |
| mako                     | 11.9 ms                                                | 12.7 ms: 1.07x slower                                          |
| python_startup           | 9.55 ms                                                | 10.2 ms: 1.07x slower                                          |
| pprint_pformat           | 1.57 sec                                               | 1.68 sec: 1.07x slower                                         |
| go                       | 139 ms                                                 | 152 ms: 1.09x slower                                           |
| deltablue                | 3.72 ms                                                | 4.07 ms: 1.09x slower                                          |
| nqueens                  | 83.3 ms                                                | 91.2 ms: 1.09x slower                                          |
| nbody                    | 97.0 ms                                                | 106 ms: 1.10x slower                                           |
| regex_v8                 | 23.1 ms                                                | 26.1 ms: 1.13x slower                                          |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 5.72 ms: 1.13x slower                                          |
| telco                    | 7.10 ms                                                | 8.50 ms: 1.20x slower                                          |
| spectral_norm            | 115 ms                                                 | 141 ms: 1.23x slower                                           |
| hexiom                   | 6.41 ms                                                | 8.11 ms: 1.26x slower                                          |
| python_startup_no_site   | 6.94 ms                                                | 8.87 ms: 1.28x slower                                          |
| coverage                 | 72.7 ms                                                | 95.4 ms: 1.31x slower                                          |
| Geometric mean           | (ref)                                                  | 1.00x slower                                                   |

Benchmark hidden because not significant (10): crypto_pyaes, pycparser, async_tree_none_tg, pickle, bench_mp_pool, scimark_monte_carlo, asyncio_websockets, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 88.74% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.96x