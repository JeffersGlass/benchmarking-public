# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_jumps
- machine: linux-x86_64
- commit hash: 594cca3
- commit date: 2024-02-29
- overall geometric mean: 1.01x faster \*
- HPT reliability: 99.82%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.17x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 276 ms: 1.01x slower                                                 |
| chameleon      | 7.41 ms                                                | 6.69 ms: 1.11x faster                                                |
| docutils       | 2.77 sec                                               | 2.70 sec: 1.02x faster                                               |
| tornado_http   | 103 ms                                                 | 96.6 ms: 1.06x faster                                                |
| Geometric mean | (ref)                                                  | 1.05x faster                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 434 ms: 1.09x faster                                                 |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 702 ms: 1.03x faster                                                 |
| async_tree_memoization     | 578 ms                                                 | 560 ms: 1.03x faster                                                 |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 716 ms: 1.01x faster                                                 |
| async_tree_none_tg         | 450 ms                                                 | 445 ms: 1.01x faster                                                 |
| async_tree_io_tg           | 1.18 sec                                               | 1.20 sec: 1.02x slower                                               |
| async_tree_io              | 1.16 sec                                               | 1.18 sec: 1.02x slower                                               |
| Geometric mean             | (ref)                                                  | 1.02x faster                                                         |

Benchmark hidden because not significant (1): async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| float          | 84.7 ms                                                | 78.2 ms: 1.08x faster                                                |
| nbody          | 97.0 ms                                                | 92.9 ms: 1.04x faster                                                |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x faster                                                 |
| Geometric mean | (ref)                                                  | 1.04x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 143 ms: 1.04x faster                                                 |
| regex_effbot   | 3.61 ms                                                | 3.56 ms: 1.01x faster                                                |
| regex_v8       | 23.1 ms                                                | 24.3 ms: 1.05x slower                                                |
| regex_dna      | 212 ms                                                 | 224 ms: 1.06x slower                                                 |
| Geometric mean | (ref)                                                  | 1.01x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.03 sec: 1.15x faster                                               |
| unpickle             | 15.9 us                                                | 14.6 us: 1.09x faster                                                |
| pickle_pure_python   | 324 us                                                 | 299 us: 1.08x faster                                                 |
| pickle_dict          | 35.5 us                                                | 33.3 us: 1.07x faster                                                |
| xml_etree_process    | 61.7 ms                                                | 58.2 ms: 1.06x faster                                                |
| unpickle_list        | 5.29 us                                                | 5.05 us: 1.05x faster                                                |
| json_loads           | 28.5 us                                                | 27.4 us: 1.04x faster                                                |
| xml_etree_generate   | 89.2 ms                                                | 85.9 ms: 1.04x faster                                                |
| pickle               | 11.6 us                                                | 11.3 us: 1.02x faster                                                |
| xml_etree_parse      | 159 ms                                                 | 156 ms: 1.02x faster                                                 |
| pickle_list          | 5.08 us                                                | 5.01 us: 1.01x faster                                                |
| json_dumps           | 10.4 ms                                                | 10.3 ms: 1.01x faster                                                |
| xml_etree_iterparse  | 107 ms                                                 | 106 ms: 1.01x faster                                                 |
| unpickle_pure_python | 230 us                                                 | 236 us: 1.03x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.04x faster                                                         |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 12.2 ms: 1.28x slower                                                |
| python_startup_no_site | 6.94 ms                                                | 10.9 ms: 1.57x slower                                                |
| Geometric mean         | (ref)                                                  | 1.42x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 10.8 ms: 1.10x faster                                                |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 111 us: 1.42x faster                                                 |
| comprehensions             | 21.8 us                                                | 17.0 us: 1.28x faster                                                |
| logging_format             | 7.23 us                                                | 6.17 us: 1.17x faster                                                |
| logging_simple             | 6.46 us                                                | 5.61 us: 1.15x faster                                                |
| tomli_loads                | 2.33 sec                                               | 2.03 sec: 1.15x faster                                               |
| scimark_fft                | 382 ms                                                 | 337 ms: 1.13x faster                                                 |
| crypto_pyaes               | 81.9 ms                                                | 72.5 ms: 1.13x faster                                                |
| chameleon                  | 7.41 ms                                                | 6.69 ms: 1.11x faster                                                |
| mako                       | 11.9 ms                                                | 10.8 ms: 1.10x faster                                                |
| deepcopy_reduce            | 3.35 us                                                | 3.05 us: 1.10x faster                                                |
| deltablue                  | 3.72 ms                                                | 3.40 ms: 1.09x faster                                                |
| async_tree_none            | 472 ms                                                 | 434 ms: 1.09x faster                                                 |
| unpickle                   | 15.9 us                                                | 14.6 us: 1.09x faster                                                |
| pickle_pure_python         | 324 us                                                 | 299 us: 1.08x faster                                                 |
| float                      | 84.7 ms                                                | 78.2 ms: 1.08x faster                                                |
| raytrace                   | 312 ms                                                 | 288 ms: 1.08x faster                                                 |
| chaos                      | 67.0 ms                                                | 62.4 ms: 1.07x faster                                                |
| sympy_sum                  | 169 ms                                                 | 158 ms: 1.07x faster                                                 |
| sympy_str                  | 300 ms                                                 | 281 ms: 1.07x faster                                                 |
| pickle_dict                | 35.5 us                                                | 33.3 us: 1.07x faster                                                |
| generators                 | 31.2 ms                                                | 29.3 ms: 1.06x faster                                                |
| tornado_http               | 103 ms                                                 | 96.6 ms: 1.06x faster                                                |
| deepcopy                   | 371 us                                                 | 350 us: 1.06x faster                                                 |
| xml_etree_process          | 61.7 ms                                                | 58.2 ms: 1.06x faster                                                |
| scimark_monte_carlo        | 75.1 ms                                                | 70.9 ms: 1.06x faster                                                |
| sqlglot_parse              | 1.36 ms                                                | 1.29 ms: 1.06x faster                                                |
| fannkuch                   | 417 ms                                                 | 396 ms: 1.05x faster                                                 |
| json                       | 5.26 ms                                                | 5.00 ms: 1.05x faster                                                |
| unpickle_list              | 5.29 us                                                | 5.05 us: 1.05x faster                                                |
| deepcopy_memo              | 40.7 us                                                | 38.9 us: 1.05x faster                                                |
| pathlib                    | 19.3 ms                                                | 18.5 ms: 1.05x faster                                                |
| pprint_safe_repr           | 776 ms                                                 | 742 ms: 1.04x faster                                                 |
| logging_silent             | 104 ns                                                 | 100.0 ns: 1.04x faster                                               |
| nbody                      | 97.0 ms                                                | 92.9 ms: 1.04x faster                                                |
| meteor_contest             | 112 ms                                                 | 108 ms: 1.04x faster                                                 |
| regex_compile              | 148 ms                                                 | 143 ms: 1.04x faster                                                 |
| json_loads                 | 28.5 us                                                | 27.4 us: 1.04x faster                                                |
| xml_etree_generate         | 89.2 ms                                                | 85.9 ms: 1.04x faster                                                |
| sqlglot_transpile          | 1.68 ms                                                | 1.63 ms: 1.04x faster                                                |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 702 ms: 1.03x faster                                                 |
| async_tree_memoization     | 578 ms                                                 | 560 ms: 1.03x faster                                                 |
| sqlglot_normalize          | 110 ms                                                 | 107 ms: 1.03x faster                                                 |
| scimark_sor                | 129 ms                                                 | 126 ms: 1.03x faster                                                 |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 4.93 ms: 1.03x faster                                                |
| sympy_integrate            | 21.4 ms                                                | 20.9 ms: 1.03x faster                                                |
| docutils                   | 2.77 sec                                               | 2.70 sec: 1.02x faster                                               |
| pickle                     | 11.6 us                                                | 11.3 us: 1.02x faster                                                |
| xml_etree_parse            | 159 ms                                                 | 156 ms: 1.02x faster                                                 |
| spectral_norm              | 115 ms                                                 | 113 ms: 1.02x faster                                                 |
| pickle_list                | 5.08 us                                                | 5.01 us: 1.01x faster                                                |
| pycparser                  | 1.18 sec                                               | 1.16 sec: 1.01x faster                                               |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 716 ms: 1.01x faster                                                 |
| regex_effbot               | 3.61 ms                                                | 3.56 ms: 1.01x faster                                                |
| pprint_pformat             | 1.57 sec                                               | 1.55 sec: 1.01x faster                                               |
| async_generators           | 463 ms                                                 | 457 ms: 1.01x faster                                                 |
| coroutines                 | 23.2 ms                                                | 22.9 ms: 1.01x faster                                                |
| gc_traversal               | 3.79 ms                                                | 3.75 ms: 1.01x faster                                                |
| async_tree_none_tg         | 450 ms                                                 | 445 ms: 1.01x faster                                                 |
| sqlite_synth               | 2.83 us                                                | 2.81 us: 1.01x faster                                                |
| json_dumps                 | 10.4 ms                                                | 10.3 ms: 1.01x faster                                                |
| mdp                        | 2.63 sec                                               | 2.61 sec: 1.01x faster                                               |
| asyncio_tcp                | 491 ms                                                 | 488 ms: 1.01x faster                                                 |
| xml_etree_iterparse        | 107 ms                                                 | 106 ms: 1.01x faster                                                 |
| pidigits                   | 187 ms                                                 | 187 ms: 1.00x faster                                                 |
| dulwich_log                | 68.5 ms                                                | 68.7 ms: 1.00x slower                                                |
| pyflate                    | 482 ms                                                 | 484 ms: 1.00x slower                                                 |
| bench_thread_pool          | 842 us                                                 | 846 us: 1.01x slower                                                 |
| 2to3                       | 274 ms                                                 | 276 ms: 1.01x slower                                                 |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.80 sec: 1.01x slower                                               |
| create_gc_cycles           | 1.48 ms                                                | 1.49 ms: 1.01x slower                                                |
| richards_super             | 51.5 ms                                                | 52.2 ms: 1.01x slower                                                |
| async_tree_io_tg           | 1.18 sec                                               | 1.20 sec: 1.02x slower                                               |
| richards                   | 45.8 ms                                                | 46.7 ms: 1.02x slower                                                |
| async_tree_io              | 1.16 sec                                               | 1.18 sec: 1.02x slower                                               |
| sqlglot_optimize           | 54.8 ms                                                | 56.0 ms: 1.02x slower                                                |
| unpickle_pure_python       | 230 us                                                 | 236 us: 1.03x slower                                                 |
| regex_v8                   | 23.1 ms                                                | 24.3 ms: 1.05x slower                                                |
| regex_dna                  | 212 ms                                                 | 224 ms: 1.06x slower                                                 |
| nqueens                    | 83.3 ms                                                | 90.7 ms: 1.09x slower                                                |
| hexiom                     | 6.41 ms                                                | 7.02 ms: 1.09x slower                                                |
| scimark_lu                 | 118 ms                                                 | 131 ms: 1.11x slower                                                 |
| go                         | 139 ms                                                 | 157 ms: 1.13x slower                                                 |
| bench_mp_pool              | 24.0 ms                                                | 27.8 ms: 1.16x slower                                                |
| telco                      | 7.10 ms                                                | 8.37 ms: 1.18x slower                                                |
| python_startup             | 9.55 ms                                                | 12.2 ms: 1.28x slower                                                |
| coverage                   | 72.7 ms                                                | 95.6 ms: 1.31x slower                                                |
| python_startup_no_site     | 6.94 ms                                                | 10.9 ms: 1.57x slower                                                |
| unpack_sequence            | 54.0 ns                                                | 84.9 ns: 1.57x slower                                                |
| Geometric mean             | (ref)                                                  | 1.01x faster                                                         |

Benchmark hidden because not significant (4): async_tree_memoization_tg, sympy_expand, asyncio_websockets, mypy2
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.82% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.17x