# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_relax_absolut
- machine: linux-x86_64
- commit hash: 89ade43
- commit date: 2024-03-14
- overall geometric mean: 1.01x slower
- HPT reliability: 96.36%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 282 ms: 1.03x slower                                                         |
| chameleon      | 7.41 ms                                                | 6.89 ms: 1.08x faster                                                        |
| docutils       | 2.77 sec                                               | 2.79 sec: 1.01x slower                                                       |
| tornado_http   | 103 ms                                                 | 98.8 ms: 1.04x faster                                                        |
| Geometric mean | (ref)                                                  | 1.02x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 452 ms: 1.04x faster                                                         |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 744 ms: 1.03x slower                                                         |
| async_tree_none_tg         | 450 ms                                                 | 461 ms: 1.03x slower                                                         |
| async_tree_memoization_tg  | 575 ms                                                 | 600 ms: 1.04x slower                                                         |
| async_tree_io_tg           | 1.18 sec                                               | 1.25 sec: 1.06x slower                                                       |
| async_tree_io              | 1.16 sec                                               | 1.22 sec: 1.06x slower                                                       |
| Geometric mean             | (ref)                                                  | 1.02x slower                                                                 |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 92.3 ms: 1.05x faster                                                        |
| float          | 84.7 ms                                                | 82.7 ms: 1.02x faster                                                        |
| pidigits       | 187 ms                                                 | 189 ms: 1.01x slower                                                         |
| Geometric mean | (ref)                                                  | 1.02x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 144 ms: 1.03x faster                                                         |
| regex_effbot   | 3.61 ms                                                | 3.74 ms: 1.04x slower                                                        |
| regex_dna      | 212 ms                                                 | 227 ms: 1.07x slower                                                         |
| regex_v8       | 23.1 ms                                                | 25.9 ms: 1.12x slower                                                        |
| Geometric mean | (ref)                                                  | 1.05x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.07 sec: 1.13x faster                                                       |
| unpickle_list        | 5.29 us                                                | 4.83 us: 1.10x faster                                                        |
| pickle_pure_python   | 324 us                                                 | 301 us: 1.08x faster                                                         |
| xml_etree_process    | 61.7 ms                                                | 60.2 ms: 1.03x faster                                                        |
| unpickle             | 15.9 us                                                | 15.5 us: 1.02x faster                                                        |
| pickle_dict          | 35.5 us                                                | 34.9 us: 1.02x faster                                                        |
| xml_etree_generate   | 89.2 ms                                                | 88.3 ms: 1.01x faster                                                        |
| json_dumps           | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                        |
| xml_etree_parse      | 159 ms                                                 | 162 ms: 1.01x slower                                                         |
| xml_etree_iterparse  | 107 ms                                                 | 109 ms: 1.02x slower                                                         |
| unpickle_pure_python | 230 us                                                 | 244 us: 1.06x slower                                                         |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                                 |

