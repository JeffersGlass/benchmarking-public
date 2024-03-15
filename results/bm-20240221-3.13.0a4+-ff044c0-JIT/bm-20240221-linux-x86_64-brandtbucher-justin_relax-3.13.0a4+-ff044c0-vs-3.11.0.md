
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_relax
- machine: linux-x86_64
- commit hash: ff044c0
- commit date: 2024-02-21
- overall geometric mean: 1.02x faster \*
- HPT reliability: 50.62%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.23x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 280 ms: 1.06x slower                                                 |
| chameleon      | 6.70 ms                                                | 6.91 ms: 1.03x slower                                                |
| docutils       | 2.66 sec                                               | 2.72 sec: 1.02x slower                                               |
| tornado_http   | 98.1 ms                                                | 96.9 ms: 1.01x faster                                                |
| Geometric mean | (ref)                                                  | 1.02x slower                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 439 ms: 1.20x faster                                                 |
| async_tree_memoization     | 639 ms                                                 | 563 ms: 1.13x faster                                                 |
| async_tree_none_tg         | 491 ms                                                 | 447 ms: 1.10x faster                                                 |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                               |
| async_tree_memoization_tg  | 626 ms                                                 | 581 ms: 1.08x faster                                                 |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.07x faster                                               |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 708 ms: 1.06x faster                                                 |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 722 ms: 1.06x faster                                                 |
| Geometric mean             | (ref)                                                  | 1.10x faster                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                                 |
| nbody          | 96.0 ms                                                | 97.7 ms: 1.02x slower                                                |
| float          | 78.9 ms                                                | 80.7 ms: 1.02x slower                                                |
| Geometric mean | (ref)                                                  | 1.00x slower                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 150 ms: 1.06x slower                                                 |
| regex_effbot   | 3.51 ms                                                | 3.72 ms: 1.06x slower                                                |
| regex_v8       | 22.9 ms                                                | 24.7 ms: 1.08x slower                                                |
| regex_dna      | 205 ms                                                 | 224 ms: 1.09x slower                                                 |
| Geometric mean | (ref)                                                  | 1.07x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                |
| pickle_pure_python   | 320 us                                                 | 299 us: 1.07x faster                                                 |
| json_loads           | 29.2 us                                                | 27.3 us: 1.07x faster                                                |
| tomli_loads          | 2.30 sec                                               | 2.17 sec: 1.06x faster                                               |
| xml_etree_parse      | 164 ms                                                 | 157 ms: 1.04x faster                                                 |
| unpickle_list        | 5.21 us                                                | 5.01 us: 1.04x faster                                                |
| xml_etree_iterparse  | 108 ms                                                 | 106 ms: 1.02x faster                                                 |
| unpickle_pure_python | 242 us                                                 | 244 us: 1.01x slower                                                 |
| pickle_dict          | 34.6 us                                                | 35.2 us: 1.02x slower                                                |
| xml_etree_process    | 56.9 ms                                                | 59.1 ms: 1.04x slower                                                |
| xml_etree_generate   | 81.1 ms                                                | 86.6 ms: 1.07x slower                                                |
| pickle               | 11.0 us                                                | 11.8 us: 1.08x slower                                                |
| unpickle             | 13.8 us                                                | 15.1 us: 1.09x slower                                                |
| pickle_list          | 4.59 us                                                | 5.26 us: 1.15x slower                                                |
| Geometric mean       | (ref)                                                  | 1.01x faster                                                         |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 12.2 ms: 1.43x slower                                                |
| python_startup_no_site | 6.01 ms                                                | 10.9 ms: 1.81x slower                                                |
| Geometric mean         | (ref)                                                  | 1.61x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.6 ms: 1.09x slower                                                |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 108 us: 4.80x faster                                                 |
| generators                 | 74.9 ms                                                | 29.3 ms: 2.55x faster                                                |
| asyncio_tcp                | 875 ms                                                 | 497 ms: 1.76x faster                                                 |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.73x faster                                               |
| comprehensions             | 23.6 us                                                | 17.7 us: 1.33x faster                                                |
| json_dumps                 | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                |
| coroutines                 | 27.0 ms                                                | 21.7 ms: 1.24x faster                                                |
| async_tree_none            | 528 ms                                                 | 439 ms: 1.20x faster                                                 |
| gc_traversal               | 4.01 ms                                                | 3.48 ms: 1.15x faster                                                |
| deltablue                  | 3.92 ms                                                | 3.44 ms: 1.14x faster                                                |
| async_tree_memoization     | 639 ms                                                 | 563 ms: 1.13x faster                                                 |
| logging_silent             | 111 ns                                                 | 98.9 ns: 1.12x faster                                                |
| chaos                      | 71.9 ms                                                | 64.8 ms: 1.11x faster                                                |
| richards_super             | 61.9 ms                                                | 55.9 ms: 1.11x faster                                                |
| async_tree_none_tg         | 491 ms                                                 | 447 ms: 1.10x faster                                                 |
| sqlglot_parse              | 1.43 ms                                                | 1.31 ms: 1.09x faster                                                |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                               |
| async_tree_memoization_tg  | 626 ms                                                 | 581 ms: 1.08x faster                                                 |
| logging_simple             | 6.22 us                                                | 5.77 us: 1.08x faster                                                |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.07x faster                                               |
| logging_format             | 6.81 us                                                | 6.34 us: 1.07x faster                                                |
| pickle_pure_python         | 320 us                                                 | 299 us: 1.07x faster                                                 |
| json_loads                 | 29.2 us                                                | 27.3 us: 1.07x faster                                                |
| tomli_loads                | 2.30 sec                                               | 2.17 sec: 1.06x faster                                               |
| sympy_sum                  | 169 ms                                                 | 159 ms: 1.06x faster                                                 |
| sqlglot_transpile          | 1.75 ms                                                | 1.65 ms: 1.06x faster                                                |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 708 ms: 1.06x faster                                                 |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 722 ms: 1.06x faster                                                 |
| json                       | 5.24 ms                                                | 5.00 ms: 1.05x faster                                                |
| sympy_str                  | 297 ms                                                 | 284 ms: 1.05x faster                                                 |
| xml_etree_parse            | 164 ms                                                 | 157 ms: 1.04x faster                                                 |
| mdp                        | 2.77 sec                                               | 2.66 sec: 1.04x faster                                               |
| deepcopy                   | 365 us                                                 | 350 us: 1.04x faster                                                 |
| unpickle_list              | 5.21 us                                                | 5.01 us: 1.04x faster                                                |
| sqlglot_normalize          | 113 ms                                                 | 109 ms: 1.04x faster                                                 |
| deepcopy_memo              | 40.2 us                                                | 38.7 us: 1.04x faster                                                |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                                 |
| raytrace                   | 309 ms                                                 | 299 ms: 1.03x faster                                                 |
| sympy_integrate            | 21.5 ms                                                | 20.9 ms: 1.03x faster                                                |
| deepcopy_reduce            | 3.22 us                                                | 3.15 us: 1.02x faster                                                |
| crypto_pyaes               | 76.7 ms                                                | 75.5 ms: 1.02x faster                                                |
| xml_etree_iterparse        | 108 ms                                                 | 106 ms: 1.02x faster                                                 |
| tornado_http               | 98.1 ms                                                | 96.9 ms: 1.01x faster                                                |
| sympy_expand               | 484 ms                                                 | 482 ms: 1.00x faster                                                 |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                                 |
| unpickle_pure_python       | 242 us                                                 | 244 us: 1.01x slower                                                 |
| nbody                      | 96.0 ms                                                | 97.7 ms: 1.02x slower                                                |
| pickle_dict                | 34.6 us                                                | 35.2 us: 1.02x slower                                                |
| bench_thread_pool          | 834 us                                                 | 851 us: 1.02x slower                                                 |
| float                      | 78.9 ms                                                | 80.7 ms: 1.02x slower                                                |
| docutils                   | 2.66 sec                                               | 2.72 sec: 1.02x slower                                               |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.15 ms: 1.02x slower                                                |
| sqlglot_optimize           | 55.3 ms                                                | 56.7 ms: 1.03x slower                                                |
| pycparser                  | 1.19 sec                                               | 1.22 sec: 1.03x slower                                               |
| pprint_safe_repr           | 747 ms                                                 | 769 ms: 1.03x slower                                                 |
| pprint_pformat             | 1.55 sec                                               | 1.60 sec: 1.03x slower                                               |
| chameleon                  | 6.70 ms                                                | 6.91 ms: 1.03x slower                                                |
| create_gc_cycles           | 1.43 ms                                                | 1.49 ms: 1.04x slower                                                |
| scimark_fft                | 345 ms                                                 | 359 ms: 1.04x slower                                                 |
| xml_etree_process          | 56.9 ms                                                | 59.1 ms: 1.04x slower                                                |
| fannkuch                   | 405 ms                                                 | 421 ms: 1.04x slower                                                 |
| nqueens                    | 87.9 ms                                                | 91.4 ms: 1.04x slower                                                |
| 2to3                       | 264 ms                                                 | 280 ms: 1.06x slower                                                 |
| regex_compile              | 141 ms                                                 | 150 ms: 1.06x slower                                                 |
| regex_effbot               | 3.51 ms                                                | 3.72 ms: 1.06x slower                                                |
| go                         | 149 ms                                                 | 158 ms: 1.06x slower                                                 |
| xml_etree_generate         | 81.1 ms                                                | 86.6 ms: 1.07x slower                                                |
| dulwich_log                | 64.6 ms                                                | 69.2 ms: 1.07x slower                                                |
| scimark_sor                | 121 ms                                                 | 130 ms: 1.07x slower                                                 |
| pickle                     | 11.0 us                                                | 11.8 us: 1.08x slower                                                |
| scimark_monte_carlo        | 70.7 ms                                                | 76.1 ms: 1.08x slower                                                |
| regex_v8                   | 22.9 ms                                                | 24.7 ms: 1.08x slower                                                |
| mako                       | 10.7 ms                                                | 11.6 ms: 1.09x slower                                                |
| unpickle                   | 13.8 us                                                | 15.1 us: 1.09x slower                                                |
| regex_dna                  | 205 ms                                                 | 224 ms: 1.09x slower                                                 |
| hexiom                     | 6.89 ms                                                | 7.54 ms: 1.09x slower                                                |
| sqlite_synth               | 2.57 us                                                | 2.85 us: 1.11x slower                                                |
| spectral_norm              | 108 ms                                                 | 120 ms: 1.11x slower                                                 |
| scimark_lu                 | 116 ms                                                 | 131 ms: 1.13x slower                                                 |
| pickle_list                | 4.59 us                                                | 5.26 us: 1.15x slower                                                |
| bench_mp_pool              | 24.0 ms                                                | 28.0 ms: 1.17x slower                                                |
| pyflate                    | 434 ms                                                 | 508 ms: 1.17x slower                                                 |
| coverage                   | 78.8 ms                                                | 95.5 ms: 1.21x slower                                                |
| telco                      | 6.86 ms                                                | 8.44 ms: 1.23x slower                                                |
| async_generators           | 374 ms                                                 | 463 ms: 1.24x slower                                                 |
| mypy2                      | 686 ms                                                 | 883 ms: 1.29x slower                                                 |
| python_startup             | 8.56 ms                                                | 12.2 ms: 1.43x slower                                                |
| python_startup_no_site     | 6.01 ms                                                | 10.9 ms: 1.81x slower                                                |
| unpack_sequence            | 43.5 ns                                                | 132 ns: 3.05x slower                                                 |
| Geometric mean             | (ref)                                                  | 1.02x faster                                                         |

Benchmark hidden because not significant (3): richards, meteor_contest, pathlib
Ignored benchmarks (13) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 50.62% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.23x