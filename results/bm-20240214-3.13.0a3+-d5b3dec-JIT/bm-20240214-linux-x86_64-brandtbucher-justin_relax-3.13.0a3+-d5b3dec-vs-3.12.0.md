
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_relax
- machine: linux-x86_64
- commit hash: d5b3dec
- commit date: 2024-02-14
- overall geometric mean: 1.03x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 270 ms: 1.02x faster                                                 |
| chameleon      | 7.41 ms                                                | 6.82 ms: 1.09x faster                                                |
| docutils       | 2.77 sec                                               | 2.63 sec: 1.05x faster                                               |
| tornado_http   | 103 ms                                                 | 95.6 ms: 1.07x faster                                                |
| Geometric mean | (ref)                                                  | 1.06x faster                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 438 ms: 1.08x faster                                                 |
| async_tree_memoization     | 578 ms                                                 | 561 ms: 1.03x faster                                                 |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 709 ms: 1.02x faster                                                 |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 717 ms: 1.01x faster                                                 |
| async_tree_none_tg         | 450 ms                                                 | 447 ms: 1.01x faster                                                 |
| async_tree_io_tg           | 1.18 sec                                               | 1.19 sec: 1.01x slower                                               |
| async_tree_io              | 1.16 sec                                               | 1.18 sec: 1.02x slower                                               |
| Geometric mean             | (ref)                                                  | 1.02x faster                                                         |

Benchmark hidden because not significant (1): async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| float          | 84.7 ms                                                | 81.8 ms: 1.04x faster                                                |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x faster                                                 |
| nbody          | 97.0 ms                                                | 99.1 ms: 1.02x slower                                                |
| Geometric mean | (ref)                                                  | 1.00x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 134 ms: 1.11x faster                                                 |
| regex_effbot   | 3.61 ms                                                | 3.74 ms: 1.04x slower                                                |
| regex_dna      | 212 ms                                                 | 231 ms: 1.09x slower                                                 |
| regex_v8       | 23.1 ms                                                | 25.3 ms: 1.09x slower                                                |
| Geometric mean | (ref)                                                  | 1.03x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.05 sec: 1.14x faster                                               |
| pickle_pure_python   | 324 us                                                 | 293 us: 1.11x faster                                                 |
| pickle_dict          | 35.5 us                                                | 33.6 us: 1.06x faster                                                |
| xml_etree_process    | 61.7 ms                                                | 58.5 ms: 1.06x faster                                                |
| unpickle_pure_python | 230 us                                                 | 219 us: 1.05x faster                                                 |
| json_loads           | 28.5 us                                                | 27.3 us: 1.04x faster                                                |
| xml_etree_generate   | 89.2 ms                                                | 85.7 ms: 1.04x faster                                                |
| unpickle_list        | 5.29 us                                                | 5.09 us: 1.04x faster                                                |
| xml_etree_parse      | 159 ms                                                 | 155 ms: 1.03x faster                                                 |
| pickle_list          | 5.08 us                                                | 4.99 us: 1.02x faster                                                |
| json_dumps           | 10.4 ms                                                | 10.3 ms: 1.01x faster                                                |
| pickle               | 11.6 us                                                | 11.7 us: 1.01x slower                                                |
| Geometric mean       | (ref)                                                  | 1.04x faster                                                         |

