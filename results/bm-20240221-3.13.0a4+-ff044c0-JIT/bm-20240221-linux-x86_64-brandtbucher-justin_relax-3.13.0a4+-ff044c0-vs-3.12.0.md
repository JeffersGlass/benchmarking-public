
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_relax
- machine: linux-x86_64
- commit hash: ff044c0
- commit date: 2024-02-21
- overall geometric mean: 1.01x slower \*
- HPT reliability: 74.35%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.16x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 280 ms: 1.02x slower                                                 |
| chameleon      | 7.41 ms                                                | 6.91 ms: 1.07x faster                                                |
| docutils       | 2.77 sec                                               | 2.72 sec: 1.02x faster                                               |
| tornado_http   | 103 ms                                                 | 96.9 ms: 1.06x faster                                                |
| Geometric mean | (ref)                                                  | 1.03x faster                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none         | 472 ms                                                 | 439 ms: 1.08x faster                                                 |
| async_tree_memoization  | 578 ms                                                 | 563 ms: 1.03x faster                                                 |
| async_tree_cpu_io_mixed | 726 ms                                                 | 708 ms: 1.03x faster                                                 |
| async_tree_none_tg      | 450 ms                                                 | 447 ms: 1.01x faster                                                 |
| async_tree_io_tg        | 1.18 sec                                               | 1.20 sec: 1.02x slower                                               |
| async_tree_io           | 1.16 sec                                               | 1.19 sec: 1.03x slower                                               |
| Geometric mean          | (ref)                                                  | 1.01x faster                                                         |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| float          | 84.7 ms                                                | 80.7 ms: 1.05x faster                                                |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x faster                                                 |
| nbody          | 97.0 ms                                                | 97.7 ms: 1.01x slower                                                |
| Geometric mean | (ref)                                                  | 1.01x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 150 ms: 1.01x slower                                                 |
| regex_effbot   | 3.61 ms                                                | 3.72 ms: 1.03x slower                                                |
| regex_dna      | 212 ms                                                 | 224 ms: 1.05x slower                                                 |
| regex_v8       | 23.1 ms                                                | 24.7 ms: 1.07x slower                                                |
| Geometric mean | (ref)                                                  | 1.04x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 299 us: 1.08x faster                                                 |
| tomli_loads          | 2.33 sec                                               | 2.17 sec: 1.07x faster                                               |
| unpickle_list        | 5.29 us                                                | 5.01 us: 1.06x faster                                                |
| unpickle             | 15.9 us                                                | 15.1 us: 1.05x faster                                                |
| xml_etree_process    | 61.7 ms                                                | 59.1 ms: 1.05x faster                                                |
| json_loads           | 28.5 us                                                | 27.3 us: 1.04x faster                                                |
| xml_etree_generate   | 89.2 ms                                                | 86.6 ms: 1.03x faster                                                |
| xml_etree_parse      | 159 ms                                                 | 157 ms: 1.01x faster                                                 |
| pickle_dict          | 35.5 us                                                | 35.2 us: 1.01x faster                                                |
| pickle               | 11.6 us                                                | 11.8 us: 1.02x slower                                                |
| pickle_list          | 5.08 us                                                | 5.26 us: 1.03x slower                                                |
| unpickle_pure_python | 230 us                                                 | 244 us: 1.06x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                         |

