
# Results vs. 3.11.0

- fork: python
- ref: 1ae7ceba29771baf8f2e
- machine: linux-x86_64
- commit hash: 1ae7ceb
- commit date: 2024-01-04
- overall geometric mean: 1.07x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 264 ms: 1.00x faster                                                   |
| chameleon      | 6.70 ms                                                | 6.90 ms: 1.03x slower                                                  |
| docutils       | 2.66 sec                                               | 2.59 sec: 1.03x faster                                                 |
| tornado_http   | 98.1 ms                                                | 94.1 ms: 1.04x faster                                                  |
| Geometric mean | (ref)                                                  | 1.01x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 434 ms: 1.22x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 559 ms: 1.14x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 438 ms: 1.12x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.17 sec: 1.10x faster                                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 574 ms: 1.09x faster                                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                                 |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 706 ms: 1.06x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 720 ms: 1.06x faster                                                   |
| Geometric mean             | (ref)                                                  | 1.11x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 87.4 ms: 1.10x faster                                                  |
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                                   |
| float          | 78.9 ms                                                | 79.7 ms: 1.01x slower                                                  |
| Geometric mean | (ref)                                                  | 1.04x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 130 ms: 1.09x faster                                                   |
| regex_effbot   | 3.51 ms                                                | 3.65 ms: 1.04x slower                                                  |
| regex_dna      | 205 ms                                                 | 223 ms: 1.09x slower                                                   |
| regex_v8       | 22.9 ms                                                | 25.0 ms: 1.09x slower                                                  |
| Geometric mean | (ref)                                                  | 1.03x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.26x faster                                                  |
| unpickle_pure_python | 242 us                                                 | 216 us: 1.12x faster                                                   |
| tomli_loads          | 2.30 sec                                               | 2.13 sec: 1.08x faster                                                 |
| pickle_pure_python   | 320 us                                                 | 302 us: 1.06x faster                                                   |
| xml_etree_parse      | 164 ms                                                 | 157 ms: 1.05x faster                                                   |
| json_loads           | 29.2 us                                                | 28.1 us: 1.04x faster                                                  |
| xml_etree_iterparse  | 108 ms                                                 | 105 ms: 1.03x faster                                                   |
| unpickle_list        | 5.21 us                                                | 5.05 us: 1.03x faster                                                  |
| pickle_dict          | 34.6 us                                                | 35.5 us: 1.03x slower                                                  |
| xml_etree_process    | 56.9 ms                                                | 58.6 ms: 1.03x slower                                                  |
| xml_etree_generate   | 81.1 ms                                                | 85.1 ms: 1.05x slower                                                  |
| pickle               | 11.0 us                                                | 11.7 us: 1.06x slower                                                  |
| unpickle             | 13.8 us                                                | 14.9 us: 1.08x slower                                                  |
| pickle_list          | 4.59 us                                                | 5.20 us: 1.13x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                  |
| python_startup_no_site | 6.01 ms                                                | 8.71 ms: 1.45x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.31x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.2 ms: 1.05x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 111 us: 4.69x faster                                                   |
| generators                 | 74.9 ms                                                | 29.4 ms: 2.54x faster                                                  |
| asyncio_tcp                | 875 ms                                                 | 480 ms: 1.82x faster                                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.77 sec: 1.75x faster                                                 |
| comprehensions             | 23.6 us                                                | 16.0 us: 1.47x faster                                                  |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.26x faster                                                  |
| chaos                      | 71.9 ms                                                | 58.9 ms: 1.22x faster                                                  |
| async_tree_none            | 528 ms                                                 | 434 ms: 1.22x faster                                                   |
| coroutines                 | 27.0 ms                                                | 22.4 ms: 1.21x faster                                                  |
| deltablue                  | 3.92 ms                                                | 3.26 ms: 1.20x faster                                                  |
| raytrace                   | 309 ms                                                 | 262 ms: 1.18x faster                                                   |
| sqlglot_parse              | 1.43 ms                                                | 1.25 ms: 1.15x faster                                                  |
| async_tree_memoization     | 639 ms                                                 | 559 ms: 1.14x faster                                                   |
| sympy_sum                  | 169 ms                                                 | 148 ms: 1.14x faster                                                   |
| hexiom                     | 6.89 ms                                                | 6.07 ms: 1.13x faster                                                  |
| richards_super             | 61.9 ms                                                | 55.0 ms: 1.13x faster                                                  |
| unpickle_pure_python       | 242 us                                                 | 216 us: 1.12x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 438 ms: 1.12x faster                                                   |
| sqlglot_transpile          | 1.75 ms                                                | 1.57 ms: 1.11x faster                                                  |
| logging_simple             | 6.22 us                                                | 5.62 us: 1.11x faster                                                  |
| sympy_integrate            | 21.5 ms                                                | 19.5 ms: 1.10x faster                                                  |
| logging_format             | 6.81 us                                                | 6.18 us: 1.10x faster                                                  |
| mdp                        | 2.77 sec                                               | 2.53 sec: 1.10x faster                                                 |
| nbody                      | 96.0 ms                                                | 87.4 ms: 1.10x faster                                                  |
| crypto_pyaes               | 76.7 ms                                                | 70.0 ms: 1.10x faster                                                  |
| async_tree_io              | 1.29 sec                                               | 1.17 sec: 1.10x faster                                                 |
| logging_silent             | 111 ns                                                 | 102 ns: 1.09x faster                                                   |
| nqueens                    | 87.9 ms                                                | 80.6 ms: 1.09x faster                                                  |
| async_tree_memoization_tg  | 626 ms                                                 | 574 ms: 1.09x faster                                                   |
| regex_compile              | 141 ms                                                 | 130 ms: 1.09x faster                                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                                 |
| gc_traversal               | 4.01 ms                                                | 3.69 ms: 1.09x faster                                                  |
| tomli_loads                | 2.30 sec                                               | 2.13 sec: 1.08x faster                                                 |
| sympy_str                  | 297 ms                                                 | 276 ms: 1.08x faster                                                   |
| go                         | 149 ms                                                 | 139 ms: 1.07x faster                                                   |
| deepcopy_reduce            | 3.22 us                                                | 3.02 us: 1.06x faster                                                  |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 706 ms: 1.06x faster                                                   |
| deepcopy                   | 365 us                                                 | 344 us: 1.06x faster                                                   |
| pickle_pure_python         | 320 us                                                 | 302 us: 1.06x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 720 ms: 1.06x faster                                                   |
| pprint_pformat             | 1.55 sec                                               | 1.48 sec: 1.05x faster                                                 |
| sqlglot_normalize          | 113 ms                                                 | 108 ms: 1.05x faster                                                   |
| xml_etree_parse            | 164 ms                                                 | 157 ms: 1.05x faster                                                   |
| deepcopy_memo              | 40.2 us                                                | 38.4 us: 1.05x faster                                                  |
| scimark_monte_carlo        | 70.7 ms                                                | 67.6 ms: 1.05x faster                                                  |
| tornado_http               | 98.1 ms                                                | 94.1 ms: 1.04x faster                                                  |
| sympy_expand               | 484 ms                                                 | 465 ms: 1.04x faster                                                   |
| json_loads                 | 29.2 us                                                | 28.1 us: 1.04x faster                                                  |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                                   |
| scimark_lu                 | 116 ms                                                 | 112 ms: 1.04x faster                                                   |
| xml_etree_iterparse        | 108 ms                                                 | 105 ms: 1.03x faster                                                   |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.87 ms: 1.03x faster                                                  |
| unpickle_list              | 5.21 us                                                | 5.05 us: 1.03x faster                                                  |
| pprint_safe_repr           | 747 ms                                                 | 724 ms: 1.03x faster                                                   |
| richards                   | 49.8 ms                                                | 48.3 ms: 1.03x faster                                                  |
| docutils                   | 2.66 sec                                               | 2.59 sec: 1.03x faster                                                 |
| sqlglot_optimize           | 55.3 ms                                                | 53.9 ms: 1.03x faster                                                  |
| dask                       | 365 ms                                                 | 359 ms: 1.02x faster                                                   |
| fannkuch                   | 405 ms                                                 | 399 ms: 1.02x faster                                                   |
| pathlib                    | 18.5 ms                                                | 18.3 ms: 1.01x faster                                                  |
| json                       | 5.24 ms                                                | 5.18 ms: 1.01x faster                                                  |
| bench_thread_pool          | 834 us                                                 | 827 us: 1.01x faster                                                   |
| meteor_contest             | 109 ms                                                 | 108 ms: 1.01x faster                                                   |
| 2to3                       | 264 ms                                                 | 264 ms: 1.00x faster                                                   |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                                   |
| spectral_norm              | 108 ms                                                 | 109 ms: 1.01x slower                                                   |
| float                      | 78.9 ms                                                | 79.7 ms: 1.01x slower                                                  |
| dulwich_log                | 64.6 ms                                                | 65.3 ms: 1.01x slower                                                  |
| unpack_sequence            | 43.5 ns                                                | 44.4 ns: 1.02x slower                                                  |
| create_gc_cycles           | 1.43 ms                                                | 1.47 ms: 1.03x slower                                                  |
| pickle_dict                | 34.6 us                                                | 35.5 us: 1.03x slower                                                  |
| xml_etree_process          | 56.9 ms                                                | 58.6 ms: 1.03x slower                                                  |
| chameleon                  | 6.70 ms                                                | 6.90 ms: 1.03x slower                                                  |
| regex_effbot               | 3.51 ms                                                | 3.65 ms: 1.04x slower                                                  |
| scimark_fft                | 345 ms                                                 | 362 ms: 1.05x slower                                                   |
| pyflate                    | 434 ms                                                 | 455 ms: 1.05x slower                                                   |
| xml_etree_generate         | 81.1 ms                                                | 85.1 ms: 1.05x slower                                                  |
| mako                       | 10.7 ms                                                | 11.2 ms: 1.05x slower                                                  |
| scimark_sor                | 121 ms                                                 | 128 ms: 1.06x slower                                                   |
| pickle                     | 11.0 us                                                | 11.7 us: 1.06x slower                                                  |
| unpickle                   | 13.8 us                                                | 14.9 us: 1.08x slower                                                  |
| regex_dna                  | 205 ms                                                 | 223 ms: 1.09x slower                                                   |
| regex_v8                   | 22.9 ms                                                | 25.0 ms: 1.09x slower                                                  |
| sqlite_synth               | 2.57 us                                                | 2.85 us: 1.11x slower                                                  |
| pickle_list                | 4.59 us                                                | 5.20 us: 1.13x slower                                                  |
| async_generators           | 374 ms                                                 | 439 ms: 1.17x slower                                                   |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                  |
| coverage                   | 78.8 ms                                                | 95.0 ms: 1.21x slower                                                  |
| telco                      | 6.86 ms                                                | 8.35 ms: 1.22x slower                                                  |
| mypy2                      | 686 ms                                                 | 838 ms: 1.22x slower                                                   |
| python_startup_no_site     | 6.01 ms                                                | 8.71 ms: 1.45x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.07x faster                                                           |

Benchmark hidden because not significant (2): bench_mp_pool, pycparser
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 0.98x