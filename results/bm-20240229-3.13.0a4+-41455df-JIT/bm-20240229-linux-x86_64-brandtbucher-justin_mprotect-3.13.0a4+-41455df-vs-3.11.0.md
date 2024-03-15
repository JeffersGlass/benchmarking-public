# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_mprotect
- machine: linux-x86_64
- commit hash: 41455df
- commit date: 2024-02-29
- overall geometric mean: 1.04x faster \*
- HPT reliability: 98.25%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.13x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 275 ms: 1.04x slower                                                    |
| chameleon      | 6.70 ms                                                | 6.77 ms: 1.01x slower                                                   |
| docutils       | 2.66 sec                                               | 2.70 sec: 1.01x slower                                                  |
| tornado_http   | 98.1 ms                                                | 96.3 ms: 1.02x faster                                                   |
| Geometric mean | (ref)                                                  | 1.01x slower                                                            |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df |
|----------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 439 ms: 1.20x faster                                                    |
| async_tree_memoization     | 639 ms                                                 | 564 ms: 1.13x faster                                                    |
| async_tree_none_tg         | 491 ms                                                 | 445 ms: 1.10x faster                                                    |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                                  |
| async_tree_memoization_tg  | 626 ms                                                 | 576 ms: 1.09x faster                                                    |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                                  |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 708 ms: 1.06x faster                                                    |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 724 ms: 1.05x faster                                                    |
| Geometric mean             | (ref)                                                  | 1.10x faster                                                            |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                                    |
| nbody          | 96.0 ms                                                | 93.1 ms: 1.03x faster                                                   |
| float          | 78.9 ms                                                | 78.5 ms: 1.01x faster                                                   |
| Geometric mean | (ref)                                                  | 1.03x faster                                                            |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| regex_v8       | 22.9 ms                                                | 24.6 ms: 1.08x slower                                                   |
| regex_effbot   | 3.51 ms                                                | 3.82 ms: 1.09x slower                                                   |
| regex_dna      | 205 ms                                                 | 234 ms: 1.14x slower                                                    |
| Geometric mean | (ref)                                                  | 1.08x slower                                                            |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.3 ms: 1.29x faster                                                   |
| tomli_loads          | 2.30 sec                                               | 2.04 sec: 1.13x faster                                                  |
| unpickle_list        | 5.21 us                                                | 4.70 us: 1.11x faster                                                   |
| json_loads           | 29.2 us                                                | 27.6 us: 1.06x faster                                                   |
| pickle_pure_python   | 320 us                                                 | 305 us: 1.05x faster                                                    |
| xml_etree_parse      | 164 ms                                                 | 157 ms: 1.05x faster                                                    |
| xml_etree_iterparse  | 108 ms                                                 | 106 ms: 1.02x faster                                                    |
| unpickle_pure_python | 242 us                                                 | 238 us: 1.02x faster                                                    |
| pickle_dict          | 34.6 us                                                | 34.4 us: 1.00x faster                                                   |
| xml_etree_process    | 56.9 ms                                                | 58.6 ms: 1.03x slower                                                   |
| unpickle             | 13.8 us                                                | 14.5 us: 1.05x slower                                                   |
| xml_etree_generate   | 81.1 ms                                                | 85.7 ms: 1.06x slower                                                   |
| pickle               | 11.0 us                                                | 11.8 us: 1.07x slower                                                   |
| pickle_list          | 4.59 us                                                | 5.14 us: 1.12x slower                                                   |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                            |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 11.2 ms: 1.31x slower                                                   |
| python_startup_no_site | 6.01 ms                                                | 9.85 ms: 1.64x slower                                                   |
| Geometric mean         | (ref)                                                  | 1.47x slower                                                            |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df |
|-----------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 10.8 ms: 1.01x slower                                                   |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df |
|----------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 110 us: 4.74x faster                                                    |
| generators                 | 74.9 ms                                                | 29.3 ms: 2.55x faster                                                   |
| asyncio_tcp                | 875 ms                                                 | 475 ms: 1.84x faster                                                    |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.73x faster                                                  |
| comprehensions             | 23.6 us                                                | 17.2 us: 1.37x faster                                                   |
| json_dumps                 | 13.3 ms                                                | 10.3 ms: 1.29x faster                                                   |
| async_tree_none            | 528 ms                                                 | 439 ms: 1.20x faster                                                    |
| richards_super             | 61.9 ms                                                | 51.7 ms: 1.20x faster                                                   |
| coroutines                 | 27.0 ms                                                | 22.7 ms: 1.19x faster                                                   |
| deltablue                  | 3.92 ms                                                | 3.38 ms: 1.16x faster                                                   |
| chaos                      | 71.9 ms                                                | 62.3 ms: 1.15x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 564 ms: 1.13x faster                                                    |
| tomli_loads                | 2.30 sec                                               | 2.04 sec: 1.13x faster                                                  |
| sqlglot_parse              | 1.43 ms                                                | 1.29 ms: 1.11x faster                                                   |
| unpickle_list              | 5.21 us                                                | 4.70 us: 1.11x faster                                                   |
| logging_format             | 6.81 us                                                | 6.16 us: 1.11x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 445 ms: 1.10x faster                                                    |
| logging_simple             | 6.22 us                                                | 5.65 us: 1.10x faster                                                   |
| richards                   | 49.8 ms                                                | 45.5 ms: 1.09x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                                  |
| logging_silent             | 111 ns                                                 | 102 ns: 1.09x faster                                                    |
| async_tree_memoization_tg  | 626 ms                                                 | 576 ms: 1.09x faster                                                    |
| sympy_sum                  | 169 ms                                                 | 156 ms: 1.08x faster                                                    |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                                  |
| sqlglot_transpile          | 1.75 ms                                                | 1.63 ms: 1.08x faster                                                   |
| sympy_str                  | 297 ms                                                 | 279 ms: 1.07x faster                                                    |
| raytrace                   | 309 ms                                                 | 289 ms: 1.07x faster                                                    |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 708 ms: 1.06x faster                                                    |
| json_loads                 | 29.2 us                                                | 27.6 us: 1.06x faster                                                   |
| deepcopy_reduce            | 3.22 us                                                | 3.05 us: 1.05x faster                                                   |
| sqlglot_normalize          | 113 ms                                                 | 107 ms: 1.05x faster                                                    |
| crypto_pyaes               | 76.7 ms                                                | 72.8 ms: 1.05x faster                                                   |
| gc_traversal               | 4.01 ms                                                | 3.80 ms: 1.05x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 724 ms: 1.05x faster                                                    |
| deepcopy                   | 365 us                                                 | 348 us: 1.05x faster                                                    |
| pickle_pure_python         | 320 us                                                 | 305 us: 1.05x faster                                                    |
| xml_etree_parse            | 164 ms                                                 | 157 ms: 1.05x faster                                                    |
| deepcopy_memo              | 40.2 us                                                | 38.5 us: 1.04x faster                                                   |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                                    |
| json                       | 5.24 ms                                                | 5.05 ms: 1.04x faster                                                   |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.85 ms: 1.04x faster                                                   |
| fannkuch                   | 405 ms                                                 | 392 ms: 1.03x faster                                                    |
| sympy_integrate            | 21.5 ms                                                | 20.8 ms: 1.03x faster                                                   |
| nbody                      | 96.0 ms                                                | 93.1 ms: 1.03x faster                                                   |
| scimark_fft                | 345 ms                                                 | 337 ms: 1.02x faster                                                    |
| sympy_expand               | 484 ms                                                 | 473 ms: 1.02x faster                                                    |
| tornado_http               | 98.1 ms                                                | 96.3 ms: 1.02x faster                                                   |
| xml_etree_iterparse        | 108 ms                                                 | 106 ms: 1.02x faster                                                    |
| unpickle_pure_python       | 242 us                                                 | 238 us: 1.02x faster                                                    |
| meteor_contest             | 109 ms                                                 | 108 ms: 1.01x faster                                                    |
| float                      | 78.9 ms                                                | 78.5 ms: 1.01x faster                                                   |
| mdp                        | 2.77 sec                                               | 2.76 sec: 1.01x faster                                                  |
| pickle_dict                | 34.6 us                                                | 34.4 us: 1.00x faster                                                   |
| sqlglot_optimize           | 55.3 ms                                                | 55.5 ms: 1.00x slower                                                   |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                                    |
| bench_thread_pool          | 834 us                                                 | 841 us: 1.01x slower                                                    |
| chameleon                  | 6.70 ms                                                | 6.77 ms: 1.01x slower                                                   |
| mako                       | 10.7 ms                                                | 10.8 ms: 1.01x slower                                                   |
| docutils                   | 2.66 sec                                               | 2.70 sec: 1.01x slower                                                  |
| pycparser                  | 1.19 sec                                               | 1.21 sec: 1.02x slower                                                  |
| hexiom                     | 6.89 ms                                                | 7.01 ms: 1.02x slower                                                   |
| spectral_norm              | 108 ms                                                 | 110 ms: 1.02x slower                                                    |
| nqueens                    | 87.9 ms                                                | 89.8 ms: 1.02x slower                                                   |
| xml_etree_process          | 56.9 ms                                                | 58.6 ms: 1.03x slower                                                   |
| 2to3                       | 264 ms                                                 | 275 ms: 1.04x slower                                                    |
| go                         | 149 ms                                                 | 155 ms: 1.04x slower                                                    |
| unpickle                   | 13.8 us                                                | 14.5 us: 1.05x slower                                                   |
| scimark_sor                | 121 ms                                                 | 127 ms: 1.05x slower                                                    |
| create_gc_cycles           | 1.43 ms                                                | 1.51 ms: 1.06x slower                                                   |
| xml_etree_generate         | 81.1 ms                                                | 85.7 ms: 1.06x slower                                                   |
| dulwich_log                | 64.6 ms                                                | 68.7 ms: 1.06x slower                                                   |
| pickle                     | 11.0 us                                                | 11.8 us: 1.07x slower                                                   |
| regex_v8                   | 22.9 ms                                                | 24.6 ms: 1.08x slower                                                   |
| pyflate                    | 434 ms                                                 | 471 ms: 1.09x slower                                                    |
| regex_effbot               | 3.51 ms                                                | 3.82 ms: 1.09x slower                                                   |
| sqlite_synth               | 2.57 us                                                | 2.85 us: 1.11x slower                                                   |
| scimark_lu                 | 116 ms                                                 | 129 ms: 1.11x slower                                                    |
| pickle_list                | 4.59 us                                                | 5.14 us: 1.12x slower                                                   |
| regex_dna                  | 205 ms                                                 | 234 ms: 1.14x slower                                                    |
| telco                      | 6.86 ms                                                | 8.36 ms: 1.22x slower                                                   |
| coverage                   | 78.8 ms                                                | 96.4 ms: 1.22x slower                                                   |
| async_generators           | 374 ms                                                 | 460 ms: 1.23x slower                                                    |
| mypy2                      | 686 ms                                                 | 878 ms: 1.28x slower                                                    |
| python_startup             | 8.56 ms                                                | 11.2 ms: 1.31x slower                                                   |
| dask                       | 365 ms                                                 | 530 ms: 1.45x slower                                                    |
| python_startup_no_site     | 6.01 ms                                                | 9.85 ms: 1.64x slower                                                   |
| unpack_sequence            | 43.5 ns                                                | 96.7 ns: 2.23x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.04x faster                                                            |

Benchmark hidden because not significant (6): pprint_pformat, pathlib, scimark_monte_carlo, bench_mp_pool, regex_compile, pprint_safe_repr
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 98.25% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.13x