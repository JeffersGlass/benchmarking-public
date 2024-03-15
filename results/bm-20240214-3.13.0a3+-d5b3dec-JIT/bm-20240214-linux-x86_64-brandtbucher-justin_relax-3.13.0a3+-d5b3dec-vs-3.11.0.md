
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_relax
- machine: linux-x86_64
- commit hash: d5b3dec
- commit date: 2024-02-14
- overall geometric mean: 1.06x faster \*
- HPT reliability: 99.99%
- HPT 99th percentile: 1.01x faster
- Memory change: 1.03x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 270 ms: 1.02x slower                                                 |
| chameleon      | 6.70 ms                                                | 6.82 ms: 1.02x slower                                                |
| docutils       | 2.66 sec                                               | 2.63 sec: 1.01x faster                                               |
| tornado_http   | 98.1 ms                                                | 95.6 ms: 1.03x faster                                                |
| Geometric mean | (ref)                                                  | 1.00x faster                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 438 ms: 1.21x faster                                                 |
| async_tree_memoization     | 639 ms                                                 | 561 ms: 1.14x faster                                                 |
| async_tree_none_tg         | 491 ms                                                 | 447 ms: 1.10x faster                                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 571 ms: 1.10x faster                                                 |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                               |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                               |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 717 ms: 1.06x faster                                                 |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 709 ms: 1.06x faster                                                 |
| Geometric mean             | (ref)                                                  | 1.10x faster                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                                 |
| nbody          | 96.0 ms                                                | 99.1 ms: 1.03x slower                                                |
| float          | 78.9 ms                                                | 81.8 ms: 1.04x slower                                                |
| Geometric mean | (ref)                                                  | 1.01x slower                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 134 ms: 1.05x faster                                                 |
| regex_effbot   | 3.51 ms                                                | 3.74 ms: 1.07x slower                                                |
| regex_v8       | 22.9 ms                                                | 25.3 ms: 1.11x slower                                                |
| regex_dna      | 205 ms                                                 | 231 ms: 1.13x slower                                                 |
| Geometric mean | (ref)                                                  | 1.06x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.3 ms: 1.30x faster                                                |
| tomli_loads          | 2.30 sec                                               | 2.05 sec: 1.12x faster                                               |
| unpickle_pure_python | 242 us                                                 | 219 us: 1.10x faster                                                 |
| pickle_pure_python   | 320 us                                                 | 293 us: 1.09x faster                                                 |
| json_loads           | 29.2 us                                                | 27.3 us: 1.07x faster                                                |
| xml_etree_parse      | 164 ms                                                 | 155 ms: 1.06x faster                                                 |
| pickle_dict          | 34.6 us                                                | 33.6 us: 1.03x faster                                                |
| unpickle_list        | 5.21 us                                                | 5.09 us: 1.02x faster                                                |
| xml_etree_iterparse  | 108 ms                                                 | 106 ms: 1.02x faster                                                 |
| xml_etree_process    | 56.9 ms                                                | 58.5 ms: 1.03x slower                                                |
| xml_etree_generate   | 81.1 ms                                                | 85.7 ms: 1.06x slower                                                |
| pickle               | 11.0 us                                                | 11.7 us: 1.07x slower                                                |
| pickle_list          | 4.59 us                                                | 4.99 us: 1.09x slower                                                |
| unpickle             | 13.8 us                                                | 16.1 us: 1.17x slower                                                |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                         |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                |
| python_startup_no_site | 6.01 ms                                                | 8.80 ms: 1.46x slower                                                |
| Geometric mean         | (ref)                                                  | 1.32x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.3 ms: 1.06x slower                                                |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 111 us: 4.68x faster                                                 |
| generators                 | 74.9 ms                                                | 29.2 ms: 2.56x faster                                                |
| asyncio_tcp                | 875 ms                                                 | 491 ms: 1.78x faster                                                 |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.73x faster                                               |
| comprehensions             | 23.6 us                                                | 18.1 us: 1.31x faster                                                |
| json_dumps                 | 13.3 ms                                                | 10.3 ms: 1.30x faster                                                |
| async_tree_none            | 528 ms                                                 | 438 ms: 1.21x faster                                                 |
| coroutines                 | 27.0 ms                                                | 22.6 ms: 1.20x faster                                                |
| deltablue                  | 3.92 ms                                                | 3.28 ms: 1.19x faster                                                |
| richards_super             | 61.9 ms                                                | 53.2 ms: 1.16x faster                                                |
| chaos                      | 71.9 ms                                                | 62.5 ms: 1.15x faster                                                |
| gc_traversal               | 4.01 ms                                                | 3.50 ms: 1.15x faster                                                |
| raytrace                   | 309 ms                                                 | 269 ms: 1.15x faster                                                 |
| async_tree_memoization     | 639 ms                                                 | 561 ms: 1.14x faster                                                 |
| sqlglot_parse              | 1.43 ms                                                | 1.26 ms: 1.13x faster                                                |
| logging_simple             | 6.22 us                                                | 5.53 us: 1.13x faster                                                |
| logging_format             | 6.81 us                                                | 6.06 us: 1.12x faster                                                |
| tomli_loads                | 2.30 sec                                               | 2.05 sec: 1.12x faster                                               |
| logging_silent             | 111 ns                                                 | 100 ns: 1.11x faster                                                 |
| sqlglot_transpile          | 1.75 ms                                                | 1.58 ms: 1.10x faster                                                |
| unpickle_pure_python       | 242 us                                                 | 219 us: 1.10x faster                                                 |
| async_tree_none_tg         | 491 ms                                                 | 447 ms: 1.10x faster                                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 571 ms: 1.10x faster                                                 |
| pickle_pure_python         | 320 us                                                 | 293 us: 1.09x faster                                                 |
| sympy_sum                  | 169 ms                                                 | 155 ms: 1.09x faster                                                 |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                               |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                               |
| deepcopy_reduce            | 3.22 us                                                | 2.98 us: 1.08x faster                                                |
| sympy_str                  | 297 ms                                                 | 276 ms: 1.08x faster                                                 |
| deepcopy                   | 365 us                                                 | 341 us: 1.07x faster                                                 |
| json_loads                 | 29.2 us                                                | 27.3 us: 1.07x faster                                                |
| deepcopy_memo              | 40.2 us                                                | 37.7 us: 1.06x faster                                                |
| mdp                        | 2.77 sec                                               | 2.61 sec: 1.06x faster                                               |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 717 ms: 1.06x faster                                                 |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 709 ms: 1.06x faster                                                 |
| xml_etree_parse            | 164 ms                                                 | 155 ms: 1.06x faster                                                 |
| regex_compile              | 141 ms                                                 | 134 ms: 1.05x faster                                                 |
| json                       | 5.24 ms                                                | 5.00 ms: 1.05x faster                                                |
| sqlglot_normalize          | 113 ms                                                 | 108 ms: 1.05x faster                                                 |
| richards                   | 49.8 ms                                                | 47.5 ms: 1.05x faster                                                |
| sympy_integrate            | 21.5 ms                                                | 20.5 ms: 1.05x faster                                                |
| crypto_pyaes               | 76.7 ms                                                | 73.7 ms: 1.04x faster                                                |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                                 |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.85 ms: 1.04x faster                                                |
| sympy_expand               | 484 ms                                                 | 467 ms: 1.04x faster                                                 |
| pprint_pformat             | 1.55 sec                                               | 1.50 sec: 1.03x faster                                               |
| pickle_dict                | 34.6 us                                                | 33.6 us: 1.03x faster                                                |
| go                         | 149 ms                                                 | 144 ms: 1.03x faster                                                 |
| nqueens                    | 87.9 ms                                                | 85.4 ms: 1.03x faster                                                |
| tornado_http               | 98.1 ms                                                | 95.6 ms: 1.03x faster                                                |
| scimark_lu                 | 116 ms                                                 | 113 ms: 1.03x faster                                                 |
| unpickle_list              | 5.21 us                                                | 5.09 us: 1.02x faster                                                |
| meteor_contest             | 109 ms                                                 | 107 ms: 1.02x faster                                                 |
| pprint_safe_repr           | 747 ms                                                 | 736 ms: 1.02x faster                                                 |
| xml_etree_iterparse        | 108 ms                                                 | 106 ms: 1.02x faster                                                 |
| scimark_monte_carlo        | 70.7 ms                                                | 69.7 ms: 1.01x faster                                                |
| sqlglot_optimize           | 55.3 ms                                                | 54.5 ms: 1.01x faster                                                |
| docutils                   | 2.66 sec                                               | 2.63 sec: 1.01x faster                                               |
| hexiom                     | 6.89 ms                                                | 6.81 ms: 1.01x faster                                                |
| dask                       | 365 ms                                                 | 361 ms: 1.01x faster                                                 |
| scimark_sor                | 121 ms                                                 | 120 ms: 1.01x faster                                                 |
| pathlib                    | 18.5 ms                                                | 18.4 ms: 1.01x faster                                                |
| fannkuch                   | 405 ms                                                 | 403 ms: 1.01x faster                                                 |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                                 |
| chameleon                  | 6.70 ms                                                | 6.82 ms: 1.02x slower                                                |
| create_gc_cycles           | 1.43 ms                                                | 1.46 ms: 1.02x slower                                                |
| 2to3                       | 264 ms                                                 | 270 ms: 1.02x slower                                                 |
| scimark_fft                | 345 ms                                                 | 355 ms: 1.03x slower                                                 |
| xml_etree_process          | 56.9 ms                                                | 58.5 ms: 1.03x slower                                                |
| nbody                      | 96.0 ms                                                | 99.1 ms: 1.03x slower                                                |
| dulwich_log                | 64.6 ms                                                | 66.8 ms: 1.03x slower                                                |
| float                      | 78.9 ms                                                | 81.8 ms: 1.04x slower                                                |
| mako                       | 10.7 ms                                                | 11.3 ms: 1.06x slower                                                |
| xml_etree_generate         | 81.1 ms                                                | 85.7 ms: 1.06x slower                                                |
| pickle                     | 11.0 us                                                | 11.7 us: 1.07x slower                                                |
| regex_effbot               | 3.51 ms                                                | 3.74 ms: 1.07x slower                                                |
| unpack_sequence            | 43.5 ns                                                | 46.4 ns: 1.07x slower                                                |
| pickle_list                | 4.59 us                                                | 4.99 us: 1.09x slower                                                |
| sqlite_synth               | 2.57 us                                                | 2.81 us: 1.09x slower                                                |
| pyflate                    | 434 ms                                                 | 478 ms: 1.10x slower                                                 |
| regex_v8                   | 22.9 ms                                                | 25.3 ms: 1.11x slower                                                |
| regex_dna                  | 205 ms                                                 | 231 ms: 1.13x slower                                                 |
| unpickle                   | 13.8 us                                                | 16.1 us: 1.17x slower                                                |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                |
| coverage                   | 78.8 ms                                                | 95.7 ms: 1.21x slower                                                |
| async_generators           | 374 ms                                                 | 460 ms: 1.23x slower                                                 |
| telco                      | 6.86 ms                                                | 8.44 ms: 1.23x slower                                                |
| mypy2                      | 686 ms                                                 | 858 ms: 1.25x slower                                                 |
| python_startup_no_site     | 6.01 ms                                                | 8.80 ms: 1.46x slower                                                |
| Geometric mean             | (ref)                                                  | 1.06x faster                                                         |

Benchmark hidden because not significant (4): bench_mp_pool, bench_thread_pool, spectral_norm, pycparser
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.99% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 1.03x