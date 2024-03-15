
# Results vs. 3.11.0

- fork: python
- ref: 2f0ec7fa9450caeac820
- machine: linux-x86_64
- commit hash: 2f0ec7f
- commit date: 2023-12-17
- overall geometric mean: 1.00x faster
- HPT reliability: 93.94%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 282 ms: 1.07x slower                                                   |
| chameleon      | 6.70 ms                                                | 7.33 ms: 1.09x slower                                                  |
| docutils       | 2.66 sec                                               | 2.71 sec: 1.02x slower                                                 |
| Geometric mean | (ref)                                                  | 1.04x slower                                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 454 ms: 1.16x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 581 ms: 1.10x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 454 ms: 1.08x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.06x faster                                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 591 ms: 1.06x faster                                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                 |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 734 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 726 ms: 1.03x faster                                                   |
| Geometric mean             | (ref)                                                  | 1.07x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 188 ms: 1.03x faster                                                   |
| float          | 78.9 ms                                                | 92.2 ms: 1.17x slower                                                  |
| nbody          | 96.0 ms                                                | 116 ms: 1.21x slower                                                   |
| Geometric mean | (ref)                                                  | 1.11x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.58 ms: 1.02x slower                                                  |
| regex_compile  | 141 ms                                                 | 151 ms: 1.07x slower                                                   |
| regex_v8       | 22.9 ms                                                | 25.1 ms: 1.10x slower                                                  |
| regex_dna      | 205 ms                                                 | 225 ms: 1.10x slower                                                   |
| Geometric mean | (ref)                                                  | 1.07x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                  |
| pickle_pure_python   | 320 us                                                 | 302 us: 1.06x faster                                                   |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                                   |
| unpickle_pure_python | 242 us                                                 | 234 us: 1.04x faster                                                   |
| pickle_dict          | 34.6 us                                                | 33.5 us: 1.03x faster                                                  |
| json_loads           | 29.2 us                                                | 28.3 us: 1.03x faster                                                  |
| pickle               | 11.0 us                                                | 10.9 us: 1.01x faster                                                  |
| xml_etree_iterparse  | 108 ms                                                 | 111 ms: 1.03x slower                                                   |
| tomli_loads          | 2.30 sec                                               | 2.41 sec: 1.05x slower                                                 |
| pickle_list          | 4.59 us                                                | 4.88 us: 1.06x slower                                                  |
| unpickle             | 13.8 us                                                | 14.9 us: 1.08x slower                                                  |
| xml_etree_process    | 56.9 ms                                                | 61.4 ms: 1.08x slower                                                  |
| xml_etree_generate   | 81.1 ms                                                | 89.5 ms: 1.10x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.00x faster                                                           |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                  |
| python_startup_no_site | 6.01 ms                                                | 8.72 ms: 1.45x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.31x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 14.1 ms: 1.32x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 117 us: 4.46x faster                                                   |
| generators                 | 74.9 ms                                                | 29.8 ms: 2.51x faster                                                  |
| asyncio_tcp                | 875 ms                                                 | 493 ms: 1.78x faster                                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.79 sec: 1.74x faster                                                 |
| json_dumps                 | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                  |
| coroutines                 | 27.0 ms                                                | 22.7 ms: 1.19x faster                                                  |
| async_tree_none            | 528 ms                                                 | 454 ms: 1.16x faster                                                   |
| richards_super             | 61.9 ms                                                | 54.8 ms: 1.13x faster                                                  |
| comprehensions             | 23.6 us                                                | 21.4 us: 1.10x faster                                                  |
| async_tree_memoization     | 639 ms                                                 | 581 ms: 1.10x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 454 ms: 1.08x faster                                                   |
| sqlglot_parse              | 1.43 ms                                                | 1.33 ms: 1.08x faster                                                  |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.06x faster                                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 591 ms: 1.06x faster                                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                 |
| pickle_pure_python         | 320 us                                                 | 302 us: 1.06x faster                                                   |
| logging_silent             | 111 ns                                                 | 105 ns: 1.06x faster                                                   |
| sqlglot_transpile          | 1.75 ms                                                | 1.65 ms: 1.06x faster                                                  |
| mdp                        | 2.77 sec                                               | 2.65 sec: 1.05x faster                                                 |
| sympy_sum                  | 169 ms                                                 | 161 ms: 1.05x faster                                                   |
| xml_etree_parse            | 164 ms                                                 | 158 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 734 ms: 1.04x faster                                                   |
| unpickle_pure_python       | 242 us                                                 | 234 us: 1.04x faster                                                   |
| deepcopy                   | 365 us                                                 | 353 us: 1.03x faster                                                   |
| richards                   | 49.8 ms                                                | 48.2 ms: 1.03x faster                                                  |
| pickle_dict                | 34.6 us                                                | 33.5 us: 1.03x faster                                                  |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 726 ms: 1.03x faster                                                   |
| json_loads                 | 29.2 us                                                | 28.3 us: 1.03x faster                                                  |
| pidigits                   | 194 ms                                                 | 188 ms: 1.03x faster                                                   |
| deepcopy_reduce            | 3.22 us                                                | 3.13 us: 1.03x faster                                                  |
| raytrace                   | 309 ms                                                 | 301 ms: 1.03x faster                                                   |
| logging_simple             | 6.22 us                                                | 6.07 us: 1.03x faster                                                  |
| sympy_str                  | 297 ms                                                 | 293 ms: 1.02x faster                                                   |
| sympy_integrate            | 21.5 ms                                                | 21.2 ms: 1.01x faster                                                  |
| gc_traversal               | 4.01 ms                                                | 3.97 ms: 1.01x faster                                                  |
| json                       | 5.24 ms                                                | 5.19 ms: 1.01x faster                                                  |
| pickle                     | 11.0 us                                                | 10.9 us: 1.01x faster                                                  |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                                   |
| sqlglot_normalize          | 113 ms                                                 | 113 ms: 1.01x slower                                                   |
| scimark_lu                 | 116 ms                                                 | 118 ms: 1.01x slower                                                   |
| sympy_expand               | 484 ms                                                 | 490 ms: 1.01x slower                                                   |
| logging_format             | 6.81 us                                                | 6.91 us: 1.02x slower                                                  |
| pycparser                  | 1.19 sec                                               | 1.20 sec: 1.02x slower                                                 |
| bench_thread_pool          | 834 us                                                 | 848 us: 1.02x slower                                                   |
| create_gc_cycles           | 1.43 ms                                                | 1.46 ms: 1.02x slower                                                  |
| docutils                   | 2.66 sec                                               | 2.71 sec: 1.02x slower                                                 |
| chaos                      | 71.9 ms                                                | 73.2 ms: 1.02x slower                                                  |
| regex_effbot               | 3.51 ms                                                | 3.58 ms: 1.02x slower                                                  |
| scimark_sor                | 121 ms                                                 | 124 ms: 1.02x slower                                                   |
| xml_etree_iterparse        | 108 ms                                                 | 111 ms: 1.03x slower                                                   |
| sqlglot_optimize           | 55.3 ms                                                | 57.7 ms: 1.04x slower                                                  |
| meteor_contest             | 109 ms                                                 | 114 ms: 1.05x slower                                                   |
| tomli_loads                | 2.30 sec                                               | 2.41 sec: 1.05x slower                                                 |
| go                         | 149 ms                                                 | 156 ms: 1.05x slower                                                   |
| pickle_list                | 4.59 us                                                | 4.88 us: 1.06x slower                                                  |
| unpack_sequence            | 43.5 ns                                                | 46.2 ns: 1.06x slower                                                  |
| 2to3                       | 264 ms                                                 | 282 ms: 1.07x slower                                                   |
| regex_compile              | 141 ms                                                 | 151 ms: 1.07x slower                                                   |
| unpickle                   | 13.8 us                                                | 14.9 us: 1.08x slower                                                  |
| xml_etree_process          | 56.9 ms                                                | 61.4 ms: 1.08x slower                                                  |
| dulwich_log                | 64.6 ms                                                | 69.9 ms: 1.08x slower                                                  |
| nqueens                    | 87.9 ms                                                | 95.1 ms: 1.08x slower                                                  |
| pprint_safe_repr           | 747 ms                                                 | 809 ms: 1.08x slower                                                   |
| crypto_pyaes               | 76.7 ms                                                | 83.2 ms: 1.08x slower                                                  |
| pprint_pformat             | 1.55 sec                                               | 1.69 sec: 1.09x slower                                                 |
| chameleon                  | 6.70 ms                                                | 7.33 ms: 1.09x slower                                                  |
| regex_v8                   | 22.9 ms                                                | 25.1 ms: 1.10x slower                                                  |
| regex_dna                  | 205 ms                                                 | 225 ms: 1.10x slower                                                   |
| xml_etree_generate         | 81.1 ms                                                | 89.5 ms: 1.10x slower                                                  |
| sqlite_synth               | 2.57 us                                                | 2.88 us: 1.12x slower                                                  |
| fannkuch                   | 405 ms                                                 | 457 ms: 1.13x slower                                                   |
| scimark_monte_carlo        | 70.7 ms                                                | 81.0 ms: 1.15x slower                                                  |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.85 ms: 1.16x slower                                                  |
| float                      | 78.9 ms                                                | 92.2 ms: 1.17x slower                                                  |
| pyflate                    | 434 ms                                                 | 509 ms: 1.17x slower                                                   |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                  |
| deltablue                  | 3.92 ms                                                | 4.67 ms: 1.19x slower                                                  |
| coverage                   | 78.8 ms                                                | 93.8 ms: 1.19x slower                                                  |
| nbody                      | 96.0 ms                                                | 116 ms: 1.21x slower                                                   |
| async_generators           | 374 ms                                                 | 452 ms: 1.21x slower                                                   |
| hexiom                     | 6.89 ms                                                | 8.59 ms: 1.25x slower                                                  |
| telco                      | 6.86 ms                                                | 8.56 ms: 1.25x slower                                                  |
| mypy2                      | 686 ms                                                 | 866 ms: 1.26x slower                                                   |
| scimark_fft                | 345 ms                                                 | 442 ms: 1.28x slower                                                   |
| mako                       | 10.7 ms                                                | 14.1 ms: 1.32x slower                                                  |
| spectral_norm              | 108 ms                                                 | 146 ms: 1.35x slower                                                   |
| python_startup_no_site     | 6.01 ms                                                | 8.72 ms: 1.45x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.00x faster                                                           |

Benchmark hidden because not significant (6): pathlib, tornado_http, unpickle_list, deepcopy_memo, bench_mp_pool, dask
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 93.94% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.98x