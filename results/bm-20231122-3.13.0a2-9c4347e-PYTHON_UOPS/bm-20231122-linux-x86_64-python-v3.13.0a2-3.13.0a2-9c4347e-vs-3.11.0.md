
# Results vs. 3.11.0

- fork: python
- ref: v3.13.0a2
- machine: linux-x86_64
- commit hash: 9c4347e
- commit date: 2023-11-22
- overall geometric mean: 1.01x slower
- HPT reliability: 99.88%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.97x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-linux-x86_64-python-v3.13.0a2-3.13.0a2-9c4347e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 288 ms: 1.09x slower                                       |
| chameleon      | 6.70 ms                                                | 7.54 ms: 1.12x slower                                      |
| docutils       | 2.66 sec                                               | 2.73 sec: 1.02x slower                                     |
| tornado_http   | 98.1 ms                                                | 99.5 ms: 1.01x slower                                      |
| Geometric mean | (ref)                                                  | 1.06x slower                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-linux-x86_64-python-v3.13.0a2-3.13.0a2-9c4347e |
|---------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| async_tree_none           | 528 ms                                                 | 456 ms: 1.16x faster                                       |
| async_tree_memoization    | 639 ms                                                 | 583 ms: 1.10x faster                                       |
| async_tree_io             | 1.29 sec                                               | 1.22 sec: 1.06x faster                                     |
| async_tree_none_tg        | 491 ms                                                 | 471 ms: 1.04x faster                                       |
| async_tree_io_tg          | 1.29 sec                                               | 1.25 sec: 1.03x faster                                     |
| async_tree_cpu_io_mixed   | 749 ms                                                 | 731 ms: 1.03x faster                                       |
| async_tree_memoization_tg | 626 ms                                                 | 611 ms: 1.03x faster                                       |
| Geometric mean            | (ref)                                                  | 1.05x faster                                               |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-linux-x86_64-python-v3.13.0a2-3.13.0a2-9c4347e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 196 ms: 1.01x slower                                       |
| float          | 78.9 ms                                                | 92.4 ms: 1.17x slower                                      |
| nbody          | 96.0 ms                                                | 119 ms: 1.23x slower                                       |
| Geometric mean | (ref)                                                  | 1.13x slower                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-linux-x86_64-python-v3.13.0a2-3.13.0a2-9c4347e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.73 ms: 1.06x slower                                      |
| regex_dna      | 205 ms                                                 | 224 ms: 1.09x slower                                       |
| regex_compile  | 141 ms                                                 | 157 ms: 1.11x slower                                       |
| regex_v8       | 22.9 ms                                                | 25.9 ms: 1.13x slower                                      |
| Geometric mean | (ref)                                                  | 1.10x slower                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-linux-x86_64-python-v3.13.0a2-3.13.0a2-9c4347e |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.6 ms: 1.26x faster                                      |
| pickle_pure_python   | 320 us                                                 | 308 us: 1.04x faster                                       |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                       |
| json_loads           | 29.2 us                                                | 28.2 us: 1.03x faster                                      |
| pickle_dict          | 34.6 us                                                | 34.0 us: 1.02x faster                                      |
| unpickle_pure_python | 242 us                                                 | 240 us: 1.01x faster                                       |
| pickle               | 11.0 us                                                | 11.1 us: 1.01x slower                                      |
| xml_etree_iterparse  | 108 ms                                                 | 112 ms: 1.03x slower                                       |
| tomli_loads          | 2.30 sec                                               | 2.39 sec: 1.04x slower                                     |
| pickle_list          | 4.59 us                                                | 4.94 us: 1.08x slower                                      |
| xml_etree_process    | 56.9 ms                                                | 61.8 ms: 1.09x slower                                      |
| xml_etree_generate   | 81.1 ms                                                | 90.2 ms: 1.11x slower                                      |
| unpickle             | 13.8 us                                                | 15.6 us: 1.12x slower                                      |
| Geometric mean       | (ref)                                                  | 1.01x slower                                               |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-linux-x86_64-python-v3.13.0a2-3.13.0a2-9c4347e |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.3 ms: 1.21x slower                                      |
| python_startup_no_site | 6.01 ms                                                | 9.00 ms: 1.50x slower                                      |
| Geometric mean         | (ref)                                                  | 1.34x slower                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-linux-x86_64-python-v3.13.0a2-3.13.0a2-9c4347e |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------:|
| mako      | 10.7 ms                                                | 13.7 ms: 1.29x slower                                      |

