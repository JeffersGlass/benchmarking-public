# Results vs. 3.12.0

- fork: python
- ref: ffed8d985b57a97def2e
- machine: linux-x86_64
- commit hash: ffed8d9
- commit date: 2024-03-04
- overall geometric mean: 1.06x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 0.94x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 293 ms: 1.07x slower                                                   |
| chameleon      | 7.41 ms                                                | 6.90 ms: 1.07x faster                                                  |
| docutils       | 2.77 sec                                               | 2.82 sec: 1.02x slower                                                 |
| tornado_http   | 103 ms                                                 | 99.7 ms: 1.03x faster                                                  |
| Geometric mean | (ref)                                                  | 1.00x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|---------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none           | 472 ms                                                 | 450 ms: 1.05x faster                                                   |
| async_tree_none_tg        | 450 ms                                                 | 457 ms: 1.02x slower                                                   |
| async_tree_memoization_tg | 575 ms                                                 | 590 ms: 1.03x slower                                                   |
| async_tree_io_tg          | 1.18 sec                                               | 1.23 sec: 1.04x slower                                                 |
| async_tree_io             | 1.16 sec                                               | 1.21 sec: 1.04x slower                                                 |
| Geometric mean            | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (3): async_tree_cpu_io_mixed, async_tree_memoization, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 188 ms: 1.01x slower                                                   |
| float          | 84.7 ms                                                | 95.3 ms: 1.12x slower                                                  |
| nbody          | 97.0 ms                                                | 121 ms: 1.25x slower                                                   |
| Geometric mean | (ref)                                                  | 1.12x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.45 ms: 1.05x faster                                                  |
| regex_dna      | 212 ms                                                 | 216 ms: 1.02x slower                                                   |
| regex_v8       | 23.1 ms                                                | 24.0 ms: 1.04x slower                                                  |
| regex_compile  | 148 ms                                                 | 176 ms: 1.18x slower                                                   |
| Geometric mean | (ref)                                                  | 1.05x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| unpickle_list        | 5.29 us                                                | 4.74 us: 1.11x faster                                                  |
| pickle_pure_python   | 324 us                                                 | 305 us: 1.06x faster                                                   |
| json_loads           | 28.5 us                                                | 27.5 us: 1.03x faster                                                  |
| pickle_dict          | 35.5 us                                                | 34.8 us: 1.02x faster                                                  |
| xml_etree_parse      | 159 ms                                                 | 158 ms: 1.01x faster                                                   |
| xml_etree_process    | 61.7 ms                                                | 61.5 ms: 1.00x faster                                                  |
| xml_etree_generate   | 89.2 ms                                                | 89.8 ms: 1.01x slower                                                  |
| json_dumps           | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                  |
| pickle_list          | 5.08 us                                                | 5.18 us: 1.02x slower                                                  |
| pickle               | 11.6 us                                                | 11.8 us: 1.02x slower                                                  |
| xml_etree_iterparse  | 107 ms                                                 | 111 ms: 1.04x slower                                                   |
| tomli_loads          | 2.33 sec                                               | 2.56 sec: 1.10x slower                                                 |
| unpickle_pure_python | 230 us                                                 | 282 us: 1.23x slower                                                   |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.2 ms: 1.06x slower                                                  |
| python_startup_no_site | 6.94 ms                                                | 8.81 ms: 1.27x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.16x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 13.4 ms: 1.13x slower                                                  |

