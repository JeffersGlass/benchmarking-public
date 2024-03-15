
# Results vs. 3.11.0

- fork: python
- ref: 1ae7ceba29771baf8f2e
- machine: linux-x86_64
- commit hash: 1ae7ceb
- commit date: 2024-01-04
- overall geometric mean: 1.07x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 263 ms: 1.00x faster                                                   |
| chameleon      | 6.70 ms                                                | 6.97 ms: 1.04x slower                                                  |
| docutils       | 2.66 sec                                               | 2.61 sec: 1.02x faster                                                 |
| tornado_http   | 98.1 ms                                                | 94.5 ms: 1.04x faster                                                  |
| Geometric mean | (ref)                                                  | 1.01x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 434 ms: 1.22x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 559 ms: 1.14x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 441 ms: 1.11x faster                                                   |
| async_tree_memoization_tg  | 626 ms                                                 | 574 ms: 1.09x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                                 |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                                 |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 704 ms: 1.06x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 721 ms: 1.06x faster                                                   |
| Geometric mean             | (ref)                                                  | 1.11x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 88.9 ms: 1.08x faster                                                  |
| pidigits       | 194 ms                                                 | 195 ms: 1.00x slower                                                   |
| float          | 78.9 ms                                                | 79.4 ms: 1.01x slower                                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 129 ms: 1.09x faster                                                   |
| regex_effbot   | 3.51 ms                                                | 3.77 ms: 1.07x slower                                                  |
| regex_dna      | 205 ms                                                 | 224 ms: 1.09x slower                                                   |
| regex_v8       | 22.9 ms                                                | 25.3 ms: 1.11x slower                                                  |
| Geometric mean | (ref)                                                  | 1.04x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                  |
| unpickle_pure_python | 242 us                                                 | 213 us: 1.13x faster                                                   |
| tomli_loads          | 2.30 sec                                               | 2.11 sec: 1.09x faster                                                 |
| pickle_pure_python   | 320 us                                                 | 300 us: 1.07x faster                                                   |
| xml_etree_parse      | 164 ms                                                 | 156 ms: 1.05x faster                                                   |
| json_loads           | 29.2 us                                                | 28.1 us: 1.04x faster                                                  |
| xml_etree_iterparse  | 108 ms                                                 | 104 ms: 1.04x faster                                                   |
| pickle_dict          | 34.6 us                                                | 33.4 us: 1.04x faster                                                  |
| unpickle_list        | 5.21 us                                                | 5.13 us: 1.02x faster                                                  |
| xml_etree_process    | 56.9 ms                                                | 58.5 ms: 1.03x slower                                                  |
| xml_etree_generate   | 81.1 ms                                                | 84.9 ms: 1.05x slower                                                  |
| pickle               | 11.0 us                                                | 11.5 us: 1.05x slower                                                  |
| pickle_list          | 4.59 us                                                | 4.92 us: 1.07x slower                                                  |
| unpickle             | 13.8 us                                                | 15.0 us: 1.08x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                  |
| python_startup_no_site | 6.01 ms                                                | 8.70 ms: 1.45x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.31x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.1 ms: 1.04x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 112 us: 4.66x faster                                                   |
| generators                 | 74.9 ms                                                | 29.6 ms: 2.53x faster                                                  |
| asyncio_tcp                | 875 ms                                                 | 484 ms: 1.81x faster                                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.78 sec: 1.75x faster                                                 |
| comprehensions             | 23.6 us                                                | 16.0 us: 1.47x faster                                                  |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                  |
| coroutines                 | 27.0 ms                                                | 21.6 ms: 1.25x faster                                                  |
| async_tree_none            | 528 ms                                                 | 434 ms: 1.22x faster                                                   |
| chaos                      | 71.9 ms                                                | 59.2 ms: 1.21x faster                                                  |
| deltablue                  | 3.92 ms                                                | 3.23 ms: 1.21x faster                                                  |
| raytrace                   | 309 ms                                                 | 260 ms: 1.19x faster                                                   |
| sqlglot_parse              | 1.43 ms                                                | 1.24 ms: 1.16x faster                                                  |
| richards_super             | 61.9 ms                                                | 53.8 ms: 1.15x faster                                                  |
| async_tree_memoization     | 639 ms                                                 | 559 ms: 1.14x faster                                                   |
| sympy_sum                  | 169 ms                                                 | 148 ms: 1.14x faster                                                   |
| unpickle_pure_python       | 242 us                                                 | 213 us: 1.13x faster                                                   |
| sqlglot_transpile          | 1.75 ms                                                | 1.57 ms: 1.12x faster                                                  |
| async_tree_none_tg         | 491 ms                                                 | 441 ms: 1.11x faster                                                   |
| hexiom                     | 6.89 ms                                                | 6.20 ms: 1.11x faster                                                  |
| logging_simple             | 6.22 us                                                | 5.60 us: 1.11x faster                                                  |
| sympy_str                  | 297 ms                                                 | 269 ms: 1.10x faster                                                   |
| sympy_integrate            | 21.5 ms                                                | 19.5 ms: 1.10x faster                                                  |
| logging_format             | 6.81 us                                                | 6.18 us: 1.10x faster                                                  |
| mdp                        | 2.77 sec                                               | 2.53 sec: 1.10x faster                                                 |
| logging_silent             | 111 ns                                                 | 101 ns: 1.09x faster                                                   |
| regex_compile              | 141 ms                                                 | 129 ms: 1.09x faster                                                   |
| async_tree_memoization_tg  | 626 ms                                                 | 574 ms: 1.09x faster                                                   |
| tomli_loads                | 2.30 sec                                               | 2.11 sec: 1.09x faster                                                 |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                                 |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                                 |
| nbody                      | 96.0 ms                                                | 88.9 ms: 1.08x faster                                                  |
| gc_traversal               | 4.01 ms                                                | 3.72 ms: 1.08x faster                                                  |
| crypto_pyaes               | 76.7 ms                                                | 71.3 ms: 1.08x faster                                                  |
| go                         | 149 ms                                                 | 138 ms: 1.07x faster                                                   |
| unpack_sequence            | 43.5 ns                                                | 40.5 ns: 1.07x faster                                                  |
| pickle_pure_python         | 320 us                                                 | 300 us: 1.07x faster                                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 704 ms: 1.06x faster                                                   |
| sqlglot_normalize          | 113 ms                                                 | 106 ms: 1.06x faster                                                   |
| sympy_expand               | 484 ms                                                 | 457 ms: 1.06x faster                                                   |
| deepcopy_memo              | 40.2 us                                                | 37.9 us: 1.06x faster                                                  |
| deepcopy                   | 365 us                                                 | 345 us: 1.06x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 721 ms: 1.06x faster                                                   |
| deepcopy_reduce            | 3.22 us                                                | 3.05 us: 1.05x faster                                                  |
| xml_etree_parse            | 164 ms                                                 | 156 ms: 1.05x faster                                                   |
| scimark_lu                 | 116 ms                                                 | 111 ms: 1.05x faster                                                   |
| richards                   | 49.8 ms                                                | 47.4 ms: 1.05x faster                                                  |
| nqueens                    | 87.9 ms                                                | 83.9 ms: 1.05x faster                                                  |
| pprint_pformat             | 1.55 sec                                               | 1.49 sec: 1.04x faster                                                 |
| json_loads                 | 29.2 us                                                | 28.1 us: 1.04x faster                                                  |
| xml_etree_iterparse        | 108 ms                                                 | 104 ms: 1.04x faster                                                   |
| tornado_http               | 98.1 ms                                                | 94.5 ms: 1.04x faster                                                  |
| scimark_monte_carlo        | 70.7 ms                                                | 68.3 ms: 1.04x faster                                                  |
| sqlglot_optimize           | 55.3 ms                                                | 53.4 ms: 1.04x faster                                                  |
| pickle_dict                | 34.6 us                                                | 33.4 us: 1.04x faster                                                  |
| pprint_safe_repr           | 747 ms                                                 | 728 ms: 1.03x faster                                                   |
| docutils                   | 2.66 sec                                               | 2.61 sec: 1.02x faster                                                 |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.93 ms: 1.02x faster                                                  |
| unpickle_list              | 5.21 us                                                | 5.13 us: 1.02x faster                                                  |
| dask                       | 365 ms                                                 | 360 ms: 1.02x faster                                                   |
| meteor_contest             | 109 ms                                                 | 107 ms: 1.01x faster                                                   |
| fannkuch                   | 405 ms                                                 | 400 ms: 1.01x faster                                                   |
| bench_thread_pool          | 834 us                                                 | 828 us: 1.01x faster                                                   |
| 2to3                       | 264 ms                                                 | 263 ms: 1.00x faster                                                   |
| pidigits                   | 194 ms                                                 | 195 ms: 1.00x slower                                                   |
| float                      | 78.9 ms                                                | 79.4 ms: 1.01x slower                                                  |
| dulwich_log                | 64.6 ms                                                | 65.4 ms: 1.01x slower                                                  |
| pycparser                  | 1.19 sec                                               | 1.20 sec: 1.01x slower                                                 |
| scimark_fft                | 345 ms                                                 | 352 ms: 1.02x slower                                                   |
| create_gc_cycles           | 1.43 ms                                                | 1.47 ms: 1.03x slower                                                  |
| xml_etree_process          | 56.9 ms                                                | 58.5 ms: 1.03x slower                                                  |
| chameleon                  | 6.70 ms                                                | 6.97 ms: 1.04x slower                                                  |
| mako                       | 10.7 ms                                                | 11.1 ms: 1.04x slower                                                  |
| xml_etree_generate         | 81.1 ms                                                | 84.9 ms: 1.05x slower                                                  |
| pickle                     | 11.0 us                                                | 11.5 us: 1.05x slower                                                  |
| spectral_norm              | 108 ms                                                 | 114 ms: 1.05x slower                                                   |
| scimark_sor                | 121 ms                                                 | 129 ms: 1.06x slower                                                   |
| pyflate                    | 434 ms                                                 | 464 ms: 1.07x slower                                                   |
| pickle_list                | 4.59 us                                                | 4.92 us: 1.07x slower                                                  |
| regex_effbot               | 3.51 ms                                                | 3.77 ms: 1.07x slower                                                  |
| unpickle                   | 13.8 us                                                | 15.0 us: 1.08x slower                                                  |
| regex_dna                  | 205 ms                                                 | 224 ms: 1.09x slower                                                   |
| sqlite_synth               | 2.57 us                                                | 2.82 us: 1.10x slower                                                  |
| regex_v8                   | 22.9 ms                                                | 25.3 ms: 1.11x slower                                                  |
| async_generators           | 374 ms                                                 | 438 ms: 1.17x slower                                                   |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                  |
| telco                      | 6.86 ms                                                | 8.32 ms: 1.21x slower                                                  |
| coverage                   | 78.8 ms                                                | 96.2 ms: 1.22x slower                                                  |
| mypy2                      | 686 ms                                                 | 841 ms: 1.23x slower                                                   |
| python_startup_no_site     | 6.01 ms                                                | 8.70 ms: 1.45x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.07x faster                                                           |

Benchmark hidden because not significant (4): json, pathlib, bench_mp_pool, asyncio_websockets
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 0.98x