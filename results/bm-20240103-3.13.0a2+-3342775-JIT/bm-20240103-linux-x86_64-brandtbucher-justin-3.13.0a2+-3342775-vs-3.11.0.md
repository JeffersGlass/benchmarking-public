
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin
- machine: linux-x86_64
- commit hash: 3342775
- commit date: 2024-01-03
- overall geometric mean: 1.02x faster
- HPT reliability: 85.00%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240103-linux-x86_64-brandtbucher-justin-3.13.0a2+-3342775 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 278 ms: 1.05x slower                                           |
| chameleon      | 6.70 ms                                                | 7.20 ms: 1.07x slower                                          |
| docutils       | 2.66 sec                                               | 2.68 sec: 1.01x slower                                         |
| tornado_http   | 98.1 ms                                                | 97.3 ms: 1.01x faster                                          |
| Geometric mean | (ref)                                                  | 1.03x slower                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240103-linux-x86_64-brandtbucher-justin-3.13.0a2+-3342775 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 443 ms: 1.19x faster                                           |
| async_tree_memoization     | 639 ms                                                 | 566 ms: 1.13x faster                                           |
| async_tree_none_tg         | 491 ms                                                 | 451 ms: 1.09x faster                                           |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                         |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                         |
| async_tree_memoization_tg  | 626 ms                                                 | 589 ms: 1.06x faster                                           |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 712 ms: 1.05x faster                                           |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 725 ms: 1.05x faster                                           |
| Geometric mean             | (ref)                                                  | 1.09x faster                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240103-linux-x86_64-brandtbucher-justin-3.13.0a2+-3342775 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 188 ms: 1.03x faster                                           |
| nbody          | 96.0 ms                                                | 104 ms: 1.08x slower                                           |
| float          | 78.9 ms                                                | 87.7 ms: 1.11x slower                                          |
| Geometric mean | (ref)                                                  | 1.05x slower                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240103-linux-x86_64-brandtbucher-justin-3.13.0a2+-3342775 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 145 ms: 1.03x slower                                           |
| regex_effbot   | 3.51 ms                                                | 3.62 ms: 1.03x slower                                          |
| regex_dna      | 205 ms                                                 | 218 ms: 1.07x slower                                           |
| regex_v8       | 22.9 ms                                                | 25.6 ms: 1.12x slower                                          |
| Geometric mean | (ref)                                                  | 1.06x slower                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240103-linux-x86_64-brandtbucher-justin-3.13.0a2+-3342775 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.27x faster                                          |
| unpickle_pure_python | 242 us                                                 | 228 us: 1.06x faster                                           |
| pickle_pure_python   | 320 us                                                 | 303 us: 1.05x faster                                           |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                           |
| json_loads           | 29.2 us                                                | 28.3 us: 1.03x faster                                          |
| tomli_loads          | 2.30 sec                                               | 2.26 sec: 1.02x faster                                         |
| pickle_dict          | 34.6 us                                                | 35.0 us: 1.01x slower                                          |
| xml_etree_iterparse  | 108 ms                                                 | 110 ms: 1.01x slower                                           |
| unpickle_list        | 5.21 us                                                | 5.32 us: 1.02x slower                                          |
| xml_etree_process    | 56.9 ms                                                | 59.4 ms: 1.04x slower                                          |
| pickle               | 11.0 us                                                | 11.6 us: 1.05x slower                                          |
| unpickle             | 13.8 us                                                | 14.7 us: 1.06x slower                                          |
| xml_etree_generate   | 81.1 ms                                                | 87.4 ms: 1.08x slower                                          |
| pickle_list          | 4.59 us                                                | 5.12 us: 1.12x slower                                          |
| Geometric mean       | (ref)                                                  | 1.00x faster                                                   |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240103-linux-x86_64-brandtbucher-justin-3.13.0a2+-3342775 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.19x slower                                          |
| python_startup_no_site | 6.01 ms                                                | 8.88 ms: 1.48x slower                                          |
| Geometric mean         | (ref)                                                  | 1.33x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240103-linux-x86_64-brandtbucher-justin-3.13.0a2+-3342775 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 12.9 ms: 1.21x slower                                          |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240103-linux-x86_64-brandtbucher-justin-3.13.0a2+-3342775 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 114 us: 4.54x faster                                           |
| generators                 | 74.9 ms                                                | 29.6 ms: 2.53x faster                                          |
| asyncio_tcp                | 875 ms                                                 | 488 ms: 1.79x faster                                           |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.72x faster                                         |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.27x faster                                          |
| async_tree_none            | 528 ms                                                 | 443 ms: 1.19x faster                                           |
| comprehensions             | 23.6 us                                                | 20.0 us: 1.18x faster                                          |
| richards_super             | 61.9 ms                                                | 52.6 ms: 1.18x faster                                          |
| coroutines                 | 27.0 ms                                                | 23.2 ms: 1.16x faster                                          |
| async_tree_memoization     | 639 ms                                                 | 566 ms: 1.13x faster                                           |
| gc_traversal               | 4.01 ms                                                | 3.58 ms: 1.12x faster                                          |
| sqlglot_parse              | 1.43 ms                                                | 1.30 ms: 1.10x faster                                          |
| async_tree_none_tg         | 491 ms                                                 | 451 ms: 1.09x faster                                           |
| raytrace                   | 309 ms                                                 | 284 ms: 1.08x faster                                           |
| logging_simple             | 6.22 us                                                | 5.75 us: 1.08x faster                                          |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                         |
| richards                   | 49.8 ms                                                | 46.4 ms: 1.07x faster                                          |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                         |
| sqlglot_transpile          | 1.75 ms                                                | 1.64 ms: 1.07x faster                                          |
| logging_format             | 6.81 us                                                | 6.39 us: 1.07x faster                                          |
| async_tree_memoization_tg  | 626 ms                                                 | 589 ms: 1.06x faster                                           |
| unpickle_pure_python       | 242 us                                                 | 228 us: 1.06x faster                                           |
| pickle_pure_python         | 320 us                                                 | 303 us: 1.05x faster                                           |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 712 ms: 1.05x faster                                           |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 725 ms: 1.05x faster                                           |
| sympy_sum                  | 169 ms                                                 | 161 ms: 1.05x faster                                           |
| xml_etree_parse            | 164 ms                                                 | 158 ms: 1.04x faster                                           |
| pidigits                   | 194 ms                                                 | 188 ms: 1.03x faster                                           |
| deepcopy                   | 365 us                                                 | 354 us: 1.03x faster                                           |
| json_loads                 | 29.2 us                                                | 28.3 us: 1.03x faster                                          |
| sympy_str                  | 297 ms                                                 | 290 ms: 1.03x faster                                           |
| deepcopy_reduce            | 3.22 us                                                | 3.13 us: 1.03x faster                                          |
| tomli_loads                | 2.30 sec                                               | 2.26 sec: 1.02x faster                                         |
| sqlglot_normalize          | 113 ms                                                 | 111 ms: 1.02x faster                                           |
| tornado_http               | 98.1 ms                                                | 97.3 ms: 1.01x faster                                          |
| sympy_integrate            | 21.5 ms                                                | 21.3 ms: 1.01x faster                                          |
| asyncio_websockets         | 550 ms                                                 | 553 ms: 1.00x slower                                           |
| docutils                   | 2.66 sec                                               | 2.68 sec: 1.01x slower                                         |
| sympy_expand               | 484 ms                                                 | 489 ms: 1.01x slower                                           |
| bench_thread_pool          | 834 us                                                 | 844 us: 1.01x slower                                           |
| pickle_dict                | 34.6 us                                                | 35.0 us: 1.01x slower                                          |
| xml_etree_iterparse        | 108 ms                                                 | 110 ms: 1.01x slower                                           |
| deepcopy_memo              | 40.2 us                                                | 40.8 us: 1.02x slower                                          |
| mdp                        | 2.77 sec                                               | 2.82 sec: 1.02x slower                                         |
| pathlib                    | 18.5 ms                                                | 18.8 ms: 1.02x slower                                          |
| unpickle_list              | 5.21 us                                                | 5.32 us: 1.02x slower                                          |
| pycparser                  | 1.19 sec                                               | 1.21 sec: 1.02x slower                                         |
| sqlglot_optimize           | 55.3 ms                                                | 56.8 ms: 1.03x slower                                          |
| regex_compile              | 141 ms                                                 | 145 ms: 1.03x slower                                           |
| meteor_contest             | 109 ms                                                 | 112 ms: 1.03x slower                                           |
| create_gc_cycles           | 1.43 ms                                                | 1.48 ms: 1.03x slower                                          |
| regex_effbot               | 3.51 ms                                                | 3.62 ms: 1.03x slower                                          |
| go                         | 149 ms                                                 | 153 ms: 1.03x slower                                           |
| crypto_pyaes               | 76.7 ms                                                | 79.8 ms: 1.04x slower                                          |
| deltablue                  | 3.92 ms                                                | 4.08 ms: 1.04x slower                                          |
| xml_etree_process          | 56.9 ms                                                | 59.4 ms: 1.04x slower                                          |
| 2to3                       | 264 ms                                                 | 278 ms: 1.05x slower                                           |
| nqueens                    | 87.9 ms                                                | 92.6 ms: 1.05x slower                                          |
| pickle                     | 11.0 us                                                | 11.6 us: 1.05x slower                                          |
| dulwich_log                | 64.6 ms                                                | 68.3 ms: 1.06x slower                                          |
| unpickle                   | 13.8 us                                                | 14.7 us: 1.06x slower                                          |
| regex_dna                  | 205 ms                                                 | 218 ms: 1.07x slower                                           |
| scimark_sor                | 121 ms                                                 | 130 ms: 1.07x slower                                           |
| chameleon                  | 6.70 ms                                                | 7.20 ms: 1.07x slower                                          |
| xml_etree_generate         | 81.1 ms                                                | 87.4 ms: 1.08x slower                                          |
| nbody                      | 96.0 ms                                                | 104 ms: 1.08x slower                                           |
| pprint_safe_repr           | 747 ms                                                 | 811 ms: 1.09x slower                                           |
| unpack_sequence            | 43.5 ns                                                | 47.4 ns: 1.09x slower                                          |
| scimark_monte_carlo        | 70.7 ms                                                | 77.6 ms: 1.10x slower                                          |
| pprint_pformat             | 1.55 sec                                               | 1.71 sec: 1.10x slower                                         |
| fannkuch                   | 405 ms                                                 | 447 ms: 1.10x slower                                           |
| float                      | 78.9 ms                                                | 87.7 ms: 1.11x slower                                          |
| pickle_list                | 4.59 us                                                | 5.12 us: 1.12x slower                                          |
| sqlite_synth               | 2.57 us                                                | 2.88 us: 1.12x slower                                          |
| regex_v8                   | 22.9 ms                                                | 25.6 ms: 1.12x slower                                          |
| scimark_fft                | 345 ms                                                 | 393 ms: 1.14x slower                                           |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.88 ms: 1.17x slower                                          |
| pyflate                    | 434 ms                                                 | 514 ms: 1.19x slower                                           |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.19x slower                                          |
| hexiom                     | 6.89 ms                                                | 8.23 ms: 1.19x slower                                          |
| async_generators           | 374 ms                                                 | 451 ms: 1.21x slower                                           |
| mako                       | 10.7 ms                                                | 12.9 ms: 1.21x slower                                          |
| coverage                   | 78.8 ms                                                | 95.9 ms: 1.22x slower                                          |
| telco                      | 6.86 ms                                                | 8.52 ms: 1.24x slower                                          |
| mypy2                      | 686 ms                                                 | 871 ms: 1.27x slower                                           |
| spectral_norm              | 108 ms                                                 | 140 ms: 1.29x slower                                           |
| python_startup_no_site     | 6.01 ms                                                | 8.88 ms: 1.48x slower                                          |
| Geometric mean             | (ref)                                                  | 1.02x faster                                                   |

Benchmark hidden because not significant (6): logging_silent, chaos, json, scimark_lu, bench_mp_pool, dask
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 85.00% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.02x