All benchmarks:
===============

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|---------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols  | 158 us                                                 | 115 us: 1.38x faster                                                   |
| unpickle_list             | 5.29 us                                                | 4.74 us: 1.11x faster                                                  |
| chameleon                 | 7.41 ms                                                | 6.90 ms: 1.07x faster                                                  |
| deepcopy_reduce           | 3.35 us                                                | 3.14 us: 1.07x faster                                                  |
| pickle_pure_python        | 324 us                                                 | 305 us: 1.06x faster                                                   |
| logging_simple            | 6.46 us                                                | 6.15 us: 1.05x faster                                                  |
| async_tree_none           | 472 ms                                                 | 450 ms: 1.05x faster                                                   |
| coroutines                | 23.2 ms                                                | 22.1 ms: 1.05x faster                                                  |
| logging_format            | 7.23 us                                                | 6.91 us: 1.05x faster                                                  |
| generators                | 31.2 ms                                                | 29.8 ms: 1.05x faster                                                  |
| regex_effbot              | 3.61 ms                                                | 3.45 ms: 1.05x faster                                                  |
| deepcopy                  | 371 us                                                 | 357 us: 1.04x faster                                                   |
| json_loads                | 28.5 us                                                | 27.5 us: 1.03x faster                                                  |
| sympy_sum                 | 169 ms                                                 | 164 ms: 1.03x faster                                                   |
| tornado_http              | 103 ms                                                 | 99.7 ms: 1.03x faster                                                  |
| asyncio_tcp               | 491 ms                                                 | 478 ms: 1.03x faster                                                   |
| logging_silent            | 104 ns                                                 | 102 ns: 1.03x faster                                                   |
| json                      | 5.26 ms                                                | 5.13 ms: 1.03x faster                                                  |
| pickle_dict               | 35.5 us                                                | 34.8 us: 1.02x faster                                                  |
| pathlib                   | 19.3 ms                                                | 19.0 ms: 1.02x faster                                                  |
| xml_etree_parse           | 159 ms                                                 | 158 ms: 1.01x faster                                                   |
| sympy_integrate           | 21.4 ms                                                | 21.3 ms: 1.01x faster                                                  |
| xml_etree_process         | 61.7 ms                                                | 61.5 ms: 1.00x faster                                                  |
| comprehensions            | 21.8 us                                                | 21.7 us: 1.00x faster                                                  |
| asyncio_tcp_ssl           | 1.79 sec                                               | 1.80 sec: 1.01x slower                                                 |
| pidigits                  | 187 ms                                                 | 188 ms: 1.01x slower                                                   |
| xml_etree_generate        | 89.2 ms                                                | 89.8 ms: 1.01x slower                                                  |
| async_generators          | 463 ms                                                 | 466 ms: 1.01x slower                                                   |
| json_dumps                | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                  |
| sqlglot_normalize         | 110 ms                                                 | 112 ms: 1.01x slower                                                   |
| async_tree_none_tg        | 450 ms                                                 | 457 ms: 1.02x slower                                                   |
| deepcopy_memo             | 40.7 us                                                | 41.4 us: 1.02x slower                                                  |
| docutils                  | 2.77 sec                                               | 2.82 sec: 1.02x slower                                                 |
| pickle_list               | 5.08 us                                                | 5.18 us: 1.02x slower                                                  |
| bench_thread_pool         | 842 us                                                 | 858 us: 1.02x slower                                                   |
| pickle                    | 11.6 us                                                | 11.8 us: 1.02x slower                                                  |
| regex_dna                 | 212 ms                                                 | 216 ms: 1.02x slower                                                   |
| gc_traversal              | 3.79 ms                                                | 3.87 ms: 1.02x slower                                                  |
| create_gc_cycles          | 1.48 ms                                                | 1.51 ms: 1.02x slower                                                  |
| unpack_sequence           | 54.0 ns                                                | 55.4 ns: 1.03x slower                                                  |
| async_tree_memoization_tg | 575 ms                                                 | 590 ms: 1.03x slower                                                   |
| mdp                       | 2.63 sec                                               | 2.71 sec: 1.03x slower                                                 |
| sqlite_synth              | 2.83 us                                                | 2.92 us: 1.03x slower                                                  |
| deltablue                 | 3.72 ms                                                | 3.83 ms: 1.03x slower                                                  |
| xml_etree_iterparse       | 107 ms                                                 | 111 ms: 1.04x slower                                                   |
| async_tree_io_tg          | 1.18 sec                                               | 1.23 sec: 1.04x slower                                                 |
| regex_v8                  | 23.1 ms                                                | 24.0 ms: 1.04x slower                                                  |
| async_tree_io             | 1.16 sec                                               | 1.21 sec: 1.04x slower                                                 |
| crypto_pyaes              | 81.9 ms                                                | 85.5 ms: 1.04x slower                                                  |
| meteor_contest            | 112 ms                                                 | 118 ms: 1.05x slower                                                   |
| sqlglot_parse             | 1.36 ms                                                | 1.43 ms: 1.05x slower                                                  |
| sympy_expand              | 478 ms                                                 | 504 ms: 1.05x slower                                                   |
| sqlglot_transpile         | 1.68 ms                                                | 1.78 ms: 1.06x slower                                                  |
| dulwich_log               | 68.5 ms                                                | 72.6 ms: 1.06x slower                                                  |
| python_startup            | 9.55 ms                                                | 10.2 ms: 1.06x slower                                                  |
| 2to3                      | 274 ms                                                 | 293 ms: 1.07x slower                                                   |
| pycparser                 | 1.18 sec                                               | 1.27 sec: 1.08x slower                                                 |
| raytrace                  | 312 ms                                                 | 340 ms: 1.09x slower                                                   |
| tomli_loads               | 2.33 sec                                               | 2.56 sec: 1.10x slower                                                 |
| sqlglot_optimize          | 54.8 ms                                                | 60.5 ms: 1.10x slower                                                  |
| chaos                     | 67.0 ms                                                | 74.4 ms: 1.11x slower                                                  |
| scimark_sor               | 129 ms                                                 | 144 ms: 1.12x slower                                                   |
| float                     | 84.7 ms                                                | 95.3 ms: 1.12x slower                                                  |
| scimark_fft               | 382 ms                                                 | 430 ms: 1.13x slower                                                   |
| mako                      | 11.9 ms                                                | 13.4 ms: 1.13x slower                                                  |
| pprint_safe_repr          | 776 ms                                                 | 877 ms: 1.13x slower                                                   |
| pprint_pformat            | 1.57 sec                                               | 1.83 sec: 1.17x slower                                                 |
| scimark_sparse_mat_mult   | 5.06 ms                                                | 5.94 ms: 1.17x slower                                                  |
| regex_compile             | 148 ms                                                 | 176 ms: 1.18x slower                                                   |
| richards_super            | 51.5 ms                                                | 61.9 ms: 1.20x slower                                                  |
| fannkuch                  | 417 ms                                                 | 502 ms: 1.20x slower                                                   |
| telco                     | 7.10 ms                                                | 8.64 ms: 1.22x slower                                                  |
| spectral_norm             | 115 ms                                                 | 140 ms: 1.22x slower                                                   |
| pyflate                   | 482 ms                                                 | 589 ms: 1.22x slower                                                   |
| nqueens                   | 83.3 ms                                                | 102 ms: 1.22x slower                                                   |
| scimark_monte_carlo       | 75.1 ms                                                | 92.0 ms: 1.23x slower                                                  |
| richards                  | 45.8 ms                                                | 56.2 ms: 1.23x slower                                                  |
| unpickle_pure_python      | 230 us                                                 | 282 us: 1.23x slower                                                   |
| nbody                     | 97.0 ms                                                | 121 ms: 1.25x slower                                                   |
| python_startup_no_site    | 6.94 ms                                                | 8.81 ms: 1.27x slower                                                  |
| go                        | 139 ms                                                 | 177 ms: 1.27x slower                                                   |
| coverage                  | 72.7 ms                                                | 95.6 ms: 1.31x slower                                                  |
| scimark_lu                | 118 ms                                                 | 162 ms: 1.37x slower                                                   |
| dask                      | 372 ms                                                 | 537 ms: 1.44x slower                                                   |
| hexiom                    | 6.41 ms                                                | 9.55 ms: 1.49x slower                                                  |
| Geometric mean            | (ref)                                                  | 1.06x slower                                                           |

Benchmark hidden because not significant (8): unpickle, async_tree_cpu_io_mixed, async_tree_memoization, sympy_str, bench_mp_pool, asyncio_websockets, async_tree_cpu_io_mixed_tg, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.03x
- 95% likely to have a slowdown of 1.03x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 0.94x