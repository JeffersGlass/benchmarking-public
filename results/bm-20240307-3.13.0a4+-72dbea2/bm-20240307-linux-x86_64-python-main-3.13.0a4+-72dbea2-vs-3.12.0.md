# Results vs. 3.12.0

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: 72dbea2
- commit date: 2024-03-07
- overall geometric mean: 1.04x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240307-linux-x86_64-python-main-3.13.0a4+-72dbea2 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 262 ms: 1.05x faster                                   |
| chameleon      | 7.41 ms                                                | 6.92 ms: 1.07x faster                                  |
| docutils       | 2.77 sec                                               | 2.63 sec: 1.05x faster                                 |
| tornado_http   | 103 ms                                                 | 95.1 ms: 1.08x faster                                  |
| Geometric mean | (ref)                                                  | 1.06x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240307-linux-x86_64-python-main-3.13.0a4+-72dbea2 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 430 ms: 1.10x faster                                   |
| async_tree_memoization     | 578 ms                                                 | 554 ms: 1.04x faster                                   |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 703 ms: 1.03x faster                                   |
| async_tree_memoization_tg  | 575 ms                                                 | 562 ms: 1.02x faster                                   |
| async_tree_none_tg         | 450 ms                                                 | 443 ms: 1.01x faster                                   |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 718 ms: 1.01x faster                                   |
| async_tree_io              | 1.16 sec                                               | 1.17 sec: 1.01x slower                                 |
| Geometric mean             | (ref)                                                  | 1.03x faster                                           |

Benchmark hidden because not significant (1): async_tree_io_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240307-linux-x86_64-python-main-3.13.0a4+-72dbea2 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 92.0 ms: 1.05x faster                                  |
| float          | 84.7 ms                                                | 80.4 ms: 1.05x faster                                  |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x faster                                   |
| Geometric mean | (ref)                                                  | 1.04x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240307-linux-x86_64-python-main-3.13.0a4+-72dbea2 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 131 ms: 1.13x faster                                   |
| regex_effbot   | 3.61 ms                                                | 3.54 ms: 1.02x faster                                  |
| regex_dna      | 212 ms                                                 | 217 ms: 1.03x slower                                   |
| regex_v8       | 23.1 ms                                                | 25.2 ms: 1.09x slower                                  |
| Geometric mean | (ref)                                                  | 1.01x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240307-linux-x86_64-python-main-3.13.0a4+-72dbea2 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 296 us: 1.09x faster                                   |
| unpickle             | 15.9 us                                                | 14.6 us: 1.09x faster                                  |
| tomli_loads          | 2.33 sec                                               | 2.16 sec: 1.08x faster                                 |
| unpickle_pure_python | 230 us                                                 | 214 us: 1.08x faster                                   |
| xml_etree_process    | 61.7 ms                                                | 57.8 ms: 1.07x faster                                  |
| xml_etree_generate   | 89.2 ms                                                | 84.4 ms: 1.06x faster                                  |
| unpickle_list        | 5.29 us                                                | 5.02 us: 1.05x faster                                  |
| xml_etree_iterparse  | 107 ms                                                 | 104 ms: 1.03x faster                                   |
| xml_etree_parse      | 159 ms                                                 | 156 ms: 1.02x faster                                   |
| json_loads           | 28.5 us                                                | 28.0 us: 1.02x faster                                  |
| pickle               | 11.6 us                                                | 11.5 us: 1.01x faster                                  |
| pickle_dict          | 35.5 us                                                | 35.9 us: 1.01x slower                                  |
| Geometric mean       | (ref)                                                  | 1.04x faster                                           |