All benchmarks:
===============

| Benchmark                 | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-linux-x86_64-python-v3.13.0a2-3.13.0a2-9c4347e |
|---------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| typing_runtime_protocols  | 520 us                                                 | 122 us: 4.25x faster                                       |
| generators                | 74.9 ms                                                | 29.6 ms: 2.53x faster                                      |
| asyncio_tcp               | 875 ms                                                 | 487 ms: 1.80x faster                                       |
| asyncio_tcp_ssl           | 3.11 sec                                               | 1.80 sec: 1.72x faster                                     |
| json_dumps                | 13.3 ms                                                | 10.6 ms: 1.26x faster                                      |
| coroutines                | 27.0 ms                                                | 22.4 ms: 1.20x faster                                      |
| async_tree_none           | 528 ms                                                 | 456 ms: 1.16x faster                                       |
| comprehensions            | 23.6 us                                                | 20.9 us: 1.13x faster                                      |
| async_tree_memoization    | 639 ms                                                 | 583 ms: 1.10x faster                                       |
| richards_super            | 61.9 ms                                                | 57.2 ms: 1.08x faster                                      |
| sympy_sum                 | 169 ms                                                 | 160 ms: 1.06x faster                                       |
| async_tree_io             | 1.29 sec                                               | 1.22 sec: 1.06x faster                                     |
| sqlglot_parse             | 1.43 ms                                                | 1.36 ms: 1.05x faster                                      |
| async_tree_none_tg        | 491 ms                                                 | 471 ms: 1.04x faster                                       |
| pickle_pure_python        | 320 us                                                 | 308 us: 1.04x faster                                       |
| xml_etree_parse           | 164 ms                                                 | 158 ms: 1.04x faster                                       |
| async_tree_io_tg          | 1.29 sec                                               | 1.25 sec: 1.03x faster                                     |
| json_loads                | 29.2 us                                                | 28.2 us: 1.03x faster                                      |
| logging_silent            | 111 ns                                                 | 108 ns: 1.03x faster                                       |
| sqlglot_transpile         | 1.75 ms                                                | 1.70 ms: 1.03x faster                                      |
| logging_simple            | 6.22 us                                                | 6.03 us: 1.03x faster                                      |
| async_tree_cpu_io_mixed   | 749 ms                                                 | 731 ms: 1.03x faster                                       |
| async_tree_memoization_tg | 626 ms                                                 | 611 ms: 1.03x faster                                       |
| pickle_dict               | 34.6 us                                                | 34.0 us: 1.02x faster                                      |
| deepcopy_reduce           | 3.22 us                                                | 3.18 us: 1.01x faster                                      |
| deepcopy                  | 365 us                                                 | 362 us: 1.01x faster                                       |
| sympy_str                 | 297 ms                                                 | 294 ms: 1.01x faster                                       |
| sympy_integrate           | 21.5 ms                                                | 21.3 ms: 1.01x faster                                      |
| unpickle_pure_python      | 242 us                                                 | 240 us: 1.01x faster                                       |
| asyncio_websockets        | 550 ms                                                 | 552 ms: 1.00x slower                                       |
| mdp                       | 2.77 sec                                               | 2.79 sec: 1.00x slower                                     |
| raytrace                  | 309 ms                                                 | 310 ms: 1.01x slower                                       |
| logging_format            | 6.81 us                                                | 6.86 us: 1.01x slower                                      |
| pidigits                  | 194 ms                                                 | 196 ms: 1.01x slower                                       |
| pickle                    | 11.0 us                                                | 11.1 us: 1.01x slower                                      |
| tornado_http              | 98.1 ms                                                | 99.5 ms: 1.01x slower                                      |
| sympy_expand              | 484 ms                                                 | 493 ms: 1.02x slower                                       |
| create_gc_cycles          | 1.43 ms                                                | 1.46 ms: 1.02x slower                                      |
| dask                      | 365 ms                                                 | 372 ms: 1.02x slower                                       |
| deepcopy_memo             | 40.2 us                                                | 41.0 us: 1.02x slower                                      |
| bench_thread_pool         | 834 us                                                 | 854 us: 1.02x slower                                       |
| docutils                  | 2.66 sec                                               | 2.73 sec: 1.02x slower                                     |
| sqlglot_normalize         | 113 ms                                                 | 115 ms: 1.02x slower                                       |
| pathlib                   | 18.5 ms                                                | 19.0 ms: 1.03x slower                                      |
| scimark_lu                | 116 ms                                                 | 120 ms: 1.03x slower                                       |
| unpack_sequence           | 43.5 ns                                                | 44.8 ns: 1.03x slower                                      |
| xml_etree_iterparse       | 108 ms                                                 | 112 ms: 1.03x slower                                       |
| chaos                     | 71.9 ms                                                | 74.2 ms: 1.03x slower                                      |
| tomli_loads               | 2.30 sec                                               | 2.39 sec: 1.04x slower                                     |
| sqlglot_optimize          | 55.3 ms                                                | 58.5 ms: 1.06x slower                                      |
| pycparser                 | 1.19 sec                                               | 1.26 sec: 1.06x slower                                     |
| meteor_contest            | 109 ms                                                 | 116 ms: 1.06x slower                                       |
| regex_effbot              | 3.51 ms                                                | 3.73 ms: 1.06x slower                                      |
| dulwich_log               | 64.6 ms                                                | 69.0 ms: 1.07x slower                                      |
| gc_traversal              | 4.01 ms                                                | 4.29 ms: 1.07x slower                                      |
| nqueens                   | 87.9 ms                                                | 94.1 ms: 1.07x slower                                      |
| pprint_pformat            | 1.55 sec                                               | 1.68 sec: 1.08x slower                                     |
| pickle_list               | 4.59 us                                                | 4.94 us: 1.08x slower                                      |
| pprint_safe_repr          | 747 ms                                                 | 809 ms: 1.08x slower                                       |
| xml_etree_process         | 56.9 ms                                                | 61.8 ms: 1.09x slower                                      |
| crypto_pyaes              | 76.7 ms                                                | 83.3 ms: 1.09x slower                                      |
| 2to3                      | 264 ms                                                 | 288 ms: 1.09x slower                                       |
| regex_dna                 | 205 ms                                                 | 224 ms: 1.09x slower                                       |
| go                        | 149 ms                                                 | 163 ms: 1.10x slower                                       |
| scimark_sor               | 121 ms                                                 | 134 ms: 1.10x slower                                       |
| fannkuch                  | 405 ms                                                 | 450 ms: 1.11x slower                                       |
| regex_compile             | 141 ms                                                 | 157 ms: 1.11x slower                                       |
| xml_etree_generate        | 81.1 ms                                                | 90.2 ms: 1.11x slower                                      |
| unpickle                  | 13.8 us                                                | 15.6 us: 1.12x slower                                      |
| chameleon                 | 6.70 ms                                                | 7.54 ms: 1.12x slower                                      |
| sqlite_synth              | 2.57 us                                                | 2.91 us: 1.13x slower                                      |
| regex_v8                  | 22.9 ms                                                | 25.9 ms: 1.13x slower                                      |
| scimark_sparse_mat_mult   | 5.03 ms                                                | 5.74 ms: 1.14x slower                                      |
| scimark_monte_carlo       | 70.7 ms                                                | 81.4 ms: 1.15x slower                                      |
| float                     | 78.9 ms                                                | 92.4 ms: 1.17x slower                                      |
| deltablue                 | 3.92 ms                                                | 4.67 ms: 1.19x slower                                      |
| pyflate                   | 434 ms                                                 | 521 ms: 1.20x slower                                       |
| python_startup            | 8.56 ms                                                | 10.3 ms: 1.21x slower                                      |
| coverage                  | 78.8 ms                                                | 95.6 ms: 1.21x slower                                      |
| async_generators          | 374 ms                                                 | 457 ms: 1.22x slower                                       |
| telco                     | 6.86 ms                                                | 8.46 ms: 1.23x slower                                      |
| hexiom                    | 6.89 ms                                                | 8.49 ms: 1.23x slower                                      |
| nbody                     | 96.0 ms                                                | 119 ms: 1.23x slower                                       |
| scimark_fft               | 345 ms                                                 | 436 ms: 1.26x slower                                       |
| mypy2                     | 686 ms                                                 | 869 ms: 1.27x slower                                       |
| mako                      | 10.7 ms                                                | 13.7 ms: 1.29x slower                                      |
| spectral_norm             | 108 ms                                                 | 140 ms: 1.30x slower                                       |
| python_startup_no_site    | 6.01 ms                                                | 9.00 ms: 1.50x slower                                      |
| Geometric mean            | (ref)                                                  | 1.01x slower                                               |

Benchmark hidden because not significant (5): json, unpickle_list, async_tree_cpu_io_mixed_tg, bench_mp_pool, richards
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.88% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.97x