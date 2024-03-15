
# Results vs. 3.12.0

- fork: python
- ref: v3.11.6
- machine: linux-x86_64
- commit hash: 8b6ee5b
- commit date: 2023-10-02
- overall geometric mean: 1.02x faster \*
- HPT reliability: 99.98%
- HPT 99th percentile: 1.02x faster
- Memory change: 0.96x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231002-linux-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 257 ms: 1.07x faster                                   |
| chameleon      | 7.41 ms                                                | 6.61 ms: 1.12x faster                                  |
| docutils       | 2.77 sec                                               | 2.58 sec: 1.07x faster                                 |
| tornado_http   | 103 ms                                                 | 96.9 ms: 1.06x faster                                  |
| Geometric mean | (ref)                                                  | 1.08x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231002-linux-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_cpu_io_mixed | 726 ms                                                 | 742 ms: 1.02x slower                                   |
| async_tree_memoization  | 578 ms                                                 | 632 ms: 1.09x slower                                   |
| async_tree_none         | 472 ms                                                 | 522 ms: 1.11x slower                                   |
| async_tree_io           | 1.16 sec                                               | 1.30 sec: 1.13x slower                                 |
| Geometric mean          | (ref)                                                  | 1.09x slower                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231002-linux-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| float          | 84.7 ms                                                | 75.7 ms: 1.12x faster                                  |
| nbody          | 97.0 ms                                                | 92.6 ms: 1.05x faster                                  |
| pidigits       | 187 ms                                                 | 199 ms: 1.06x slower                                   |
| Geometric mean | (ref)                                                  | 1.03x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231002-linux-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 136 ms: 1.09x faster                                   |
| regex_dna      | 212 ms                                                 | 199 ms: 1.07x faster                                   |
| regex_v8       | 23.1 ms                                                | 21.9 ms: 1.05x faster                                  |
| regex_effbot   | 3.61 ms                                                | 3.47 ms: 1.04x faster                                  |
| Geometric mean | (ref)                                                  | 1.06x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231002-linux-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|---------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_list         | 5.08 us                                                | 4.05 us: 1.25x faster                                  |
| json_loads          | 28.5 us                                                | 23.9 us: 1.19x faster                                  |
| unpickle            | 15.9 us                                                | 13.3 us: 1.19x faster                                  |
| pickle_dict         | 35.5 us                                                | 29.9 us: 1.19x faster                                  |
| pickle              | 11.6 us                                                | 9.82 us: 1.18x faster                                  |
| xml_etree_generate  | 89.2 ms                                                | 76.7 ms: 1.16x faster                                  |
| xml_etree_process   | 61.7 ms                                                | 53.7 ms: 1.15x faster                                  |
| pickle_pure_python  | 324 us                                                 | 306 us: 1.06x faster                                   |
| unpickle_list       | 5.29 us                                                | 5.08 us: 1.04x faster                                  |
| tomli_loads         | 2.33 sec                                               | 2.25 sec: 1.03x faster                                 |
| xml_etree_iterparse | 107 ms                                                 | 103 ms: 1.03x faster                                   |
| xml_etree_parse     | 159 ms                                                 | 158 ms: 1.01x faster                                   |
| json_dumps          | 10.4 ms                                                | 12.7 ms: 1.22x slower                                  |
| Geometric mean      | (ref)                                                  | 1.09x faster                                           |

