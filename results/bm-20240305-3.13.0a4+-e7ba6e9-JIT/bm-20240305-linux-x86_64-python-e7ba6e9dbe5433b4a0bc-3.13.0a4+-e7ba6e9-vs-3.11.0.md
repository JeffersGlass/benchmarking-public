# Results vs. 3.11.0

- fork: python
- ref: e7ba6e9dbe5433b4a0bc
- machine: linux-x86_64
- commit hash: e7ba6e9
- commit date: 2024-03-05
- overall geometric mean: 1.03x faster \*
- HPT reliability: 98.05%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.24x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 276 ms: 1.04x slower                                                   |
| chameleon      | 6.70 ms                                                | 6.81 ms: 1.02x slower                                                  |
| docutils       | 2.66 sec                                               | 2.70 sec: 1.02x slower                                                 |
| tornado_http   | 98.1 ms                                                | 96.9 ms: 1.01x faster                                                  |
| Geometric mean | (ref)                                                  | 1.02x slower                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 434 ms: 1.22x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 561 ms: 1.14x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 446 ms: 1.10x faster                                                   |
| async_tree_memoization_tg  | 626 ms                                                 | 572 ms: 1.10x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                                 |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                                 |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 704 ms: 1.06x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 725 ms: 1.05x faster                                                   |
| Geometric mean             | (ref)                                                  | 1.10x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                                   |
| nbody          | 96.0 ms                                                | 94.5 ms: 1.02x faster                                                  |
| float          | 78.9 ms                                                | 78.3 ms: 1.01x faster                                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 142 ms: 1.01x slower                                                   |
| regex_effbot   | 3.51 ms                                                | 3.69 ms: 1.05x slower                                                  |
| regex_dna      | 205 ms                                                 | 222 ms: 1.09x slower                                                   |
| regex_v8       | 22.9 ms                                                | 25.3 ms: 1.11x slower                                                  |
| Geometric mean | (ref)                                                  | 1.06x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.29x faster                                                  |
| tomli_loads          | 2.30 sec                                               | 2.01 sec: 1.14x faster                                                 |
| pickle_pure_python   | 320 us                                                 | 297 us: 1.08x faster                                                   |
| json_loads           | 29.2 us                                                | 27.4 us: 1.06x faster                                                  |
| unpickle_list        | 5.21 us                                                | 4.91 us: 1.06x faster                                                  |
| xml_etree_parse      | 164 ms                                                 | 157 ms: 1.05x faster                                                   |
| unpickle_pure_python | 242 us                                                 | 236 us: 1.03x faster                                                   |
| pickle_dict          | 34.6 us                                                | 33.8 us: 1.02x faster                                                  |
| xml_etree_iterparse  | 108 ms                                                 | 106 ms: 1.02x faster                                                   |
| xml_etree_process    | 56.9 ms                                                | 58.7 ms: 1.03x slower                                                  |
| pickle               | 11.0 us                                                | 11.6 us: 1.06x slower                                                  |
| pickle_list          | 4.59 us                                                | 4.89 us: 1.07x slower                                                  |
| xml_etree_generate   | 81.1 ms                                                | 86.5 ms: 1.07x slower                                                  |
| unpickle             | 13.8 us                                                | 15.0 us: 1.08x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 12.3 ms: 1.44x slower                                                  |
| python_startup_no_site | 6.01 ms                                                | 11.0 ms: 1.82x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.62x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.0 ms: 1.04x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 112 us: 4.63x faster                                                   |
| generators                 | 74.9 ms                                                | 29.5 ms: 2.54x faster                                                  |
| asyncio_tcp                | 875 ms                                                 | 486 ms: 1.80x faster                                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.73x faster                                                 |
| comprehensions             | 23.6 us                                                | 17.2 us: 1.37x faster                                                  |
| json_dumps                 | 13.3 ms                                                | 10.4 ms: 1.29x faster                                                  |
| async_tree_none            | 528 ms                                                 | 434 ms: 1.22x faster                                                   |
| coroutines                 | 27.0 ms                                                | 22.3 ms: 1.21x faster                                                  |
| richards_super             | 61.9 ms                                                | 53.1 ms: 1.17x faster                                                  |
| deltablue                  | 3.92 ms                                                | 3.41 ms: 1.15x faster                                                  |
| tomli_loads                | 2.30 sec                                               | 2.01 sec: 1.14x faster                                                 |
| async_tree_memoization     | 639 ms                                                 | 561 ms: 1.14x faster                                                   |
| chaos                      | 71.9 ms                                                | 63.6 ms: 1.13x faster                                                  |
| sqlglot_parse              | 1.43 ms                                                | 1.28 ms: 1.12x faster                                                  |
| logging_silent             | 111 ns                                                 | 99.5 ns: 1.12x faster                                                  |
| logging_simple             | 6.22 us                                                | 5.62 us: 1.11x faster                                                  |
| async_tree_none_tg         | 491 ms                                                 | 446 ms: 1.10x faster                                                   |
| async_tree_memoization_tg  | 626 ms                                                 | 572 ms: 1.10x faster                                                   |
| logging_format             | 6.81 us                                                | 6.23 us: 1.09x faster                                                  |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                                 |
| richards                   | 49.8 ms                                                | 46.0 ms: 1.08x faster                                                  |
| sqlglot_transpile          | 1.75 ms                                                | 1.62 ms: 1.08x faster                                                  |
| sympy_sum                  | 169 ms                                                 | 157 ms: 1.08x faster                                                   |
| pickle_pure_python         | 320 us                                                 | 297 us: 1.08x faster                                                   |
| raytrace                   | 309 ms                                                 | 287 ms: 1.08x faster                                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                                 |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.68 ms: 1.07x faster                                                  |
| sympy_str                  | 297 ms                                                 | 279 ms: 1.07x faster                                                   |
| json_loads                 | 29.2 us                                                | 27.4 us: 1.06x faster                                                  |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 704 ms: 1.06x faster                                                   |
| unpickle_list              | 5.21 us                                                | 4.91 us: 1.06x faster                                                  |
| deepcopy_reduce            | 3.22 us                                                | 3.04 us: 1.06x faster                                                  |
| crypto_pyaes               | 76.7 ms                                                | 72.6 ms: 1.06x faster                                                  |
| sqlglot_normalize          | 113 ms                                                 | 107 ms: 1.06x faster                                                   |
| deepcopy                   | 365 us                                                 | 346 us: 1.05x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 725 ms: 1.05x faster                                                   |
| xml_etree_parse            | 164 ms                                                 | 157 ms: 1.05x faster                                                   |
| deepcopy_memo              | 40.2 us                                                | 38.6 us: 1.04x faster                                                  |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                                   |
| sympy_integrate            | 21.5 ms                                                | 20.8 ms: 1.03x faster                                                  |
| scimark_fft                | 345 ms                                                 | 335 ms: 1.03x faster                                                   |
| fannkuch                   | 405 ms                                                 | 394 ms: 1.03x faster                                                   |
| unpickle_pure_python       | 242 us                                                 | 236 us: 1.03x faster                                                   |
| json                       | 5.24 ms                                                | 5.12 ms: 1.02x faster                                                  |
| sympy_expand               | 484 ms                                                 | 474 ms: 1.02x faster                                                   |
| pickle_dict                | 34.6 us                                                | 33.8 us: 1.02x faster                                                  |
| xml_etree_iterparse        | 108 ms                                                 | 106 ms: 1.02x faster                                                   |
| scimark_monte_carlo        | 70.7 ms                                                | 69.5 ms: 1.02x faster                                                  |
| nbody                      | 96.0 ms                                                | 94.5 ms: 1.02x faster                                                  |
| pycparser                  | 1.19 sec                                               | 1.17 sec: 1.01x faster                                                 |
| tornado_http               | 98.1 ms                                                | 96.9 ms: 1.01x faster                                                  |
| float                      | 78.9 ms                                                | 78.3 ms: 1.01x faster                                                  |
| meteor_contest             | 109 ms                                                 | 108 ms: 1.01x faster                                                   |
| pathlib                    | 18.5 ms                                                | 18.4 ms: 1.01x faster                                                  |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                                   |
| regex_compile              | 141 ms                                                 | 142 ms: 1.01x slower                                                   |
| gc_traversal               | 4.01 ms                                                | 4.04 ms: 1.01x slower                                                  |
| sqlglot_optimize           | 55.3 ms                                                | 55.7 ms: 1.01x slower                                                  |
| bench_thread_pool          | 834 us                                                 | 844 us: 1.01x slower                                                   |
| docutils                   | 2.66 sec                                               | 2.70 sec: 1.02x slower                                                 |
| chameleon                  | 6.70 ms                                                | 6.81 ms: 1.02x slower                                                  |
| nqueens                    | 87.9 ms                                                | 89.6 ms: 1.02x slower                                                  |
| hexiom                     | 6.89 ms                                                | 7.05 ms: 1.02x slower                                                  |
| xml_etree_process          | 56.9 ms                                                | 58.7 ms: 1.03x slower                                                  |
| mako                       | 10.7 ms                                                | 11.0 ms: 1.04x slower                                                  |
| 2to3                       | 264 ms                                                 | 276 ms: 1.04x slower                                                   |
| create_gc_cycles           | 1.43 ms                                                | 1.50 ms: 1.05x slower                                                  |
| spectral_norm              | 108 ms                                                 | 113 ms: 1.05x slower                                                   |
| go                         | 149 ms                                                 | 155 ms: 1.05x slower                                                   |
| scimark_sor                | 121 ms                                                 | 127 ms: 1.05x slower                                                   |
| regex_effbot               | 3.51 ms                                                | 3.69 ms: 1.05x slower                                                  |
| pickle                     | 11.0 us                                                | 11.6 us: 1.06x slower                                                  |
| dulwich_log                | 64.6 ms                                                | 68.4 ms: 1.06x slower                                                  |
| pickle_list                | 4.59 us                                                | 4.89 us: 1.07x slower                                                  |
| xml_etree_generate         | 81.1 ms                                                | 86.5 ms: 1.07x slower                                                  |
| unpickle                   | 13.8 us                                                | 15.0 us: 1.08x slower                                                  |
| regex_dna                  | 205 ms                                                 | 222 ms: 1.09x slower                                                   |
| sqlite_synth               | 2.57 us                                                | 2.82 us: 1.10x slower                                                  |
| scimark_lu                 | 116 ms                                                 | 128 ms: 1.10x slower                                                   |
| regex_v8                   | 22.9 ms                                                | 25.3 ms: 1.11x slower                                                  |
| pyflate                    | 434 ms                                                 | 489 ms: 1.13x slower                                                   |
| bench_mp_pool              | 24.0 ms                                                | 28.0 ms: 1.17x slower                                                  |
| telco                      | 6.86 ms                                                | 8.24 ms: 1.20x slower                                                  |
| coverage                   | 78.8 ms                                                | 95.4 ms: 1.21x slower                                                  |
| async_generators           | 374 ms                                                 | 468 ms: 1.25x slower                                                   |
| mypy2                      | 686 ms                                                 | 881 ms: 1.28x slower                                                   |
| python_startup             | 8.56 ms                                                | 12.3 ms: 1.44x slower                                                  |
| dask                       | 365 ms                                                 | 530 ms: 1.45x slower                                                   |
| python_startup_no_site     | 6.01 ms                                                | 11.0 ms: 1.82x slower                                                  |
| unpack_sequence            | 43.5 ns                                                | 86.3 ns: 1.99x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.03x faster                                                           |

Benchmark hidden because not significant (3): pprint_pformat, pprint_safe_repr, mdp
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 98.05% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.24x