
# Results vs. 3.12.0

- fork: iritkatriel
- ref: expected_attrs
- machine: linux-x86_64
- commit hash: ad434a2
- commit date: 2024-02-27
- overall geometric mean: 1.05x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 262 ms: 1.05x faster                                                  |
| chameleon      | 7.41 ms                                                | 6.64 ms: 1.12x faster                                                 |
| docutils       | 2.77 sec                                               | 2.57 sec: 1.08x faster                                                |
| tornado_http   | 103 ms                                                 | 94.6 ms: 1.08x faster                                                 |
| Geometric mean | (ref)                                                  | 1.08x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|---------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_none           | 472 ms                                                 | 431 ms: 1.09x faster                                                  |
| async_tree_memoization    | 578 ms                                                 | 555 ms: 1.04x faster                                                  |
| async_tree_cpu_io_mixed   | 726 ms                                                 | 702 ms: 1.03x faster                                                  |
| async_tree_none_tg        | 450 ms                                                 | 441 ms: 1.02x faster                                                  |
| async_tree_memoization_tg | 575 ms                                                 | 567 ms: 1.01x faster                                                  |
| async_tree_io_tg          | 1.18 sec                                               | 1.19 sec: 1.01x slower                                                |
| async_tree_io             | 1.16 sec                                               | 1.17 sec: 1.01x slower                                                |
| Geometric mean            | (ref)                                                  | 1.02x faster                                                          |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 88.2 ms: 1.10x faster                                                 |
| float          | 84.7 ms                                                | 80.6 ms: 1.05x faster                                                 |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x faster                                                  |
| Geometric mean | (ref)                                                  | 1.05x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 131 ms: 1.14x faster                                                  |
| regex_dna      | 212 ms                                                 | 224 ms: 1.05x slower                                                  |
| regex_effbot   | 3.61 ms                                                | 3.81 ms: 1.05x slower                                                 |
| regex_v8       | 23.1 ms                                                | 26.3 ms: 1.14x slower                                                 |
| Geometric mean | (ref)                                                  | 1.03x slower                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 292 us: 1.11x faster                                                  |
| unpickle_pure_python | 230 us                                                 | 210 us: 1.10x faster                                                  |
| tomli_loads          | 2.33 sec                                               | 2.14 sec: 1.09x faster                                                |
| unpickle_list        | 5.29 us                                                | 4.90 us: 1.08x faster                                                 |
| xml_etree_process    | 61.7 ms                                                | 57.6 ms: 1.07x faster                                                 |
| xml_etree_generate   | 89.2 ms                                                | 84.0 ms: 1.06x faster                                                 |
| pickle_dict          | 35.5 us                                                | 33.6 us: 1.06x faster                                                 |
| unpickle             | 15.9 us                                                | 15.0 us: 1.06x faster                                                 |
| pickle_list          | 5.08 us                                                | 4.82 us: 1.06x faster                                                 |
| json_loads           | 28.5 us                                                | 27.5 us: 1.04x faster                                                 |
| xml_etree_iterparse  | 107 ms                                                 | 103 ms: 1.03x faster                                                  |
| pickle               | 11.6 us                                                | 11.4 us: 1.02x faster                                                 |
| xml_etree_parse      | 159 ms                                                 | 156 ms: 1.02x faster                                                  |
| json_dumps           | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.05x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                 |
| python_startup_no_site | 6.94 ms                                                | 8.76 ms: 1.26x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.16x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|-----------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 10.9 ms: 1.09x faster                                                 |

