# Results vs. 3.11.0

- fork: python
- ref: f0df35eeca2ccdfd58cf
- machine: linux-x86_64
- commit hash: f0df35e
- commit date: 2024-02-29
- overall geometric mean: 1.02x faster \*
- HPT reliability: 55.57%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.24x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 280 ms: 1.06x slower                                                   |
| chameleon      | 6.70 ms                                                | 6.77 ms: 1.01x slower                                                  |
| docutils       | 2.66 sec                                               | 2.72 sec: 1.02x slower                                                 |
| tornado_http   | 98.1 ms                                                | 97.0 ms: 1.01x faster                                                  |
| Geometric mean | (ref)                                                  | 1.02x slower                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 439 ms: 1.20x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 566 ms: 1.13x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 449 ms: 1.09x faster                                                   |
| async_tree_memoization_tg  | 626 ms                                                 | 579 ms: 1.08x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                 |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                 |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 712 ms: 1.05x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 724 ms: 1.05x faster                                                   |
| Geometric mean             | (ref)                                                  | 1.09x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 188 ms: 1.03x faster                                                   |
| nbody          | 96.0 ms                                                | 95.0 ms: 1.01x faster                                                  |
| float          | 78.9 ms                                                | 81.5 ms: 1.03x slower                                                  |
| Geometric mean | (ref)                                                  | 1.00x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.63 ms: 1.04x slower                                                  |
| regex_compile  | 141 ms                                                 | 151 ms: 1.07x slower                                                   |
| regex_v8       | 22.9 ms                                                | 24.7 ms: 1.08x slower                                                  |
| regex_dna      | 205 ms                                                 | 224 ms: 1.09x slower                                                   |
| Geometric mean | (ref)                                                  | 1.07x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.3 ms: 1.29x faster                                                  |
| json_loads           | 29.2 us                                                | 27.3 us: 1.07x faster                                                  |
| unpickle_list        | 5.21 us                                                | 4.94 us: 1.06x faster                                                  |
| tomli_loads          | 2.30 sec                                               | 2.18 sec: 1.06x faster                                                 |
| pickle_pure_python   | 320 us                                                 | 305 us: 1.05x faster                                                   |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                                   |
| unpickle_pure_python | 242 us                                                 | 245 us: 1.01x slower                                                   |
| pickle_dict          | 34.6 us                                                | 35.2 us: 1.02x slower                                                  |
| xml_etree_process    | 56.9 ms                                                | 58.7 ms: 1.03x slower                                                  |
| pickle               | 11.0 us                                                | 11.6 us: 1.06x slower                                                  |
| xml_etree_generate   | 81.1 ms                                                | 86.2 ms: 1.06x slower                                                  |
| unpickle             | 13.8 us                                                | 15.0 us: 1.09x slower                                                  |
| pickle_list          | 4.59 us                                                | 5.26 us: 1.15x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.01x faster                                                           |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 12.3 ms: 1.43x slower                                                  |
| python_startup_no_site | 6.01 ms                                                | 10.9 ms: 1.82x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.61x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.6 ms: 1.08x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 110 us: 4.73x faster                                                   |
| generators                 | 74.9 ms                                                | 29.1 ms: 2.57x faster                                                  |
| asyncio_tcp                | 875 ms                                                 | 487 ms: 1.80x faster                                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.72x faster                                                 |
| comprehensions             | 23.6 us                                                | 18.0 us: 1.31x faster                                                  |
| json_dumps                 | 13.3 ms                                                | 10.3 ms: 1.29x faster                                                  |
| coroutines                 | 27.0 ms                                                | 22.3 ms: 1.21x faster                                                  |
| async_tree_none            | 528 ms                                                 | 439 ms: 1.20x faster                                                   |
| richards_super             | 61.9 ms                                                | 52.9 ms: 1.17x faster                                                  |
| deltablue                  | 3.92 ms                                                | 3.43 ms: 1.14x faster                                                  |
| async_tree_memoization     | 639 ms                                                 | 566 ms: 1.13x faster                                                   |
| chaos                      | 71.9 ms                                                | 64.0 ms: 1.12x faster                                                  |
| logging_silent             | 111 ns                                                 | 100 ns: 1.11x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 449 ms: 1.09x faster                                                   |
| logging_format             | 6.81 us                                                | 6.25 us: 1.09x faster                                                  |
| logging_simple             | 6.22 us                                                | 5.71 us: 1.09x faster                                                  |
| sqlglot_parse              | 1.43 ms                                                | 1.32 ms: 1.08x faster                                                  |
| async_tree_memoization_tg  | 626 ms                                                 | 579 ms: 1.08x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                 |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                 |
| json_loads                 | 29.2 us                                                | 27.3 us: 1.07x faster                                                  |
| gc_traversal               | 4.01 ms                                                | 3.77 ms: 1.06x faster                                                  |
| sympy_sum                  | 169 ms                                                 | 160 ms: 1.06x faster                                                   |
| unpickle_list              | 5.21 us                                                | 4.94 us: 1.06x faster                                                  |
| tomli_loads                | 2.30 sec                                               | 2.18 sec: 1.06x faster                                                 |
| sqlglot_transpile          | 1.75 ms                                                | 1.66 ms: 1.05x faster                                                  |
| deepcopy_reduce            | 3.22 us                                                | 3.05 us: 1.05x faster                                                  |
| raytrace                   | 309 ms                                                 | 293 ms: 1.05x faster                                                   |
| richards                   | 49.8 ms                                                | 47.3 ms: 1.05x faster                                                  |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 712 ms: 1.05x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 724 ms: 1.05x faster                                                   |
| pickle_pure_python         | 320 us                                                 | 305 us: 1.05x faster                                                   |
| sympy_str                  | 297 ms                                                 | 284 ms: 1.05x faster                                                   |
| sqlglot_normalize          | 113 ms                                                 | 108 ms: 1.05x faster                                                   |
| xml_etree_parse            | 164 ms                                                 | 158 ms: 1.04x faster                                                   |
| deepcopy                   | 365 us                                                 | 352 us: 1.04x faster                                                   |
| pidigits                   | 194 ms                                                 | 188 ms: 1.03x faster                                                   |
| json                       | 5.24 ms                                                | 5.08 ms: 1.03x faster                                                  |
| crypto_pyaes               | 76.7 ms                                                | 74.9 ms: 1.02x faster                                                  |
| sympy_integrate            | 21.5 ms                                                | 21.0 ms: 1.02x faster                                                  |
| deepcopy_memo              | 40.2 us                                                | 39.4 us: 1.02x faster                                                  |
| tornado_http               | 98.1 ms                                                | 97.0 ms: 1.01x faster                                                  |
| nbody                      | 96.0 ms                                                | 95.0 ms: 1.01x faster                                                  |
| mdp                        | 2.77 sec                                               | 2.76 sec: 1.01x faster                                                 |
| meteor_contest             | 109 ms                                                 | 110 ms: 1.01x slower                                                   |
| chameleon                  | 6.70 ms                                                | 6.77 ms: 1.01x slower                                                  |
| unpickle_pure_python       | 242 us                                                 | 245 us: 1.01x slower                                                   |
| bench_thread_pool          | 834 us                                                 | 850 us: 1.02x slower                                                   |
| pickle_dict                | 34.6 us                                                | 35.2 us: 1.02x slower                                                  |
| docutils                   | 2.66 sec                                               | 2.72 sec: 1.02x slower                                                 |
| pycparser                  | 1.19 sec                                               | 1.22 sec: 1.03x slower                                                 |
| scimark_fft                | 345 ms                                                 | 354 ms: 1.03x slower                                                   |
| sqlglot_optimize           | 55.3 ms                                                | 56.9 ms: 1.03x slower                                                  |
| xml_etree_process          | 56.9 ms                                                | 58.7 ms: 1.03x slower                                                  |
| float                      | 78.9 ms                                                | 81.5 ms: 1.03x slower                                                  |
| regex_effbot               | 3.51 ms                                                | 3.63 ms: 1.04x slower                                                  |
| fannkuch                   | 405 ms                                                 | 423 ms: 1.04x slower                                                   |
| create_gc_cycles           | 1.43 ms                                                | 1.50 ms: 1.05x slower                                                  |
| nqueens                    | 87.9 ms                                                | 92.0 ms: 1.05x slower                                                  |
| 2to3                       | 264 ms                                                 | 280 ms: 1.06x slower                                                   |
| pickle                     | 11.0 us                                                | 11.6 us: 1.06x slower                                                  |
| scimark_sor                | 121 ms                                                 | 129 ms: 1.06x slower                                                   |
| pprint_safe_repr           | 747 ms                                                 | 794 ms: 1.06x slower                                                   |
| go                         | 149 ms                                                 | 158 ms: 1.06x slower                                                   |
| xml_etree_generate         | 81.1 ms                                                | 86.2 ms: 1.06x slower                                                  |
| regex_compile              | 141 ms                                                 | 151 ms: 1.07x slower                                                   |
| dulwich_log                | 64.6 ms                                                | 69.3 ms: 1.07x slower                                                  |
| pprint_pformat             | 1.55 sec                                               | 1.67 sec: 1.08x slower                                                 |
| scimark_monte_carlo        | 70.7 ms                                                | 76.2 ms: 1.08x slower                                                  |
| regex_v8                   | 22.9 ms                                                | 24.7 ms: 1.08x slower                                                  |
| mako                       | 10.7 ms                                                | 11.6 ms: 1.08x slower                                                  |
| unpickle                   | 13.8 us                                                | 15.0 us: 1.09x slower                                                  |
| sqlite_synth               | 2.57 us                                                | 2.81 us: 1.09x slower                                                  |
| hexiom                     | 6.89 ms                                                | 7.53 ms: 1.09x slower                                                  |
| regex_dna                  | 205 ms                                                 | 224 ms: 1.09x slower                                                   |
| spectral_norm              | 108 ms                                                 | 119 ms: 1.10x slower                                                   |
| scimark_lu                 | 116 ms                                                 | 133 ms: 1.14x slower                                                   |
| pickle_list                | 4.59 us                                                | 5.26 us: 1.15x slower                                                  |
| bench_mp_pool              | 24.0 ms                                                | 28.0 ms: 1.16x slower                                                  |
| pyflate                    | 434 ms                                                 | 513 ms: 1.18x slower                                                   |
| coverage                   | 78.8 ms                                                | 96.3 ms: 1.22x slower                                                  |
| async_generators           | 374 ms                                                 | 462 ms: 1.24x slower                                                   |
| telco                      | 6.86 ms                                                | 8.66 ms: 1.26x slower                                                  |
| mypy2                      | 686 ms                                                 | 889 ms: 1.30x slower                                                   |
| python_startup             | 8.56 ms                                                | 12.3 ms: 1.43x slower                                                  |
| python_startup_no_site     | 6.01 ms                                                | 10.9 ms: 1.82x slower                                                  |
| unpack_sequence            | 43.5 ns                                                | 121 ns: 2.79x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.02x faster                                                           |

Benchmark hidden because not significant (5): xml_etree_iterparse, sympy_expand, asyncio_websockets, scimark_sparse_mat_mult, pathlib
Ignored benchmarks (13) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 55.57% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.24x