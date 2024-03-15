
# Results vs. 3.12.0

- fork: faster-cpython
- ref: cold_exits
- machine: linux-x86_64
- commit hash: d73fe0a
- commit date: 2024-01-16
- overall geometric mean: 1.06x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 290 ms: 1.06x slower                                                   |
| chameleon      | 7.41 ms                                                | 7.32 ms: 1.01x faster                                                  |
| docutils       | 2.77 sec                                               | 2.85 sec: 1.03x slower                                                 |
| tornado_http   | 103 ms                                                 | 98.0 ms: 1.05x faster                                                  |
| Geometric mean | (ref)                                                  | 1.01x slower                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|---------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none           | 472 ms                                                 | 450 ms: 1.05x faster                                                   |
| async_tree_none_tg        | 450 ms                                                 | 452 ms: 1.00x slower                                                   |
| async_tree_memoization_tg | 575 ms                                                 | 587 ms: 1.02x slower                                                   |
| async_tree_io_tg          | 1.18 sec                                               | 1.21 sec: 1.02x slower                                                 |
| async_tree_io             | 1.16 sec                                               | 1.21 sec: 1.04x slower                                                 |
| Geometric mean            | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (3): async_tree_cpu_io_mixed, async_tree_memoization, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 189 ms: 1.01x slower                                                   |
| float          | 84.7 ms                                                | 93.4 ms: 1.10x slower                                                  |
| nbody          | 97.0 ms                                                | 120 ms: 1.23x slower                                                   |
| Geometric mean | (ref)                                                  | 1.11x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_dna      | 212 ms                                                 | 227 ms: 1.07x slower                                                   |
| regex_v8       | 23.1 ms                                                | 25.2 ms: 1.09x slower                                                  |
| regex_compile  | 148 ms                                                 | 172 ms: 1.16x slower                                                   |
| Geometric mean | (ref)                                                  | 1.08x slower                                                           |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 299 us: 1.08x faster                                                   |
| unpickle_list        | 5.29 us                                                | 4.93 us: 1.07x faster                                                  |
| unpickle             | 15.9 us                                                | 14.8 us: 1.07x faster                                                  |
| pickle               | 11.6 us                                                | 11.4 us: 1.02x faster                                                  |
| xml_etree_parse      | 159 ms                                                 | 158 ms: 1.01x faster                                                   |
| json_loads           | 28.5 us                                                | 28.4 us: 1.00x faster                                                  |
| xml_etree_process    | 61.7 ms                                                | 62.2 ms: 1.01x slower                                                  |
| xml_etree_generate   | 89.2 ms                                                | 90.8 ms: 1.02x slower                                                  |
| json_dumps           | 10.4 ms                                                | 10.6 ms: 1.02x slower                                                  |
| pickle_dict          | 35.5 us                                                | 37.0 us: 1.04x slower                                                  |
| pickle_list          | 5.08 us                                                | 5.34 us: 1.05x slower                                                  |
| xml_etree_iterparse  | 107 ms                                                 | 112 ms: 1.05x slower                                                   |
| tomli_loads          | 2.33 sec                                               | 2.73 sec: 1.17x slower                                                 |
| unpickle_pure_python | 230 us                                                 | 278 us: 1.21x slower                                                   |
| Geometric mean       | (ref)                                                  | 1.02x slower                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                  |
| python_startup_no_site | 6.94 ms                                                | 8.74 ms: 1.26x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.15x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 14.0 ms: 1.18x slower                                                  |