Benchmark hidden because not significant (2): json_dumps, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240307-linux-x86_64-python-main-3.13.0a4+-72dbea2 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.1 ms: 1.06x slower                                  |
| python_startup_no_site | 6.94 ms                                                | 8.72 ms: 1.26x slower                                  |
| Geometric mean         | (ref)                                                  | 1.15x slower                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240307-linux-x86_64-python-main-3.13.0a4+-72dbea2 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako            | 11.9 ms                                                | 11.1 ms: 1.07x faster                                  |
| django_template | 34.6 ms                                                | 33.8 ms: 1.02x faster                                  |
| Geometric mean  | (ref)                                                  | 1.05x faster                                           |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240307-linux-x86_64-python-main-3.13.0a4+-72dbea2 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 110 us: 1.43x faster                                   |
| comprehensions             | 21.8 us                                                | 15.8 us: 1.38x faster                                  |
| unpack_sequence            | 54.0 ns                                                | 44.7 ns: 1.21x faster                                  |
| raytrace                   | 312 ms                                                 | 262 ms: 1.19x faster                                   |
| deltablue                  | 3.72 ms                                                | 3.15 ms: 1.18x faster                                  |
| logging_format             | 7.23 us                                                | 6.15 us: 1.18x faster                                  |
| logging_simple             | 6.46 us                                                | 5.58 us: 1.16x faster                                  |
| sympy_sum                  | 169 ms                                                 | 147 ms: 1.15x faster                                   |
| crypto_pyaes               | 81.9 ms                                                | 71.7 ms: 1.14x faster                                  |
| scimark_monte_carlo        | 75.1 ms                                                | 65.9 ms: 1.14x faster                                  |
| sympy_str                  | 300 ms                                                 | 265 ms: 1.13x faster                                   |
| regex_compile              | 148 ms                                                 | 131 ms: 1.13x faster                                   |
| chaos                      | 67.0 ms                                                | 59.6 ms: 1.12x faster                                  |
| scimark_sor                | 129 ms                                                 | 116 ms: 1.11x faster                                   |
| deepcopy_reduce            | 3.35 us                                                | 3.03 us: 1.10x faster                                  |
| async_tree_none            | 472 ms                                                 | 430 ms: 1.10x faster                                   |
| sqlglot_parse              | 1.36 ms                                                | 1.24 ms: 1.10x faster                                  |
| sympy_integrate            | 21.4 ms                                                | 19.5 ms: 1.10x faster                                  |
| pickle_pure_python         | 324 us                                                 | 296 us: 1.09x faster                                   |
| unpickle                   | 15.9 us                                                | 14.6 us: 1.09x faster                                  |
| sqlglot_transpile          | 1.68 ms                                                | 1.56 ms: 1.08x faster                                  |
| tomli_loads                | 2.33 sec                                               | 2.16 sec: 1.08x faster                                 |
| deepcopy                   | 371 us                                                 | 344 us: 1.08x faster                                   |
| tornado_http               | 103 ms                                                 | 95.1 ms: 1.08x faster                                  |
| unpickle_pure_python       | 230 us                                                 | 214 us: 1.08x faster                                   |
| mako                       | 11.9 ms                                                | 11.1 ms: 1.07x faster                                  |
| chameleon                  | 7.41 ms                                                | 6.92 ms: 1.07x faster                                  |
| pprint_safe_repr           | 776 ms                                                 | 725 ms: 1.07x faster                                   |
| meteor_contest             | 112 ms                                                 | 105 ms: 1.07x faster                                   |
| xml_etree_process          | 61.7 ms                                                | 57.8 ms: 1.07x faster                                  |
| deepcopy_memo              | 40.7 us                                                | 38.2 us: 1.07x faster                                  |
| fannkuch                   | 417 ms                                                 | 391 ms: 1.07x faster                                   |
| sympy_expand               | 478 ms                                                 | 450 ms: 1.06x faster                                   |
| pyflate                    | 482 ms                                                 | 455 ms: 1.06x faster                                   |
| hexiom                     | 6.41 ms                                                | 6.04 ms: 1.06x faster                                  |
| pathlib                    | 19.3 ms                                                | 18.2 ms: 1.06x faster                                  |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 4.78 ms: 1.06x faster                                  |
| sqlglot_normalize          | 110 ms                                                 | 104 ms: 1.06x faster                                   |
| coroutines                 | 23.2 ms                                                | 21.9 ms: 1.06x faster                                  |
| xml_etree_generate         | 89.2 ms                                                | 84.4 ms: 1.06x faster                                  |
| mdp                        | 2.63 sec                                               | 2.49 sec: 1.06x faster                                 |
| nbody                      | 97.0 ms                                                | 92.0 ms: 1.05x faster                                  |
| pprint_pformat             | 1.57 sec                                               | 1.49 sec: 1.05x faster                                 |
| unpickle_list              | 5.29 us                                                | 5.02 us: 1.05x faster                                  |
| float                      | 84.7 ms                                                | 80.4 ms: 1.05x faster                                  |
| docutils                   | 2.77 sec                                               | 2.63 sec: 1.05x faster                                 |
| scimark_lu                 | 118 ms                                                 | 112 ms: 1.05x faster                                   |
| scimark_fft                | 382 ms                                                 | 364 ms: 1.05x faster                                   |
| 2to3                       | 274 ms                                                 | 262 ms: 1.05x faster                                   |
| dulwich_log                | 68.5 ms                                                | 65.4 ms: 1.05x faster                                  |
| spectral_norm              | 115 ms                                                 | 110 ms: 1.05x faster                                   |
| async_generators           | 463 ms                                                 | 443 ms: 1.05x faster                                   |
| generators                 | 31.2 ms                                                | 29.9 ms: 1.04x faster                                  |
| logging_silent             | 104 ns                                                 | 100 ns: 1.04x faster                                   |
| async_tree_memoization     | 578 ms                                                 | 554 ms: 1.04x faster                                   |
| nqueens                    | 83.3 ms                                                | 80.1 ms: 1.04x faster                                  |
| sqlglot_optimize           | 54.8 ms                                                | 52.9 ms: 1.04x faster                                  |
| gc_traversal               | 3.79 ms                                                | 3.67 ms: 1.03x faster                                  |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 703 ms: 1.03x faster                                   |
| richards                   | 45.8 ms                                                | 44.5 ms: 1.03x faster                                  |
| xml_etree_iterparse        | 107 ms                                                 | 104 ms: 1.03x faster                                   |
| go                         | 139 ms                                                 | 136 ms: 1.03x faster                                   |
| json                       | 5.26 ms                                                | 5.13 ms: 1.02x faster                                  |
| bench_thread_pool          | 842 us                                                 | 823 us: 1.02x faster                                   |
| django_template            | 34.6 ms                                                | 33.8 ms: 1.02x faster                                  |
| async_tree_memoization_tg  | 575 ms                                                 | 562 ms: 1.02x faster                                   |
| xml_etree_parse            | 159 ms                                                 | 156 ms: 1.02x faster                                   |
| regex_effbot               | 3.61 ms                                                | 3.54 ms: 1.02x faster                                  |
| richards_super             | 51.5 ms                                                | 50.7 ms: 1.02x faster                                  |
| json_loads                 | 28.5 us                                                | 28.0 us: 1.02x faster                                  |
| async_tree_none_tg         | 450 ms                                                 | 443 ms: 1.01x faster                                   |
| asyncio_tcp                | 491 ms                                                 | 484 ms: 1.01x faster                                   |
| aiohttp                    | 1.15 ms                                                | 1.14 ms: 1.01x faster                                  |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 718 ms: 1.01x faster                                   |
| pickle                     | 11.6 us                                                | 11.5 us: 1.01x faster                                  |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.78 sec: 1.00x faster                                 |
| pidigits                   | 187 ms                                                 | 187 ms: 1.00x faster                                   |
| gunicorn                   | 1.24 ms                                                | 1.25 ms: 1.00x slower                                  |
| create_gc_cycles           | 1.48 ms                                                | 1.49 ms: 1.01x slower                                  |
| pycparser                  | 1.18 sec                                               | 1.19 sec: 1.01x slower                                 |
| pickle_dict                | 35.5 us                                                | 35.9 us: 1.01x slower                                  |
| async_tree_io              | 1.16 sec                                               | 1.17 sec: 1.01x slower                                 |
| sqlite_synth               | 2.83 us                                                | 2.87 us: 1.01x slower                                  |
| regex_dna                  | 212 ms                                                 | 217 ms: 1.03x slower                                   |
| python_startup             | 9.55 ms                                                | 10.1 ms: 1.06x slower                                  |
| regex_v8                   | 23.1 ms                                                | 25.2 ms: 1.09x slower                                  |
| telco                      | 7.10 ms                                                | 8.28 ms: 1.17x slower                                  |
| python_startup_no_site     | 6.94 ms                                                | 8.72 ms: 1.26x slower                                  |
| coverage                   | 72.7 ms                                                | 95.7 ms: 1.32x slower                                  |
| dask                       | 372 ms                                                 | 519 ms: 1.40x slower                                   |
| Geometric mean             | (ref)                                                  | 1.04x faster                                           |

Benchmark hidden because not significant (6): json_dumps, asyncio_websockets, bench_mp_pool, async_tree_io_tg, pickle_list, mypy2
Ignored benchmarks (2) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (6) of results/bm-20240307-3.13.0a4+-72dbea2/bm-20240307-linux-x86_64-python-main-3.13.0a4+-72dbea2.json: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 0.93x