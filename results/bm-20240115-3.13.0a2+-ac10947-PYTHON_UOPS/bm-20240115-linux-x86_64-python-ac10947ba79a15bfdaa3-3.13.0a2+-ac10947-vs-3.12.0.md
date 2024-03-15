
# Results vs. 3.12.0

- fork: python
- ref: ac10947ba79a15bfdaa3
- machine: linux-x86_64
- commit hash: ac10947
- commit date: 2024-01-15
- overall geometric mean: 1.05x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 284 ms: 1.04x slower                                                   |
| chameleon      | 7.41 ms                                                | 7.37 ms: 1.01x faster                                                  |
| docutils       | 2.77 sec                                               | 2.72 sec: 1.02x faster                                                 |
| tornado_http   | 103 ms                                                 | 97.7 ms: 1.05x faster                                                  |
| Geometric mean | (ref)                                                  | 1.01x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 |
|---------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none           | 472 ms                                                 | 450 ms: 1.05x faster                                                   |
| async_tree_io_tg          | 1.18 sec                                               | 1.21 sec: 1.02x slower                                                 |
| async_tree_memoization_tg | 575 ms                                                 | 588 ms: 1.02x slower                                                   |
| async_tree_io             | 1.16 sec                                               | 1.21 sec: 1.04x slower                                                 |
| Geometric mean            | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (4): async_tree_cpu_io_mixed, async_tree_memoization, async_tree_none_tg, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 197 ms: 1.05x slower                                                   |
| float          | 84.7 ms                                                | 100 ms: 1.18x slower                                                   |
| nbody          | 97.0 ms                                                | 131 ms: 1.35x slower                                                   |
| Geometric mean | (ref)                                                  | 1.19x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.64 ms: 1.01x slower                                                  |
| regex_compile  | 148 ms                                                 | 156 ms: 1.05x slower                                                   |
| regex_dna      | 212 ms                                                 | 223 ms: 1.05x slower                                                   |
| regex_v8       | 23.1 ms                                                | 24.9 ms: 1.08x slower                                                  |
| Geometric mean | (ref)                                                  | 1.05x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 302 us: 1.07x faster                                                   |
| unpickle             | 15.9 us                                                | 14.9 us: 1.07x faster                                                  |
| pickle_dict          | 35.5 us                                                | 34.9 us: 1.02x faster                                                  |
| xml_etree_parse      | 159 ms                                                 | 157 ms: 1.01x faster                                                   |
| pickle               | 11.6 us                                                | 11.7 us: 1.01x slower                                                  |
| xml_etree_generate   | 89.2 ms                                                | 90.4 ms: 1.01x slower                                                  |
| json_dumps           | 10.4 ms                                                | 10.7 ms: 1.03x slower                                                  |
| unpickle_list        | 5.29 us                                                | 5.51 us: 1.04x slower                                                  |
| unpickle_pure_python | 230 us                                                 | 240 us: 1.04x slower                                                   |
| pickle_list          | 5.08 us                                                | 5.32 us: 1.05x slower                                                  |
| xml_etree_iterparse  | 107 ms                                                 | 113 ms: 1.06x slower                                                   |
| tomli_loads          | 2.33 sec                                               | 2.54 sec: 1.09x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (2): json_loads, xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.1 ms: 1.05x slower                                                  |
| python_startup_no_site | 6.94 ms                                                | 8.71 ms: 1.26x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.15x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 15.0 ms: 1.26x slower                                                  |