Benchmark hidden because not significant (1): unpickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231002-linux-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup_no_site | 6.94 ms                                                | 6.00 ms: 1.16x faster                                  |
| python_startup         | 9.55 ms                                                | 8.50 ms: 1.12x faster                                  |
| Geometric mean         | (ref)                                                  | 1.14x faster                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231002-linux-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako            | 11.9 ms                                                | 9.88 ms: 1.20x faster                                  |
| django_template | 34.6 ms                                                | 33.1 ms: 1.05x faster                                  |
| Geometric mean  | (ref)                                                  | 1.12x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231002-linux-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_generators         | 463 ms                                                 | 356 ms: 1.30x faster                                   |
| unpack_sequence          | 54.0 ns                                                | 42.9 ns: 1.26x faster                                  |
| pickle_list              | 5.08 us                                                | 4.05 us: 1.25x faster                                  |
| mako                     | 11.9 ms                                                | 9.88 ms: 1.20x faster                                  |
| json_loads               | 28.5 us                                                | 23.9 us: 1.19x faster                                  |
| unpickle                 | 15.9 us                                                | 13.3 us: 1.19x faster                                  |
| pickle_dict              | 35.5 us                                                | 29.9 us: 1.19x faster                                  |
| pickle                   | 11.6 us                                                | 9.82 us: 1.18x faster                                  |
| pyflate                  | 482 ms                                                 | 412 ms: 1.17x faster                                   |
| xml_etree_generate       | 89.2 ms                                                | 76.7 ms: 1.16x faster                                  |
| python_startup_no_site   | 6.94 ms                                                | 6.00 ms: 1.16x faster                                  |
| scimark_fft              | 382 ms                                                 | 332 ms: 1.15x faster                                   |
| xml_etree_process        | 61.7 ms                                                | 53.7 ms: 1.15x faster                                  |
| json                     | 5.26 ms                                                | 4.59 ms: 1.14x faster                                  |
| sqlite_synth             | 2.83 us                                                | 2.50 us: 1.13x faster                                  |
| python_startup           | 9.55 ms                                                | 8.50 ms: 1.12x faster                                  |
| deepcopy_memo            | 40.7 us                                                | 36.3 us: 1.12x faster                                  |
| deepcopy_reduce          | 3.35 us                                                | 2.98 us: 1.12x faster                                  |
| chameleon                | 7.41 ms                                                | 6.61 ms: 1.12x faster                                  |
| float                    | 84.7 ms                                                | 75.7 ms: 1.12x faster                                  |
| spectral_norm            | 115 ms                                                 | 103 ms: 1.11x faster                                   |
| logging_format           | 7.23 us                                                | 6.52 us: 1.11x faster                                  |
| pprint_safe_repr         | 776 ms                                                 | 703 ms: 1.10x faster                                   |
| crypto_pyaes             | 81.9 ms                                                | 74.4 ms: 1.10x faster                                  |
| scimark_monte_carlo      | 75.1 ms                                                | 68.5 ms: 1.10x faster                                  |
| scimark_sor              | 129 ms                                                 | 118 ms: 1.10x faster                                   |
| regex_compile            | 148 ms                                                 | 136 ms: 1.09x faster                                   |
| logging_simple           | 6.46 us                                                | 5.93 us: 1.09x faster                                  |
| deepcopy                 | 371 us                                                 | 342 us: 1.09x faster                                   |
| pprint_pformat           | 1.57 sec                                               | 1.45 sec: 1.08x faster                                 |
| fannkuch                 | 417 ms                                                 | 387 ms: 1.08x faster                                   |
| scimark_lu               | 118 ms                                                 | 110 ms: 1.08x faster                                   |
| docutils                 | 2.77 sec                                               | 2.58 sec: 1.07x faster                                 |
| meteor_contest           | 112 ms                                                 | 105 ms: 1.07x faster                                   |
| 2to3                     | 274 ms                                                 | 257 ms: 1.07x faster                                   |
| regex_dna                | 212 ms                                                 | 199 ms: 1.07x faster                                   |
| telco                    | 7.10 ms                                                | 6.66 ms: 1.07x faster                                  |
| raytrace                 | 312 ms                                                 | 293 ms: 1.06x faster                                   |
| pathlib                  | 19.3 ms                                                | 18.2 ms: 1.06x faster                                  |
| dulwich_log              | 68.5 ms                                                | 64.5 ms: 1.06x faster                                  |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 4.76 ms: 1.06x faster                                  |
| sqlalchemy_declarative   | 147 ms                                                 | 139 ms: 1.06x faster                                   |
| tornado_http             | 103 ms                                                 | 96.9 ms: 1.06x faster                                  |
| pickle_pure_python       | 324 us                                                 | 306 us: 1.06x faster                                   |
| gunicorn                 | 1.24 ms                                                | 1.17 ms: 1.06x faster                                  |
| sqlalchemy_imperative    | 18.7 ms                                                | 17.7 ms: 1.06x faster                                  |
| pycparser                | 1.18 sec                                               | 1.12 sec: 1.06x faster                                 |
| regex_v8                 | 23.1 ms                                                | 21.9 ms: 1.05x faster                                  |
| aiohttp                  | 1.15 ms                                                | 1.10 ms: 1.05x faster                                  |
| nbody                    | 97.0 ms                                                | 92.6 ms: 1.05x faster                                  |
| django_template          | 34.6 ms                                                | 33.1 ms: 1.05x faster                                  |
| sympy_str                | 300 ms                                                 | 287 ms: 1.04x faster                                   |
| unpickle_list            | 5.29 us                                                | 5.08 us: 1.04x faster                                  |
| regex_effbot             | 3.61 ms                                                | 3.47 ms: 1.04x faster                                  |
| dask                     | 372 ms                                                 | 358 ms: 1.04x faster                                   |
| sqlglot_optimize         | 54.8 ms                                                | 53.0 ms: 1.03x faster                                  |
| tomli_loads              | 2.33 sec                                               | 2.25 sec: 1.03x faster                                 |
| xml_etree_iterparse      | 107 ms                                                 | 103 ms: 1.03x faster                                   |
| logging_silent           | 104 ns                                                 | 101 ns: 1.03x faster                                   |
| sympy_integrate          | 21.4 ms                                                | 20.8 ms: 1.03x faster                                  |
| bench_thread_pool        | 842 us                                                 | 821 us: 1.03x faster                                   |
| sympy_sum                | 169 ms                                                 | 165 ms: 1.02x faster                                   |
| sqlglot_normalize        | 110 ms                                                 | 108 ms: 1.02x faster                                   |
| sympy_expand             | 478 ms                                                 | 471 ms: 1.01x faster                                   |
| xml_etree_parse          | 159 ms                                                 | 158 ms: 1.01x faster                                   |
| nqueens                  | 83.3 ms                                                | 83.7 ms: 1.01x slower                                  |
| sqlglot_parse            | 1.36 ms                                                | 1.37 ms: 1.01x slower                                  |
| hexiom                   | 6.41 ms                                                | 6.49 ms: 1.01x slower                                  |
| comprehensions           | 21.8 us                                                | 22.2 us: 1.02x slower                                  |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 742 ms: 1.02x slower                                   |
| chaos                    | 67.0 ms                                                | 68.8 ms: 1.03x slower                                  |
| richards                 | 45.8 ms                                                | 47.9 ms: 1.05x slower                                  |
| deltablue                | 3.72 ms                                                | 3.94 ms: 1.06x slower                                  |
| pidigits                 | 187 ms                                                 | 199 ms: 1.06x slower                                   |
| mdp                      | 2.63 sec                                               | 2.81 sec: 1.07x slower                                 |
| async_tree_memoization   | 578 ms                                                 | 632 ms: 1.09x slower                                   |
| async_tree_none          | 472 ms                                                 | 522 ms: 1.11x slower                                   |
| coroutines               | 23.2 ms                                                | 25.9 ms: 1.12x slower                                  |
| gc_traversal             | 3.79 ms                                                | 4.25 ms: 1.12x slower                                  |
| async_tree_io            | 1.16 sec                                               | 1.30 sec: 1.13x slower                                 |
| richards_super           | 51.5 ms                                                | 59.0 ms: 1.15x slower                                  |
| json_dumps               | 10.4 ms                                                | 12.7 ms: 1.22x slower                                  |
| asyncio_tcp_ssl          | 1.79 sec                                               | 3.14 sec: 1.76x slower                                 |
| asyncio_tcp              | 491 ms                                                 | 934 ms: 1.90x slower                                   |
| generators               | 31.2 ms                                                | 72.2 ms: 2.31x slower                                  |
| typing_runtime_protocols | 158 us                                                 | 493 us: 3.13x slower                                   |
| Geometric mean           | (ref)                                                  | 1.02x faster                                           |

Benchmark hidden because not significant (5): unpickle_pure_python, sqlglot_transpile, create_gc_cycles, bench_mp_pool, go
Ignored benchmarks (7) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, coverage, mypy2
Ignored benchmarks (7) of results/bm-20231002-3.11.6-8b6ee5b/bm-20231002-linux-x86_64-python-v3.11.6-3.11.6-8b6ee5b.json: djangocms, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 99.98% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 0.96x