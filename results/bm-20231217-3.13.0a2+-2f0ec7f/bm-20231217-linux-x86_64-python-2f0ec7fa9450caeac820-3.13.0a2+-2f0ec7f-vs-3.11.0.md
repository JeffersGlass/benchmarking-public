
# Results vs. 3.11.0

- fork: python
- ref: 2f0ec7fa9450caeac820
- machine: linux-x86_64
- commit hash: 2f0ec7f
- commit date: 2023-12-17
- overall geometric mean: 1.07x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 262 ms: 1.01x faster                                                   |
| chameleon      | 6.70 ms                                                | 6.96 ms: 1.04x slower                                                  |
| docutils       | 2.66 sec                                               | 2.61 sec: 1.02x faster                                                 |
| tornado_http   | 98.1 ms                                                | 93.8 ms: 1.05x faster                                                  |
| Geometric mean | (ref)                                                  | 1.01x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 438 ms: 1.21x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 564 ms: 1.13x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 444 ms: 1.10x faster                                                   |
| async_tree_memoization_tg  | 626 ms                                                 | 578 ms: 1.08x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                 |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.07x faster                                                 |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 710 ms: 1.06x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 722 ms: 1.05x faster                                                   |
| Geometric mean             | (ref)                                                  | 1.10x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 88.8 ms: 1.08x faster                                                  |
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                                   |
| float          | 78.9 ms                                                | 80.8 ms: 1.02x slower                                                  |
| Geometric mean | (ref)                                                  | 1.03x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 129 ms: 1.09x faster                                                   |
| regex_v8       | 22.9 ms                                                | 23.8 ms: 1.04x slower                                                  |
| regex_effbot   | 3.51 ms                                                | 3.72 ms: 1.06x slower                                                  |
| regex_dna      | 205 ms                                                 | 229 ms: 1.12x slower                                                   |
| Geometric mean | (ref)                                                  | 1.03x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.3 ms: 1.29x faster                                                  |
| unpickle_pure_python | 242 us                                                 | 215 us: 1.12x faster                                                   |
| pickle_pure_python   | 320 us                                                 | 295 us: 1.09x faster                                                   |
| tomli_loads          | 2.30 sec                                               | 2.13 sec: 1.08x faster                                                 |
| xml_etree_parse      | 164 ms                                                 | 157 ms: 1.04x faster                                                   |
| xml_etree_iterparse  | 108 ms                                                 | 104 ms: 1.04x faster                                                   |
| json_loads           | 29.2 us                                                | 28.1 us: 1.04x faster                                                  |
| unpickle_list        | 5.21 us                                                | 5.06 us: 1.03x faster                                                  |
| pickle_dict          | 34.6 us                                                | 33.7 us: 1.03x faster                                                  |
| pickle               | 11.0 us                                                | 11.2 us: 1.02x slower                                                  |
| xml_etree_process    | 56.9 ms                                                | 58.3 ms: 1.02x slower                                                  |
| xml_etree_generate   | 81.1 ms                                                | 85.2 ms: 1.05x slower                                                  |
| unpickle             | 13.8 us                                                | 14.6 us: 1.05x slower                                                  |
| pickle_list          | 4.59 us                                                | 4.96 us: 1.08x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.17x slower                                                  |
| python_startup_no_site | 6.01 ms                                                | 8.70 ms: 1.45x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.30x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.4 ms: 1.07x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 111 us: 4.67x faster                                                   |
| generators                 | 74.9 ms                                                | 28.3 ms: 2.64x faster                                                  |
| asyncio_tcp                | 875 ms                                                 | 478 ms: 1.83x faster                                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.78 sec: 1.75x faster                                                 |
| comprehensions             | 23.6 us                                                | 16.0 us: 1.47x faster                                                  |
| json_dumps                 | 13.3 ms                                                | 10.3 ms: 1.29x faster                                                  |
| coroutines                 | 27.0 ms                                                | 21.8 ms: 1.24x faster                                                  |
| deltablue                  | 3.92 ms                                                | 3.19 ms: 1.23x faster                                                  |
| async_tree_none            | 528 ms                                                 | 438 ms: 1.21x faster                                                   |
| chaos                      | 71.9 ms                                                | 59.7 ms: 1.20x faster                                                  |
| raytrace                   | 309 ms                                                 | 260 ms: 1.19x faster                                                   |
| richards_super             | 61.9 ms                                                | 53.2 ms: 1.16x faster                                                  |
| sqlglot_parse              | 1.43 ms                                                | 1.24 ms: 1.15x faster                                                  |
| hexiom                     | 6.89 ms                                                | 6.00 ms: 1.15x faster                                                  |
| sympy_sum                  | 169 ms                                                 | 149 ms: 1.14x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 564 ms: 1.13x faster                                                   |
| gc_traversal               | 4.01 ms                                                | 3.54 ms: 1.13x faster                                                  |
| unpickle_pure_python       | 242 us                                                 | 215 us: 1.12x faster                                                   |
| sqlglot_transpile          | 1.75 ms                                                | 1.57 ms: 1.12x faster                                                  |
| async_tree_none_tg         | 491 ms                                                 | 444 ms: 1.10x faster                                                   |
| logging_simple             | 6.22 us                                                | 5.63 us: 1.10x faster                                                  |
| sympy_str                  | 297 ms                                                 | 269 ms: 1.10x faster                                                   |
| sympy_integrate            | 21.5 ms                                                | 19.5 ms: 1.10x faster                                                  |
| nqueens                    | 87.9 ms                                                | 79.8 ms: 1.10x faster                                                  |
| logging_format             | 6.81 us                                                | 6.20 us: 1.10x faster                                                  |
| mdp                        | 2.77 sec                                               | 2.53 sec: 1.10x faster                                                 |
| regex_compile              | 141 ms                                                 | 129 ms: 1.09x faster                                                   |
| pickle_pure_python         | 320 us                                                 | 295 us: 1.09x faster                                                   |
| async_tree_memoization_tg  | 626 ms                                                 | 578 ms: 1.08x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                 |
| logging_silent             | 111 ns                                                 | 103 ns: 1.08x faster                                                   |
| nbody                      | 96.0 ms                                                | 88.8 ms: 1.08x faster                                                  |
| tomli_loads                | 2.30 sec                                               | 2.13 sec: 1.08x faster                                                 |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.07x faster                                                 |
| go                         | 149 ms                                                 | 139 ms: 1.07x faster                                                   |
| sqlglot_normalize          | 113 ms                                                 | 106 ms: 1.07x faster                                                   |
| crypto_pyaes               | 76.7 ms                                                | 71.9 ms: 1.07x faster                                                  |
| sympy_expand               | 484 ms                                                 | 455 ms: 1.06x faster                                                   |
| scimark_monte_carlo        | 70.7 ms                                                | 66.5 ms: 1.06x faster                                                  |
| richards                   | 49.8 ms                                                | 47.0 ms: 1.06x faster                                                  |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 710 ms: 1.06x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 722 ms: 1.05x faster                                                   |
| deepcopy_memo              | 40.2 us                                                | 38.4 us: 1.05x faster                                                  |
| tornado_http               | 98.1 ms                                                | 93.8 ms: 1.05x faster                                                  |
| xml_etree_parse            | 164 ms                                                 | 157 ms: 1.04x faster                                                   |
| deepcopy                   | 365 us                                                 | 351 us: 1.04x faster                                                   |
| scimark_lu                 | 116 ms                                                 | 112 ms: 1.04x faster                                                   |
| xml_etree_iterparse        | 108 ms                                                 | 104 ms: 1.04x faster                                                   |
| json_loads                 | 29.2 us                                                | 28.1 us: 1.04x faster                                                  |
| sqlglot_optimize           | 55.3 ms                                                | 53.2 ms: 1.04x faster                                                  |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                                   |
| unpickle_list              | 5.21 us                                                | 5.06 us: 1.03x faster                                                  |
| pprint_pformat             | 1.55 sec                                               | 1.51 sec: 1.03x faster                                                 |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.89 ms: 1.03x faster                                                  |
| pickle_dict                | 34.6 us                                                | 33.7 us: 1.03x faster                                                  |
| fannkuch                   | 405 ms                                                 | 397 ms: 1.02x faster                                                   |
| deepcopy_reduce            | 3.22 us                                                | 3.15 us: 1.02x faster                                                  |
| docutils                   | 2.66 sec                                               | 2.61 sec: 1.02x faster                                                 |
| meteor_contest             | 109 ms                                                 | 107 ms: 1.01x faster                                                   |
| dask                       | 365 ms                                                 | 361 ms: 1.01x faster                                                   |
| bench_thread_pool          | 834 us                                                 | 824 us: 1.01x faster                                                   |
| json                       | 5.24 ms                                                | 5.18 ms: 1.01x faster                                                  |
| 2to3                       | 264 ms                                                 | 262 ms: 1.01x faster                                                   |
| pprint_safe_repr           | 747 ms                                                 | 744 ms: 1.00x faster                                                   |
| dulwich_log                | 64.6 ms                                                | 65.5 ms: 1.01x slower                                                  |
| pickle                     | 11.0 us                                                | 11.2 us: 1.02x slower                                                  |
| float                      | 78.9 ms                                                | 80.8 ms: 1.02x slower                                                  |
| xml_etree_process          | 56.9 ms                                                | 58.3 ms: 1.02x slower                                                  |
| spectral_norm              | 108 ms                                                 | 111 ms: 1.03x slower                                                   |
| create_gc_cycles           | 1.43 ms                                                | 1.48 ms: 1.03x slower                                                  |
| regex_v8                   | 22.9 ms                                                | 23.8 ms: 1.04x slower                                                  |
| chameleon                  | 6.70 ms                                                | 6.96 ms: 1.04x slower                                                  |
| xml_etree_generate         | 81.1 ms                                                | 85.2 ms: 1.05x slower                                                  |
| unpickle                   | 13.8 us                                                | 14.6 us: 1.05x slower                                                  |
| pyflate                    | 434 ms                                                 | 458 ms: 1.06x slower                                                   |
| regex_effbot               | 3.51 ms                                                | 3.72 ms: 1.06x slower                                                  |
| mako                       | 10.7 ms                                                | 11.4 ms: 1.07x slower                                                  |
| scimark_fft                | 345 ms                                                 | 371 ms: 1.07x slower                                                   |
| pickle_list                | 4.59 us                                                | 4.96 us: 1.08x slower                                                  |
| sqlite_synth               | 2.57 us                                                | 2.80 us: 1.09x slower                                                  |
| regex_dna                  | 205 ms                                                 | 229 ms: 1.12x slower                                                   |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.17x slower                                                  |
| async_generators           | 374 ms                                                 | 440 ms: 1.18x slower                                                   |
| telco                      | 6.86 ms                                                | 8.20 ms: 1.20x slower                                                  |
| coverage                   | 78.8 ms                                                | 95.2 ms: 1.21x slower                                                  |
| mypy2                      | 686 ms                                                 | 836 ms: 1.22x slower                                                   |
| unpack_sequence            | 43.5 ns                                                | 53.1 ns: 1.22x slower                                                  |
| python_startup_no_site     | 6.01 ms                                                | 8.70 ms: 1.45x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.07x faster                                                           |

Benchmark hidden because not significant (5): pycparser, scimark_sor, bench_mp_pool, pathlib, asyncio_websockets
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 0.98x