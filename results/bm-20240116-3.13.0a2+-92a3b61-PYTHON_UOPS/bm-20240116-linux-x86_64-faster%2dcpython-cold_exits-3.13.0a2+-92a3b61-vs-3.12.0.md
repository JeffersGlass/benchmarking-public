
# Results vs. 3.12.0

- fork: faster-cpython
- ref: cold_exits
- machine: linux-x86_64
- commit hash: 92a3b61
- commit date: 2024-01-16
- overall geometric mean: 1.04x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 288 ms: 1.05x slower                                                   |
| chameleon      | 7.41 ms                                                | 7.11 ms: 1.04x faster                                                  |
| docutils       | 2.77 sec                                               | 2.71 sec: 1.02x faster                                                 |
| tornado_http   | 103 ms                                                 | 98.2 ms: 1.05x faster                                                  |
| Geometric mean | (ref)                                                  | 1.01x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|---------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none           | 472 ms                                                 | 445 ms: 1.06x faster                                                   |
| async_tree_cpu_io_mixed   | 726 ms                                                 | 717 ms: 1.01x faster                                                   |
| async_tree_none_tg        | 450 ms                                                 | 452 ms: 1.01x slower                                                   |
| async_tree_io_tg          | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                 |
| async_tree_memoization_tg | 575 ms                                                 | 588 ms: 1.02x slower                                                   |
| async_tree_io             | 1.16 sec                                               | 1.20 sec: 1.04x slower                                                 |
| Geometric mean            | (ref)                                                  | 1.00x slower                                                           |

Benchmark hidden because not significant (2): async_tree_memoization, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 189 ms: 1.01x slower                                                   |
| float          | 84.7 ms                                                | 94.2 ms: 1.11x slower                                                  |
| nbody          | 97.0 ms                                                | 120 ms: 1.24x slower                                                   |
| Geometric mean | (ref)                                                  | 1.12x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.65 ms: 1.01x slower                                                  |
| regex_dna      | 212 ms                                                 | 223 ms: 1.05x slower                                                   |
| regex_v8       | 23.1 ms                                                | 24.7 ms: 1.07x slower                                                  |
| regex_compile  | 148 ms                                                 | 164 ms: 1.11x slower                                                   |
| Geometric mean | (ref)                                                  | 1.06x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 301 us: 1.08x faster                                                   |
| unpickle             | 15.9 us                                                | 14.8 us: 1.07x faster                                                  |
| pickle_dict          | 35.5 us                                                | 33.9 us: 1.05x faster                                                  |
| xml_etree_parse      | 159 ms                                                 | 157 ms: 1.01x faster                                                   |
| xml_etree_process    | 61.7 ms                                                | 60.9 ms: 1.01x faster                                                  |
| pickle               | 11.6 us                                                | 11.7 us: 1.01x slower                                                  |
| unpickle_list        | 5.29 us                                                | 5.32 us: 1.01x slower                                                  |
| pickle_list          | 5.08 us                                                | 5.13 us: 1.01x slower                                                  |
| unpickle_pure_python | 230 us                                                 | 233 us: 1.01x slower                                                   |
| xml_etree_iterparse  | 107 ms                                                 | 111 ms: 1.04x slower                                                   |
| json_dumps           | 10.4 ms                                                | 10.8 ms: 1.04x slower                                                  |
| tomli_loads          | 2.33 sec                                               | 2.49 sec: 1.07x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.00x faster                                                           |

Benchmark hidden because not significant (2): json_loads, xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.1 ms: 1.05x slower                                                  |
| python_startup_no_site | 6.94 ms                                                | 8.70 ms: 1.25x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.15x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 14.2 ms: 1.20x slower                                                  |