Benchmark hidden because not significant (2): xml_etree_iterparse, json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 12.2 ms: 1.28x slower                                                |
| python_startup_no_site | 6.94 ms                                                | 10.9 ms: 1.57x slower                                                |
| Geometric mean         | (ref)                                                  | 1.42x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 11.6 ms: 1.03x faster                                                |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols | 158 us                                                 | 108 us: 1.46x faster                                                 |
| comprehensions           | 21.8 us                                                | 17.7 us: 1.23x faster                                                |
| logging_format           | 7.23 us                                                | 6.34 us: 1.14x faster                                                |
| logging_simple           | 6.46 us                                                | 5.77 us: 1.12x faster                                                |
| gc_traversal             | 3.79 ms                                                | 3.48 ms: 1.09x faster                                                |
| crypto_pyaes             | 81.9 ms                                                | 75.5 ms: 1.08x faster                                                |
| pickle_pure_python       | 324 us                                                 | 299 us: 1.08x faster                                                 |
| deltablue                | 3.72 ms                                                | 3.44 ms: 1.08x faster                                                |
| async_tree_none          | 472 ms                                                 | 439 ms: 1.08x faster                                                 |
| tomli_loads              | 2.33 sec                                               | 2.17 sec: 1.07x faster                                               |
| chameleon                | 7.41 ms                                                | 6.91 ms: 1.07x faster                                                |
| coroutines               | 23.2 ms                                                | 21.7 ms: 1.07x faster                                                |
| scimark_fft              | 382 ms                                                 | 359 ms: 1.07x faster                                                 |
| generators               | 31.2 ms                                                | 29.3 ms: 1.06x faster                                                |
| deepcopy_reduce          | 3.35 us                                                | 3.15 us: 1.06x faster                                                |
| sympy_sum                | 169 ms                                                 | 159 ms: 1.06x faster                                                 |
| deepcopy                 | 371 us                                                 | 350 us: 1.06x faster                                                 |
| tornado_http             | 103 ms                                                 | 96.9 ms: 1.06x faster                                                |
| logging_silent           | 104 ns                                                 | 98.9 ns: 1.06x faster                                                |
| unpickle_list            | 5.29 us                                                | 5.01 us: 1.06x faster                                                |
| sympy_str                | 300 ms                                                 | 284 ms: 1.05x faster                                                 |
| deepcopy_memo            | 40.7 us                                                | 38.7 us: 1.05x faster                                                |
| json                     | 5.26 ms                                                | 5.00 ms: 1.05x faster                                                |
| float                    | 84.7 ms                                                | 80.7 ms: 1.05x faster                                                |
| unpickle                 | 15.9 us                                                | 15.1 us: 1.05x faster                                                |
| xml_etree_process        | 61.7 ms                                                | 59.1 ms: 1.05x faster                                                |
| raytrace                 | 312 ms                                                 | 299 ms: 1.04x faster                                                 |
| json_loads               | 28.5 us                                                | 27.3 us: 1.04x faster                                                |
| pathlib                  | 19.3 ms                                                | 18.6 ms: 1.04x faster                                                |
| sqlglot_parse            | 1.36 ms                                                | 1.31 ms: 1.04x faster                                                |
| chaos                    | 67.0 ms                                                | 64.8 ms: 1.03x faster                                                |
| meteor_contest           | 112 ms                                                 | 109 ms: 1.03x faster                                                 |
| xml_etree_generate       | 89.2 ms                                                | 86.6 ms: 1.03x faster                                                |
| mako                     | 11.9 ms                                                | 11.6 ms: 1.03x faster                                                |
| async_tree_memoization   | 578 ms                                                 | 563 ms: 1.03x faster                                                 |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 708 ms: 1.03x faster                                                 |
| sympy_integrate          | 21.4 ms                                                | 20.9 ms: 1.02x faster                                                |
| sqlglot_transpile        | 1.68 ms                                                | 1.65 ms: 1.02x faster                                                |
| docutils                 | 2.77 sec                                               | 2.72 sec: 1.02x faster                                               |
| sqlglot_normalize        | 110 ms                                                 | 109 ms: 1.02x faster                                                 |
| xml_etree_parse          | 159 ms                                                 | 157 ms: 1.01x faster                                                 |
| pickle_dict              | 35.5 us                                                | 35.2 us: 1.01x faster                                                |
| pprint_safe_repr         | 776 ms                                                 | 769 ms: 1.01x faster                                                 |
| async_tree_none_tg       | 450 ms                                                 | 447 ms: 1.01x faster                                                 |
| pidigits                 | 187 ms                                                 | 187 ms: 1.00x faster                                                 |
| sqlite_synth             | 2.83 us                                                | 2.85 us: 1.01x slower                                                |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.80 sec: 1.01x slower                                               |
| create_gc_cycles         | 1.48 ms                                                | 1.49 ms: 1.01x slower                                                |
| nbody                    | 97.0 ms                                                | 97.7 ms: 1.01x slower                                                |
| scimark_sor              | 129 ms                                                 | 130 ms: 1.01x slower                                                 |
| sympy_expand             | 478 ms                                                 | 482 ms: 1.01x slower                                                 |
| regex_compile            | 148 ms                                                 | 150 ms: 1.01x slower                                                 |
| dulwich_log              | 68.5 ms                                                | 69.2 ms: 1.01x slower                                                |
| fannkuch                 | 417 ms                                                 | 421 ms: 1.01x slower                                                 |
| mdp                      | 2.63 sec                                               | 2.66 sec: 1.01x slower                                               |
| bench_thread_pool        | 842 us                                                 | 851 us: 1.01x slower                                                 |
| scimark_monte_carlo      | 75.1 ms                                                | 76.1 ms: 1.01x slower                                                |
| asyncio_tcp              | 491 ms                                                 | 497 ms: 1.01x slower                                                 |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 5.15 ms: 1.02x slower                                                |
| async_tree_io_tg         | 1.18 sec                                               | 1.20 sec: 1.02x slower                                               |
| pickle                   | 11.6 us                                                | 11.8 us: 1.02x slower                                                |
| 2to3                     | 274 ms                                                 | 280 ms: 1.02x slower                                                 |
| pprint_pformat           | 1.57 sec                                               | 1.60 sec: 1.02x slower                                               |
| async_tree_io            | 1.16 sec                                               | 1.19 sec: 1.03x slower                                               |
| regex_effbot             | 3.61 ms                                                | 3.72 ms: 1.03x slower                                                |
| pycparser                | 1.18 sec                                               | 1.22 sec: 1.03x slower                                               |
| pickle_list              | 5.08 us                                                | 5.26 us: 1.03x slower                                                |
| sqlglot_optimize         | 54.8 ms                                                | 56.7 ms: 1.04x slower                                                |
| spectral_norm            | 115 ms                                                 | 120 ms: 1.05x slower                                                 |
| pyflate                  | 482 ms                                                 | 508 ms: 1.05x slower                                                 |
| regex_dna                | 212 ms                                                 | 224 ms: 1.05x slower                                                 |
| unpickle_pure_python     | 230 us                                                 | 244 us: 1.06x slower                                                 |
| regex_v8                 | 23.1 ms                                                | 24.7 ms: 1.07x slower                                                |
| richards                 | 45.8 ms                                                | 49.6 ms: 1.08x slower                                                |
| richards_super           | 51.5 ms                                                | 55.9 ms: 1.08x slower                                                |
| nqueens                  | 83.3 ms                                                | 91.4 ms: 1.10x slower                                                |
| scimark_lu               | 118 ms                                                 | 131 ms: 1.11x slower                                                 |
| go                       | 139 ms                                                 | 158 ms: 1.13x slower                                                 |
| bench_mp_pool            | 24.0 ms                                                | 28.0 ms: 1.17x slower                                                |
| hexiom                   | 6.41 ms                                                | 7.54 ms: 1.18x slower                                                |
| telco                    | 7.10 ms                                                | 8.44 ms: 1.19x slower                                                |
| python_startup           | 9.55 ms                                                | 12.2 ms: 1.28x slower                                                |
| coverage                 | 72.7 ms                                                | 95.5 ms: 1.31x slower                                                |
| python_startup_no_site   | 6.94 ms                                                | 10.9 ms: 1.57x slower                                                |
| unpack_sequence          | 54.0 ns                                                | 132 ns: 2.45x slower                                                 |
| Geometric mean           | (ref)                                                  | 1.01x slower                                                         |

Benchmark hidden because not significant (7): async_tree_cpu_io_mixed_tg, xml_etree_iterparse, json_dumps, async_generators, asyncio_websockets, async_tree_memoization_tg, mypy2
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 74.35% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.16x