All benchmarks:
===============

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|---------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols  | 158 us                                                 | 116 us: 1.36x faster                                                   |
| pickle_pure_python        | 324 us                                                 | 299 us: 1.08x faster                                                   |
| gc_traversal              | 3.79 ms                                                | 3.52 ms: 1.08x faster                                                  |
| unpickle_list             | 5.29 us                                                | 4.93 us: 1.07x faster                                                  |
| unpickle                  | 15.9 us                                                | 14.8 us: 1.07x faster                                                  |
| deepcopy_reduce           | 3.35 us                                                | 3.15 us: 1.06x faster                                                  |
| generators                | 31.2 ms                                                | 29.4 ms: 1.06x faster                                                  |
| tornado_http              | 103 ms                                                 | 98.0 ms: 1.05x faster                                                  |
| async_tree_none           | 472 ms                                                 | 450 ms: 1.05x faster                                                   |
| deepcopy                  | 371 us                                                 | 358 us: 1.04x faster                                                   |
| coroutines                | 23.2 ms                                                | 22.4 ms: 1.03x faster                                                  |
| sympy_sum                 | 169 ms                                                 | 164 ms: 1.03x faster                                                   |
| pickle                    | 11.6 us                                                | 11.4 us: 1.02x faster                                                  |
| chameleon                 | 7.41 ms                                                | 7.32 ms: 1.01x faster                                                  |
| async_generators          | 463 ms                                                 | 458 ms: 1.01x faster                                                   |
| xml_etree_parse           | 159 ms                                                 | 158 ms: 1.01x faster                                                   |
| pathlib                   | 19.3 ms                                                | 19.1 ms: 1.01x faster                                                  |
| json_loads                | 28.5 us                                                | 28.4 us: 1.00x faster                                                  |
| async_tree_none_tg        | 450 ms                                                 | 452 ms: 1.00x slower                                                   |
| unpack_sequence           | 54.0 ns                                                | 54.3 ns: 1.01x slower                                                  |
| xml_etree_process         | 61.7 ms                                                | 62.2 ms: 1.01x slower                                                  |
| sympy_str                 | 300 ms                                                 | 302 ms: 1.01x slower                                                   |
| sqlite_synth              | 2.83 us                                                | 2.86 us: 1.01x slower                                                  |
| pidigits                  | 187 ms                                                 | 189 ms: 1.01x slower                                                   |
| asyncio_tcp               | 491 ms                                                 | 495 ms: 1.01x slower                                                   |
| create_gc_cycles          | 1.48 ms                                                | 1.49 ms: 1.01x slower                                                  |
| mdp                       | 2.63 sec                                               | 2.66 sec: 1.01x slower                                                 |
| comprehensions            | 21.8 us                                                | 22.0 us: 1.01x slower                                                  |
| raytrace                  | 312 ms                                                 | 316 ms: 1.01x slower                                                   |
| deepcopy_memo             | 40.7 us                                                | 41.3 us: 1.01x slower                                                  |
| logging_silent            | 104 ns                                                 | 106 ns: 1.01x slower                                                   |
| asyncio_tcp_ssl           | 1.79 sec                                               | 1.81 sec: 1.01x slower                                                 |
| bench_thread_pool         | 842 us                                                 | 855 us: 1.02x slower                                                   |
| xml_etree_generate        | 89.2 ms                                                | 90.8 ms: 1.02x slower                                                  |
| sympy_integrate           | 21.4 ms                                                | 21.8 ms: 1.02x slower                                                  |
| json_dumps                | 10.4 ms                                                | 10.6 ms: 1.02x slower                                                  |
| async_tree_memoization_tg | 575 ms                                                 | 587 ms: 1.02x slower                                                   |
| async_tree_io_tg          | 1.18 sec                                               | 1.21 sec: 1.02x slower                                                 |
| docutils                  | 2.77 sec                                               | 2.85 sec: 1.03x slower                                                 |
| crypto_pyaes              | 81.9 ms                                                | 84.6 ms: 1.03x slower                                                  |
| meteor_contest            | 112 ms                                                 | 116 ms: 1.04x slower                                                   |
| pickle_dict               | 35.5 us                                                | 37.0 us: 1.04x slower                                                  |
| dulwich_log               | 68.5 ms                                                | 71.3 ms: 1.04x slower                                                  |
| sqlglot_transpile         | 1.68 ms                                                | 1.75 ms: 1.04x slower                                                  |
| async_tree_io             | 1.16 sec                                               | 1.21 sec: 1.04x slower                                                 |
| sqlglot_parse             | 1.36 ms                                                | 1.42 ms: 1.05x slower                                                  |
| pickle_list               | 5.08 us                                                | 5.34 us: 1.05x slower                                                  |
| xml_etree_iterparse       | 107 ms                                                 | 112 ms: 1.05x slower                                                   |
| sympy_expand              | 478 ms                                                 | 503 ms: 1.05x slower                                                   |
| 2to3                      | 274 ms                                                 | 290 ms: 1.06x slower                                                   |
| python_startup            | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                  |
| regex_dna                 | 212 ms                                                 | 227 ms: 1.07x slower                                                   |
| sqlglot_normalize         | 110 ms                                                 | 119 ms: 1.08x slower                                                   |
| pycparser                 | 1.18 sec                                               | 1.28 sec: 1.09x slower                                                 |
| regex_v8                  | 23.1 ms                                                | 25.2 ms: 1.09x slower                                                  |
| float                     | 84.7 ms                                                | 93.4 ms: 1.10x slower                                                  |
| sqlglot_optimize          | 54.8 ms                                                | 61.5 ms: 1.12x slower                                                  |
| pprint_safe_repr          | 776 ms                                                 | 873 ms: 1.13x slower                                                   |
| chaos                     | 67.0 ms                                                | 75.7 ms: 1.13x slower                                                  |
| pprint_pformat            | 1.57 sec                                               | 1.80 sec: 1.15x slower                                                 |
| regex_compile             | 148 ms                                                 | 172 ms: 1.16x slower                                                   |
| scimark_sor               | 129 ms                                                 | 150 ms: 1.16x slower                                                   |
| fannkuch                  | 417 ms                                                 | 485 ms: 1.16x slower                                                   |
| tomli_loads               | 2.33 sec                                               | 2.73 sec: 1.17x slower                                                 |
| mako                      | 11.9 ms                                                | 14.0 ms: 1.18x slower                                                  |
| scimark_fft               | 382 ms                                                 | 452 ms: 1.18x slower                                                   |
| nqueens                   | 83.3 ms                                                | 99.0 ms: 1.19x slower                                                  |
| scimark_monte_carlo       | 75.1 ms                                                | 89.4 ms: 1.19x slower                                                  |
| scimark_sparse_mat_mult   | 5.06 ms                                                | 6.05 ms: 1.20x slower                                                  |
| pyflate                   | 482 ms                                                 | 579 ms: 1.20x slower                                                   |
| unpickle_pure_python      | 230 us                                                 | 278 us: 1.21x slower                                                   |
| telco                     | 7.10 ms                                                | 8.72 ms: 1.23x slower                                                  |
| nbody                     | 97.0 ms                                                | 120 ms: 1.23x slower                                                   |
| python_startup_no_site    | 6.94 ms                                                | 8.74 ms: 1.26x slower                                                  |
| go                        | 139 ms                                                 | 176 ms: 1.26x slower                                                   |
| scimark_lu                | 118 ms                                                 | 152 ms: 1.29x slower                                                   |
| spectral_norm             | 115 ms                                                 | 149 ms: 1.29x slower                                                   |
| coverage                  | 72.7 ms                                                | 95.4 ms: 1.31x slower                                                  |
| deltablue                 | 3.72 ms                                                | 5.14 ms: 1.38x slower                                                  |
| hexiom                    | 6.41 ms                                                | 9.28 ms: 1.45x slower                                                  |
| richards                  | 45.8 ms                                                | 68.4 ms: 1.49x slower                                                  |
| richards_super            | 51.5 ms                                                | 77.6 ms: 1.51x slower                                                  |
| Geometric mean            | (ref)                                                  | 1.06x slower                                                           |

Benchmark hidden because not significant (11): dask, async_tree_cpu_io_mixed, logging_simple, regex_effbot, bench_mp_pool, async_tree_memoization, asyncio_websockets, logging_format, json, async_tree_cpu_io_mixed_tg, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.03x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 0.93x