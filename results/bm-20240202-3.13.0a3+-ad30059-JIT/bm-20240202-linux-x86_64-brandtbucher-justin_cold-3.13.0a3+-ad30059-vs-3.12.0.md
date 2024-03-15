
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_cold
- machine: linux-x86_64
- commit hash: ad30059
- commit date: 2024-02-02
- overall geometric mean: 1.00x slower \*
- HPT reliability: 89.73%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 277 ms: 1.01x slower                                                |
| chameleon      | 7.41 ms                                                | 6.98 ms: 1.06x faster                                               |
| docutils       | 2.77 sec                                               | 2.66 sec: 1.04x faster                                              |
| tornado_http   | 103 ms                                                 | 97.6 ms: 1.05x faster                                               |
| Geometric mean | (ref)                                                  | 1.04x faster                                                        |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|---------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| async_tree_none           | 472 ms                                                 | 441 ms: 1.07x faster                                                |
| async_tree_memoization    | 578 ms                                                 | 566 ms: 1.02x faster                                                |
| async_tree_cpu_io_mixed   | 726 ms                                                 | 713 ms: 1.02x faster                                                |
| async_tree_none_tg        | 450 ms                                                 | 454 ms: 1.01x slower                                                |
| async_tree_io_tg          | 1.18 sec                                               | 1.20 sec: 1.02x slower                                              |
| async_tree_io             | 1.16 sec                                               | 1.18 sec: 1.02x slower                                              |
| async_tree_memoization_tg | 575 ms                                                 | 593 ms: 1.03x slower                                                |
| Geometric mean            | (ref)                                                  | 1.00x faster                                                        |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 188 ms: 1.01x slower                                                |
| float          | 84.7 ms                                                | 86.5 ms: 1.02x slower                                               |
| nbody          | 97.0 ms                                                | 106 ms: 1.09x slower                                                |
| Geometric mean | (ref)                                                  | 1.04x slower                                                        |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 144 ms: 1.03x faster                                                |
| regex_effbot   | 3.61 ms                                                | 3.67 ms: 1.02x slower                                               |
| regex_dna      | 212 ms                                                 | 222 ms: 1.05x slower                                                |
| regex_v8       | 23.1 ms                                                | 24.9 ms: 1.08x slower                                               |
| Geometric mean | (ref)                                                  | 1.03x slower                                                        |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 295 us: 1.10x faster                                                |
| xml_etree_process    | 61.7 ms                                                | 58.5 ms: 1.06x faster                                               |
| tomli_loads          | 2.33 sec                                               | 2.22 sec: 1.05x faster                                              |
| unpickle_list        | 5.29 us                                                | 5.04 us: 1.05x faster                                               |
| unpickle             | 15.9 us                                                | 15.3 us: 1.04x faster                                               |
| xml_etree_generate   | 89.2 ms                                                | 86.6 ms: 1.03x faster                                               |
| xml_etree_parse      | 159 ms                                                 | 157 ms: 1.01x faster                                                |
| pickle_dict          | 35.5 us                                                | 35.1 us: 1.01x faster                                               |
| unpickle_pure_python | 230 us                                                 | 228 us: 1.01x faster                                                |
| json_loads           | 28.5 us                                                | 28.3 us: 1.01x faster                                               |
| xml_etree_iterparse  | 107 ms                                                 | 109 ms: 1.02x slower                                                |
| pickle               | 11.6 us                                                | 11.9 us: 1.02x slower                                               |
| pickle_list          | 5.08 us                                                | 5.20 us: 1.02x slower                                               |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                        |

Benchmark hidden because not significant (1): json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.2 ms: 1.07x slower                                               |
| python_startup_no_site | 6.94 ms                                                | 8.83 ms: 1.27x slower                                               |
| Geometric mean         | (ref)                                                  | 1.17x slower                                                        |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|-----------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 12.7 ms: 1.07x slower                                               |

