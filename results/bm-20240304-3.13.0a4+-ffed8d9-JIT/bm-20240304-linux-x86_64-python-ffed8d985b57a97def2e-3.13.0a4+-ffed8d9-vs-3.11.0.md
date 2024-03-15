# Results vs. 3.11.0

- fork: python
- ref: ffed8d985b57a97def2e
- machine: linux-x86_64
- commit hash: ffed8d9
- commit date: 2024-03-04
- overall geometric mean: 1.03x faster \*
- HPT reliability: 96.37%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.23x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 276 ms: 1.05x slower                                                   |
| chameleon      | 6.70 ms                                                | 6.76 ms: 1.01x slower                                                  |
| docutils       | 2.66 sec                                               | 2.70 sec: 1.01x slower                                                 |
| tornado_http   | 98.1 ms                                                | 97.0 ms: 1.01x faster                                                  |
| Geometric mean | (ref)                                                  | 1.01x slower                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 437 ms: 1.21x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 561 ms: 1.14x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 448 ms: 1.10x faster                                                   |
| async_tree_memoization_tg  | 626 ms                                                 | 574 ms: 1.09x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                                 |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                                 |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 709 ms: 1.06x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 723 ms: 1.05x faster                                                   |
| Geometric mean             | (ref)                                                  | 1.10x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 188 ms: 1.04x faster                                                   |
| nbody          | 96.0 ms                                                | 95.4 ms: 1.01x faster                                                  |
| Geometric mean | (ref)                                                  | 1.01x faster                                                           |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 143 ms: 1.01x slower                                                   |
| regex_effbot   | 3.51 ms                                                | 3.67 ms: 1.05x slower                                                  |
| regex_v8       | 22.9 ms                                                | 25.2 ms: 1.10x slower                                                  |
| regex_dna      | 205 ms                                                 | 226 ms: 1.10x slower                                                   |
| Geometric mean | (ref)                                                  | 1.06x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.29x faster                                                  |
| tomli_loads          | 2.30 sec                                               | 2.02 sec: 1.14x faster                                                 |
| unpickle_list        | 5.21 us                                                | 4.90 us: 1.06x faster                                                  |
| json_loads           | 29.2 us                                                | 27.4 us: 1.06x faster                                                  |
| xml_etree_parse      | 164 ms                                                 | 156 ms: 1.05x faster                                                   |
| pickle_pure_python   | 320 us                                                 | 305 us: 1.05x faster                                                   |
| unpickle_pure_python | 242 us                                                 | 233 us: 1.04x faster                                                   |
| xml_etree_iterparse  | 108 ms                                                 | 106 ms: 1.02x faster                                                   |
| pickle_dict          | 34.6 us                                                | 34.9 us: 1.01x slower                                                  |
| xml_etree_process    | 56.9 ms                                                | 58.7 ms: 1.03x slower                                                  |
| xml_etree_generate   | 81.1 ms                                                | 86.2 ms: 1.06x slower                                                  |
| pickle               | 11.0 us                                                | 11.8 us: 1.07x slower                                                  |
| unpickle             | 13.8 us                                                | 14.9 us: 1.08x slower                                                  |
| pickle_list          | 4.59 us                                                | 5.16 us: 1.13x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 12.3 ms: 1.44x slower                                                  |
| python_startup_no_site | 6.01 ms                                                | 10.9 ms: 1.82x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.61x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 10.8 ms: 1.02x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 110 us: 4.71x faster                                                   |
| generators                 | 74.9 ms                                                | 29.4 ms: 2.55x faster                                                  |
| asyncio_tcp                | 875 ms                                                 | 479 ms: 1.83x faster                                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.73x faster                                                 |
| comprehensions             | 23.6 us                                                | 17.0 us: 1.39x faster                                                  |
| json_dumps                 | 13.3 ms                                                | 10.4 ms: 1.29x faster                                                  |
| async_tree_none            | 528 ms                                                 | 437 ms: 1.21x faster                                                   |
| coroutines                 | 27.0 ms                                                | 22.7 ms: 1.19x faster                                                  |
| richards_super             | 61.9 ms                                                | 52.2 ms: 1.19x faster                                                  |
| deltablue                  | 3.92 ms                                                | 3.38 ms: 1.16x faster                                                  |
| chaos                      | 71.9 ms                                                | 62.4 ms: 1.15x faster                                                  |
| tomli_loads                | 2.30 sec                                               | 2.02 sec: 1.14x faster                                                 |
| async_tree_memoization     | 639 ms                                                 | 561 ms: 1.14x faster                                                   |
| sqlglot_parse              | 1.43 ms                                                | 1.29 ms: 1.11x faster                                                  |
| logging_silent             | 111 ns                                                 | 101 ns: 1.11x faster                                                   |
| logging_simple             | 6.22 us                                                | 5.67 us: 1.10x faster                                                  |
| async_tree_none_tg         | 491 ms                                                 | 448 ms: 1.10x faster                                                   |
| logging_format             | 6.81 us                                                | 6.23 us: 1.09x faster                                                  |
| async_tree_memoization_tg  | 626 ms                                                 | 574 ms: 1.09x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                                 |
| richards                   | 49.8 ms                                                | 45.8 ms: 1.09x faster                                                  |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                                 |
| sqlglot_transpile          | 1.75 ms                                                | 1.63 ms: 1.07x faster                                                  |
| sympy_sum                  | 169 ms                                                 | 157 ms: 1.07x faster                                                   |
| raytrace                   | 309 ms                                                 | 288 ms: 1.07x faster                                                   |
| unpickle_list              | 5.21 us                                                | 4.90 us: 1.06x faster                                                  |
| json_loads                 | 29.2 us                                                | 27.4 us: 1.06x faster                                                  |
| mdp                        | 2.77 sec                                               | 2.61 sec: 1.06x faster                                                 |
| sqlglot_normalize          | 113 ms                                                 | 106 ms: 1.06x faster                                                   |
| sympy_str                  | 297 ms                                                 | 280 ms: 1.06x faster                                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 709 ms: 1.06x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 723 ms: 1.05x faster                                                   |
| xml_etree_parse            | 164 ms                                                 | 156 ms: 1.05x faster                                                   |
| deepcopy_reduce            | 3.22 us                                                | 3.06 us: 1.05x faster                                                  |
| pickle_pure_python         | 320 us                                                 | 305 us: 1.05x faster                                                   |
| deepcopy                   | 365 us                                                 | 350 us: 1.04x faster                                                   |
| json                       | 5.24 ms                                                | 5.03 ms: 1.04x faster                                                  |
| crypto_pyaes               | 76.7 ms                                                | 73.9 ms: 1.04x faster                                                  |
| unpickle_pure_python       | 242 us                                                 | 233 us: 1.04x faster                                                   |
| pidigits                   | 194 ms                                                 | 188 ms: 1.04x faster                                                   |
| fannkuch                   | 405 ms                                                 | 392 ms: 1.03x faster                                                   |
| deepcopy_memo              | 40.2 us                                                | 38.9 us: 1.03x faster                                                  |
| sympy_integrate            | 21.5 ms                                                | 20.9 ms: 1.03x faster                                                  |
| sympy_expand               | 484 ms                                                 | 475 ms: 1.02x faster                                                   |
| xml_etree_iterparse        | 108 ms                                                 | 106 ms: 1.02x faster                                                   |
| meteor_contest             | 109 ms                                                 | 107 ms: 1.02x faster                                                   |
| scimark_fft                | 345 ms                                                 | 341 ms: 1.01x faster                                                   |
| tornado_http               | 98.1 ms                                                | 97.0 ms: 1.01x faster                                                  |
| pathlib                    | 18.5 ms                                                | 18.3 ms: 1.01x faster                                                  |
| pprint_pformat             | 1.55 sec                                               | 1.54 sec: 1.01x faster                                                 |
| nbody                      | 96.0 ms                                                | 95.4 ms: 1.01x faster                                                  |
| sqlglot_optimize           | 55.3 ms                                                | 55.6 ms: 1.01x slower                                                  |
| gc_traversal               | 4.01 ms                                                | 4.03 ms: 1.01x slower                                                  |
| asyncio_websockets         | 550 ms                                                 | 554 ms: 1.01x slower                                                   |
| pickle_dict                | 34.6 us                                                | 34.9 us: 1.01x slower                                                  |
| hexiom                     | 6.89 ms                                                | 6.95 ms: 1.01x slower                                                  |
| chameleon                  | 6.70 ms                                                | 6.76 ms: 1.01x slower                                                  |
| regex_compile              | 141 ms                                                 | 143 ms: 1.01x slower                                                   |
| docutils                   | 2.66 sec                                               | 2.70 sec: 1.01x slower                                                 |
| bench_thread_pool          | 834 us                                                 | 846 us: 1.01x slower                                                   |
| pycparser                  | 1.19 sec                                               | 1.20 sec: 1.02x slower                                                 |
| mako                       | 10.7 ms                                                | 10.8 ms: 1.02x slower                                                  |
| nqueens                    | 87.9 ms                                                | 90.2 ms: 1.03x slower                                                  |
| xml_etree_process          | 56.9 ms                                                | 58.7 ms: 1.03x slower                                                  |
| spectral_norm              | 108 ms                                                 | 112 ms: 1.04x slower                                                   |
| scimark_sor                | 121 ms                                                 | 127 ms: 1.04x slower                                                   |
| create_gc_cycles           | 1.43 ms                                                | 1.50 ms: 1.05x slower                                                  |
| 2to3                       | 264 ms                                                 | 276 ms: 1.05x slower                                                   |
| go                         | 149 ms                                                 | 156 ms: 1.05x slower                                                   |
| regex_effbot               | 3.51 ms                                                | 3.67 ms: 1.05x slower                                                  |
| dulwich_log                | 64.6 ms                                                | 68.1 ms: 1.05x slower                                                  |
| xml_etree_generate         | 81.1 ms                                                | 86.2 ms: 1.06x slower                                                  |
| pickle                     | 11.0 us                                                | 11.8 us: 1.07x slower                                                  |
| unpickle                   | 13.8 us                                                | 14.9 us: 1.08x slower                                                  |
| pyflate                    | 434 ms                                                 | 469 ms: 1.08x slower                                                   |
| sqlite_synth               | 2.57 us                                                | 2.79 us: 1.09x slower                                                  |
| regex_v8                   | 22.9 ms                                                | 25.2 ms: 1.10x slower                                                  |
| regex_dna                  | 205 ms                                                 | 226 ms: 1.10x slower                                                   |
| scimark_lu                 | 116 ms                                                 | 130 ms: 1.12x slower                                                   |
| pickle_list                | 4.59 us                                                | 5.16 us: 1.13x slower                                                  |
| bench_mp_pool              | 24.0 ms                                                | 28.0 ms: 1.16x slower                                                  |
| coverage                   | 78.8 ms                                                | 97.0 ms: 1.23x slower                                                  |
| telco                      | 6.86 ms                                                | 8.45 ms: 1.23x slower                                                  |
| async_generators           | 374 ms                                                 | 462 ms: 1.24x slower                                                   |
| mypy2                      | 686 ms                                                 | 884 ms: 1.29x slower                                                   |
| python_startup             | 8.56 ms                                                | 12.3 ms: 1.44x slower                                                  |
| dask                       | 365 ms                                                 | 532 ms: 1.46x slower                                                   |
| python_startup_no_site     | 6.01 ms                                                | 10.9 ms: 1.82x slower                                                  |
| unpack_sequence            | 43.5 ns                                                | 85.0 ns: 1.96x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.03x faster                                                           |

Benchmark hidden because not significant (4): scimark_sparse_mat_mult, pprint_safe_repr, scimark_monte_carlo, float
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 96.37% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.23x