All benchmarks:
===============

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 |
|---------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols  | 158 us                                                 | 116 us: 1.36x faster                                                   |
| logging_format            | 7.23 us                                                | 6.71 us: 1.08x faster                                                  |
| pickle_pure_python        | 324 us                                                 | 302 us: 1.07x faster                                                   |
| deepcopy_reduce           | 3.35 us                                                | 3.13 us: 1.07x faster                                                  |
| logging_simple            | 6.46 us                                                | 6.05 us: 1.07x faster                                                  |
| unpickle                  | 15.9 us                                                | 14.9 us: 1.07x faster                                                  |
| coroutines                | 23.2 ms                                                | 22.0 ms: 1.05x faster                                                  |
| tornado_http              | 103 ms                                                 | 97.7 ms: 1.05x faster                                                  |
| async_tree_none           | 472 ms                                                 | 450 ms: 1.05x faster                                                   |
| sympy_sum                 | 169 ms                                                 | 162 ms: 1.04x faster                                                   |
| deepcopy                  | 371 us                                                 | 358 us: 1.04x faster                                                   |
| pathlib                   | 19.3 ms                                                | 18.7 ms: 1.04x faster                                                  |
| gc_traversal              | 3.79 ms                                                | 3.70 ms: 1.02x faster                                                  |
| sqlglot_parse             | 1.36 ms                                                | 1.33 ms: 1.02x faster                                                  |
| async_generators          | 463 ms                                                 | 454 ms: 1.02x faster                                                   |
| pickle_dict               | 35.5 us                                                | 34.9 us: 1.02x faster                                                  |
| docutils                  | 2.77 sec                                               | 2.72 sec: 1.02x faster                                                 |
| sympy_str                 | 300 ms                                                 | 296 ms: 1.01x faster                                                   |
| xml_etree_parse           | 159 ms                                                 | 157 ms: 1.01x faster                                                   |
| sqlglot_transpile         | 1.68 ms                                                | 1.66 ms: 1.01x faster                                                  |
| raytrace                  | 312 ms                                                 | 308 ms: 1.01x faster                                                   |
| dask                      | 372 ms                                                 | 368 ms: 1.01x faster                                                   |
| chameleon                 | 7.41 ms                                                | 7.37 ms: 1.01x faster                                                  |
| create_gc_cycles          | 1.48 ms                                                | 1.47 ms: 1.00x faster                                                  |
| mdp                       | 2.63 sec                                               | 2.65 sec: 1.01x slower                                                 |
| scimark_lu                | 118 ms                                                 | 119 ms: 1.01x slower                                                   |
| regex_effbot              | 3.61 ms                                                | 3.64 ms: 1.01x slower                                                  |
| dulwich_log               | 68.5 ms                                                | 69.2 ms: 1.01x slower                                                  |
| asyncio_tcp_ssl           | 1.79 sec                                               | 1.80 sec: 1.01x slower                                                 |
| asyncio_tcp               | 491 ms                                                 | 496 ms: 1.01x slower                                                   |
| bench_thread_pool         | 842 us                                                 | 851 us: 1.01x slower                                                   |
| pickle                    | 11.6 us                                                | 11.7 us: 1.01x slower                                                  |
| logging_silent            | 104 ns                                                 | 106 ns: 1.01x slower                                                   |
| xml_etree_generate        | 89.2 ms                                                | 90.4 ms: 1.01x slower                                                  |
| sqlite_synth              | 2.83 us                                                | 2.88 us: 1.02x slower                                                  |
| async_tree_io_tg          | 1.18 sec                                               | 1.21 sec: 1.02x slower                                                 |
| scimark_sor               | 129 ms                                                 | 132 ms: 1.02x slower                                                   |
| async_tree_memoization_tg | 575 ms                                                 | 588 ms: 1.02x slower                                                   |
| json_dumps                | 10.4 ms                                                | 10.7 ms: 1.03x slower                                                  |
| sympy_expand              | 478 ms                                                 | 493 ms: 1.03x slower                                                   |
| 2to3                      | 274 ms                                                 | 284 ms: 1.04x slower                                                   |
| sqlglot_normalize         | 110 ms                                                 | 115 ms: 1.04x slower                                                   |
| deepcopy_memo             | 40.7 us                                                | 42.4 us: 1.04x slower                                                  |
| unpickle_list             | 5.29 us                                                | 5.51 us: 1.04x slower                                                  |
| meteor_contest            | 112 ms                                                 | 117 ms: 1.04x slower                                                   |
| async_tree_io             | 1.16 sec                                               | 1.21 sec: 1.04x slower                                                 |
| unpickle_pure_python      | 230 us                                                 | 240 us: 1.04x slower                                                   |
| pickle_list               | 5.08 us                                                | 5.32 us: 1.05x slower                                                  |
| regex_compile             | 148 ms                                                 | 156 ms: 1.05x slower                                                   |
| regex_dna                 | 212 ms                                                 | 223 ms: 1.05x slower                                                   |
| pidigits                  | 187 ms                                                 | 197 ms: 1.05x slower                                                   |
| python_startup            | 9.55 ms                                                | 10.1 ms: 1.05x slower                                                  |
| comprehensions            | 21.8 us                                                | 22.9 us: 1.05x slower                                                  |
| xml_etree_iterparse       | 107 ms                                                 | 113 ms: 1.06x slower                                                   |
| pycparser                 | 1.18 sec                                               | 1.25 sec: 1.06x slower                                                 |
| richards                  | 45.8 ms                                                | 48.9 ms: 1.07x slower                                                  |
| sqlglot_optimize          | 54.8 ms                                                | 58.6 ms: 1.07x slower                                                  |
| crypto_pyaes              | 81.9 ms                                                | 87.7 ms: 1.07x slower                                                  |
| richards_super            | 51.5 ms                                                | 55.2 ms: 1.07x slower                                                  |
| regex_v8                  | 23.1 ms                                                | 24.9 ms: 1.08x slower                                                  |
| pprint_safe_repr          | 776 ms                                                 | 845 ms: 1.09x slower                                                   |
| tomli_loads               | 2.33 sec                                               | 2.54 sec: 1.09x slower                                                 |
| pprint_pformat            | 1.57 sec                                               | 1.77 sec: 1.13x slower                                                 |
| fannkuch                  | 417 ms                                                 | 479 ms: 1.15x slower                                                   |
| scimark_monte_carlo       | 75.1 ms                                                | 86.2 ms: 1.15x slower                                                  |
| go                        | 139 ms                                                 | 160 ms: 1.15x slower                                                   |
| pyflate                   | 482 ms                                                 | 562 ms: 1.17x slower                                                   |
| generators                | 31.2 ms                                                | 36.4 ms: 1.17x slower                                                  |
| chaos                     | 67.0 ms                                                | 78.2 ms: 1.17x slower                                                  |
| float                     | 84.7 ms                                                | 100 ms: 1.18x slower                                                   |
| nqueens                   | 83.3 ms                                                | 99.2 ms: 1.19x slower                                                  |
| telco                     | 7.10 ms                                                | 8.69 ms: 1.22x slower                                                  |
| python_startup_no_site    | 6.94 ms                                                | 8.71 ms: 1.26x slower                                                  |
| scimark_fft               | 382 ms                                                 | 480 ms: 1.26x slower                                                   |
| mako                      | 11.9 ms                                                | 15.0 ms: 1.26x slower                                                  |
| scimark_sparse_mat_mult   | 5.06 ms                                                | 6.40 ms: 1.27x slower                                                  |
| coverage                  | 72.7 ms                                                | 95.7 ms: 1.32x slower                                                  |
| nbody                     | 97.0 ms                                                | 131 ms: 1.35x slower                                                   |
| deltablue                 | 3.72 ms                                                | 5.11 ms: 1.37x slower                                                  |
| spectral_norm             | 115 ms                                                 | 161 ms: 1.40x slower                                                   |
| hexiom                    | 6.41 ms                                                | 9.08 ms: 1.42x slower                                                  |
| Geometric mean            | (ref)                                                  | 1.05x slower                                                           |

Benchmark hidden because not significant (12): async_tree_cpu_io_mixed, json_loads, async_tree_memoization, sympy_integrate, bench_mp_pool, asyncio_websockets, unpack_sequence, xml_etree_process, async_tree_none_tg, json, async_tree_cpu_io_mixed_tg, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 0.93x