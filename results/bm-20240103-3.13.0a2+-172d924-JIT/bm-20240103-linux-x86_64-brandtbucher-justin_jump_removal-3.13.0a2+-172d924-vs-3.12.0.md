
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_jump_removal
- machine: linux-x86_64
- commit hash: 172d924
- commit date: 2024-01-03
- overall geometric mean: 1.01x faster
- HPT reliability: 86.88%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.96x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------------:|
| chameleon      | 7.41 ms                                                | 7.00 ms: 1.06x faster                                                       |
| docutils       | 2.77 sec                                               | 2.65 sec: 1.04x faster                                                      |
| tornado_http   | 103 ms                                                 | 96.6 ms: 1.06x faster                                                       |
| Geometric mean | (ref)                                                  | 1.04x faster                                                                |

Benchmark hidden because not significant (1): 2to3

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 441 ms: 1.07x faster                                                        |
| async_tree_memoization     | 578 ms                                                 | 570 ms: 1.01x faster                                                        |
| async_tree_io_tg           | 1.18 sec                                               | 1.19 sec: 1.00x slower                                                      |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 733 ms: 1.01x slower                                                        |
| async_tree_memoization_tg  | 575 ms                                                 | 582 ms: 1.01x slower                                                        |
| async_tree_io              | 1.16 sec                                               | 1.17 sec: 1.02x slower                                                      |
| Geometric mean             | (ref)                                                  | 1.01x faster                                                                |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed, async_tree_none_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 95.8 ms: 1.01x faster                                                       |
| float          | 84.7 ms                                                | 84.3 ms: 1.01x faster                                                       |
| pidigits       | 187 ms                                                 | 188 ms: 1.00x slower                                                        |
| Geometric mean | (ref)                                                  | 1.01x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 139 ms: 1.06x faster                                                        |
| regex_effbot   | 3.61 ms                                                | 3.68 ms: 1.02x slower                                                       |
| regex_dna      | 212 ms                                                 | 222 ms: 1.05x slower                                                        |
| regex_v8       | 23.1 ms                                                | 25.3 ms: 1.09x slower                                                       |
| Geometric mean | (ref)                                                  | 1.02x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 300 us: 1.08x faster                                                        |
| tomli_loads          | 2.33 sec                                               | 2.16 sec: 1.08x faster                                                      |
| xml_etree_process    | 61.7 ms                                                | 59.1 ms: 1.04x faster                                                       |
| unpickle             | 15.9 us                                                | 15.3 us: 1.04x faster                                                       |
| pickle_dict          | 35.5 us                                                | 34.4 us: 1.03x faster                                                       |
| xml_etree_generate   | 89.2 ms                                                | 86.9 ms: 1.03x faster                                                       |
| unpickle_pure_python | 230 us                                                 | 226 us: 1.02x faster                                                        |
| pickle_list          | 5.08 us                                                | 5.03 us: 1.01x faster                                                       |
| pickle               | 11.6 us                                                | 11.5 us: 1.01x faster                                                       |
| json_dumps           | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                       |
| unpickle_list        | 5.29 us                                                | 5.37 us: 1.02x slower                                                       |
| xml_etree_iterparse  | 107 ms                                                 | 109 ms: 1.02x slower                                                        |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                                |

