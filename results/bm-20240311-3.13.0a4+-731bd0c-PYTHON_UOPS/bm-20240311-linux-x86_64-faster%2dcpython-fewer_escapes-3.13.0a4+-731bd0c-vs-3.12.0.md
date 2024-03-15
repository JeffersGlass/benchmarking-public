# Results vs. 3.12.0

- fork: faster-cpython
- ref: fewer_escapes
- machine: linux-x86_64
- commit hash: 731bd0c
- commit date: 2024-03-11
- overall geometric mean: 1.08x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x slower
- Memory change: 0.94x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240311-linux-x86_64-faster%2dcpython-fewer_escapes-3.13.0a4+-731bd0c |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 300 ms: 1.09x slower                                                      |
| chameleon      | 7.41 ms                                                | 7.20 ms: 1.03x faster                                                     |
| docutils       | 2.77 sec                                               | 2.90 sec: 1.05x slower                                                    |
| tornado_http   | 103 ms                                                 | 104 ms: 1.02x slower                                                      |
| Geometric mean | (ref)                                                  | 1.03x slower                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240311-linux-x86_64-faster%2dcpython-fewer_escapes-3.13.0a4+-731bd0c |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 460 ms: 1.03x faster                                                      |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 739 ms: 1.02x slower                                                      |
| async_tree_memoization     | 578 ms                                                 | 595 ms: 1.03x slower                                                      |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 752 ms: 1.04x slower                                                      |
| async_tree_none_tg         | 450 ms                                                 | 468 ms: 1.04x slower                                                      |
| async_tree_memoization_tg  | 575 ms                                                 | 600 ms: 1.04x slower                                                      |
| async_tree_io_tg           | 1.18 sec                                               | 1.25 sec: 1.06x slower                                                    |
| async_tree_io              | 1.16 sec                                               | 1.22 sec: 1.06x slower                                                    |
| Geometric mean             | (ref)                                                  | 1.03x slower                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240311-linux-x86_64-faster%2dcpython-fewer_escapes-3.13.0a4+-731bd0c |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 191 ms: 1.02x slower                                                      |
| float          | 84.7 ms                                                | 97.0 ms: 1.15x slower                                                     |
| nbody          | 97.0 ms                                                | 125 ms: 1.29x slower                                                      |
| Geometric mean | (ref)                                                  | 1.15x slower                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240311-linux-x86_64-faster%2dcpython-fewer_escapes-3.13.0a4+-731bd0c |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.52 ms: 1.03x faster                                                     |
| regex_dna      | 212 ms                                                 | 225 ms: 1.06x slower                                                      |
| regex_v8       | 23.1 ms                                                | 25.6 ms: 1.11x slower                                                     |
| regex_compile  | 148 ms                                                 | 178 ms: 1.20x slower                                                      |
| Geometric mean | (ref)                                                  | 1.08x slower                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240311-linux-x86_64-faster%2dcpython-fewer_escapes-3.13.0a4+-731bd0c |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| unpickle_list        | 5.29 us                                                | 5.02 us: 1.05x faster                                                     |
| pickle_pure_python   | 324 us                                                 | 310 us: 1.05x faster                                                      |
| pickle_dict          | 35.5 us                                                | 34.4 us: 1.03x faster                                                     |
| pickle_list          | 5.08 us                                                | 4.97 us: 1.02x faster                                                     |
| json_loads           | 28.5 us                                                | 28.2 us: 1.01x faster                                                     |
| pickle               | 11.6 us                                                | 11.7 us: 1.01x slower                                                     |
| xml_etree_parse      | 159 ms                                                 | 162 ms: 1.02x slower                                                      |
| json_dumps           | 10.4 ms                                                | 10.7 ms: 1.03x slower                                                     |
| xml_etree_process    | 61.7 ms                                                | 63.6 ms: 1.03x slower                                                     |
| xml_etree_generate   | 89.2 ms                                                | 92.7 ms: 1.04x slower                                                     |
| xml_etree_iterparse  | 107 ms                                                 | 113 ms: 1.06x slower                                                      |
| tomli_loads          | 2.33 sec                                               | 2.53 sec: 1.08x slower                                                    |
| unpickle_pure_python | 230 us                                                 | 285 us: 1.24x slower                                                      |
| Geometric mean       | (ref)                                                  | 1.02x slower                                                              |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240311-linux-x86_64-faster%2dcpython-fewer_escapes-3.13.0a4+-731bd0c |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.4 ms: 1.09x slower                                                     |
| python_startup_no_site | 6.94 ms                                                | 8.98 ms: 1.30x slower                                                     |
| Geometric mean         | (ref)                                                  | 1.19x slower                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240311-linux-x86_64-faster%2dcpython-fewer_escapes-3.13.0a4+-731bd0c |
|-----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| django_template | 34.6 ms                                                | 35.3 ms: 1.02x slower                                                     |
| mako            | 11.9 ms                                                | 13.3 ms: 1.12x slower                                                     |
| Geometric mean  | (ref)                                                  | 1.07x slower                                                              |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240311-linux-x86_64-faster%2dcpython-fewer_escapes-3.13.0a4+-731bd0c |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 117 us: 1.35x faster                                                      |
| deepcopy_reduce            | 3.35 us                                                | 3.16 us: 1.06x faster                                                     |
| unpickle_list              | 5.29 us                                                | 5.02 us: 1.05x faster                                                     |
| pickle_pure_python         | 324 us                                                 | 310 us: 1.05x faster                                                      |
| logging_format             | 7.23 us                                                | 7.00 us: 1.03x faster                                                     |
| pickle_dict                | 35.5 us                                                | 34.4 us: 1.03x faster                                                     |
| chameleon                  | 7.41 ms                                                | 7.20 ms: 1.03x faster                                                     |
| logging_simple             | 6.46 us                                                | 6.29 us: 1.03x faster                                                     |
| generators                 | 31.2 ms                                                | 30.4 ms: 1.03x faster                                                     |
| async_tree_none            | 472 ms                                                 | 460 ms: 1.03x faster                                                      |
| regex_effbot               | 3.61 ms                                                | 3.52 ms: 1.03x faster                                                     |
| pickle_list                | 5.08 us                                                | 4.97 us: 1.02x faster                                                     |
| json_loads                 | 28.5 us                                                | 28.2 us: 1.01x faster                                                     |
| gc_traversal               | 3.79 ms                                                | 3.81 ms: 1.01x slower                                                     |
| pickle                     | 11.6 us                                                | 11.7 us: 1.01x slower                                                     |
| logging_silent             | 104 ns                                                 | 105 ns: 1.01x slower                                                      |
| comprehensions             | 21.8 us                                                | 22.1 us: 1.01x slower                                                     |
| sympy_integrate            | 21.4 ms                                                | 21.8 ms: 1.02x slower                                                     |
| tornado_http               | 103 ms                                                 | 104 ms: 1.02x slower                                                      |
| xml_etree_parse            | 159 ms                                                 | 162 ms: 1.02x slower                                                      |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 739 ms: 1.02x slower                                                      |
| dask                       | 372 ms                                                 | 379 ms: 1.02x slower                                                      |
| pidigits                   | 187 ms                                                 | 191 ms: 1.02x slower                                                      |
| async_generators           | 463 ms                                                 | 473 ms: 1.02x slower                                                      |
| asyncio_websockets         | 551 ms                                                 | 563 ms: 1.02x slower                                                      |
| django_template            | 34.6 ms                                                | 35.3 ms: 1.02x slower                                                     |
| sympy_str                  | 300 ms                                                 | 306 ms: 1.02x slower                                                      |
| json_dumps                 | 10.4 ms                                                | 10.7 ms: 1.03x slower                                                     |
| async_tree_memoization     | 578 ms                                                 | 595 ms: 1.03x slower                                                      |
| xml_etree_process          | 61.7 ms                                                | 63.6 ms: 1.03x slower                                                     |
| asyncio_tcp                | 491 ms                                                 | 506 ms: 1.03x slower                                                      |
| sqlglot_normalize          | 110 ms                                                 | 114 ms: 1.03x slower                                                      |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 752 ms: 1.04x slower                                                      |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.85 sec: 1.04x slower                                                    |
| create_gc_cycles           | 1.48 ms                                                | 1.53 ms: 1.04x slower                                                     |
| xml_etree_generate         | 89.2 ms                                                | 92.7 ms: 1.04x slower                                                     |
| bench_thread_pool          | 842 us                                                 | 875 us: 1.04x slower                                                      |
| async_tree_none_tg         | 450 ms                                                 | 468 ms: 1.04x slower                                                      |
| async_tree_memoization_tg  | 575 ms                                                 | 600 ms: 1.04x slower                                                      |
| docutils                   | 2.77 sec                                               | 2.90 sec: 1.05x slower                                                    |
| mdp                        | 2.63 sec                                               | 2.76 sec: 1.05x slower                                                    |
| sqlite_synth               | 2.83 us                                                | 2.98 us: 1.05x slower                                                     |
| deltablue                  | 3.72 ms                                                | 3.91 ms: 1.05x slower                                                     |
| async_tree_io_tg           | 1.18 sec                                               | 1.25 sec: 1.06x slower                                                    |
| async_tree_io              | 1.16 sec                                               | 1.22 sec: 1.06x slower                                                    |
| xml_etree_iterparse        | 107 ms                                                 | 113 ms: 1.06x slower                                                      |
| regex_dna                  | 212 ms                                                 | 225 ms: 1.06x slower                                                      |
| gunicorn                   | 1.24 ms                                                | 1.32 ms: 1.06x slower                                                     |
| aiohttp                    | 1.15 ms                                                | 1.22 ms: 1.06x slower                                                     |
| dulwich_log                | 68.5 ms                                                | 72.9 ms: 1.06x slower                                                     |
| deepcopy_memo              | 40.7 us                                                | 43.3 us: 1.06x slower                                                     |
| sqlglot_transpile          | 1.68 ms                                                | 1.80 ms: 1.07x slower                                                     |
| sqlglot_parse              | 1.36 ms                                                | 1.45 ms: 1.07x slower                                                     |
| meteor_contest             | 112 ms                                                 | 121 ms: 1.08x slower                                                      |
| sympy_expand               | 478 ms                                                 | 516 ms: 1.08x slower                                                      |
| tomli_loads                | 2.33 sec                                               | 2.53 sec: 1.08x slower                                                    |
| python_startup             | 9.55 ms                                                | 10.4 ms: 1.09x slower                                                     |
| 2to3                       | 274 ms                                                 | 300 ms: 1.09x slower                                                      |
| crypto_pyaes               | 81.9 ms                                                | 89.6 ms: 1.10x slower                                                     |
| regex_v8                   | 23.1 ms                                                | 25.6 ms: 1.11x slower                                                     |
| mypy2                      | 830 ms                                                 | 920 ms: 1.11x slower                                                      |
| unpack_sequence            | 54.0 ns                                                | 60.0 ns: 1.11x slower                                                     |
| mako                       | 11.9 ms                                                | 13.3 ms: 1.12x slower                                                     |
| sqlglot_optimize           | 54.8 ms                                                | 61.6 ms: 1.12x slower                                                     |
| raytrace                   | 312 ms                                                 | 356 ms: 1.14x slower                                                      |
| scimark_fft                | 382 ms                                                 | 436 ms: 1.14x slower                                                      |
| float                      | 84.7 ms                                                | 97.0 ms: 1.15x slower                                                     |
| pycparser                  | 1.18 sec                                               | 1.37 sec: 1.16x slower                                                    |
| chaos                      | 67.0 ms                                                | 77.7 ms: 1.16x slower                                                     |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 5.92 ms: 1.17x slower                                                     |
| pprint_safe_repr           | 776 ms                                                 | 913 ms: 1.18x slower                                                      |
| scimark_sor                | 129 ms                                                 | 152 ms: 1.18x slower                                                      |
| scimark_monte_carlo        | 75.1 ms                                                | 89.4 ms: 1.19x slower                                                     |
| fannkuch                   | 417 ms                                                 | 497 ms: 1.19x slower                                                      |
| regex_compile              | 148 ms                                                 | 178 ms: 1.20x slower                                                      |
| pprint_pformat             | 1.57 sec                                               | 1.91 sec: 1.22x slower                                                    |
| pyflate                    | 482 ms                                                 | 597 ms: 1.24x slower                                                      |
| unpickle_pure_python       | 230 us                                                 | 285 us: 1.24x slower                                                      |
| telco                      | 7.10 ms                                                | 8.84 ms: 1.24x slower                                                     |
| richards_super             | 51.5 ms                                                | 64.4 ms: 1.25x slower                                                     |
| nqueens                    | 83.3 ms                                                | 105 ms: 1.26x slower                                                      |
| richards                   | 45.8 ms                                                | 58.2 ms: 1.27x slower                                                     |
| nbody                      | 97.0 ms                                                | 125 ms: 1.29x slower                                                      |
| python_startup_no_site     | 6.94 ms                                                | 8.98 ms: 1.30x slower                                                     |
| spectral_norm              | 115 ms                                                 | 150 ms: 1.30x slower                                                      |
| go                         | 139 ms                                                 | 182 ms: 1.31x slower                                                      |
| coverage                   | 72.7 ms                                                | 98.0 ms: 1.35x slower                                                     |
| scimark_lu                 | 118 ms                                                 | 163 ms: 1.38x slower                                                      |
| hexiom                     | 6.41 ms                                                | 9.40 ms: 1.47x slower                                                     |
| Geometric mean             | (ref)                                                  | 1.08x slower                                                              |

Benchmark hidden because not significant (7): sympy_sum, pathlib, bench_mp_pool, deepcopy, coroutines, json, unpickle
Ignored benchmarks (2) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (6) of results/bm-20240311-3.13.0a4+-731bd0c-PYTHON_UOPS/bm-20240311-linux-x86_64-faster%2dcpython-fewer_escapes-3.13.0a4+-731bd0c.json: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.05x
- 95% likely to have a slowdown of 1.05x
- 99% likely to have a slowdown of 1.04x


# Memory

- memory change: 0.94x