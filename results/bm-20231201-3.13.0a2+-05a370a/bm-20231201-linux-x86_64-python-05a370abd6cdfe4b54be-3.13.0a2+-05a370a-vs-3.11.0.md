
# Results vs. 3.11.0

- fork: python
- ref: 05a370abd6cdfe4b54be
- machine: linux-x86_64
- commit hash: 05a370a
- commit date: 2023-12-01
- overall geometric mean: 1.06x faster
- HPT reliability: 99.98%
- HPT 99th percentile: 1.01x faster
- Memory change: 0.97x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 263 ms: 1.01x faster                                                   |
| chameleon      | 6.70 ms                                                | 7.00 ms: 1.05x slower                                                  |
| docutils       | 2.66 sec                                               | 2.61 sec: 1.02x faster                                                 |
| tornado_http   | 98.1 ms                                                | 94.3 ms: 1.04x faster                                                  |
| Geometric mean | (ref)                                                  | 1.00x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 435 ms: 1.21x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 568 ms: 1.12x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                                 |
| async_tree_none_tg         | 491 ms                                                 | 457 ms: 1.08x faster                                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                 |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 710 ms: 1.05x faster                                                   |
| async_tree_memoization_tg  | 626 ms                                                 | 598 ms: 1.05x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 738 ms: 1.03x faster                                                   |
| Geometric mean             | (ref)                                                  | 1.09x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 92.4 ms: 1.04x faster                                                  |
| pidigits       | 194 ms                                                 | 196 ms: 1.01x slower                                                   |
| float          | 78.9 ms                                                | 80.9 ms: 1.02x slower                                                  |
| Geometric mean | (ref)                                                  | 1.00x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 133 ms: 1.06x faster                                                   |
| regex_effbot   | 3.51 ms                                                | 3.68 ms: 1.05x slower                                                  |
| regex_dna      | 205 ms                                                 | 219 ms: 1.07x slower                                                   |
| regex_v8       | 22.9 ms                                                | 25.7 ms: 1.12x slower                                                  |
| Geometric mean | (ref)                                                  | 1.04x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.29x faster                                                  |
| unpickle_pure_python | 242 us                                                 | 217 us: 1.11x faster                                                   |
| tomli_loads          | 2.30 sec                                               | 2.14 sec: 1.08x faster                                                 |
| pickle_pure_python   | 320 us                                                 | 302 us: 1.06x faster                                                   |
| xml_etree_parse      | 164 ms                                                 | 157 ms: 1.04x faster                                                   |
| unpickle_list        | 5.21 us                                                | 5.04 us: 1.03x faster                                                  |
| json_loads           | 29.2 us                                                | 28.2 us: 1.03x faster                                                  |
| xml_etree_iterparse  | 108 ms                                                 | 106 ms: 1.02x faster                                                   |
| pickle_dict          | 34.6 us                                                | 34.3 us: 1.01x faster                                                  |
| xml_etree_process    | 56.9 ms                                                | 59.4 ms: 1.04x slower                                                  |
| pickle               | 11.0 us                                                | 11.6 us: 1.06x slower                                                  |
| xml_etree_generate   | 81.1 ms                                                | 86.6 ms: 1.07x slower                                                  |
| pickle_list          | 4.59 us                                                | 5.09 us: 1.11x slower                                                  |
| unpickle             | 13.8 us                                                | 15.5 us: 1.12x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.4 ms: 1.21x slower                                                  |
| python_startup_no_site | 6.01 ms                                                | 9.01 ms: 1.50x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.35x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.4 ms: 1.07x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 117 us: 4.43x faster                                                   |
| generators                 | 74.9 ms                                                | 28.6 ms: 2.61x faster                                                  |
| asyncio_tcp                | 875 ms                                                 | 483 ms: 1.81x faster                                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.78 sec: 1.75x faster                                                 |
| comprehensions             | 23.6 us                                                | 16.3 us: 1.45x faster                                                  |
| json_dumps                 | 13.3 ms                                                | 10.4 ms: 1.29x faster                                                  |
| coroutines                 | 27.0 ms                                                | 21.7 ms: 1.25x faster                                                  |
| async_tree_none            | 528 ms                                                 | 435 ms: 1.21x faster                                                   |
| deltablue                  | 3.92 ms                                                | 3.25 ms: 1.21x faster                                                  |
| chaos                      | 71.9 ms                                                | 60.9 ms: 1.18x faster                                                  |
| richards_super             | 61.9 ms                                                | 53.3 ms: 1.16x faster                                                  |
| sympy_sum                  | 169 ms                                                 | 147 ms: 1.15x faster                                                   |
| sqlglot_parse              | 1.43 ms                                                | 1.26 ms: 1.14x faster                                                  |
| raytrace                   | 309 ms                                                 | 272 ms: 1.13x faster                                                   |
| hexiom                     | 6.89 ms                                                | 6.09 ms: 1.13x faster                                                  |
| async_tree_memoization     | 639 ms                                                 | 568 ms: 1.12x faster                                                   |
| unpickle_pure_python       | 242 us                                                 | 217 us: 1.11x faster                                                   |
| sympy_str                  | 297 ms                                                 | 267 ms: 1.11x faster                                                   |
| sqlglot_transpile          | 1.75 ms                                                | 1.57 ms: 1.11x faster                                                  |
| sympy_integrate            | 21.5 ms                                                | 19.5 ms: 1.10x faster                                                  |
| nqueens                    | 87.9 ms                                                | 80.0 ms: 1.10x faster                                                  |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                                 |
| mdp                        | 2.77 sec                                               | 2.56 sec: 1.08x faster                                                 |
| logging_simple             | 6.22 us                                                | 5.74 us: 1.08x faster                                                  |
| crypto_pyaes               | 76.7 ms                                                | 70.9 ms: 1.08x faster                                                  |
| logging_format             | 6.81 us                                                | 6.32 us: 1.08x faster                                                  |
| tomli_loads                | 2.30 sec                                               | 2.14 sec: 1.08x faster                                                 |
| async_tree_none_tg         | 491 ms                                                 | 457 ms: 1.08x faster                                                   |
| sympy_expand               | 484 ms                                                 | 451 ms: 1.07x faster                                                   |
| sqlglot_normalize          | 113 ms                                                 | 105 ms: 1.07x faster                                                   |
| logging_silent             | 111 ns                                                 | 104 ns: 1.06x faster                                                   |
| regex_compile              | 141 ms                                                 | 133 ms: 1.06x faster                                                   |
| pickle_pure_python         | 320 us                                                 | 302 us: 1.06x faster                                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                 |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 710 ms: 1.05x faster                                                   |
| async_tree_memoization_tg  | 626 ms                                                 | 598 ms: 1.05x faster                                                   |
| deepcopy                   | 365 us                                                 | 349 us: 1.05x faster                                                   |
| xml_etree_parse            | 164 ms                                                 | 157 ms: 1.04x faster                                                   |
| go                         | 149 ms                                                 | 142 ms: 1.04x faster                                                   |
| richards                   | 49.8 ms                                                | 47.9 ms: 1.04x faster                                                  |
| deepcopy_reduce            | 3.22 us                                                | 3.09 us: 1.04x faster                                                  |
| tornado_http               | 98.1 ms                                                | 94.3 ms: 1.04x faster                                                  |
| nbody                      | 96.0 ms                                                | 92.4 ms: 1.04x faster                                                  |
| unpickle_list              | 5.21 us                                                | 5.04 us: 1.03x faster                                                  |
| sqlglot_optimize           | 55.3 ms                                                | 53.5 ms: 1.03x faster                                                  |
| json_loads                 | 29.2 us                                                | 28.2 us: 1.03x faster                                                  |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 738 ms: 1.03x faster                                                   |
| pprint_pformat             | 1.55 sec                                               | 1.51 sec: 1.03x faster                                                 |
| deepcopy_memo              | 40.2 us                                                | 39.0 us: 1.03x faster                                                  |
| fannkuch                   | 405 ms                                                 | 394 ms: 1.03x faster                                                   |
| pathlib                    | 18.5 ms                                                | 18.1 ms: 1.02x faster                                                  |
| xml_etree_iterparse        | 108 ms                                                 | 106 ms: 1.02x faster                                                   |
| scimark_monte_carlo        | 70.7 ms                                                | 69.3 ms: 1.02x faster                                                  |
| docutils                   | 2.66 sec                                               | 2.61 sec: 1.02x faster                                                 |
| dask                       | 365 ms                                                 | 360 ms: 1.01x faster                                                   |
| scimark_lu                 | 116 ms                                                 | 115 ms: 1.01x faster                                                   |
| pprint_safe_repr           | 747 ms                                                 | 739 ms: 1.01x faster                                                   |
| json                       | 5.24 ms                                                | 5.19 ms: 1.01x faster                                                  |
| pickle_dict                | 34.6 us                                                | 34.3 us: 1.01x faster                                                  |
| bench_thread_pool          | 834 us                                                 | 828 us: 1.01x faster                                                   |
| 2to3                       | 264 ms                                                 | 263 ms: 1.01x faster                                                   |
| meteor_contest             | 109 ms                                                 | 109 ms: 1.00x slower                                                   |
| pidigits                   | 194 ms                                                 | 196 ms: 1.01x slower                                                   |
| dulwich_log                | 64.6 ms                                                | 65.5 ms: 1.01x slower                                                  |
| pycparser                  | 1.19 sec                                               | 1.20 sec: 1.01x slower                                                 |
| scimark_sor                | 121 ms                                                 | 123 ms: 1.02x slower                                                   |
| create_gc_cycles           | 1.43 ms                                                | 1.46 ms: 1.02x slower                                                  |
| float                      | 78.9 ms                                                | 80.9 ms: 1.02x slower                                                  |
| spectral_norm              | 108 ms                                                 | 112 ms: 1.03x slower                                                   |
| gc_traversal               | 4.01 ms                                                | 4.16 ms: 1.04x slower                                                  |
| xml_etree_process          | 56.9 ms                                                | 59.4 ms: 1.04x slower                                                  |
| chameleon                  | 6.70 ms                                                | 7.00 ms: 1.05x slower                                                  |
| regex_effbot               | 3.51 ms                                                | 3.68 ms: 1.05x slower                                                  |
| pickle                     | 11.0 us                                                | 11.6 us: 1.06x slower                                                  |
| pyflate                    | 434 ms                                                 | 459 ms: 1.06x slower                                                   |
| scimark_fft                | 345 ms                                                 | 366 ms: 1.06x slower                                                   |
| mako                       | 10.7 ms                                                | 11.4 ms: 1.07x slower                                                  |
| xml_etree_generate         | 81.1 ms                                                | 86.6 ms: 1.07x slower                                                  |
| unpack_sequence            | 43.5 ns                                                | 46.6 ns: 1.07x slower                                                  |
| regex_dna                  | 205 ms                                                 | 219 ms: 1.07x slower                                                   |
| sqlite_synth               | 2.57 us                                                | 2.81 us: 1.09x slower                                                  |
| pickle_list                | 4.59 us                                                | 5.09 us: 1.11x slower                                                  |
| unpickle                   | 13.8 us                                                | 15.5 us: 1.12x slower                                                  |
| regex_v8                   | 22.9 ms                                                | 25.7 ms: 1.12x slower                                                  |
| async_generators           | 374 ms                                                 | 443 ms: 1.18x slower                                                   |
| coverage                   | 78.8 ms                                                | 95.4 ms: 1.21x slower                                                  |
| python_startup             | 8.56 ms                                                | 10.4 ms: 1.21x slower                                                  |
| telco                      | 6.86 ms                                                | 8.34 ms: 1.22x slower                                                  |
| mypy2                      | 686 ms                                                 | 839 ms: 1.22x slower                                                   |
| python_startup_no_site     | 6.01 ms                                                | 9.01 ms: 1.50x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.06x faster                                                           |

Benchmark hidden because not significant (3): scimark_sparse_mat_mult, bench_mp_pool, asyncio_websockets
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.98% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 0.97x