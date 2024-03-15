
# Results vs. 3.11.0

- fork: python
- ref: a571a2fd3fdaeafdfd71
- machine: linux-x86_64
- commit hash: a571a2f
- commit date: 2024-01-18
- overall geometric mean: 1.07x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 264 ms: 1.00x faster                                                   |
| chameleon      | 6.70 ms                                                | 6.86 ms: 1.02x slower                                                  |
| docutils       | 2.66 sec                                               | 2.60 sec: 1.02x faster                                                 |
| tornado_http   | 98.1 ms                                                | 94.5 ms: 1.04x faster                                                  |
| Geometric mean | (ref)                                                  | 1.01x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 432 ms: 1.22x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 560 ms: 1.14x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 440 ms: 1.11x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.17 sec: 1.10x faster                                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 572 ms: 1.09x faster                                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                                 |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 703 ms: 1.07x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 715 ms: 1.06x faster                                                   |
| Geometric mean             | (ref)                                                  | 1.11x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 86.2 ms: 1.11x faster                                                  |
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                                   |
| float          | 78.9 ms                                                | 80.3 ms: 1.02x slower                                                  |
| Geometric mean | (ref)                                                  | 1.04x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 129 ms: 1.09x faster                                                   |
| regex_effbot   | 3.51 ms                                                | 3.63 ms: 1.03x slower                                                  |
| regex_dna      | 205 ms                                                 | 219 ms: 1.07x slower                                                   |
| regex_v8       | 22.9 ms                                                | 25.1 ms: 1.10x slower                                                  |
| Geometric mean | (ref)                                                  | 1.03x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.3 ms: 1.29x faster                                                  |
| unpickle_pure_python | 242 us                                                 | 213 us: 1.13x faster                                                   |
| tomli_loads          | 2.30 sec                                               | 2.10 sec: 1.10x faster                                                 |
| pickle_pure_python   | 320 us                                                 | 296 us: 1.08x faster                                                   |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                                   |
| unpickle_list        | 5.21 us                                                | 5.04 us: 1.03x faster                                                  |
| xml_etree_iterparse  | 108 ms                                                 | 104 ms: 1.03x faster                                                   |
| json_loads           | 29.2 us                                                | 28.3 us: 1.03x faster                                                  |
| pickle_dict          | 34.6 us                                                | 34.8 us: 1.01x slower                                                  |
| xml_etree_process    | 56.9 ms                                                | 58.8 ms: 1.03x slower                                                  |
| xml_etree_generate   | 81.1 ms                                                | 85.6 ms: 1.06x slower                                                  |
| pickle               | 11.0 us                                                | 11.7 us: 1.06x slower                                                  |
| unpickle             | 13.8 us                                                | 15.0 us: 1.09x slower                                                  |
| pickle_list          | 4.59 us                                                | 5.17 us: 1.13x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                  |
| python_startup_no_site | 6.01 ms                                                | 8.73 ms: 1.45x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.31x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.1 ms: 1.04x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 109 us: 4.77x faster                                                   |
| generators                 | 74.9 ms                                                | 29.6 ms: 2.53x faster                                                  |
| asyncio_tcp                | 875 ms                                                 | 481 ms: 1.82x faster                                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.79 sec: 1.74x faster                                                 |
| comprehensions             | 23.6 us                                                | 16.1 us: 1.46x faster                                                  |
| json_dumps                 | 13.3 ms                                                | 10.3 ms: 1.29x faster                                                  |
| chaos                      | 71.9 ms                                                | 58.5 ms: 1.23x faster                                                  |
| async_tree_none            | 528 ms                                                 | 432 ms: 1.22x faster                                                   |
| deltablue                  | 3.92 ms                                                | 3.21 ms: 1.22x faster                                                  |
| coroutines                 | 27.0 ms                                                | 22.7 ms: 1.19x faster                                                  |
| raytrace                   | 309 ms                                                 | 260 ms: 1.18x faster                                                   |
| richards_super             | 61.9 ms                                                | 53.7 ms: 1.15x faster                                                  |
| sqlglot_parse              | 1.43 ms                                                | 1.25 ms: 1.14x faster                                                  |
| sympy_sum                  | 169 ms                                                 | 148 ms: 1.14x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 560 ms: 1.14x faster                                                   |
| unpickle_pure_python       | 242 us                                                 | 213 us: 1.13x faster                                                   |
| hexiom                     | 6.89 ms                                                | 6.09 ms: 1.13x faster                                                  |
| async_tree_none_tg         | 491 ms                                                 | 440 ms: 1.11x faster                                                   |
| sqlglot_transpile          | 1.75 ms                                                | 1.57 ms: 1.11x faster                                                  |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.51 ms: 1.11x faster                                                  |
| nbody                      | 96.0 ms                                                | 86.2 ms: 1.11x faster                                                  |
| logging_silent             | 111 ns                                                 | 100 ns: 1.11x faster                                                   |
| nqueens                    | 87.9 ms                                                | 79.6 ms: 1.10x faster                                                  |
| sympy_integrate            | 21.5 ms                                                | 19.5 ms: 1.10x faster                                                  |
| mdp                        | 2.77 sec                                               | 2.52 sec: 1.10x faster                                                 |
| sympy_str                  | 297 ms                                                 | 270 ms: 1.10x faster                                                   |
| tomli_loads                | 2.30 sec                                               | 2.10 sec: 1.10x faster                                                 |
| async_tree_io              | 1.29 sec                                               | 1.17 sec: 1.10x faster                                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 572 ms: 1.09x faster                                                   |
| regex_compile              | 141 ms                                                 | 129 ms: 1.09x faster                                                   |
| logging_simple             | 6.22 us                                                | 5.70 us: 1.09x faster                                                  |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                                 |
| logging_format             | 6.81 us                                                | 6.27 us: 1.09x faster                                                  |
| go                         | 149 ms                                                 | 138 ms: 1.08x faster                                                   |
| crypto_pyaes               | 76.7 ms                                                | 71.1 ms: 1.08x faster                                                  |
| pickle_pure_python         | 320 us                                                 | 296 us: 1.08x faster                                                   |
| deepcopy_memo              | 40.2 us                                                | 37.4 us: 1.07x faster                                                  |
| scimark_monte_carlo        | 70.7 ms                                                | 66.1 ms: 1.07x faster                                                  |
| deepcopy                   | 365 us                                                 | 342 us: 1.07x faster                                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 703 ms: 1.07x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 715 ms: 1.06x faster                                                   |
| sympy_expand               | 484 ms                                                 | 458 ms: 1.06x faster                                                   |
| deepcopy_reduce            | 3.22 us                                                | 3.04 us: 1.06x faster                                                  |
| scimark_lu                 | 116 ms                                                 | 110 ms: 1.05x faster                                                   |
| sqlglot_normalize          | 113 ms                                                 | 108 ms: 1.05x faster                                                   |
| richards                   | 49.8 ms                                                | 47.7 ms: 1.04x faster                                                  |
| pprint_pformat             | 1.55 sec                                               | 1.49 sec: 1.04x faster                                                 |
| xml_etree_parse            | 164 ms                                                 | 158 ms: 1.04x faster                                                   |
| gc_traversal               | 4.01 ms                                                | 3.86 ms: 1.04x faster                                                  |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                                   |
| tornado_http               | 98.1 ms                                                | 94.5 ms: 1.04x faster                                                  |
| unpickle_list              | 5.21 us                                                | 5.04 us: 1.03x faster                                                  |
| xml_etree_iterparse        | 108 ms                                                 | 104 ms: 1.03x faster                                                   |
| json_loads                 | 29.2 us                                                | 28.3 us: 1.03x faster                                                  |
| pprint_safe_repr           | 747 ms                                                 | 728 ms: 1.03x faster                                                   |
| docutils                   | 2.66 sec                                               | 2.60 sec: 1.02x faster                                                 |
| sqlglot_optimize           | 55.3 ms                                                | 54.1 ms: 1.02x faster                                                  |
| pathlib                    | 18.5 ms                                                | 18.2 ms: 1.02x faster                                                  |
| json                       | 5.24 ms                                                | 5.16 ms: 1.02x faster                                                  |
| dask                       | 365 ms                                                 | 360 ms: 1.01x faster                                                   |
| meteor_contest             | 109 ms                                                 | 107 ms: 1.01x faster                                                   |
| fannkuch                   | 405 ms                                                 | 400 ms: 1.01x faster                                                   |
| bench_thread_pool          | 834 us                                                 | 828 us: 1.01x faster                                                   |
| 2to3                       | 264 ms                                                 | 264 ms: 1.00x faster                                                   |
| pickle_dict                | 34.6 us                                                | 34.8 us: 1.01x slower                                                  |
| scimark_fft                | 345 ms                                                 | 350 ms: 1.01x slower                                                   |
| dulwich_log                | 64.6 ms                                                | 65.5 ms: 1.01x slower                                                  |
| pycparser                  | 1.19 sec                                               | 1.20 sec: 1.01x slower                                                 |
| float                      | 78.9 ms                                                | 80.3 ms: 1.02x slower                                                  |
| chameleon                  | 6.70 ms                                                | 6.86 ms: 1.02x slower                                                  |
| xml_etree_process          | 56.9 ms                                                | 58.8 ms: 1.03x slower                                                  |
| unpack_sequence            | 43.5 ns                                                | 44.9 ns: 1.03x slower                                                  |
| regex_effbot               | 3.51 ms                                                | 3.63 ms: 1.03x slower                                                  |
| mako                       | 10.7 ms                                                | 11.1 ms: 1.04x slower                                                  |
| create_gc_cycles           | 1.43 ms                                                | 1.49 ms: 1.04x slower                                                  |
| scimark_sor                | 121 ms                                                 | 127 ms: 1.05x slower                                                   |
| pyflate                    | 434 ms                                                 | 457 ms: 1.05x slower                                                   |
| xml_etree_generate         | 81.1 ms                                                | 85.6 ms: 1.06x slower                                                  |
| pickle                     | 11.0 us                                                | 11.7 us: 1.06x slower                                                  |
| regex_dna                  | 205 ms                                                 | 219 ms: 1.07x slower                                                   |
| unpickle                   | 13.8 us                                                | 15.0 us: 1.09x slower                                                  |
| regex_v8                   | 22.9 ms                                                | 25.1 ms: 1.10x slower                                                  |
| sqlite_synth               | 2.57 us                                                | 2.82 us: 1.10x slower                                                  |
| pickle_list                | 4.59 us                                                | 5.17 us: 1.13x slower                                                  |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                  |
| async_generators           | 374 ms                                                 | 446 ms: 1.19x slower                                                   |
| telco                      | 6.86 ms                                                | 8.24 ms: 1.20x slower                                                  |
| coverage                   | 78.8 ms                                                | 94.9 ms: 1.21x slower                                                  |
| mypy2                      | 686 ms                                                 | 841 ms: 1.23x slower                                                   |
| python_startup_no_site     | 6.01 ms                                                | 8.73 ms: 1.45x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.07x faster                                                           |

Benchmark hidden because not significant (3): spectral_norm, bench_mp_pool, asyncio_websockets
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 0.98x