Benchmark hidden because not significant (2): xml_etree_parse, json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                       |
| python_startup_no_site | 6.94 ms                                                | 8.86 ms: 1.28x slower                                                       |
| Geometric mean         | (ref)                                                  | 1.17x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|-----------|:------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 12.1 ms: 1.02x slower                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 111 us: 1.42x faster                                                        |
| comprehensions             | 21.8 us                                                | 18.3 us: 1.19x faster                                                       |
| logging_format             | 7.23 us                                                | 6.42 us: 1.13x faster                                                       |
| raytrace                   | 312 ms                                                 | 280 ms: 1.12x faster                                                        |
| logging_simple             | 6.46 us                                                | 5.92 us: 1.09x faster                                                       |
| unpack_sequence            | 54.0 ns                                                | 49.7 ns: 1.09x faster                                                       |
| pickle_pure_python         | 324 us                                                 | 300 us: 1.08x faster                                                        |
| tomli_loads                | 2.33 sec                                               | 2.16 sec: 1.08x faster                                                      |
| deepcopy_reduce            | 3.35 us                                                | 3.12 us: 1.07x faster                                                       |
| async_tree_none            | 472 ms                                                 | 441 ms: 1.07x faster                                                        |
| sympy_sum                  | 169 ms                                                 | 158 ms: 1.07x faster                                                        |
| regex_compile              | 148 ms                                                 | 139 ms: 1.06x faster                                                        |
| generators                 | 31.2 ms                                                | 29.4 ms: 1.06x faster                                                       |
| tornado_http               | 103 ms                                                 | 96.6 ms: 1.06x faster                                                       |
| sqlglot_parse              | 1.36 ms                                                | 1.28 ms: 1.06x faster                                                       |
| chameleon                  | 7.41 ms                                                | 7.00 ms: 1.06x faster                                                       |
| sympy_str                  | 300 ms                                                 | 283 ms: 1.06x faster                                                        |
| deepcopy                   | 371 us                                                 | 351 us: 1.06x faster                                                        |
| coroutines                 | 23.2 ms                                                | 22.0 ms: 1.06x faster                                                       |
| crypto_pyaes               | 81.9 ms                                                | 77.6 ms: 1.05x faster                                                       |
| pathlib                    | 19.3 ms                                                | 18.4 ms: 1.05x faster                                                       |
| scimark_sor                | 129 ms                                                 | 123 ms: 1.05x faster                                                        |
| xml_etree_process          | 61.7 ms                                                | 59.1 ms: 1.04x faster                                                       |
| docutils                   | 2.77 sec                                               | 2.65 sec: 1.04x faster                                                      |
| scimark_fft                | 382 ms                                                 | 367 ms: 1.04x faster                                                        |
| sqlglot_transpile          | 1.68 ms                                                | 1.62 ms: 1.04x faster                                                       |
| deepcopy_memo              | 40.7 us                                                | 39.2 us: 1.04x faster                                                       |
| unpickle                   | 15.9 us                                                | 15.3 us: 1.04x faster                                                       |
| pickle_dict                | 35.5 us                                                | 34.4 us: 1.03x faster                                                       |
| sympy_integrate            | 21.4 ms                                                | 20.8 ms: 1.03x faster                                                       |
| scimark_lu                 | 118 ms                                                 | 115 ms: 1.03x faster                                                        |
| xml_etree_generate         | 89.2 ms                                                | 86.9 ms: 1.03x faster                                                       |
| async_generators           | 463 ms                                                 | 452 ms: 1.02x faster                                                        |
| dulwich_log                | 68.5 ms                                                | 66.9 ms: 1.02x faster                                                       |
| dask                       | 372 ms                                                 | 365 ms: 1.02x faster                                                        |
| sqlglot_normalize          | 110 ms                                                 | 108 ms: 1.02x faster                                                        |
| unpickle_pure_python       | 230 us                                                 | 226 us: 1.02x faster                                                        |
| mdp                        | 2.63 sec                                               | 2.59 sec: 1.02x faster                                                      |
| async_tree_memoization     | 578 ms                                                 | 570 ms: 1.01x faster                                                        |
| nbody                      | 97.0 ms                                                | 95.8 ms: 1.01x faster                                                       |
| pycparser                  | 1.18 sec                                               | 1.17 sec: 1.01x faster                                                      |
| pickle_list                | 5.08 us                                                | 5.03 us: 1.01x faster                                                       |
| gc_traversal               | 3.79 ms                                                | 3.76 ms: 1.01x faster                                                       |
| scimark_monte_carlo        | 75.1 ms                                                | 74.4 ms: 1.01x faster                                                       |
| asyncio_tcp                | 491 ms                                                 | 487 ms: 1.01x faster                                                        |
| sympy_expand               | 478 ms                                                 | 474 ms: 1.01x faster                                                        |
| pickle                     | 11.6 us                                                | 11.5 us: 1.01x faster                                                       |
| float                      | 84.7 ms                                                | 84.3 ms: 1.01x faster                                                       |
| pidigits                   | 187 ms                                                 | 188 ms: 1.00x slower                                                        |
| async_tree_io_tg           | 1.18 sec                                               | 1.19 sec: 1.00x slower                                                      |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.80 sec: 1.01x slower                                                      |
| richards_super             | 51.5 ms                                                | 52.0 ms: 1.01x slower                                                       |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 733 ms: 1.01x slower                                                        |
| sqlglot_optimize           | 54.8 ms                                                | 55.4 ms: 1.01x slower                                                       |
| async_tree_memoization_tg  | 575 ms                                                 | 582 ms: 1.01x slower                                                        |
| create_gc_cycles           | 1.48 ms                                                | 1.50 ms: 1.01x slower                                                       |
| json_dumps                 | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                       |
| unpickle_list              | 5.29 us                                                | 5.37 us: 1.02x slower                                                       |
| mako                       | 11.9 ms                                                | 12.1 ms: 1.02x slower                                                       |
| pprint_safe_repr           | 776 ms                                                 | 788 ms: 1.02x slower                                                        |
| async_tree_io              | 1.16 sec                                               | 1.17 sec: 1.02x slower                                                      |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 5.14 ms: 1.02x slower                                                       |
| logging_silent             | 104 ns                                                 | 106 ns: 1.02x slower                                                        |
| xml_etree_iterparse        | 107 ms                                                 | 109 ms: 1.02x slower                                                        |
| regex_effbot               | 3.61 ms                                                | 3.68 ms: 1.02x slower                                                       |
| fannkuch                   | 417 ms                                                 | 426 ms: 1.02x slower                                                        |
| pyflate                    | 482 ms                                                 | 502 ms: 1.04x slower                                                        |
| regex_dna                  | 212 ms                                                 | 222 ms: 1.05x slower                                                        |
| pprint_pformat             | 1.57 sec                                               | 1.65 sec: 1.05x slower                                                      |
| deltablue                  | 3.72 ms                                                | 3.91 ms: 1.05x slower                                                       |
| python_startup             | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                       |
| go                         | 139 ms                                                 | 149 ms: 1.07x slower                                                        |
| nqueens                    | 83.3 ms                                                | 89.4 ms: 1.07x slower                                                       |
| regex_v8                   | 23.1 ms                                                | 25.3 ms: 1.09x slower                                                       |
| spectral_norm              | 115 ms                                                 | 131 ms: 1.14x slower                                                        |
| hexiom                     | 6.41 ms                                                | 7.58 ms: 1.18x slower                                                       |
| telco                      | 7.10 ms                                                | 8.60 ms: 1.21x slower                                                       |
| python_startup_no_site     | 6.94 ms                                                | 8.86 ms: 1.28x slower                                                       |
| coverage                   | 72.7 ms                                                | 94.6 ms: 1.30x slower                                                       |
| Geometric mean             | (ref)                                                  | 1.01x faster                                                                |

Benchmark hidden because not significant (14): async_tree_cpu_io_mixed, richards, json, xml_etree_parse, meteor_contest, async_tree_none_tg, chaos, 2to3, bench_mp_pool, sqlite_synth, bench_thread_pool, asyncio_websockets, json_loads, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 86.88% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.96x