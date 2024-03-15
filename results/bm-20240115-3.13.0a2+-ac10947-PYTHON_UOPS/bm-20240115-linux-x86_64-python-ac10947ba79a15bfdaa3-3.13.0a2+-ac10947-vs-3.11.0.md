
# Results vs. 3.11.0

- fork: python
- ref: ac10947ba79a15bfdaa3
- machine: linux-x86_64
- commit hash: ac10947
- commit date: 2024-01-15
- overall geometric mean: 1.02x slower
- HPT reliability: 98.99%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 284 ms: 1.08x slower                                                   |
| chameleon      | 6.70 ms                                                | 7.37 ms: 1.10x slower                                                  |
| docutils       | 2.66 sec                                               | 2.72 sec: 1.02x slower                                                 |
| Geometric mean | (ref)                                                  | 1.05x slower                                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 450 ms: 1.17x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 577 ms: 1.11x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 451 ms: 1.09x faster                                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                 |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 588 ms: 1.07x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 731 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 721 ms: 1.04x faster                                                   |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 197 ms: 1.01x slower                                                   |
| float          | 78.9 ms                                                | 100 ms: 1.27x slower                                                   |
| nbody          | 96.0 ms                                                | 131 ms: 1.36x slower                                                   |
| Geometric mean | (ref)                                                  | 1.21x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.64 ms: 1.04x slower                                                  |
| regex_v8       | 22.9 ms                                                | 24.9 ms: 1.09x slower                                                  |
| regex_dna      | 205 ms                                                 | 223 ms: 1.09x slower                                                   |
| regex_compile  | 141 ms                                                 | 156 ms: 1.10x slower                                                   |
| Geometric mean | (ref)                                                  | 1.08x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.7 ms: 1.25x faster                                                  |
| pickle_pure_python   | 320 us                                                 | 302 us: 1.06x faster                                                   |
| xml_etree_parse      | 164 ms                                                 | 157 ms: 1.04x faster                                                   |
| json_loads           | 29.2 us                                                | 28.5 us: 1.03x faster                                                  |
| unpickle_pure_python | 242 us                                                 | 240 us: 1.01x faster                                                   |
| pickle_dict          | 34.6 us                                                | 34.9 us: 1.01x slower                                                  |
| xml_etree_iterparse  | 108 ms                                                 | 113 ms: 1.04x slower                                                   |
| unpickle_list        | 5.21 us                                                | 5.51 us: 1.06x slower                                                  |
| pickle               | 11.0 us                                                | 11.7 us: 1.07x slower                                                  |
| unpickle             | 13.8 us                                                | 14.9 us: 1.08x slower                                                  |
| xml_etree_process    | 56.9 ms                                                | 61.8 ms: 1.09x slower                                                  |
| tomli_loads          | 2.30 sec                                               | 2.54 sec: 1.10x slower                                                 |
| xml_etree_generate   | 81.1 ms                                                | 90.4 ms: 1.12x slower                                                  |
| pickle_list          | 4.59 us                                                | 5.32 us: 1.16x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.02x slower                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                  |
| python_startup_no_site | 6.01 ms                                                | 8.71 ms: 1.45x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.30x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 15.0 ms: 1.41x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 116 us: 4.48x faster                                                   |
| generators                 | 74.9 ms                                                | 36.4 ms: 2.05x faster                                                  |
| asyncio_tcp                | 875 ms                                                 | 496 ms: 1.77x faster                                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.72x faster                                                 |
| json_dumps                 | 13.3 ms                                                | 10.7 ms: 1.25x faster                                                  |
| coroutines                 | 27.0 ms                                                | 22.0 ms: 1.23x faster                                                  |
| async_tree_none            | 528 ms                                                 | 450 ms: 1.17x faster                                                   |
| richards_super             | 61.9 ms                                                | 55.2 ms: 1.12x faster                                                  |
| async_tree_memoization     | 639 ms                                                 | 577 ms: 1.11x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 451 ms: 1.09x faster                                                   |
| gc_traversal               | 4.01 ms                                                | 3.70 ms: 1.08x faster                                                  |
| sqlglot_parse              | 1.43 ms                                                | 1.33 ms: 1.08x faster                                                  |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                 |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 588 ms: 1.07x faster                                                   |
| pickle_pure_python         | 320 us                                                 | 302 us: 1.06x faster                                                   |
| sqlglot_transpile          | 1.75 ms                                                | 1.66 ms: 1.05x faster                                                  |
| logging_silent             | 111 ns                                                 | 106 ns: 1.05x faster                                                   |
| mdp                        | 2.77 sec                                               | 2.65 sec: 1.05x faster                                                 |
| sympy_sum                  | 169 ms                                                 | 162 ms: 1.04x faster                                                   |
| xml_etree_parse            | 164 ms                                                 | 157 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 731 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 721 ms: 1.04x faster                                                   |
| comprehensions             | 23.6 us                                                | 22.9 us: 1.03x faster                                                  |
| logging_simple             | 6.22 us                                                | 6.05 us: 1.03x faster                                                  |
| deepcopy_reduce            | 3.22 us                                                | 3.13 us: 1.03x faster                                                  |
| json_loads                 | 29.2 us                                                | 28.5 us: 1.03x faster                                                  |
| deepcopy                   | 365 us                                                 | 358 us: 1.02x faster                                                   |
| richards                   | 49.8 ms                                                | 48.9 ms: 1.02x faster                                                  |
| logging_format             | 6.81 us                                                | 6.71 us: 1.01x faster                                                  |
| unpickle_pure_python       | 242 us                                                 | 240 us: 1.01x faster                                                   |
| sympy_integrate            | 21.5 ms                                                | 21.4 ms: 1.00x faster                                                  |
| pathlib                    | 18.5 ms                                                | 18.7 ms: 1.01x slower                                                  |
| pickle_dict                | 34.6 us                                                | 34.9 us: 1.01x slower                                                  |
| pidigits                   | 194 ms                                                 | 197 ms: 1.01x slower                                                   |
| sympy_expand               | 484 ms                                                 | 493 ms: 1.02x slower                                                   |
| sqlglot_normalize          | 113 ms                                                 | 115 ms: 1.02x slower                                                   |
| bench_thread_pool          | 834 us                                                 | 851 us: 1.02x slower                                                   |
| scimark_lu                 | 116 ms                                                 | 119 ms: 1.02x slower                                                   |
| docutils                   | 2.66 sec                                               | 2.72 sec: 1.02x slower                                                 |
| create_gc_cycles           | 1.43 ms                                                | 1.47 ms: 1.03x slower                                                  |
| regex_effbot               | 3.51 ms                                                | 3.64 ms: 1.04x slower                                                  |
| xml_etree_iterparse        | 108 ms                                                 | 113 ms: 1.04x slower                                                   |
| deepcopy_memo              | 40.2 us                                                | 42.4 us: 1.06x slower                                                  |
| unpickle_list              | 5.21 us                                                | 5.51 us: 1.06x slower                                                  |
| pycparser                  | 1.19 sec                                               | 1.25 sec: 1.06x slower                                                 |
| sqlglot_optimize           | 55.3 ms                                                | 58.6 ms: 1.06x slower                                                  |
| pickle                     | 11.0 us                                                | 11.7 us: 1.07x slower                                                  |
| dulwich_log                | 64.6 ms                                                | 69.2 ms: 1.07x slower                                                  |
| meteor_contest             | 109 ms                                                 | 117 ms: 1.08x slower                                                   |
| unpickle                   | 13.8 us                                                | 14.9 us: 1.08x slower                                                  |
| 2to3                       | 264 ms                                                 | 284 ms: 1.08x slower                                                   |
| go                         | 149 ms                                                 | 160 ms: 1.08x slower                                                   |
| scimark_sor                | 121 ms                                                 | 132 ms: 1.08x slower                                                   |
| xml_etree_process          | 56.9 ms                                                | 61.8 ms: 1.09x slower                                                  |
| regex_v8                   | 22.9 ms                                                | 24.9 ms: 1.09x slower                                                  |
| chaos                      | 71.9 ms                                                | 78.2 ms: 1.09x slower                                                  |
| regex_dna                  | 205 ms                                                 | 223 ms: 1.09x slower                                                   |
| chameleon                  | 6.70 ms                                                | 7.37 ms: 1.10x slower                                                  |
| regex_compile              | 141 ms                                                 | 156 ms: 1.10x slower                                                   |
| tomli_loads                | 2.30 sec                                               | 2.54 sec: 1.10x slower                                                 |
| xml_etree_generate         | 81.1 ms                                                | 90.4 ms: 1.12x slower                                                  |
| sqlite_synth               | 2.57 us                                                | 2.88 us: 1.12x slower                                                  |
| nqueens                    | 87.9 ms                                                | 99.2 ms: 1.13x slower                                                  |
| pprint_safe_repr           | 747 ms                                                 | 845 ms: 1.13x slower                                                   |
| pprint_pformat             | 1.55 sec                                               | 1.77 sec: 1.14x slower                                                 |
| crypto_pyaes               | 76.7 ms                                                | 87.7 ms: 1.14x slower                                                  |
| pickle_list                | 4.59 us                                                | 5.32 us: 1.16x slower                                                  |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                  |
| fannkuch                   | 405 ms                                                 | 479 ms: 1.18x slower                                                   |
| coverage                   | 78.8 ms                                                | 95.7 ms: 1.22x slower                                                  |
| async_generators           | 374 ms                                                 | 454 ms: 1.22x slower                                                   |
| scimark_monte_carlo        | 70.7 ms                                                | 86.2 ms: 1.22x slower                                                  |
| unpack_sequence            | 43.5 ns                                                | 54.0 ns: 1.24x slower                                                  |
| mypy2                      | 686 ms                                                 | 864 ms: 1.26x slower                                                   |
| telco                      | 6.86 ms                                                | 8.69 ms: 1.27x slower                                                  |
| float                      | 78.9 ms                                                | 100 ms: 1.27x slower                                                   |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 6.40 ms: 1.27x slower                                                  |
| pyflate                    | 434 ms                                                 | 562 ms: 1.30x slower                                                   |
| deltablue                  | 3.92 ms                                                | 5.11 ms: 1.30x slower                                                  |
| hexiom                     | 6.89 ms                                                | 9.08 ms: 1.32x slower                                                  |
| nbody                      | 96.0 ms                                                | 131 ms: 1.36x slower                                                   |
| scimark_fft                | 345 ms                                                 | 480 ms: 1.39x slower                                                   |
| mako                       | 10.7 ms                                                | 15.0 ms: 1.41x slower                                                  |
| python_startup_no_site     | 6.01 ms                                                | 8.71 ms: 1.45x slower                                                  |
| spectral_norm              | 108 ms                                                 | 161 ms: 1.49x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.02x slower                                                           |

Benchmark hidden because not significant (7): sympy_str, tornado_http, raytrace, bench_mp_pool, asyncio_websockets, dask, json
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 98.99% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x