Benchmark hidden because not significant (2): xml_etree_iterparse, unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.2 ms: 1.06x slower                                                |
| python_startup_no_site | 6.94 ms                                                | 8.80 ms: 1.27x slower                                                |
| Geometric mean         | (ref)                                                  | 1.16x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 11.3 ms: 1.06x faster                                                |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 111 us: 1.42x faster                                                 |
| comprehensions             | 21.8 us                                                | 18.1 us: 1.21x faster                                                |
| logging_format             | 7.23 us                                                | 6.06 us: 1.19x faster                                                |
| logging_simple             | 6.46 us                                                | 5.53 us: 1.17x faster                                                |
| unpack_sequence            | 54.0 ns                                                | 46.4 ns: 1.16x faster                                                |
| raytrace                   | 312 ms                                                 | 269 ms: 1.16x faster                                                 |
| tomli_loads                | 2.33 sec                                               | 2.05 sec: 1.14x faster                                               |
| deltablue                  | 3.72 ms                                                | 3.28 ms: 1.13x faster                                                |
| deepcopy_reduce            | 3.35 us                                                | 2.98 us: 1.12x faster                                                |
| crypto_pyaes               | 81.9 ms                                                | 73.7 ms: 1.11x faster                                                |
| regex_compile              | 148 ms                                                 | 134 ms: 1.11x faster                                                 |
| pickle_pure_python         | 324 us                                                 | 293 us: 1.11x faster                                                 |
| sympy_sum                  | 169 ms                                                 | 155 ms: 1.09x faster                                                 |
| deepcopy                   | 371 us                                                 | 341 us: 1.09x faster                                                 |
| chameleon                  | 7.41 ms                                                | 6.82 ms: 1.09x faster                                                |
| gc_traversal               | 3.79 ms                                                | 3.50 ms: 1.09x faster                                                |
| sympy_str                  | 300 ms                                                 | 276 ms: 1.08x faster                                                 |
| deepcopy_memo              | 40.7 us                                                | 37.7 us: 1.08x faster                                                |
| sqlglot_parse              | 1.36 ms                                                | 1.26 ms: 1.08x faster                                                |
| scimark_monte_carlo        | 75.1 ms                                                | 69.7 ms: 1.08x faster                                                |
| async_tree_none            | 472 ms                                                 | 438 ms: 1.08x faster                                                 |
| scimark_fft                | 382 ms                                                 | 355 ms: 1.08x faster                                                 |
| scimark_sor                | 129 ms                                                 | 120 ms: 1.07x faster                                                 |
| tornado_http               | 103 ms                                                 | 95.6 ms: 1.07x faster                                                |
| chaos                      | 67.0 ms                                                | 62.5 ms: 1.07x faster                                                |
| generators                 | 31.2 ms                                                | 29.2 ms: 1.07x faster                                                |
| sqlglot_transpile          | 1.68 ms                                                | 1.58 ms: 1.06x faster                                                |
| spectral_norm              | 115 ms                                                 | 108 ms: 1.06x faster                                                 |
| pickle_dict                | 35.5 us                                                | 33.6 us: 1.06x faster                                                |
| mako                       | 11.9 ms                                                | 11.3 ms: 1.06x faster                                                |
| xml_etree_process          | 61.7 ms                                                | 58.5 ms: 1.06x faster                                                |
| docutils                   | 2.77 sec                                               | 2.63 sec: 1.05x faster                                               |
| pprint_safe_repr           | 776 ms                                                 | 736 ms: 1.05x faster                                                 |
| pathlib                    | 19.3 ms                                                | 18.4 ms: 1.05x faster                                                |
| json                       | 5.26 ms                                                | 5.00 ms: 1.05x faster                                                |
| meteor_contest             | 112 ms                                                 | 107 ms: 1.05x faster                                                 |
| unpickle_pure_python       | 230 us                                                 | 219 us: 1.05x faster                                                 |
| sympy_integrate            | 21.4 ms                                                | 20.5 ms: 1.04x faster                                                |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 4.85 ms: 1.04x faster                                                |
| json_loads                 | 28.5 us                                                | 27.3 us: 1.04x faster                                                |
| pprint_pformat             | 1.57 sec                                               | 1.50 sec: 1.04x faster                                               |
| logging_silent             | 104 ns                                                 | 100 ns: 1.04x faster                                                 |
| scimark_lu                 | 118 ms                                                 | 113 ms: 1.04x faster                                                 |
| xml_etree_generate         | 89.2 ms                                                | 85.7 ms: 1.04x faster                                                |
| unpickle_list              | 5.29 us                                                | 5.09 us: 1.04x faster                                                |
| float                      | 84.7 ms                                                | 81.8 ms: 1.04x faster                                                |
| fannkuch                   | 417 ms                                                 | 403 ms: 1.03x faster                                                 |
| async_tree_memoization     | 578 ms                                                 | 561 ms: 1.03x faster                                                 |
| dask                       | 372 ms                                                 | 361 ms: 1.03x faster                                                 |
| xml_etree_parse            | 159 ms                                                 | 155 ms: 1.03x faster                                                 |
| dulwich_log                | 68.5 ms                                                | 66.8 ms: 1.03x faster                                                |
| sqlglot_normalize          | 110 ms                                                 | 108 ms: 1.03x faster                                                 |
| coroutines                 | 23.2 ms                                                | 22.6 ms: 1.03x faster                                                |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 709 ms: 1.02x faster                                                 |
| sympy_expand               | 478 ms                                                 | 467 ms: 1.02x faster                                                 |
| pickle_list                | 5.08 us                                                | 4.99 us: 1.02x faster                                                |
| 2to3                       | 274 ms                                                 | 270 ms: 1.02x faster                                                 |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 717 ms: 1.01x faster                                                 |
| json_dumps                 | 10.4 ms                                                | 10.3 ms: 1.01x faster                                                |
| create_gc_cycles           | 1.48 ms                                                | 1.46 ms: 1.01x faster                                                |
| pyflate                    | 482 ms                                                 | 478 ms: 1.01x faster                                                 |
| bench_thread_pool          | 842 us                                                 | 835 us: 1.01x faster                                                 |
| sqlite_synth               | 2.83 us                                                | 2.81 us: 1.01x faster                                                |
| mdp                        | 2.63 sec                                               | 2.61 sec: 1.01x faster                                               |
| async_generators           | 463 ms                                                 | 460 ms: 1.01x faster                                                 |
| async_tree_none_tg         | 450 ms                                                 | 447 ms: 1.01x faster                                                 |
| sqlglot_optimize           | 54.8 ms                                                | 54.5 ms: 1.01x faster                                                |
| pidigits                   | 187 ms                                                 | 187 ms: 1.00x faster                                                 |
| async_tree_io_tg           | 1.18 sec                                               | 1.19 sec: 1.01x slower                                               |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.80 sec: 1.01x slower                                               |
| pickle                     | 11.6 us                                                | 11.7 us: 1.01x slower                                                |
| pycparser                  | 1.18 sec                                               | 1.19 sec: 1.01x slower                                               |
| async_tree_io              | 1.16 sec                                               | 1.18 sec: 1.02x slower                                               |
| nbody                      | 97.0 ms                                                | 99.1 ms: 1.02x slower                                                |
| nqueens                    | 83.3 ms                                                | 85.4 ms: 1.02x slower                                                |
| richards_super             | 51.5 ms                                                | 53.2 ms: 1.03x slower                                                |
| go                         | 139 ms                                                 | 144 ms: 1.03x slower                                                 |
| regex_effbot               | 3.61 ms                                                | 3.74 ms: 1.04x slower                                                |
| richards                   | 45.8 ms                                                | 47.5 ms: 1.04x slower                                                |
| hexiom                     | 6.41 ms                                                | 6.81 ms: 1.06x slower                                                |
| python_startup             | 9.55 ms                                                | 10.2 ms: 1.06x slower                                                |
| regex_dna                  | 212 ms                                                 | 231 ms: 1.09x slower                                                 |
| regex_v8                   | 23.1 ms                                                | 25.3 ms: 1.09x slower                                                |
| telco                      | 7.10 ms                                                | 8.44 ms: 1.19x slower                                                |
| python_startup_no_site     | 6.94 ms                                                | 8.80 ms: 1.27x slower                                                |
| coverage                   | 72.7 ms                                                | 95.7 ms: 1.32x slower                                                |
| Geometric mean             | (ref)                                                  | 1.03x faster                                                         |

Benchmark hidden because not significant (7): async_tree_memoization_tg, xml_etree_iterparse, bench_mp_pool, asyncio_tcp, asyncio_websockets, unpickle, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.98x