
# Results vs. 3.11.0

- fork: brandtbucher
- ref: counter_table
- machine: linux-x86_64
- commit hash: c49f898
- commit date: 2024-01-04
- overall geometric mean: 1.06x faster
- HPT reliability: 99.99%
- HPT 99th percentile: 1.01x faster
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 266 ms: 1.00x slower                                                  |
| chameleon      | 6.70 ms                                                | 6.96 ms: 1.04x slower                                                 |
| docutils       | 2.66 sec                                               | 2.62 sec: 1.02x faster                                                |
| tornado_http   | 98.1 ms                                                | 94.9 ms: 1.03x faster                                                 |
| Geometric mean | (ref)                                                  | 1.00x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 436 ms: 1.21x faster                                                  |
| async_tree_memoization     | 639 ms                                                 | 562 ms: 1.14x faster                                                  |
| async_tree_none_tg         | 491 ms                                                 | 443 ms: 1.11x faster                                                  |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                                |
| async_tree_memoization_tg  | 626 ms                                                 | 579 ms: 1.08x faster                                                  |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                                |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 707 ms: 1.06x faster                                                  |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 721 ms: 1.06x faster                                                  |
| Geometric mean             | (ref)                                                  | 1.10x faster                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 88.9 ms: 1.08x faster                                                 |
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                                  |
| float          | 78.9 ms                                                | 80.2 ms: 1.02x slower                                                 |
| Geometric mean | (ref)                                                  | 1.03x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 131 ms: 1.08x faster                                                  |
| regex_effbot   | 3.51 ms                                                | 3.60 ms: 1.03x slower                                                 |
| regex_dna      | 205 ms                                                 | 217 ms: 1.06x slower                                                  |
| regex_v8       | 22.9 ms                                                | 25.4 ms: 1.11x slower                                                 |
| Geometric mean | (ref)                                                  | 1.03x slower                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                 |
| unpickle_pure_python | 242 us                                                 | 218 us: 1.11x faster                                                  |
| pickle_pure_python   | 320 us                                                 | 295 us: 1.08x faster                                                  |
| tomli_loads          | 2.30 sec                                               | 2.13 sec: 1.08x faster                                                |
| xml_etree_parse      | 164 ms                                                 | 157 ms: 1.04x faster                                                  |
| json_loads           | 29.2 us                                                | 28.2 us: 1.03x faster                                                 |
| xml_etree_iterparse  | 108 ms                                                 | 106 ms: 1.02x faster                                                  |
| pickle_dict          | 34.6 us                                                | 34.9 us: 1.01x slower                                                 |
| unpickle_list        | 5.21 us                                                | 5.29 us: 1.02x slower                                                 |
| pickle               | 11.0 us                                                | 11.3 us: 1.03x slower                                                 |
| xml_etree_process    | 56.9 ms                                                | 60.1 ms: 1.06x slower                                                 |
| pickle_list          | 4.59 us                                                | 4.87 us: 1.06x slower                                                 |
| xml_etree_generate   | 81.1 ms                                                | 87.2 ms: 1.08x slower                                                 |
| unpickle             | 13.8 us                                                | 15.8 us: 1.14x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                 |
| python_startup_no_site | 6.01 ms                                                | 8.82 ms: 1.47x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.32x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898 |
|-----------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 10.9 ms: 1.03x slower                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 112 us: 4.66x faster                                                  |
| generators                 | 74.9 ms                                                | 29.7 ms: 2.52x faster                                                 |
| asyncio_tcp                | 875 ms                                                 | 488 ms: 1.79x faster                                                  |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.79 sec: 1.74x faster                                                |
| comprehensions             | 23.6 us                                                | 16.6 us: 1.43x faster                                                 |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                 |
| coroutines                 | 27.0 ms                                                | 21.5 ms: 1.26x faster                                                 |
| chaos                      | 71.9 ms                                                | 58.8 ms: 1.22x faster                                                 |
| async_tree_none            | 528 ms                                                 | 436 ms: 1.21x faster                                                  |
| deltablue                  | 3.92 ms                                                | 3.24 ms: 1.21x faster                                                 |
| raytrace                   | 309 ms                                                 | 261 ms: 1.18x faster                                                  |
| sqlglot_parse              | 1.43 ms                                                | 1.25 ms: 1.14x faster                                                 |
| async_tree_memoization     | 639 ms                                                 | 562 ms: 1.14x faster                                                  |
| sympy_sum                  | 169 ms                                                 | 149 ms: 1.14x faster                                                  |
| richards_super             | 61.9 ms                                                | 55.1 ms: 1.12x faster                                                 |
| gc_traversal               | 4.01 ms                                                | 3.60 ms: 1.11x faster                                                 |
| sqlglot_transpile          | 1.75 ms                                                | 1.58 ms: 1.11x faster                                                 |
| unpickle_pure_python       | 242 us                                                 | 218 us: 1.11x faster                                                  |
| async_tree_none_tg         | 491 ms                                                 | 443 ms: 1.11x faster                                                  |
| sympy_str                  | 297 ms                                                 | 270 ms: 1.10x faster                                                  |
| logging_simple             | 6.22 us                                                | 5.64 us: 1.10x faster                                                 |
| hexiom                     | 6.89 ms                                                | 6.27 ms: 1.10x faster                                                 |
| logging_format             | 6.81 us                                                | 6.24 us: 1.09x faster                                                 |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                                |
| sympy_integrate            | 21.5 ms                                                | 19.8 ms: 1.09x faster                                                 |
| pickle_pure_python         | 320 us                                                 | 295 us: 1.08x faster                                                  |
| async_tree_memoization_tg  | 626 ms                                                 | 579 ms: 1.08x faster                                                  |
| tomli_loads                | 2.30 sec                                               | 2.13 sec: 1.08x faster                                                |
| regex_compile              | 141 ms                                                 | 131 ms: 1.08x faster                                                  |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                                |
| nbody                      | 96.0 ms                                                | 88.9 ms: 1.08x faster                                                 |
| go                         | 149 ms                                                 | 138 ms: 1.08x faster                                                  |
| crypto_pyaes               | 76.7 ms                                                | 71.5 ms: 1.07x faster                                                 |
| logging_silent             | 111 ns                                                 | 104 ns: 1.07x faster                                                  |
| sympy_expand               | 484 ms                                                 | 456 ms: 1.06x faster                                                  |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 707 ms: 1.06x faster                                                  |
| nqueens                    | 87.9 ms                                                | 83.1 ms: 1.06x faster                                                 |
| sqlglot_normalize          | 113 ms                                                 | 107 ms: 1.06x faster                                                  |
| scimark_monte_carlo        | 70.7 ms                                                | 66.9 ms: 1.06x faster                                                 |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 721 ms: 1.06x faster                                                  |
| xml_etree_parse            | 164 ms                                                 | 157 ms: 1.04x faster                                                  |
| deepcopy                   | 365 us                                                 | 350 us: 1.04x faster                                                  |
| deepcopy_reduce            | 3.22 us                                                | 3.09 us: 1.04x faster                                                 |
| deepcopy_memo              | 40.2 us                                                | 38.6 us: 1.04x faster                                                 |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                                  |
| fannkuch                   | 405 ms                                                 | 392 ms: 1.03x faster                                                  |
| json_loads                 | 29.2 us                                                | 28.2 us: 1.03x faster                                                 |
| pprint_pformat             | 1.55 sec                                               | 1.50 sec: 1.03x faster                                                |
| tornado_http               | 98.1 ms                                                | 94.9 ms: 1.03x faster                                                 |
| sqlglot_optimize           | 55.3 ms                                                | 54.1 ms: 1.02x faster                                                 |
| xml_etree_iterparse        | 108 ms                                                 | 106 ms: 1.02x faster                                                  |
| docutils                   | 2.66 sec                                               | 2.62 sec: 1.02x faster                                                |
| mdp                        | 2.77 sec                                               | 2.73 sec: 1.02x faster                                                |
| richards                   | 49.8 ms                                                | 49.1 ms: 1.01x faster                                                 |
| pprint_safe_repr           | 747 ms                                                 | 739 ms: 1.01x faster                                                  |
| dask                       | 365 ms                                                 | 362 ms: 1.01x faster                                                  |
| pathlib                    | 18.5 ms                                                | 18.4 ms: 1.01x faster                                                 |
| scimark_sor                | 121 ms                                                 | 121 ms: 1.01x faster                                                  |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                                  |
| bench_thread_pool          | 834 us                                                 | 838 us: 1.00x slower                                                  |
| 2to3                       | 264 ms                                                 | 266 ms: 1.00x slower                                                  |
| meteor_contest             | 109 ms                                                 | 110 ms: 1.01x slower                                                  |
| pickle_dict                | 34.6 us                                                | 34.9 us: 1.01x slower                                                 |
| spectral_norm              | 108 ms                                                 | 110 ms: 1.01x slower                                                  |
| unpickle_list              | 5.21 us                                                | 5.29 us: 1.02x slower                                                 |
| float                      | 78.9 ms                                                | 80.2 ms: 1.02x slower                                                 |
| create_gc_cycles           | 1.43 ms                                                | 1.47 ms: 1.02x slower                                                 |
| dulwich_log                | 64.6 ms                                                | 66.2 ms: 1.02x slower                                                 |
| mako                       | 10.7 ms                                                | 10.9 ms: 1.03x slower                                                 |
| regex_effbot               | 3.51 ms                                                | 3.60 ms: 1.03x slower                                                 |
| pickle                     | 11.0 us                                                | 11.3 us: 1.03x slower                                                 |
| scimark_fft                | 345 ms                                                 | 357 ms: 1.03x slower                                                  |
| chameleon                  | 6.70 ms                                                | 6.96 ms: 1.04x slower                                                 |
| xml_etree_process          | 56.9 ms                                                | 60.1 ms: 1.06x slower                                                 |
| regex_dna                  | 205 ms                                                 | 217 ms: 1.06x slower                                                  |
| pickle_list                | 4.59 us                                                | 4.87 us: 1.06x slower                                                 |
| pyflate                    | 434 ms                                                 | 464 ms: 1.07x slower                                                  |
| xml_etree_generate         | 81.1 ms                                                | 87.2 ms: 1.08x slower                                                 |
| sqlite_synth               | 2.57 us                                                | 2.85 us: 1.11x slower                                                 |
| regex_v8                   | 22.9 ms                                                | 25.4 ms: 1.11x slower                                                 |
| unpickle                   | 13.8 us                                                | 15.8 us: 1.14x slower                                                 |
| unpack_sequence            | 43.5 ns                                                | 49.7 ns: 1.14x slower                                                 |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                 |
| telco                      | 6.86 ms                                                | 8.21 ms: 1.20x slower                                                 |
| async_generators           | 374 ms                                                 | 450 ms: 1.20x slower                                                  |
| coverage                   | 78.8 ms                                                | 95.4 ms: 1.21x slower                                                 |
| mypy2                      | 686 ms                                                 | 844 ms: 1.23x slower                                                  |
| python_startup_no_site     | 6.01 ms                                                | 8.82 ms: 1.47x slower                                                 |
| Geometric mean             | (ref)                                                  | 1.06x faster                                                          |

Benchmark hidden because not significant (5): scimark_lu, json, bench_mp_pool, pycparser, scimark_sparse_mat_mult
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.99% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 0.99x