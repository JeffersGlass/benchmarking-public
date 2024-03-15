
# Results vs. 3.11.0

- fork: python
- ref: 2feec0fc7fd0b9caae7a
- machine: linux-x86_64
- commit hash: 2feec0f
- commit date: 2023-12-18
- overall geometric mean: 1.01x faster
- HPT reliability: 94.17%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 281 ms: 1.06x slower                                                   |
| chameleon      | 6.70 ms                                                | 7.32 ms: 1.09x slower                                                  |
| docutils       | 2.66 sec                                               | 2.71 sec: 1.02x slower                                                 |
| Geometric mean | (ref)                                                  | 1.04x slower                                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 451 ms: 1.17x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 578 ms: 1.11x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 454 ms: 1.08x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.06x faster                                                 |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 592 ms: 1.06x faster                                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 723 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 736 ms: 1.03x faster                                                   |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 196 ms: 1.01x slower                                                   |
| float          | 78.9 ms                                                | 88.3 ms: 1.12x slower                                                  |
| nbody          | 96.0 ms                                                | 113 ms: 1.18x slower                                                   |
| Geometric mean | (ref)                                                  | 1.10x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.60 ms: 1.03x slower                                                  |
| regex_dna      | 205 ms                                                 | 216 ms: 1.06x slower                                                   |
| regex_compile  | 141 ms                                                 | 151 ms: 1.07x slower                                                   |
| regex_v8       | 22.9 ms                                                | 26.1 ms: 1.14x slower                                                  |
| Geometric mean | (ref)                                                  | 1.07x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.28x faster                                                  |
| pickle_pure_python   | 320 us                                                 | 303 us: 1.06x faster                                                   |
| json_loads           | 29.2 us                                                | 27.7 us: 1.05x faster                                                  |
| xml_etree_parse      | 164 ms                                                 | 157 ms: 1.05x faster                                                   |
| unpickle_pure_python | 242 us                                                 | 233 us: 1.04x faster                                                   |
| pickle_dict          | 34.6 us                                                | 34.0 us: 1.02x faster                                                  |
| tomli_loads          | 2.30 sec                                               | 2.32 sec: 1.01x slower                                                 |
| xml_etree_iterparse  | 108 ms                                                 | 109 ms: 1.01x slower                                                   |
| unpickle_list        | 5.21 us                                                | 5.28 us: 1.01x slower                                                  |
| pickle               | 11.0 us                                                | 11.3 us: 1.03x slower                                                  |
| xml_etree_process    | 56.9 ms                                                | 61.2 ms: 1.08x slower                                                  |
| unpickle             | 13.8 us                                                | 14.9 us: 1.08x slower                                                  |
| pickle_list          | 4.59 us                                                | 5.03 us: 1.10x slower                                                  |
| xml_etree_generate   | 81.1 ms                                                | 89.3 ms: 1.10x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.00x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                  |
| python_startup_no_site | 6.01 ms                                                | 8.74 ms: 1.45x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.31x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 13.5 ms: 1.27x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 115 us: 4.51x faster                                                   |
| generators                 | 74.9 ms                                                | 29.8 ms: 2.51x faster                                                  |
| asyncio_tcp                | 875 ms                                                 | 495 ms: 1.77x faster                                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.73x faster                                                 |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.28x faster                                                  |
| coroutines                 | 27.0 ms                                                | 22.6 ms: 1.20x faster                                                  |
| async_tree_none            | 528 ms                                                 | 451 ms: 1.17x faster                                                   |
| comprehensions             | 23.6 us                                                | 20.7 us: 1.14x faster                                                  |
| richards_super             | 61.9 ms                                                | 54.8 ms: 1.13x faster                                                  |
| async_tree_memoization     | 639 ms                                                 | 578 ms: 1.11x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 454 ms: 1.08x faster                                                   |
| sqlglot_parse              | 1.43 ms                                                | 1.33 ms: 1.08x faster                                                  |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.06x faster                                                 |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 592 ms: 1.06x faster                                                   |
| sqlglot_transpile          | 1.75 ms                                                | 1.66 ms: 1.06x faster                                                  |
| pickle_pure_python         | 320 us                                                 | 303 us: 1.06x faster                                                   |
| sympy_sum                  | 169 ms                                                 | 160 ms: 1.05x faster                                                   |
| json_loads                 | 29.2 us                                                | 27.7 us: 1.05x faster                                                  |
| xml_etree_parse            | 164 ms                                                 | 157 ms: 1.05x faster                                                   |
| mdp                        | 2.77 sec                                               | 2.67 sec: 1.04x faster                                                 |
| raytrace                   | 309 ms                                                 | 297 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 723 ms: 1.04x faster                                                   |
| unpickle_pure_python       | 242 us                                                 | 233 us: 1.04x faster                                                   |
| logging_simple             | 6.22 us                                                | 6.02 us: 1.03x faster                                                  |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 736 ms: 1.03x faster                                                   |
| deepcopy                   | 365 us                                                 | 354 us: 1.03x faster                                                   |
| logging_silent             | 111 ns                                                 | 108 ns: 1.03x faster                                                   |
| richards                   | 49.8 ms                                                | 48.4 ms: 1.03x faster                                                  |
| sympy_str                  | 297 ms                                                 | 290 ms: 1.03x faster                                                   |
| deepcopy_reduce            | 3.22 us                                                | 3.15 us: 1.02x faster                                                  |
| pickle_dict                | 34.6 us                                                | 34.0 us: 1.02x faster                                                  |
| sympy_integrate            | 21.5 ms                                                | 21.2 ms: 1.01x faster                                                  |
| json                       | 5.24 ms                                                | 5.17 ms: 1.01x faster                                                  |
| scimark_lu                 | 116 ms                                                 | 115 ms: 1.01x faster                                                   |
| gc_traversal               | 4.01 ms                                                | 3.97 ms: 1.01x faster                                                  |
| sqlglot_normalize          | 113 ms                                                 | 113 ms: 1.00x slower                                                   |
| asyncio_websockets         | 550 ms                                                 | 553 ms: 1.00x slower                                                   |
| pidigits                   | 194 ms                                                 | 196 ms: 1.01x slower                                                   |
| tomli_loads                | 2.30 sec                                               | 2.32 sec: 1.01x slower                                                 |
| pathlib                    | 18.5 ms                                                | 18.7 ms: 1.01x slower                                                  |
| bench_thread_pool          | 834 us                                                 | 843 us: 1.01x slower                                                   |
| xml_etree_iterparse        | 108 ms                                                 | 109 ms: 1.01x slower                                                   |
| sympy_expand               | 484 ms                                                 | 490 ms: 1.01x slower                                                   |
| unpickle_list              | 5.21 us                                                | 5.28 us: 1.01x slower                                                  |
| create_gc_cycles           | 1.43 ms                                                | 1.45 ms: 1.01x slower                                                  |
| docutils                   | 2.66 sec                                               | 2.71 sec: 1.02x slower                                                 |
| unpack_sequence            | 43.5 ns                                                | 44.3 ns: 1.02x slower                                                  |
| scimark_sor                | 121 ms                                                 | 124 ms: 1.02x slower                                                   |
| regex_effbot               | 3.51 ms                                                | 3.60 ms: 1.03x slower                                                  |
| pickle                     | 11.0 us                                                | 11.3 us: 1.03x slower                                                  |
| meteor_contest             | 109 ms                                                 | 112 ms: 1.03x slower                                                   |
| sqlglot_optimize           | 55.3 ms                                                | 57.4 ms: 1.04x slower                                                  |
| nqueens                    | 87.9 ms                                                | 91.3 ms: 1.04x slower                                                  |
| go                         | 149 ms                                                 | 155 ms: 1.04x slower                                                   |
| fannkuch                   | 405 ms                                                 | 426 ms: 1.05x slower                                                   |
| pycparser                  | 1.19 sec                                               | 1.25 sec: 1.05x slower                                                 |
| regex_dna                  | 205 ms                                                 | 216 ms: 1.06x slower                                                   |
| 2to3                       | 264 ms                                                 | 281 ms: 1.06x slower                                                   |
| pprint_safe_repr           | 747 ms                                                 | 798 ms: 1.07x slower                                                   |
| dulwich_log                | 64.6 ms                                                | 69.1 ms: 1.07x slower                                                  |
| regex_compile              | 141 ms                                                 | 151 ms: 1.07x slower                                                   |
| pprint_pformat             | 1.55 sec                                               | 1.67 sec: 1.07x slower                                                 |
| xml_etree_process          | 56.9 ms                                                | 61.2 ms: 1.08x slower                                                  |
| unpickle                   | 13.8 us                                                | 14.9 us: 1.08x slower                                                  |
| crypto_pyaes               | 76.7 ms                                                | 82.5 ms: 1.08x slower                                                  |
| chameleon                  | 6.70 ms                                                | 7.32 ms: 1.09x slower                                                  |
| pickle_list                | 4.59 us                                                | 5.03 us: 1.10x slower                                                  |
| xml_etree_generate         | 81.1 ms                                                | 89.3 ms: 1.10x slower                                                  |
| sqlite_synth               | 2.57 us                                                | 2.87 us: 1.12x slower                                                  |
| float                      | 78.9 ms                                                | 88.3 ms: 1.12x slower                                                  |
| scimark_monte_carlo        | 70.7 ms                                                | 79.7 ms: 1.13x slower                                                  |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.72 ms: 1.14x slower                                                  |
| regex_v8                   | 22.9 ms                                                | 26.1 ms: 1.14x slower                                                  |
| deltablue                  | 3.92 ms                                                | 4.57 ms: 1.16x slower                                                  |
| pyflate                    | 434 ms                                                 | 508 ms: 1.17x slower                                                   |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                  |
| nbody                      | 96.0 ms                                                | 113 ms: 1.18x slower                                                   |
| hexiom                     | 6.89 ms                                                | 8.15 ms: 1.18x slower                                                  |
| coverage                   | 78.8 ms                                                | 95.6 ms: 1.21x slower                                                  |
| async_generators           | 374 ms                                                 | 458 ms: 1.23x slower                                                   |
| mypy2                      | 686 ms                                                 | 863 ms: 1.26x slower                                                   |
| mako                       | 10.7 ms                                                | 13.5 ms: 1.27x slower                                                  |
| telco                      | 6.86 ms                                                | 8.78 ms: 1.28x slower                                                  |
| scimark_fft                | 345 ms                                                 | 443 ms: 1.28x slower                                                   |
| spectral_norm              | 108 ms                                                 | 140 ms: 1.30x slower                                                   |
| python_startup_no_site     | 6.01 ms                                                | 8.74 ms: 1.45x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.01x faster                                                           |

Benchmark hidden because not significant (6): chaos, deepcopy_memo, bench_mp_pool, logging_format, tornado_http, dask
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 94.17% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.98x