All benchmarks:
===============

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|---------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols  | 158 us                                                 | 117 us: 1.35x faster                                                   |
| pickle_pure_python        | 324 us                                                 | 301 us: 1.08x faster                                                   |
| generators                | 31.2 ms                                                | 29.1 ms: 1.07x faster                                                  |
| unpickle                  | 15.9 us                                                | 14.8 us: 1.07x faster                                                  |
| unpack_sequence           | 54.0 ns                                                | 50.9 ns: 1.06x faster                                                  |
| deepcopy_reduce           | 3.35 us                                                | 3.15 us: 1.06x faster                                                  |
| async_tree_none           | 472 ms                                                 | 445 ms: 1.06x faster                                                   |
| pickle_dict               | 35.5 us                                                | 33.9 us: 1.05x faster                                                  |
| tornado_http              | 103 ms                                                 | 98.2 ms: 1.05x faster                                                  |
| chameleon                 | 7.41 ms                                                | 7.11 ms: 1.04x faster                                                  |
| pathlib                   | 19.3 ms                                                | 18.6 ms: 1.04x faster                                                  |
| deepcopy                  | 371 us                                                 | 358 us: 1.04x faster                                                   |
| sympy_sum                 | 169 ms                                                 | 163 ms: 1.04x faster                                                   |
| logging_format            | 7.23 us                                                | 7.02 us: 1.03x faster                                                  |
| coroutines                | 23.2 ms                                                | 22.6 ms: 1.03x faster                                                  |
| logging_simple            | 6.46 us                                                | 6.29 us: 1.03x faster                                                  |
| raytrace                  | 312 ms                                                 | 304 ms: 1.03x faster                                                   |
| async_generators          | 463 ms                                                 | 452 ms: 1.03x faster                                                   |
| docutils                  | 2.77 sec                                               | 2.71 sec: 1.02x faster                                                 |
| sqlglot_parse             | 1.36 ms                                                | 1.33 ms: 1.02x faster                                                  |
| sympy_str                 | 300 ms                                                 | 295 ms: 1.02x faster                                                   |
| xml_etree_parse           | 159 ms                                                 | 157 ms: 1.01x faster                                                   |
| comprehensions            | 21.8 us                                                | 21.5 us: 1.01x faster                                                  |
| xml_etree_process         | 61.7 ms                                                | 60.9 ms: 1.01x faster                                                  |
| async_tree_cpu_io_mixed   | 726 ms                                                 | 717 ms: 1.01x faster                                                   |
| dask                      | 372 ms                                                 | 368 ms: 1.01x faster                                                   |
| sqlglot_transpile         | 1.68 ms                                                | 1.67 ms: 1.01x faster                                                  |
| deepcopy_memo             | 40.7 us                                                | 40.4 us: 1.01x faster                                                  |
| asyncio_tcp               | 491 ms                                                 | 493 ms: 1.01x slower                                                   |
| async_tree_none_tg        | 450 ms                                                 | 452 ms: 1.01x slower                                                   |
| pickle                    | 11.6 us                                                | 11.7 us: 1.01x slower                                                  |
| unpickle_list             | 5.29 us                                                | 5.32 us: 1.01x slower                                                  |
| bench_thread_pool         | 842 us                                                 | 848 us: 1.01x slower                                                   |
| pickle_list               | 5.08 us                                                | 5.13 us: 1.01x slower                                                  |
| pidigits                  | 187 ms                                                 | 189 ms: 1.01x slower                                                   |
| asyncio_tcp_ssl           | 1.79 sec                                               | 1.80 sec: 1.01x slower                                                 |
| scimark_lu                | 118 ms                                                 | 119 ms: 1.01x slower                                                   |
| regex_effbot              | 3.61 ms                                                | 3.65 ms: 1.01x slower                                                  |
| dulwich_log               | 68.5 ms                                                | 69.3 ms: 1.01x slower                                                  |
| scimark_sor               | 129 ms                                                 | 131 ms: 1.01x slower                                                   |
| unpickle_pure_python      | 230 us                                                 | 233 us: 1.01x slower                                                   |
| logging_silent            | 104 ns                                                 | 106 ns: 1.02x slower                                                   |
| async_tree_io_tg          | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                 |
| async_tree_memoization_tg | 575 ms                                                 | 588 ms: 1.02x slower                                                   |
| sqlite_synth              | 2.83 us                                                | 2.91 us: 1.03x slower                                                  |
| sympy_expand              | 478 ms                                                 | 492 ms: 1.03x slower                                                   |
| crypto_pyaes              | 81.9 ms                                                | 84.5 ms: 1.03x slower                                                  |
| xml_etree_iterparse       | 107 ms                                                 | 111 ms: 1.04x slower                                                   |
| json_dumps                | 10.4 ms                                                | 10.8 ms: 1.04x slower                                                  |
| meteor_contest            | 112 ms                                                 | 117 ms: 1.04x slower                                                   |
| async_tree_io             | 1.16 sec                                               | 1.20 sec: 1.04x slower                                                 |
| sqlglot_normalize         | 110 ms                                                 | 115 ms: 1.04x slower                                                   |
| regex_dna                 | 212 ms                                                 | 223 ms: 1.05x slower                                                   |
| 2to3                      | 274 ms                                                 | 288 ms: 1.05x slower                                                   |
| python_startup            | 9.55 ms                                                | 10.1 ms: 1.05x slower                                                  |
| gc_traversal              | 3.79 ms                                                | 4.00 ms: 1.05x slower                                                  |
| richards                  | 45.8 ms                                                | 48.3 ms: 1.05x slower                                                  |
| pycparser                 | 1.18 sec                                               | 1.26 sec: 1.06x slower                                                 |
| regex_v8                  | 23.1 ms                                                | 24.7 ms: 1.07x slower                                                  |
| richards_super            | 51.5 ms                                                | 55.0 ms: 1.07x slower                                                  |
| tomli_loads               | 2.33 sec                                               | 2.49 sec: 1.07x slower                                                 |
| sqlglot_optimize          | 54.8 ms                                                | 59.3 ms: 1.08x slower                                                  |
| chaos                     | 67.0 ms                                                | 74.0 ms: 1.11x slower                                                  |
| regex_compile             | 148 ms                                                 | 164 ms: 1.11x slower                                                   |
| float                     | 84.7 ms                                                | 94.2 ms: 1.11x slower                                                  |
| pprint_safe_repr          | 776 ms                                                 | 870 ms: 1.12x slower                                                   |
| pprint_pformat            | 1.57 sec                                               | 1.80 sec: 1.15x slower                                                 |
| fannkuch                  | 417 ms                                                 | 485 ms: 1.16x slower                                                   |
| nqueens                   | 83.3 ms                                                | 97.0 ms: 1.16x slower                                                  |
| mako                      | 11.9 ms                                                | 14.2 ms: 1.20x slower                                                  |
| scimark_fft               | 382 ms                                                 | 458 ms: 1.20x slower                                                   |
| scimark_monte_carlo       | 75.1 ms                                                | 90.2 ms: 1.20x slower                                                  |
| go                        | 139 ms                                                 | 168 ms: 1.21x slower                                                   |
| scimark_sparse_mat_mult   | 5.06 ms                                                | 6.12 ms: 1.21x slower                                                  |
| pyflate                   | 482 ms                                                 | 589 ms: 1.22x slower                                                   |
| telco                     | 7.10 ms                                                | 8.67 ms: 1.22x slower                                                  |
| nbody                     | 97.0 ms                                                | 120 ms: 1.24x slower                                                   |
| python_startup_no_site    | 6.94 ms                                                | 8.70 ms: 1.25x slower                                                  |
| spectral_norm             | 115 ms                                                 | 146 ms: 1.27x slower                                                   |
| deltablue                 | 3.72 ms                                                | 4.84 ms: 1.30x slower                                                  |
| coverage                  | 72.7 ms                                                | 96.1 ms: 1.32x slower                                                  |
| hexiom                    | 6.41 ms                                                | 8.74 ms: 1.36x slower                                                  |
| Geometric mean            | (ref)                                                  | 1.04x slower                                                           |

Benchmark hidden because not significant (11): async_tree_memoization, json, sympy_integrate, create_gc_cycles, bench_mp_pool, asyncio_websockets, json_loads, mdp, xml_etree_generate, async_tree_cpu_io_mixed_tg, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.93x