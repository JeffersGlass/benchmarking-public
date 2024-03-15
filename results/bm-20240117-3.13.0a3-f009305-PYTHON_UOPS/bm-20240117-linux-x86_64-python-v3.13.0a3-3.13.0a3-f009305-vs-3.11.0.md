
# Results vs. 3.11.0

- fork: python
- ref: v3.13.0a3
- machine: linux-x86_64
- commit hash: f009305
- commit date: 2024-01-17
- overall geometric mean: 1.01x slower
- HPT reliability: 96.43%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-python-v3.13.0a3-3.13.0a3-f009305 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 282 ms: 1.07x slower                                       |
| chameleon      | 6.70 ms                                                | 7.24 ms: 1.08x slower                                      |
| docutils       | 2.66 sec                                               | 2.71 sec: 1.02x slower                                     |
| Geometric mean | (ref)                                                  | 1.04x slower                                               |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-python-v3.13.0a3-3.13.0a3-f009305 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 448 ms: 1.18x faster                                       |
| async_tree_memoization     | 639 ms                                                 | 574 ms: 1.11x faster                                       |
| async_tree_none_tg         | 491 ms                                                 | 449 ms: 1.09x faster                                       |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                     |
| async_tree_io              | 1.29 sec                                               | 1.20 sec: 1.07x faster                                     |
| async_tree_memoization_tg  | 626 ms                                                 | 587 ms: 1.07x faster                                       |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 727 ms: 1.05x faster                                       |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 718 ms: 1.04x faster                                       |
| Geometric mean             | (ref)                                                  | 1.08x faster                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-python-v3.13.0a3-3.13.0a3-f009305 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 190 ms: 1.02x faster                                       |
| float          | 78.9 ms                                                | 94.1 ms: 1.19x slower                                      |
| nbody          | 96.0 ms                                                | 119 ms: 1.24x slower                                       |
| Geometric mean | (ref)                                                  | 1.13x slower                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-python-v3.13.0a3-3.13.0a3-f009305 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.74 ms: 1.07x slower                                      |
| regex_v8       | 22.9 ms                                                | 24.6 ms: 1.07x slower                                      |
| regex_compile  | 141 ms                                                 | 153 ms: 1.08x slower                                       |
| regex_dna      | 205 ms                                                 | 228 ms: 1.11x slower                                       |
| Geometric mean | (ref)                                                  | 1.08x slower                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-python-v3.13.0a3-3.13.0a3-f009305 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.27x faster                                      |
| pickle_pure_python   | 320 us                                                 | 301 us: 1.06x faster                                       |
| json_loads           | 29.2 us                                                | 28.2 us: 1.04x faster                                      |
| unpickle_pure_python | 242 us                                                 | 234 us: 1.03x faster                                       |
| xml_etree_parse      | 164 ms                                                 | 159 ms: 1.03x faster                                       |
| unpickle_list        | 5.21 us                                                | 5.14 us: 1.02x faster                                      |
| pickle_dict          | 34.6 us                                                | 35.0 us: 1.01x slower                                      |
| xml_etree_iterparse  | 108 ms                                                 | 112 ms: 1.04x slower                                       |
| xml_etree_process    | 56.9 ms                                                | 61.1 ms: 1.07x slower                                      |
| pickle               | 11.0 us                                                | 11.8 us: 1.07x slower                                      |
| xml_etree_generate   | 81.1 ms                                                | 89.5 ms: 1.10x slower                                      |
| tomli_loads          | 2.30 sec                                               | 2.61 sec: 1.13x slower                                     |
| pickle_list          | 4.59 us                                                | 5.24 us: 1.14x slower                                      |
| unpickle             | 13.8 us                                                | 16.1 us: 1.16x slower                                      |
| Geometric mean       | (ref)                                                  | 1.02x slower                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-python-v3.13.0a3-3.13.0a3-f009305 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                      |
| python_startup_no_site | 6.01 ms                                                | 8.72 ms: 1.45x slower                                      |
| Geometric mean         | (ref)                                                  | 1.31x slower                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-python-v3.13.0a3-3.13.0a3-f009305 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------:|
| mako      | 10.7 ms                                                | 14.2 ms: 1.33x slower                                      |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-python-v3.13.0a3-3.13.0a3-f009305 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 117 us: 4.46x faster                                       |
| generators                 | 74.9 ms                                                | 29.3 ms: 2.55x faster                                      |
| asyncio_tcp                | 875 ms                                                 | 492 ms: 1.78x faster                                       |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.81 sec: 1.72x faster                                     |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.27x faster                                      |
| coroutines                 | 27.0 ms                                                | 22.7 ms: 1.19x faster                                      |
| async_tree_none            | 528 ms                                                 | 448 ms: 1.18x faster                                       |
| richards_super             | 61.9 ms                                                | 54.7 ms: 1.13x faster                                      |
| async_tree_memoization     | 639 ms                                                 | 574 ms: 1.11x faster                                       |
| async_tree_none_tg         | 491 ms                                                 | 449 ms: 1.09x faster                                       |
| comprehensions             | 23.6 us                                                | 21.6 us: 1.09x faster                                      |
| logging_silent             | 111 ns                                                 | 102 ns: 1.09x faster                                       |
| gc_traversal               | 4.01 ms                                                | 3.69 ms: 1.09x faster                                      |
| sqlglot_parse              | 1.43 ms                                                | 1.34 ms: 1.07x faster                                      |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                     |
| async_tree_io              | 1.29 sec                                               | 1.20 sec: 1.07x faster                                     |
| async_tree_memoization_tg  | 626 ms                                                 | 587 ms: 1.07x faster                                       |
| pickle_pure_python         | 320 us                                                 | 301 us: 1.06x faster                                       |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 727 ms: 1.05x faster                                       |
| sqlglot_transpile          | 1.75 ms                                                | 1.67 ms: 1.05x faster                                      |
| sympy_sum                  | 169 ms                                                 | 161 ms: 1.05x faster                                       |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 718 ms: 1.04x faster                                       |
| mdp                        | 2.77 sec                                               | 2.67 sec: 1.04x faster                                     |
| json_loads                 | 29.2 us                                                | 28.2 us: 1.04x faster                                      |
| unpickle_pure_python       | 242 us                                                 | 234 us: 1.03x faster                                       |
| richards                   | 49.8 ms                                                | 48.3 ms: 1.03x faster                                      |
| xml_etree_parse            | 164 ms                                                 | 159 ms: 1.03x faster                                       |
| unpack_sequence            | 43.5 ns                                                | 42.4 ns: 1.03x faster                                      |
| pidigits                   | 194 ms                                                 | 190 ms: 1.02x faster                                       |
| raytrace                   | 309 ms                                                 | 302 ms: 1.02x faster                                       |
| deepcopy_reduce            | 3.22 us                                                | 3.15 us: 1.02x faster                                      |
| deepcopy                   | 365 us                                                 | 359 us: 1.02x faster                                       |
| sympy_integrate            | 21.5 ms                                                | 21.1 ms: 1.02x faster                                      |
| unpickle_list              | 5.21 us                                                | 5.14 us: 1.02x faster                                      |
| pathlib                    | 18.5 ms                                                | 18.3 ms: 1.01x faster                                      |
| json                       | 5.24 ms                                                | 5.19 ms: 1.01x faster                                      |
| dask                       | 365 ms                                                 | 369 ms: 1.01x slower                                       |
| pickle_dict                | 34.6 us                                                | 35.0 us: 1.01x slower                                      |
| sympy_str                  | 297 ms                                                 | 302 ms: 1.01x slower                                       |
| deepcopy_memo              | 40.2 us                                                | 40.8 us: 1.02x slower                                      |
| bench_thread_pool          | 834 us                                                 | 848 us: 1.02x slower                                       |
| docutils                   | 2.66 sec                                               | 2.71 sec: 1.02x slower                                     |
| sympy_expand               | 484 ms                                                 | 495 ms: 1.02x slower                                       |
| chaos                      | 71.9 ms                                                | 73.6 ms: 1.02x slower                                      |
| scimark_lu                 | 116 ms                                                 | 119 ms: 1.03x slower                                       |
| sqlglot_normalize          | 113 ms                                                 | 116 ms: 1.03x slower                                       |
| create_gc_cycles           | 1.43 ms                                                | 1.49 ms: 1.04x slower                                      |
| xml_etree_iterparse        | 108 ms                                                 | 112 ms: 1.04x slower                                       |
| logging_format             | 6.81 us                                                | 7.07 us: 1.04x slower                                      |
| meteor_contest             | 109 ms                                                 | 114 ms: 1.04x slower                                       |
| go                         | 149 ms                                                 | 156 ms: 1.05x slower                                       |
| sqlglot_optimize           | 55.3 ms                                                | 58.4 ms: 1.06x slower                                      |
| 2to3                       | 264 ms                                                 | 282 ms: 1.07x slower                                       |
| regex_effbot               | 3.51 ms                                                | 3.74 ms: 1.07x slower                                      |
| dulwich_log                | 64.6 ms                                                | 69.0 ms: 1.07x slower                                      |
| xml_etree_process          | 56.9 ms                                                | 61.1 ms: 1.07x slower                                      |
| regex_v8                   | 22.9 ms                                                | 24.6 ms: 1.07x slower                                      |
| pickle                     | 11.0 us                                                | 11.8 us: 1.07x slower                                      |
| chameleon                  | 6.70 ms                                                | 7.24 ms: 1.08x slower                                      |
| regex_compile              | 141 ms                                                 | 153 ms: 1.08x slower                                       |
| nqueens                    | 87.9 ms                                                | 95.4 ms: 1.09x slower                                      |
| pprint_safe_repr           | 747 ms                                                 | 816 ms: 1.09x slower                                       |
| pprint_pformat             | 1.55 sec                                               | 1.70 sec: 1.09x slower                                     |
| scimark_sor                | 121 ms                                                 | 134 ms: 1.10x slower                                       |
| xml_etree_generate         | 81.1 ms                                                | 89.5 ms: 1.10x slower                                      |
| crypto_pyaes               | 76.7 ms                                                | 85.0 ms: 1.11x slower                                      |
| regex_dna                  | 205 ms                                                 | 228 ms: 1.11x slower                                       |
| fannkuch                   | 405 ms                                                 | 454 ms: 1.12x slower                                       |
| sqlite_synth               | 2.57 us                                                | 2.91 us: 1.13x slower                                      |
| tomli_loads                | 2.30 sec                                               | 2.61 sec: 1.13x slower                                     |
| pickle_list                | 4.59 us                                                | 5.24 us: 1.14x slower                                      |
| scimark_monte_carlo        | 70.7 ms                                                | 81.4 ms: 1.15x slower                                      |
| unpickle                   | 13.8 us                                                | 16.1 us: 1.16x slower                                      |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                      |
| float                      | 78.9 ms                                                | 94.1 ms: 1.19x slower                                      |
| coverage                   | 78.8 ms                                                | 95.0 ms: 1.21x slower                                      |
| async_generators           | 374 ms                                                 | 461 ms: 1.23x slower                                       |
| pyflate                    | 434 ms                                                 | 536 ms: 1.24x slower                                       |
| deltablue                  | 3.92 ms                                                | 4.85 ms: 1.24x slower                                      |
| nbody                      | 96.0 ms                                                | 119 ms: 1.24x slower                                       |
| hexiom                     | 6.89 ms                                                | 8.65 ms: 1.26x slower                                      |
| telco                      | 6.86 ms                                                | 8.62 ms: 1.26x slower                                      |
| mypy2                      | 686 ms                                                 | 865 ms: 1.26x slower                                       |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 6.38 ms: 1.27x slower                                      |
| scimark_fft                | 345 ms                                                 | 457 ms: 1.32x slower                                       |
| mako                       | 10.7 ms                                                | 14.2 ms: 1.33x slower                                      |
| spectral_norm              | 108 ms                                                 | 154 ms: 1.43x slower                                       |
| python_startup_no_site     | 6.01 ms                                                | 8.72 ms: 1.45x slower                                      |
| Geometric mean             | (ref)                                                  | 1.01x slower                                               |

Benchmark hidden because not significant (5): logging_simple, tornado_http, bench_mp_pool, asyncio_websockets, pycparser
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 96.43% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x