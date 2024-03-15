# Results vs. 3.11.0

- fork: python
- ref: ffed8d985b57a97def2e
- machine: linux-x86_64
- commit hash: ffed8d9
- commit date: 2024-03-04
- overall geometric mean: 1.03x slower \*
- HPT reliability: 99.68%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 293 ms: 1.11x slower                                                   |
| chameleon      | 6.70 ms                                                | 6.90 ms: 1.03x slower                                                  |
| docutils       | 2.66 sec                                               | 2.82 sec: 1.06x slower                                                 |
| tornado_http   | 98.1 ms                                                | 99.7 ms: 1.02x slower                                                  |
| Geometric mean | (ref)                                                  | 1.05x slower                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 450 ms: 1.17x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 577 ms: 1.11x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 457 ms: 1.08x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 590 ms: 1.06x faster                                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.23 sec: 1.06x faster                                                 |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 732 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 723 ms: 1.04x faster                                                   |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 188 ms: 1.03x faster                                                   |
| float          | 78.9 ms                                                | 95.3 ms: 1.21x slower                                                  |
| nbody          | 96.0 ms                                                | 121 ms: 1.26x slower                                                   |
| Geometric mean | (ref)                                                  | 1.14x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.45 ms: 1.02x faster                                                  |
| regex_v8       | 22.9 ms                                                | 24.0 ms: 1.05x slower                                                  |
| regex_dna      | 205 ms                                                 | 216 ms: 1.06x slower                                                   |
| regex_compile  | 141 ms                                                 | 176 ms: 1.24x slower                                                   |
| Geometric mean | (ref)                                                  | 1.08x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                  |
| unpickle_list        | 5.21 us                                                | 4.74 us: 1.10x faster                                                  |
| json_loads           | 29.2 us                                                | 27.5 us: 1.06x faster                                                  |
| pickle_pure_python   | 320 us                                                 | 305 us: 1.05x faster                                                   |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                                   |
| pickle_dict          | 34.6 us                                                | 34.8 us: 1.01x slower                                                  |
| xml_etree_iterparse  | 108 ms                                                 | 111 ms: 1.02x slower                                                   |
| pickle               | 11.0 us                                                | 11.8 us: 1.08x slower                                                  |
| xml_etree_process    | 56.9 ms                                                | 61.5 ms: 1.08x slower                                                  |
| xml_etree_generate   | 81.1 ms                                                | 89.8 ms: 1.11x slower                                                  |
| tomli_loads          | 2.30 sec                                               | 2.56 sec: 1.11x slower                                                 |
| pickle_list          | 4.59 us                                                | 5.18 us: 1.13x slower                                                  |
| unpickle             | 13.8 us                                                | 15.7 us: 1.14x slower                                                  |
| unpickle_pure_python | 242 us                                                 | 282 us: 1.17x slower                                                   |
| Geometric mean       | (ref)                                                  | 1.02x slower                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                  |
| python_startup_no_site | 6.01 ms                                                | 8.81 ms: 1.46x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.32x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 13.4 ms: 1.26x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 115 us: 4.54x faster                                                   |
| generators                 | 74.9 ms                                                | 29.8 ms: 2.51x faster                                                  |
| asyncio_tcp                | 875 ms                                                 | 478 ms: 1.83x faster                                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.73x faster                                                 |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                  |
| coroutines                 | 27.0 ms                                                | 22.1 ms: 1.22x faster                                                  |
| async_tree_none            | 528 ms                                                 | 450 ms: 1.17x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 577 ms: 1.11x faster                                                   |
| unpickle_list              | 5.21 us                                                | 4.74 us: 1.10x faster                                                  |
| logging_silent             | 111 ns                                                 | 102 ns: 1.09x faster                                                   |
| comprehensions             | 23.6 us                                                | 21.7 us: 1.09x faster                                                  |
| async_tree_none_tg         | 491 ms                                                 | 457 ms: 1.08x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 590 ms: 1.06x faster                                                   |
| json_loads                 | 29.2 us                                                | 27.5 us: 1.06x faster                                                  |
| async_tree_io_tg           | 1.29 sec                                               | 1.23 sec: 1.06x faster                                                 |
| pickle_pure_python         | 320 us                                                 | 305 us: 1.05x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 732 ms: 1.04x faster                                                   |
| xml_etree_parse            | 164 ms                                                 | 158 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 723 ms: 1.04x faster                                                   |
| gc_traversal               | 4.01 ms                                                | 3.87 ms: 1.04x faster                                                  |
| pidigits                   | 194 ms                                                 | 188 ms: 1.03x faster                                                   |
| sympy_sum                  | 169 ms                                                 | 164 ms: 1.03x faster                                                   |
| deepcopy_reduce            | 3.22 us                                                | 3.14 us: 1.02x faster                                                  |
| mdp                        | 2.77 sec                                               | 2.71 sec: 1.02x faster                                                 |
| deltablue                  | 3.92 ms                                                | 3.83 ms: 1.02x faster                                                  |
| json                       | 5.24 ms                                                | 5.13 ms: 1.02x faster                                                  |
| deepcopy                   | 365 us                                                 | 357 us: 1.02x faster                                                   |
| regex_effbot               | 3.51 ms                                                | 3.45 ms: 1.02x faster                                                  |
| logging_simple             | 6.22 us                                                | 6.15 us: 1.01x faster                                                  |
| sympy_integrate            | 21.5 ms                                                | 21.3 ms: 1.01x faster                                                  |
| sqlglot_normalize          | 113 ms                                                 | 112 ms: 1.01x faster                                                   |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                                   |
| sympy_str                  | 297 ms                                                 | 299 ms: 1.01x slower                                                   |
| pickle_dict                | 34.6 us                                                | 34.8 us: 1.01x slower                                                  |
| logging_format             | 6.81 us                                                | 6.91 us: 1.01x slower                                                  |
| tornado_http               | 98.1 ms                                                | 99.7 ms: 1.02x slower                                                  |
| sqlglot_transpile          | 1.75 ms                                                | 1.78 ms: 1.02x slower                                                  |
| xml_etree_iterparse        | 108 ms                                                 | 111 ms: 1.02x slower                                                   |
| pathlib                    | 18.5 ms                                                | 19.0 ms: 1.03x slower                                                  |
| bench_thread_pool          | 834 us                                                 | 858 us: 1.03x slower                                                   |
| chameleon                  | 6.70 ms                                                | 6.90 ms: 1.03x slower                                                  |
| deepcopy_memo              | 40.2 us                                                | 41.4 us: 1.03x slower                                                  |
| chaos                      | 71.9 ms                                                | 74.4 ms: 1.03x slower                                                  |
| sympy_expand               | 484 ms                                                 | 504 ms: 1.04x slower                                                   |
| regex_v8                   | 22.9 ms                                                | 24.0 ms: 1.05x slower                                                  |
| create_gc_cycles           | 1.43 ms                                                | 1.51 ms: 1.05x slower                                                  |
| regex_dna                  | 205 ms                                                 | 216 ms: 1.06x slower                                                   |
| docutils                   | 2.66 sec                                               | 2.82 sec: 1.06x slower                                                 |
| pycparser                  | 1.19 sec                                               | 1.27 sec: 1.07x slower                                                 |
| pickle                     | 11.0 us                                                | 11.8 us: 1.08x slower                                                  |
| xml_etree_process          | 56.9 ms                                                | 61.5 ms: 1.08x slower                                                  |
| meteor_contest             | 109 ms                                                 | 118 ms: 1.08x slower                                                   |
| sqlglot_optimize           | 55.3 ms                                                | 60.5 ms: 1.09x slower                                                  |
| raytrace                   | 309 ms                                                 | 340 ms: 1.10x slower                                                   |
| xml_etree_generate         | 81.1 ms                                                | 89.8 ms: 1.11x slower                                                  |
| 2to3                       | 264 ms                                                 | 293 ms: 1.11x slower                                                   |
| tomli_loads                | 2.30 sec                                               | 2.56 sec: 1.11x slower                                                 |
| crypto_pyaes               | 76.7 ms                                                | 85.5 ms: 1.11x slower                                                  |
| dulwich_log                | 64.6 ms                                                | 72.6 ms: 1.12x slower                                                  |
| richards                   | 49.8 ms                                                | 56.2 ms: 1.13x slower                                                  |
| pickle_list                | 4.59 us                                                | 5.18 us: 1.13x slower                                                  |
| sqlite_synth               | 2.57 us                                                | 2.92 us: 1.13x slower                                                  |
| unpickle                   | 13.8 us                                                | 15.7 us: 1.14x slower                                                  |
| nqueens                    | 87.9 ms                                                | 102 ms: 1.16x slower                                                   |
| unpickle_pure_python       | 242 us                                                 | 282 us: 1.17x slower                                                   |
| pprint_safe_repr           | 747 ms                                                 | 877 ms: 1.17x slower                                                   |
| pprint_pformat             | 1.55 sec                                               | 1.83 sec: 1.18x slower                                                 |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.94 ms: 1.18x slower                                                  |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                  |
| scimark_sor                | 121 ms                                                 | 144 ms: 1.19x slower                                                   |
| go                         | 149 ms                                                 | 177 ms: 1.19x slower                                                   |
| float                      | 78.9 ms                                                | 95.3 ms: 1.21x slower                                                  |
| coverage                   | 78.8 ms                                                | 95.6 ms: 1.21x slower                                                  |
| fannkuch                   | 405 ms                                                 | 502 ms: 1.24x slower                                                   |
| regex_compile              | 141 ms                                                 | 176 ms: 1.24x slower                                                   |
| scimark_fft                | 345 ms                                                 | 430 ms: 1.25x slower                                                   |
| async_generators           | 374 ms                                                 | 466 ms: 1.25x slower                                                   |
| telco                      | 6.86 ms                                                | 8.64 ms: 1.26x slower                                                  |
| mako                       | 10.7 ms                                                | 13.4 ms: 1.26x slower                                                  |
| nbody                      | 96.0 ms                                                | 121 ms: 1.26x slower                                                   |
| unpack_sequence            | 43.5 ns                                                | 55.4 ns: 1.27x slower                                                  |
| spectral_norm              | 108 ms                                                 | 140 ms: 1.29x slower                                                   |
| scimark_monte_carlo        | 70.7 ms                                                | 92.0 ms: 1.30x slower                                                  |
| mypy2                      | 686 ms                                                 | 897 ms: 1.31x slower                                                   |
| pyflate                    | 434 ms                                                 | 589 ms: 1.36x slower                                                   |
| hexiom                     | 6.89 ms                                                | 9.55 ms: 1.39x slower                                                  |
| scimark_lu                 | 116 ms                                                 | 162 ms: 1.39x slower                                                   |
| python_startup_no_site     | 6.01 ms                                                | 8.81 ms: 1.46x slower                                                  |
| dask                       | 365 ms                                                 | 537 ms: 1.47x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.03x slower                                                           |

Benchmark hidden because not significant (3): bench_mp_pool, sqlglot_parse, richards_super
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.68% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x