# Results vs. 3.11.0

- fork: faster-cpython
- ref: fewer_escapes
- machine: linux-x86_64
- commit hash: 731bd0c
- commit date: 2024-03-11
- overall geometric mean: 1.05x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x slower
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240311-linux-x86_64-faster%2dcpython-fewer_escapes-3.13.0a4+-731bd0c |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 300 ms: 1.14x slower                                                      |
| chameleon      | 6.70 ms                                                | 7.20 ms: 1.07x slower                                                     |
| docutils       | 2.66 sec                                               | 2.90 sec: 1.09x slower                                                    |
| html5lib       | 64.8 ms                                                | 70.6 ms: 1.09x slower                                                     |
| tornado_http   | 98.1 ms                                                | 104 ms: 1.06x slower                                                      |
| Geometric mean | (ref)                                                  | 1.09x slower                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240311-linux-x86_64-faster%2dcpython-fewer_escapes-3.13.0a4+-731bd0c |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 460 ms: 1.15x faster                                                      |
| async_tree_memoization     | 639 ms                                                 | 595 ms: 1.07x faster                                                      |
| async_tree_io              | 1.29 sec                                               | 1.22 sec: 1.05x faster                                                    |
| async_tree_none_tg         | 491 ms                                                 | 468 ms: 1.05x faster                                                      |
| async_tree_memoization_tg  | 626 ms                                                 | 600 ms: 1.04x faster                                                      |
| async_tree_io_tg           | 1.29 sec                                               | 1.25 sec: 1.04x faster                                                    |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 739 ms: 1.01x faster                                                      |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 752 ms: 1.01x faster                                                      |
| Geometric mean             | (ref)                                                  | 1.05x faster                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240311-linux-x86_64-faster%2dcpython-fewer_escapes-3.13.0a4+-731bd0c |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 191 ms: 1.02x faster                                                      |
| float          | 78.9 ms                                                | 97.0 ms: 1.23x slower                                                     |
| nbody          | 96.0 ms                                                | 125 ms: 1.30x slower                                                      |
| Geometric mean | (ref)                                                  | 1.16x slower                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240311-linux-x86_64-faster%2dcpython-fewer_escapes-3.13.0a4+-731bd0c |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.52 ms: 1.00x slower                                                     |
| regex_dna      | 205 ms                                                 | 225 ms: 1.10x slower                                                      |
| regex_v8       | 22.9 ms                                                | 25.6 ms: 1.12x slower                                                     |
| regex_compile  | 141 ms                                                 | 178 ms: 1.26x slower                                                      |
| Geometric mean | (ref)                                                  | 1.12x slower                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240311-linux-x86_64-faster%2dcpython-fewer_escapes-3.13.0a4+-731bd0c |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.7 ms: 1.25x faster                                                     |
| unpickle_list        | 5.21 us                                                | 5.02 us: 1.04x faster                                                     |
| json_loads           | 29.2 us                                                | 28.2 us: 1.04x faster                                                     |
| pickle_pure_python   | 320 us                                                 | 310 us: 1.03x faster                                                      |
| xml_etree_parse      | 164 ms                                                 | 162 ms: 1.01x faster                                                      |
| pickle_dict          | 34.6 us                                                | 34.4 us: 1.00x faster                                                     |
| xml_etree_iterparse  | 108 ms                                                 | 113 ms: 1.05x slower                                                      |
| pickle               | 11.0 us                                                | 11.7 us: 1.06x slower                                                     |
| pickle_list          | 4.59 us                                                | 4.97 us: 1.08x slower                                                     |
| tomli_loads          | 2.30 sec                                               | 2.53 sec: 1.10x slower                                                    |
| xml_etree_process    | 56.9 ms                                                | 63.6 ms: 1.12x slower                                                     |
| xml_etree_generate   | 81.1 ms                                                | 92.7 ms: 1.14x slower                                                     |
| unpickle             | 13.8 us                                                | 16.1 us: 1.16x slower                                                     |
| unpickle_pure_python | 242 us                                                 | 285 us: 1.18x slower                                                      |
| Geometric mean       | (ref)                                                  | 1.04x slower                                                              |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240311-linux-x86_64-faster%2dcpython-fewer_escapes-3.13.0a4+-731bd0c |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.4 ms: 1.21x slower                                                     |
| python_startup_no_site | 6.01 ms                                                | 8.98 ms: 1.49x slower                                                     |
| Geometric mean         | (ref)                                                  | 1.35x slower                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240311-linux-x86_64-faster%2dcpython-fewer_escapes-3.13.0a4+-731bd0c |
|-----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| django_template | 33.5 ms                                                | 35.3 ms: 1.05x slower                                                     |
| genshi_xml      | 53.4 ms                                                | 65.0 ms: 1.22x slower                                                     |
| mako            | 10.7 ms                                                | 13.3 ms: 1.25x slower                                                     |
| genshi_text     | 22.5 ms                                                | 28.3 ms: 1.25x slower                                                     |
| Geometric mean  | (ref)                                                  | 1.19x slower                                                              |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240311-linux-x86_64-faster%2dcpython-fewer_escapes-3.13.0a4+-731bd0c |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 117 us: 4.46x faster                                                      |
| generators                 | 74.9 ms                                                | 30.4 ms: 2.46x faster                                                     |
| asyncio_tcp                | 875 ms                                                 | 506 ms: 1.73x faster                                                      |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.85 sec: 1.68x faster                                                    |
| pylint                     | 476 ms                                                 | 334 ms: 1.42x faster                                                      |
| json_dumps                 | 13.3 ms                                                | 10.7 ms: 1.25x faster                                                     |
| coroutines                 | 27.0 ms                                                | 23.3 ms: 1.16x faster                                                     |
| async_tree_none            | 528 ms                                                 | 460 ms: 1.15x faster                                                      |
| async_tree_memoization     | 639 ms                                                 | 595 ms: 1.07x faster                                                      |
| comprehensions             | 23.6 us                                                | 22.1 us: 1.07x faster                                                     |
| djangocms                  | 33.5 us                                                | 31.5 us: 1.06x faster                                                     |
| logging_silent             | 111 ns                                                 | 105 ns: 1.05x faster                                                      |
| gc_traversal               | 4.01 ms                                                | 3.81 ms: 1.05x faster                                                     |
| async_tree_io              | 1.29 sec                                               | 1.22 sec: 1.05x faster                                                    |
| async_tree_none_tg         | 491 ms                                                 | 468 ms: 1.05x faster                                                      |
| async_tree_memoization_tg  | 626 ms                                                 | 600 ms: 1.04x faster                                                      |
| unpickle_list              | 5.21 us                                                | 5.02 us: 1.04x faster                                                     |
| json_loads                 | 29.2 us                                                | 28.2 us: 1.04x faster                                                     |
| async_tree_io_tg           | 1.29 sec                                               | 1.25 sec: 1.04x faster                                                    |
| pickle_pure_python         | 320 us                                                 | 310 us: 1.03x faster                                                      |
| deepcopy_reduce            | 3.22 us                                                | 3.16 us: 1.02x faster                                                     |
| pidigits                   | 194 ms                                                 | 191 ms: 1.02x faster                                                      |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 739 ms: 1.01x faster                                                      |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 752 ms: 1.01x faster                                                      |
| xml_etree_parse            | 164 ms                                                 | 162 ms: 1.01x faster                                                      |
| pickle_dict                | 34.6 us                                                | 34.4 us: 1.00x faster                                                     |
| mdp                        | 2.77 sec                                               | 2.76 sec: 1.00x faster                                                    |
| regex_effbot               | 3.51 ms                                                | 3.52 ms: 1.00x slower                                                     |
| sqlglot_normalize          | 113 ms                                                 | 114 ms: 1.01x slower                                                      |
| logging_simple             | 6.22 us                                                | 6.29 us: 1.01x slower                                                     |
| sympy_integrate            | 21.5 ms                                                | 21.8 ms: 1.01x slower                                                     |
| sqlglot_parse              | 1.43 ms                                                | 1.45 ms: 1.01x slower                                                     |
| deepcopy                   | 365 us                                                 | 371 us: 1.02x slower                                                      |
| asyncio_websockets         | 550 ms                                                 | 563 ms: 1.02x slower                                                      |
| sqlglot_transpile          | 1.75 ms                                                | 1.80 ms: 1.03x slower                                                     |
| logging_format             | 6.81 us                                                | 7.00 us: 1.03x slower                                                     |
| sympy_str                  | 297 ms                                                 | 306 ms: 1.03x slower                                                      |
| dask                       | 365 ms                                                 | 379 ms: 1.04x slower                                                      |
| richards_super             | 61.9 ms                                                | 64.4 ms: 1.04x slower                                                     |
| pathlib                    | 18.5 ms                                                | 19.3 ms: 1.04x slower                                                     |
| thrift                     | 784 us                                                 | 817 us: 1.04x slower                                                      |
| xml_etree_iterparse        | 108 ms                                                 | 113 ms: 1.05x slower                                                      |
| bench_thread_pool          | 834 us                                                 | 875 us: 1.05x slower                                                      |
| django_template            | 33.5 ms                                                | 35.3 ms: 1.05x slower                                                     |
| pickle                     | 11.0 us                                                | 11.7 us: 1.06x slower                                                     |
| tornado_http               | 98.1 ms                                                | 104 ms: 1.06x slower                                                      |
| sympy_expand               | 484 ms                                                 | 516 ms: 1.07x slower                                                      |
| create_gc_cycles           | 1.43 ms                                                | 1.53 ms: 1.07x slower                                                     |
| chameleon                  | 6.70 ms                                                | 7.20 ms: 1.07x slower                                                     |
| deepcopy_memo              | 40.2 us                                                | 43.3 us: 1.08x slower                                                     |
| chaos                      | 71.9 ms                                                | 77.7 ms: 1.08x slower                                                     |
| pickle_list                | 4.59 us                                                | 4.97 us: 1.08x slower                                                     |
| docutils                   | 2.66 sec                                               | 2.90 sec: 1.09x slower                                                    |
| html5lib                   | 64.8 ms                                                | 70.6 ms: 1.09x slower                                                     |
| tomli_loads                | 2.30 sec                                               | 2.53 sec: 1.10x slower                                                    |
| aiohttp                    | 1.12 ms                                                | 1.22 ms: 1.10x slower                                                     |
| gunicorn                   | 1.20 ms                                                | 1.32 ms: 1.10x slower                                                     |
| regex_dna                  | 205 ms                                                 | 225 ms: 1.10x slower                                                      |
| meteor_contest             | 109 ms                                                 | 121 ms: 1.11x slower                                                      |
| sqlglot_optimize           | 55.3 ms                                                | 61.6 ms: 1.11x slower                                                     |
| xml_etree_process          | 56.9 ms                                                | 63.6 ms: 1.12x slower                                                     |
| regex_v8                   | 22.9 ms                                                | 25.6 ms: 1.12x slower                                                     |
| dulwich_log                | 64.6 ms                                                | 72.9 ms: 1.13x slower                                                     |
| 2to3                       | 264 ms                                                 | 300 ms: 1.14x slower                                                      |
| xml_etree_generate         | 81.1 ms                                                | 92.7 ms: 1.14x slower                                                     |
| pycparser                  | 1.19 sec                                               | 1.37 sec: 1.15x slower                                                    |
| raytrace                   | 309 ms                                                 | 356 ms: 1.15x slower                                                      |
| sqlite_synth               | 2.57 us                                                | 2.98 us: 1.16x slower                                                     |
| unpickle                   | 13.8 us                                                | 16.1 us: 1.16x slower                                                     |
| crypto_pyaes               | 76.7 ms                                                | 89.6 ms: 1.17x slower                                                     |
| richards                   | 49.8 ms                                                | 58.2 ms: 1.17x slower                                                     |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.92 ms: 1.18x slower                                                     |
| unpickle_pure_python       | 242 us                                                 | 285 us: 1.18x slower                                                      |
| nqueens                    | 87.9 ms                                                | 105 ms: 1.19x slower                                                      |
| python_startup             | 8.56 ms                                                | 10.4 ms: 1.21x slower                                                     |
| genshi_xml                 | 53.4 ms                                                | 65.0 ms: 1.22x slower                                                     |
| pprint_safe_repr           | 747 ms                                                 | 913 ms: 1.22x slower                                                      |
| fannkuch                   | 405 ms                                                 | 497 ms: 1.23x slower                                                      |
| go                         | 149 ms                                                 | 182 ms: 1.23x slower                                                      |
| pprint_pformat             | 1.55 sec                                               | 1.91 sec: 1.23x slower                                                    |
| float                      | 78.9 ms                                                | 97.0 ms: 1.23x slower                                                     |
| coverage                   | 78.8 ms                                                | 98.0 ms: 1.24x slower                                                     |
| mako                       | 10.7 ms                                                | 13.3 ms: 1.25x slower                                                     |
| scimark_sor                | 121 ms                                                 | 152 ms: 1.25x slower                                                      |
| genshi_text                | 22.5 ms                                                | 28.3 ms: 1.25x slower                                                     |
| regex_compile              | 141 ms                                                 | 178 ms: 1.26x slower                                                      |
| scimark_fft                | 345 ms                                                 | 436 ms: 1.26x slower                                                      |
| scimark_monte_carlo        | 70.7 ms                                                | 89.4 ms: 1.26x slower                                                     |
| async_generators           | 374 ms                                                 | 473 ms: 1.27x slower                                                      |
| telco                      | 6.86 ms                                                | 8.84 ms: 1.29x slower                                                     |
| nbody                      | 96.0 ms                                                | 125 ms: 1.30x slower                                                      |
| mypy2                      | 686 ms                                                 | 920 ms: 1.34x slower                                                      |
| hexiom                     | 6.89 ms                                                | 9.40 ms: 1.37x slower                                                     |
| pyflate                    | 434 ms                                                 | 597 ms: 1.38x slower                                                      |
| unpack_sequence            | 43.5 ns                                                | 60.0 ns: 1.38x slower                                                     |
| spectral_norm              | 108 ms                                                 | 150 ms: 1.38x slower                                                      |
| scimark_lu                 | 116 ms                                                 | 163 ms: 1.40x slower                                                      |
| python_startup_no_site     | 6.01 ms                                                | 8.98 ms: 1.49x slower                                                     |
| Geometric mean             | (ref)                                                  | 1.05x slower                                                              |

Benchmark hidden because not significant (4): deltablue, sympy_sum, bench_mp_pool, json
Ignored benchmarks (3) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.05x
- 95% likely to have a slowdown of 1.04x
- 99% likely to have a slowdown of 1.03x


# Memory

- memory change: 1.01x