All benchmarks:
===============

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|---------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| typing_runtime_protocols  | 158 us                                                 | 109 us: 1.45x faster                                                  |
| comprehensions            | 21.8 us                                                | 16.3 us: 1.34x faster                                                 |
| unpack_sequence           | 54.0 ns                                                | 42.9 ns: 1.26x faster                                                 |
| raytrace                  | 312 ms                                                 | 257 ms: 1.21x faster                                                  |
| crypto_pyaes              | 81.9 ms                                                | 69.0 ms: 1.19x faster                                                 |
| deltablue                 | 3.72 ms                                                | 3.14 ms: 1.18x faster                                                 |
| sympy_sum                 | 169 ms                                                 | 146 ms: 1.16x faster                                                  |
| chaos                     | 67.0 ms                                                | 58.5 ms: 1.14x faster                                                 |
| logging_format            | 7.23 us                                                | 6.35 us: 1.14x faster                                                 |
| regex_compile             | 148 ms                                                 | 131 ms: 1.14x faster                                                  |
| scimark_monte_carlo       | 75.1 ms                                                | 66.2 ms: 1.14x faster                                                 |
| sympy_str                 | 300 ms                                                 | 264 ms: 1.13x faster                                                  |
| logging_simple            | 6.46 us                                                | 5.76 us: 1.12x faster                                                 |
| chameleon                 | 7.41 ms                                                | 6.64 ms: 1.12x faster                                                 |
| fannkuch                  | 417 ms                                                 | 376 ms: 1.11x faster                                                  |
| pickle_pure_python        | 324 us                                                 | 292 us: 1.11x faster                                                  |
| deepcopy_reduce           | 3.35 us                                                | 3.01 us: 1.11x faster                                                 |
| scimark_sor               | 129 ms                                                 | 116 ms: 1.11x faster                                                  |
| sympy_integrate           | 21.4 ms                                                | 19.3 ms: 1.11x faster                                                 |
| nbody                     | 97.0 ms                                                | 88.2 ms: 1.10x faster                                                 |
| pyflate                   | 482 ms                                                 | 439 ms: 1.10x faster                                                  |
| spectral_norm             | 115 ms                                                 | 105 ms: 1.10x faster                                                  |
| unpickle_pure_python      | 230 us                                                 | 210 us: 1.10x faster                                                  |
| sqlglot_parse             | 1.36 ms                                                | 1.24 ms: 1.10x faster                                                 |
| async_tree_none           | 472 ms                                                 | 431 ms: 1.09x faster                                                  |
| deepcopy_memo             | 40.7 us                                                | 37.3 us: 1.09x faster                                                 |
| mako                      | 11.9 ms                                                | 10.9 ms: 1.09x faster                                                 |
| deepcopy                  | 371 us                                                 | 341 us: 1.09x faster                                                  |
| tomli_loads               | 2.33 sec                                               | 2.14 sec: 1.09x faster                                                |
| hexiom                    | 6.41 ms                                                | 5.89 ms: 1.09x faster                                                 |
| generators                | 31.2 ms                                                | 28.7 ms: 1.09x faster                                                 |
| pprint_safe_repr          | 776 ms                                                 | 713 ms: 1.09x faster                                                  |
| sqlglot_transpile         | 1.68 ms                                                | 1.55 ms: 1.09x faster                                                 |
| tornado_http              | 103 ms                                                 | 94.6 ms: 1.08x faster                                                 |
| pathlib                   | 19.3 ms                                                | 17.9 ms: 1.08x faster                                                 |
| unpickle_list             | 5.29 us                                                | 4.90 us: 1.08x faster                                                 |
| docutils                  | 2.77 sec                                               | 2.57 sec: 1.08x faster                                                |
| pprint_pformat            | 1.57 sec                                               | 1.46 sec: 1.07x faster                                                |
| xml_etree_process         | 61.7 ms                                                | 57.6 ms: 1.07x faster                                                 |
| scimark_fft               | 382 ms                                                 | 357 ms: 1.07x faster                                                  |
| sympy_expand              | 478 ms                                                 | 448 ms: 1.07x faster                                                  |
| logging_silent            | 104 ns                                                 | 98.1 ns: 1.06x faster                                                 |
| xml_etree_generate        | 89.2 ms                                                | 84.0 ms: 1.06x faster                                                 |
| coroutines                | 23.2 ms                                                | 21.9 ms: 1.06x faster                                                 |
| meteor_contest            | 112 ms                                                 | 106 ms: 1.06x faster                                                  |
| scimark_lu                | 118 ms                                                 | 112 ms: 1.06x faster                                                  |
| pickle_dict               | 35.5 us                                                | 33.6 us: 1.06x faster                                                 |
| unpickle                  | 15.9 us                                                | 15.0 us: 1.06x faster                                                 |
| pickle_list               | 5.08 us                                                | 4.82 us: 1.06x faster                                                 |
| dulwich_log               | 68.5 ms                                                | 65.1 ms: 1.05x faster                                                 |
| float                     | 84.7 ms                                                | 80.6 ms: 1.05x faster                                                 |
| sqlglot_normalize         | 110 ms                                                 | 105 ms: 1.05x faster                                                  |
| 2to3                      | 274 ms                                                 | 262 ms: 1.05x faster                                                  |
| scimark_sparse_mat_mult   | 5.06 ms                                                | 4.82 ms: 1.05x faster                                                 |
| mdp                       | 2.63 sec                                               | 2.53 sec: 1.04x faster                                                |
| async_tree_memoization    | 578 ms                                                 | 555 ms: 1.04x faster                                                  |
| sqlglot_optimize          | 54.8 ms                                                | 52.7 ms: 1.04x faster                                                 |
| nqueens                   | 83.3 ms                                                | 80.3 ms: 1.04x faster                                                 |
| go                        | 139 ms                                                 | 135 ms: 1.04x faster                                                  |
| json                      | 5.26 ms                                                | 5.08 ms: 1.04x faster                                                 |
| bench_thread_pool         | 842 us                                                 | 813 us: 1.04x faster                                                  |
| json_loads                | 28.5 us                                                | 27.5 us: 1.04x faster                                                 |
| async_tree_cpu_io_mixed   | 726 ms                                                 | 702 ms: 1.03x faster                                                  |
| xml_etree_iterparse       | 107 ms                                                 | 103 ms: 1.03x faster                                                  |
| async_generators          | 463 ms                                                 | 448 ms: 1.03x faster                                                  |
| pickle                    | 11.6 us                                                | 11.4 us: 1.02x faster                                                 |
| async_tree_none_tg        | 450 ms                                                 | 441 ms: 1.02x faster                                                  |
| xml_etree_parse           | 159 ms                                                 | 156 ms: 1.02x faster                                                  |
| asyncio_tcp               | 491 ms                                                 | 482 ms: 1.02x faster                                                  |
| pycparser                 | 1.18 sec                                               | 1.16 sec: 1.02x faster                                                |
| async_tree_memoization_tg | 575 ms                                                 | 567 ms: 1.01x faster                                                  |
| asyncio_tcp_ssl           | 1.79 sec                                               | 1.78 sec: 1.00x faster                                                |
| pidigits                  | 187 ms                                                 | 187 ms: 1.00x faster                                                  |
| create_gc_cycles          | 1.48 ms                                                | 1.49 ms: 1.01x slower                                                 |
| async_tree_io_tg          | 1.18 sec                                               | 1.19 sec: 1.01x slower                                                |
| json_dumps                | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                 |
| gc_traversal              | 3.79 ms                                                | 3.84 ms: 1.01x slower                                                 |
| async_tree_io             | 1.16 sec                                               | 1.17 sec: 1.01x slower                                                |
| richards                  | 45.8 ms                                                | 47.2 ms: 1.03x slower                                                 |
| richards_super            | 51.5 ms                                                | 53.2 ms: 1.03x slower                                                 |
| regex_dna                 | 212 ms                                                 | 224 ms: 1.05x slower                                                  |
| regex_effbot              | 3.61 ms                                                | 3.81 ms: 1.05x slower                                                 |
| python_startup            | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                 |
| regex_v8                  | 23.1 ms                                                | 26.3 ms: 1.14x slower                                                 |
| telco                     | 7.10 ms                                                | 8.25 ms: 1.16x slower                                                 |
| python_startup_no_site    | 6.94 ms                                                | 8.76 ms: 1.26x slower                                                 |
| coverage                  | 72.7 ms                                                | 95.2 ms: 1.31x slower                                                 |
| Geometric mean            | (ref)                                                  | 1.05x faster                                                          |

Benchmark hidden because not significant (5): async_tree_cpu_io_mixed_tg, asyncio_websockets, bench_mp_pool, sqlite_synth, mypy2
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.04x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: 0.93x