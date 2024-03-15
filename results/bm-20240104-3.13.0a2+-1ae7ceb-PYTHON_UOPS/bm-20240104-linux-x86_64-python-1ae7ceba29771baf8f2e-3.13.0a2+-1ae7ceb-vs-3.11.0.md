
# Results vs. 3.11.0

- fork: python
- ref: 1ae7ceba29771baf8f2e
- machine: linux-x86_64
- commit hash: 1ae7ceb
- commit date: 2024-01-04
- overall geometric mean: 1.02x slower
- HPT reliability: 99.91%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 286 ms: 1.08x slower                                                   |
| chameleon      | 6.70 ms                                                | 7.38 ms: 1.10x slower                                                  |
| docutils       | 2.66 sec                                               | 2.73 sec: 1.02x slower                                                 |
| tornado_http   | 98.1 ms                                                | 99.4 ms: 1.01x slower                                                  |
| Geometric mean | (ref)                                                  | 1.06x slower                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 455 ms: 1.16x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 583 ms: 1.10x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 458 ms: 1.07x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                 |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 595 ms: 1.05x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 735 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 725 ms: 1.03x faster                                                   |
| Geometric mean             | (ref)                                                  | 1.07x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 189 ms: 1.03x faster                                                   |
| float          | 78.9 ms                                                | 99.6 ms: 1.26x slower                                                  |
| nbody          | 96.0 ms                                                | 127 ms: 1.32x slower                                                   |
| Geometric mean | (ref)                                                  | 1.18x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.61 ms: 1.03x slower                                                  |
| regex_v8       | 22.9 ms                                                | 24.8 ms: 1.08x slower                                                  |
| regex_dna      | 205 ms                                                 | 226 ms: 1.11x slower                                                   |
| regex_compile  | 141 ms                                                 | 157 ms: 1.11x slower                                                   |
| Geometric mean | (ref)                                                  | 1.08x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.8 ms: 1.24x faster                                                  |
| pickle_pure_python   | 320 us                                                 | 305 us: 1.05x faster                                                   |
| xml_etree_parse      | 164 ms                                                 | 159 ms: 1.03x faster                                                   |
| json_loads           | 29.2 us                                                | 28.8 us: 1.01x faster                                                  |
| unpickle_pure_python | 242 us                                                 | 240 us: 1.01x faster                                                   |
| pickle_dict          | 34.6 us                                                | 34.4 us: 1.01x faster                                                  |
| unpickle_list        | 5.21 us                                                | 5.27 us: 1.01x slower                                                  |
| pickle               | 11.0 us                                                | 11.3 us: 1.03x slower                                                  |
| xml_etree_iterparse  | 108 ms                                                 | 114 ms: 1.05x slower                                                   |
| xml_etree_process    | 56.9 ms                                                | 61.6 ms: 1.08x slower                                                  |
| unpickle             | 13.8 us                                                | 15.0 us: 1.09x slower                                                  |
| tomli_loads          | 2.30 sec                                               | 2.53 sec: 1.10x slower                                                 |
| pickle_list          | 4.59 us                                                | 5.12 us: 1.12x slower                                                  |
| xml_etree_generate   | 81.1 ms                                                | 90.9 ms: 1.12x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.02x slower                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                  |
| python_startup_no_site | 6.01 ms                                                | 8.77 ms: 1.46x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.31x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 14.9 ms: 1.40x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 118 us: 4.40x faster                                                   |
| generators                 | 74.9 ms                                                | 29.3 ms: 2.56x faster                                                  |
| asyncio_tcp                | 875 ms                                                 | 490 ms: 1.79x faster                                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.73x faster                                                 |
| json_dumps                 | 13.3 ms                                                | 10.8 ms: 1.24x faster                                                  |
| coroutines                 | 27.0 ms                                                | 22.3 ms: 1.21x faster                                                  |
| async_tree_none            | 528 ms                                                 | 455 ms: 1.16x faster                                                   |
| gc_traversal               | 4.01 ms                                                | 3.50 ms: 1.14x faster                                                  |
| async_tree_memoization     | 639 ms                                                 | 583 ms: 1.10x faster                                                   |
| richards_super             | 61.9 ms                                                | 56.8 ms: 1.09x faster                                                  |
| async_tree_none_tg         | 491 ms                                                 | 458 ms: 1.07x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                 |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                 |
| sqlglot_parse              | 1.43 ms                                                | 1.35 ms: 1.06x faster                                                  |
| logging_silent             | 111 ns                                                 | 105 ns: 1.05x faster                                                   |
| async_tree_memoization_tg  | 626 ms                                                 | 595 ms: 1.05x faster                                                   |
| pickle_pure_python         | 320 us                                                 | 305 us: 1.05x faster                                                   |
| sqlglot_transpile          | 1.75 ms                                                | 1.69 ms: 1.04x faster                                                  |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 735 ms: 1.04x faster                                                   |
| comprehensions             | 23.6 us                                                | 22.8 us: 1.04x faster                                                  |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 725 ms: 1.03x faster                                                   |
| xml_etree_parse            | 164 ms                                                 | 159 ms: 1.03x faster                                                   |
| pidigits                   | 194 ms                                                 | 189 ms: 1.03x faster                                                   |
| sympy_sum                  | 169 ms                                                 | 165 ms: 1.03x faster                                                   |
| logging_simple             | 6.22 us                                                | 6.11 us: 1.02x faster                                                  |
| json_loads                 | 29.2 us                                                | 28.8 us: 1.01x faster                                                  |
| deepcopy                   | 365 us                                                 | 362 us: 1.01x faster                                                   |
| unpickle_pure_python       | 242 us                                                 | 240 us: 1.01x faster                                                   |
| pickle_dict                | 34.6 us                                                | 34.4 us: 1.01x faster                                                  |
| mdp                        | 2.77 sec                                               | 2.78 sec: 1.00x slower                                                 |
| raytrace                   | 309 ms                                                 | 311 ms: 1.01x slower                                                   |
| logging_format             | 6.81 us                                                | 6.87 us: 1.01x slower                                                  |
| sympy_str                  | 297 ms                                                 | 300 ms: 1.01x slower                                                   |
| unpickle_list              | 5.21 us                                                | 5.27 us: 1.01x slower                                                  |
| sympy_integrate            | 21.5 ms                                                | 21.7 ms: 1.01x slower                                                  |
| richards                   | 49.8 ms                                                | 50.4 ms: 1.01x slower                                                  |
| tornado_http               | 98.1 ms                                                | 99.4 ms: 1.01x slower                                                  |
| pycparser                  | 1.19 sec                                               | 1.20 sec: 1.02x slower                                                 |
| pathlib                    | 18.5 ms                                                | 18.8 ms: 1.02x slower                                                  |
| bench_thread_pool          | 834 us                                                 | 851 us: 1.02x slower                                                   |
| docutils                   | 2.66 sec                                               | 2.73 sec: 1.02x slower                                                 |
| regex_effbot               | 3.51 ms                                                | 3.61 ms: 1.03x slower                                                  |
| pickle                     | 11.0 us                                                | 11.3 us: 1.03x slower                                                  |
| create_gc_cycles           | 1.43 ms                                                | 1.48 ms: 1.03x slower                                                  |
| scimark_lu                 | 116 ms                                                 | 121 ms: 1.04x slower                                                   |
| sqlglot_normalize          | 113 ms                                                 | 117 ms: 1.04x slower                                                   |
| sympy_expand               | 484 ms                                                 | 503 ms: 1.04x slower                                                   |
| xml_etree_iterparse        | 108 ms                                                 | 114 ms: 1.05x slower                                                   |
| deepcopy_memo              | 40.2 us                                                | 42.6 us: 1.06x slower                                                  |
| dulwich_log                | 64.6 ms                                                | 69.0 ms: 1.07x slower                                                  |
| chaos                      | 71.9 ms                                                | 77.1 ms: 1.07x slower                                                  |
| sqlglot_optimize           | 55.3 ms                                                | 59.5 ms: 1.08x slower                                                  |
| xml_etree_process          | 56.9 ms                                                | 61.6 ms: 1.08x slower                                                  |
| meteor_contest             | 109 ms                                                 | 118 ms: 1.08x slower                                                   |
| 2to3                       | 264 ms                                                 | 286 ms: 1.08x slower                                                   |
| regex_v8                   | 22.9 ms                                                | 24.8 ms: 1.08x slower                                                  |
| unpickle                   | 13.8 us                                                | 15.0 us: 1.09x slower                                                  |
| go                         | 149 ms                                                 | 162 ms: 1.09x slower                                                   |
| tomli_loads                | 2.30 sec                                               | 2.53 sec: 1.10x slower                                                 |
| chameleon                  | 6.70 ms                                                | 7.38 ms: 1.10x slower                                                  |
| regex_dna                  | 205 ms                                                 | 226 ms: 1.11x slower                                                   |
| regex_compile              | 141 ms                                                 | 157 ms: 1.11x slower                                                   |
| scimark_sor                | 121 ms                                                 | 135 ms: 1.11x slower                                                   |
| pickle_list                | 4.59 us                                                | 5.12 us: 1.12x slower                                                  |
| xml_etree_generate         | 81.1 ms                                                | 90.9 ms: 1.12x slower                                                  |
| pprint_safe_repr           | 747 ms                                                 | 841 ms: 1.13x slower                                                   |
| nqueens                    | 87.9 ms                                                | 99.0 ms: 1.13x slower                                                  |
| pprint_pformat             | 1.55 sec                                               | 1.75 sec: 1.13x slower                                                 |
| sqlite_synth               | 2.57 us                                                | 2.93 us: 1.14x slower                                                  |
| crypto_pyaes               | 76.7 ms                                                | 87.7 ms: 1.14x slower                                                  |
| fannkuch                   | 405 ms                                                 | 468 ms: 1.15x slower                                                   |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                  |
| unpack_sequence            | 43.5 ns                                                | 52.1 ns: 1.20x slower                                                  |
| scimark_monte_carlo        | 70.7 ms                                                | 86.0 ms: 1.22x slower                                                  |
| pyflate                    | 434 ms                                                 | 528 ms: 1.22x slower                                                   |
| coverage                   | 78.8 ms                                                | 96.3 ms: 1.22x slower                                                  |
| async_generators           | 374 ms                                                 | 457 ms: 1.22x slower                                                   |
| float                      | 78.9 ms                                                | 99.6 ms: 1.26x slower                                                  |
| mypy2                      | 686 ms                                                 | 868 ms: 1.27x slower                                                   |
| telco                      | 6.86 ms                                                | 8.84 ms: 1.29x slower                                                  |
| deltablue                  | 3.92 ms                                                | 5.14 ms: 1.31x slower                                                  |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 6.61 ms: 1.31x slower                                                  |
| nbody                      | 96.0 ms                                                | 127 ms: 1.32x slower                                                   |
| hexiom                     | 6.89 ms                                                | 9.21 ms: 1.34x slower                                                  |
| scimark_fft                | 345 ms                                                 | 474 ms: 1.37x slower                                                   |
| mako                       | 10.7 ms                                                | 14.9 ms: 1.40x slower                                                  |
| python_startup_no_site     | 6.01 ms                                                | 8.77 ms: 1.46x slower                                                  |
| spectral_norm              | 108 ms                                                 | 159 ms: 1.47x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.02x slower                                                           |

Benchmark hidden because not significant (5): deepcopy_reduce, bench_mp_pool, asyncio_websockets, dask, json
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.91% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.98x