Benchmark hidden because not significant (3): json_loads, pickle, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 11.5 ms: 1.20x slower                                                        |
| python_startup_no_site | 6.94 ms                                                | 10.1 ms: 1.46x slower                                                        |
| Geometric mean         | (ref)                                                  | 1.32x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako            | 11.9 ms                                                | 10.8 ms: 1.10x faster                                                        |
| django_template | 34.6 ms                                                | 34.3 ms: 1.01x faster                                                        |
| Geometric mean  | (ref)                                                  | 1.05x faster                                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 110 us: 1.43x faster                                                         |
| comprehensions             | 21.8 us                                                | 17.9 us: 1.22x faster                                                        |
| tomli_loads                | 2.33 sec                                               | 2.07 sec: 1.13x faster                                                       |
| logging_format             | 7.23 us                                                | 6.43 us: 1.12x faster                                                        |
| logging_simple             | 6.46 us                                                | 5.82 us: 1.11x faster                                                        |
| mako                       | 11.9 ms                                                | 10.8 ms: 1.10x faster                                                        |
| unpickle_list              | 5.29 us                                                | 4.83 us: 1.10x faster                                                        |
| scimark_fft                | 382 ms                                                 | 351 ms: 1.09x faster                                                         |
| pickle_pure_python         | 324 us                                                 | 301 us: 1.08x faster                                                         |
| chameleon                  | 7.41 ms                                                | 6.89 ms: 1.08x faster                                                        |
| deepcopy_reduce            | 3.35 us                                                | 3.13 us: 1.07x faster                                                        |
| deltablue                  | 3.72 ms                                                | 3.49 ms: 1.06x faster                                                        |
| crypto_pyaes               | 81.9 ms                                                | 77.2 ms: 1.06x faster                                                        |
| generators                 | 31.2 ms                                                | 29.6 ms: 1.06x faster                                                        |
| fannkuch                   | 417 ms                                                 | 397 ms: 1.05x faster                                                         |
| deepcopy                   | 371 us                                                 | 353 us: 1.05x faster                                                         |
| nbody                      | 97.0 ms                                                | 92.3 ms: 1.05x faster                                                        |
| sympy_sum                  | 169 ms                                                 | 162 ms: 1.05x faster                                                         |
| async_tree_none            | 472 ms                                                 | 452 ms: 1.04x faster                                                         |
| sympy_str                  | 300 ms                                                 | 288 ms: 1.04x faster                                                         |
| tornado_http               | 103 ms                                                 | 98.8 ms: 1.04x faster                                                        |
| logging_silent             | 104 ns                                                 | 101 ns: 1.03x faster                                                         |
| raytrace                   | 312 ms                                                 | 302 ms: 1.03x faster                                                         |
| regex_compile              | 148 ms                                                 | 144 ms: 1.03x faster                                                         |
| pathlib                    | 19.3 ms                                                | 18.8 ms: 1.03x faster                                                        |
| deepcopy_memo              | 40.7 us                                                | 39.6 us: 1.03x faster                                                        |
| sqlglot_parse              | 1.36 ms                                                | 1.33 ms: 1.03x faster                                                        |
| pprint_safe_repr           | 776 ms                                                 | 756 ms: 1.03x faster                                                         |
| xml_etree_process          | 61.7 ms                                                | 60.2 ms: 1.03x faster                                                        |
| unpickle                   | 15.9 us                                                | 15.5 us: 1.02x faster                                                        |
| float                      | 84.7 ms                                                | 82.7 ms: 1.02x faster                                                        |
| scimark_monte_carlo        | 75.1 ms                                                | 73.4 ms: 1.02x faster                                                        |
| json                       | 5.26 ms                                                | 5.16 ms: 1.02x faster                                                        |
| pickle_dict                | 35.5 us                                                | 34.9 us: 1.02x faster                                                        |
| pprint_pformat             | 1.57 sec                                               | 1.55 sec: 1.01x faster                                                       |
| sqlglot_normalize          | 110 ms                                                 | 109 ms: 1.01x faster                                                         |
| sympy_integrate            | 21.4 ms                                                | 21.2 ms: 1.01x faster                                                        |
| django_template            | 34.6 ms                                                | 34.3 ms: 1.01x faster                                                        |
| xml_etree_generate         | 89.2 ms                                                | 88.3 ms: 1.01x faster                                                        |
| coroutines                 | 23.2 ms                                                | 23.0 ms: 1.01x faster                                                        |
| sqlglot_transpile          | 1.68 ms                                                | 1.67 ms: 1.01x faster                                                        |
| meteor_contest             | 112 ms                                                 | 112 ms: 1.00x faster                                                         |
| mdp                        | 2.63 sec                                               | 2.64 sec: 1.00x slower                                                       |
| docutils                   | 2.77 sec                                               | 2.79 sec: 1.01x slower                                                       |
| pidigits                   | 187 ms                                                 | 189 ms: 1.01x slower                                                         |
| json_dumps                 | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                        |
| xml_etree_parse            | 159 ms                                                 | 162 ms: 1.01x slower                                                         |
| scimark_sor                | 129 ms                                                 | 131 ms: 1.01x slower                                                         |
| async_generators           | 463 ms                                                 | 470 ms: 1.02x slower                                                         |
| sympy_expand               | 478 ms                                                 | 487 ms: 1.02x slower                                                         |
| richards_super             | 51.5 ms                                                | 52.5 ms: 1.02x slower                                                        |
| richards                   | 45.8 ms                                                | 46.7 ms: 1.02x slower                                                        |
| bench_thread_pool          | 842 us                                                 | 858 us: 1.02x slower                                                         |
| asyncio_websockets         | 551 ms                                                 | 562 ms: 1.02x slower                                                         |
| xml_etree_iterparse        | 107 ms                                                 | 109 ms: 1.02x slower                                                         |
| dulwich_log                | 68.5 ms                                                | 70.0 ms: 1.02x slower                                                        |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 744 ms: 1.03x slower                                                         |
| async_tree_none_tg         | 450 ms                                                 | 461 ms: 1.03x slower                                                         |
| 2to3                       | 274 ms                                                 | 282 ms: 1.03x slower                                                         |
| asyncio_tcp                | 491 ms                                                 | 505 ms: 1.03x slower                                                         |
| pyflate                    | 482 ms                                                 | 497 ms: 1.03x slower                                                         |
| regex_effbot               | 3.61 ms                                                | 3.74 ms: 1.04x slower                                                        |
| gc_traversal               | 3.79 ms                                                | 3.93 ms: 1.04x slower                                                        |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.85 sec: 1.04x slower                                                       |
| sqlglot_optimize           | 54.8 ms                                                | 57.0 ms: 1.04x slower                                                        |
| create_gc_cycles           | 1.48 ms                                                | 1.54 ms: 1.04x slower                                                        |
| async_tree_memoization_tg  | 575 ms                                                 | 600 ms: 1.04x slower                                                         |
| gunicorn                   | 1.24 ms                                                | 1.30 ms: 1.05x slower                                                        |
| aiohttp                    | 1.15 ms                                                | 1.20 ms: 1.05x slower                                                        |
| spectral_norm              | 115 ms                                                 | 120 ms: 1.05x slower                                                         |
| async_tree_io_tg           | 1.18 sec                                               | 1.25 sec: 1.06x slower                                                       |
| async_tree_io              | 1.16 sec                                               | 1.22 sec: 1.06x slower                                                       |
| unpickle_pure_python       | 230 us                                                 | 244 us: 1.06x slower                                                         |
| regex_dna                  | 212 ms                                                 | 227 ms: 1.07x slower                                                         |
| pycparser                  | 1.18 sec                                               | 1.26 sec: 1.07x slower                                                       |
| nqueens                    | 83.3 ms                                                | 91.6 ms: 1.10x slower                                                        |
| regex_v8                   | 23.1 ms                                                | 25.9 ms: 1.12x slower                                                        |
| scimark_lu                 | 118 ms                                                 | 134 ms: 1.14x slower                                                         |
| go                         | 139 ms                                                 | 160 ms: 1.15x slower                                                         |
| hexiom                     | 6.41 ms                                                | 7.37 ms: 1.15x slower                                                        |
| telco                      | 7.10 ms                                                | 8.39 ms: 1.18x slower                                                        |
| python_startup             | 9.55 ms                                                | 11.5 ms: 1.20x slower                                                        |
| coverage                   | 72.7 ms                                                | 96.6 ms: 1.33x slower                                                        |
| python_startup_no_site     | 6.94 ms                                                | 10.1 ms: 1.46x slower                                                        |
| unpack_sequence            | 54.0 ns                                                | 87.5 ns: 1.62x slower                                                        |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                                 |

Benchmark hidden because not significant (11): chaos, json_loads, pickle, pickle_list, bench_mp_pool, scimark_sparse_mat_mult, async_tree_cpu_io_mixed, sqlite_synth, dask, async_tree_memoization, mypy2
Ignored benchmarks (2) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (6) of results/bm-20240314-3.13.0a5+-89ade43-JIT/bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43.json: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 96.36% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.06x