All benchmarks:
===============

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|---------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| typing_runtime_protocols  | 158 us                                                 | 111 us: 1.42x faster                                                |
| logging_format            | 7.23 us                                                | 6.36 us: 1.14x faster                                               |
| unpack_sequence           | 54.0 ns                                                | 48.0 ns: 1.12x faster                                               |
| logging_simple            | 6.46 us                                                | 5.77 us: 1.12x faster                                               |
| comprehensions            | 21.8 us                                                | 19.7 us: 1.11x faster                                               |
| deepcopy_reduce           | 3.35 us                                                | 3.03 us: 1.10x faster                                               |
| raytrace                  | 312 ms                                                 | 283 ms: 1.10x faster                                                |
| pickle_pure_python        | 324 us                                                 | 295 us: 1.10x faster                                                |
| deepcopy_memo             | 40.7 us                                                | 37.4 us: 1.09x faster                                               |
| scimark_sor               | 129 ms                                                 | 120 ms: 1.08x faster                                                |
| deepcopy                  | 371 us                                                 | 346 us: 1.07x faster                                                |
| async_tree_none           | 472 ms                                                 | 441 ms: 1.07x faster                                                |
| chameleon                 | 7.41 ms                                                | 6.98 ms: 1.06x faster                                               |
| pathlib                   | 19.3 ms                                                | 18.2 ms: 1.06x faster                                               |
| xml_etree_process         | 61.7 ms                                                | 58.5 ms: 1.06x faster                                               |
| sqlglot_parse             | 1.36 ms                                                | 1.29 ms: 1.05x faster                                               |
| logging_silent            | 104 ns                                                 | 99.3 ns: 1.05x faster                                               |
| tomli_loads               | 2.33 sec                                               | 2.22 sec: 1.05x faster                                              |
| tornado_http              | 103 ms                                                 | 97.6 ms: 1.05x faster                                               |
| unpickle_list             | 5.29 us                                                | 5.04 us: 1.05x faster                                               |
| generators                | 31.2 ms                                                | 30.0 ms: 1.04x faster                                               |
| sympy_str                 | 300 ms                                                 | 288 ms: 1.04x faster                                                |
| sympy_sum                 | 169 ms                                                 | 162 ms: 1.04x faster                                                |
| docutils                  | 2.77 sec                                               | 2.66 sec: 1.04x faster                                              |
| sqlglot_transpile         | 1.68 ms                                                | 1.62 ms: 1.04x faster                                               |
| coroutines                | 23.2 ms                                                | 22.3 ms: 1.04x faster                                               |
| unpickle                  | 15.9 us                                                | 15.3 us: 1.04x faster                                               |
| regex_compile             | 148 ms                                                 | 144 ms: 1.03x faster                                                |
| xml_etree_generate        | 89.2 ms                                                | 86.6 ms: 1.03x faster                                               |
| scimark_lu                | 118 ms                                                 | 116 ms: 1.02x faster                                                |
| async_tree_memoization    | 578 ms                                                 | 566 ms: 1.02x faster                                                |
| async_tree_cpu_io_mixed   | 726 ms                                                 | 713 ms: 1.02x faster                                                |
| dask                      | 372 ms                                                 | 367 ms: 1.01x faster                                                |
| xml_etree_parse           | 159 ms                                                 | 157 ms: 1.01x faster                                                |
| sympy_integrate           | 21.4 ms                                                | 21.1 ms: 1.01x faster                                               |
| pickle_dict               | 35.5 us                                                | 35.1 us: 1.01x faster                                               |
| pycparser                 | 1.18 sec                                               | 1.17 sec: 1.01x faster                                              |
| unpickle_pure_python      | 230 us                                                 | 228 us: 1.01x faster                                                |
| json                      | 5.26 ms                                                | 5.20 ms: 1.01x faster                                               |
| meteor_contest            | 112 ms                                                 | 111 ms: 1.01x faster                                                |
| sqlite_synth              | 2.83 us                                                | 2.81 us: 1.01x faster                                               |
| json_loads                | 28.5 us                                                | 28.3 us: 1.01x faster                                               |
| dulwich_log               | 68.5 ms                                                | 68.0 ms: 1.01x faster                                               |
| mdp                       | 2.63 sec                                               | 2.64 sec: 1.00x slower                                              |
| bench_thread_pool         | 842 us                                                 | 845 us: 1.00x slower                                                |
| gc_traversal              | 3.79 ms                                                | 3.81 ms: 1.01x slower                                               |
| pidigits                  | 187 ms                                                 | 188 ms: 1.01x slower                                                |
| async_tree_none_tg        | 450 ms                                                 | 454 ms: 1.01x slower                                                |
| sympy_expand              | 478 ms                                                 | 482 ms: 1.01x slower                                                |
| 2to3                      | 274 ms                                                 | 277 ms: 1.01x slower                                                |
| asyncio_tcp               | 491 ms                                                 | 496 ms: 1.01x slower                                                |
| asyncio_tcp_ssl           | 1.79 sec                                               | 1.81 sec: 1.01x slower                                              |
| regex_effbot              | 3.61 ms                                                | 3.67 ms: 1.02x slower                                               |
| async_tree_io_tg          | 1.18 sec                                               | 1.20 sec: 1.02x slower                                              |
| sqlglot_optimize          | 54.8 ms                                                | 55.9 ms: 1.02x slower                                               |
| float                     | 84.7 ms                                                | 86.5 ms: 1.02x slower                                               |
| async_generators          | 463 ms                                                 | 473 ms: 1.02x slower                                                |
| xml_etree_iterparse       | 107 ms                                                 | 109 ms: 1.02x slower                                                |
| pickle                    | 11.6 us                                                | 11.9 us: 1.02x slower                                               |
| pickle_list               | 5.08 us                                                | 5.20 us: 1.02x slower                                               |
| scimark_monte_carlo       | 75.1 ms                                                | 76.9 ms: 1.02x slower                                               |
| async_tree_io             | 1.16 sec                                               | 1.18 sec: 1.02x slower                                              |
| fannkuch                  | 417 ms                                                 | 428 ms: 1.03x slower                                                |
| async_tree_memoization_tg | 575 ms                                                 | 593 ms: 1.03x slower                                                |
| regex_dna                 | 212 ms                                                 | 222 ms: 1.05x slower                                                |
| pyflate                   | 482 ms                                                 | 506 ms: 1.05x slower                                                |
| pprint_safe_repr          | 776 ms                                                 | 814 ms: 1.05x slower                                                |
| chaos                     | 67.0 ms                                                | 70.4 ms: 1.05x slower                                               |
| mako                      | 11.9 ms                                                | 12.7 ms: 1.07x slower                                               |
| python_startup            | 9.55 ms                                                | 10.2 ms: 1.07x slower                                               |
| regex_v8                  | 23.1 ms                                                | 24.9 ms: 1.08x slower                                               |
| nbody                     | 97.0 ms                                                | 106 ms: 1.09x slower                                                |
| pprint_pformat            | 1.57 sec                                               | 1.71 sec: 1.09x slower                                              |
| deltablue                 | 3.72 ms                                                | 4.06 ms: 1.09x slower                                               |
| go                        | 139 ms                                                 | 154 ms: 1.10x slower                                                |
| nqueens                   | 83.3 ms                                                | 92.0 ms: 1.11x slower                                               |
| scimark_sparse_mat_mult   | 5.06 ms                                                | 5.62 ms: 1.11x slower                                               |
| telco                     | 7.10 ms                                                | 8.49 ms: 1.20x slower                                               |
| spectral_norm             | 115 ms                                                 | 139 ms: 1.21x slower                                                |
| python_startup_no_site    | 6.94 ms                                                | 8.83 ms: 1.27x slower                                               |
| coverage                  | 72.7 ms                                                | 93.8 ms: 1.29x slower                                               |
| hexiom                    | 6.41 ms                                                | 8.28 ms: 1.29x slower                                               |
| Geometric mean            | (ref)                                                  | 1.00x slower                                                        |

Benchmark hidden because not significant (11): crypto_pyaes, richards_super, richards, sqlglot_normalize, create_gc_cycles, bench_mp_pool, asyncio_websockets, json_dumps, scimark_fft, async_tree_cpu_io_mixed_tg, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 89.73% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x