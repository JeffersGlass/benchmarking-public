
# Results vs. 3.11.0

- fork: python
- ref: v3.12.0
- machine: linux-x86_64
- commit hash: 0fb18b0
- commit date: 2023-10-02
- overall geometric mean: 1.02x faster
- HPT reliability: 79.60%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 274 ms: 1.04x slower                                   |
| chameleon      | 6.70 ms                                                | 7.41 ms: 1.11x slower                                  |
| docutils       | 2.66 sec                                               | 2.77 sec: 1.04x slower                                 |
| tornado_http   | 98.1 ms                                                | 103 ms: 1.05x slower                                   |
| Geometric mean | (ref)                                                  | 1.06x slower                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 472 ms: 1.12x faster                                   |
| async_tree_io              | 1.29 sec                                               | 1.16 sec: 1.11x faster                                 |
| async_tree_memoization     | 639 ms                                                 | 578 ms: 1.11x faster                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.18 sec: 1.09x faster                                 |
| async_tree_none_tg         | 491 ms                                                 | 450 ms: 1.09x faster                                   |
| async_tree_memoization_tg  | 626 ms                                                 | 575 ms: 1.09x faster                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 726 ms: 1.05x faster                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 726 ms: 1.03x faster                                   |
| Geometric mean             | (ref)                                                  | 1.09x faster                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                   |
| nbody          | 96.0 ms                                                | 97.0 ms: 1.01x slower                                  |
| float          | 78.9 ms                                                | 84.7 ms: 1.07x slower                                  |
| Geometric mean | (ref)                                                  | 1.02x slower                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_v8       | 22.9 ms                                                | 23.1 ms: 1.01x slower                                  |
| regex_effbot   | 3.51 ms                                                | 3.61 ms: 1.03x slower                                  |
| regex_dna      | 205 ms                                                 | 212 ms: 1.04x slower                                   |
| regex_compile  | 141 ms                                                 | 148 ms: 1.05x slower                                   |
| Geometric mean | (ref)                                                  | 1.03x slower                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.28x faster                                  |
| unpickle_pure_python | 242 us                                                 | 230 us: 1.05x faster                                   |
| xml_etree_parse      | 164 ms                                                 | 159 ms: 1.03x faster                                   |
| json_loads           | 29.2 us                                                | 28.5 us: 1.02x faster                                  |
| xml_etree_iterparse  | 108 ms                                                 | 107 ms: 1.01x faster                                   |
| tomli_loads          | 2.30 sec                                               | 2.33 sec: 1.01x slower                                 |
| pickle_pure_python   | 320 us                                                 | 324 us: 1.01x slower                                   |
| unpickle_list        | 5.21 us                                                | 5.29 us: 1.01x slower                                  |
| pickle_dict          | 34.6 us                                                | 35.5 us: 1.03x slower                                  |
| pickle               | 11.0 us                                                | 11.6 us: 1.06x slower                                  |
| xml_etree_process    | 56.9 ms                                                | 61.7 ms: 1.08x slower                                  |
| xml_etree_generate   | 81.1 ms                                                | 89.2 ms: 1.10x slower                                  |
| pickle_list          | 4.59 us                                                | 5.08 us: 1.11x slower                                  |
| unpickle             | 13.8 us                                                | 15.9 us: 1.15x slower                                  |
| Geometric mean       | (ref)                                                  | 1.01x slower                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 9.55 ms: 1.12x slower                                  |
| python_startup_no_site | 6.01 ms                                                | 6.94 ms: 1.15x slower                                  |
| Geometric mean         | (ref)                                                  | 1.13x slower                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| django_template | 33.5 ms                                                | 34.6 ms: 1.03x slower                                  |
| mako            | 10.7 ms                                                | 11.9 ms: 1.12x slower                                  |
| Geometric mean  | (ref)                                                  | 1.07x slower                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 158 us: 3.29x faster                                   |
| generators                 | 74.9 ms                                                | 31.2 ms: 2.40x faster                                  |
| asyncio_tcp                | 875 ms                                                 | 491 ms: 1.78x faster                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.79 sec: 1.74x faster                                 |
| json_dumps                 | 13.3 ms                                                | 10.4 ms: 1.28x faster                                  |
| richards_super             | 61.9 ms                                                | 51.5 ms: 1.20x faster                                  |
| coroutines                 | 27.0 ms                                                | 23.2 ms: 1.17x faster                                  |
| async_tree_none            | 528 ms                                                 | 472 ms: 1.12x faster                                   |
| async_tree_io              | 1.29 sec                                               | 1.16 sec: 1.11x faster                                 |
| async_tree_memoization     | 639 ms                                                 | 578 ms: 1.11x faster                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.18 sec: 1.09x faster                                 |
| async_tree_none_tg         | 491 ms                                                 | 450 ms: 1.09x faster                                   |
| async_tree_memoization_tg  | 626 ms                                                 | 575 ms: 1.09x faster                                   |
| richards                   | 49.8 ms                                                | 45.8 ms: 1.09x faster                                  |
| comprehensions             | 23.6 us                                                | 21.8 us: 1.08x faster                                  |
| coverage                   | 78.8 ms                                                | 72.7 ms: 1.08x faster                                  |
| hexiom                     | 6.89 ms                                                | 6.41 ms: 1.07x faster                                  |
| chaos                      | 71.9 ms                                                | 67.0 ms: 1.07x faster                                  |
| go                         | 149 ms                                                 | 139 ms: 1.07x faster                                   |
| logging_silent             | 111 ns                                                 | 104 ns: 1.06x faster                                   |
| gc_traversal               | 4.01 ms                                                | 3.79 ms: 1.06x faster                                  |
| deltablue                  | 3.92 ms                                                | 3.72 ms: 1.06x faster                                  |
| nqueens                    | 87.9 ms                                                | 83.3 ms: 1.06x faster                                  |
| mdp                        | 2.77 sec                                               | 2.63 sec: 1.05x faster                                 |
| sqlglot_parse              | 1.43 ms                                                | 1.36 ms: 1.05x faster                                  |
| unpickle_pure_python       | 242 us                                                 | 230 us: 1.05x faster                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 726 ms: 1.05x faster                                   |
| sqlglot_transpile          | 1.75 ms                                                | 1.68 ms: 1.04x faster                                  |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 726 ms: 1.03x faster                                   |
| xml_etree_parse            | 164 ms                                                 | 159 ms: 1.03x faster                                   |
| json_loads                 | 29.2 us                                                | 28.5 us: 1.02x faster                                  |
| sqlglot_normalize          | 113 ms                                                 | 110 ms: 1.02x faster                                   |
| sympy_expand               | 484 ms                                                 | 478 ms: 1.01x faster                                   |
| xml_etree_iterparse        | 108 ms                                                 | 107 ms: 1.01x faster                                   |
| sqlglot_optimize           | 55.3 ms                                                | 54.8 ms: 1.01x faster                                  |
| sympy_str                  | 297 ms                                                 | 300 ms: 1.01x slower                                   |
| bench_thread_pool          | 834 us                                                 | 842 us: 1.01x slower                                   |
| pprint_pformat             | 1.55 sec                                               | 1.57 sec: 1.01x slower                                 |
| nbody                      | 96.0 ms                                                | 97.0 ms: 1.01x slower                                  |
| regex_v8                   | 22.9 ms                                                | 23.1 ms: 1.01x slower                                  |
| tomli_loads                | 2.30 sec                                               | 2.33 sec: 1.01x slower                                 |
| raytrace                   | 309 ms                                                 | 312 ms: 1.01x slower                                   |
| pickle_pure_python         | 320 us                                                 | 324 us: 1.01x slower                                   |
| unpickle_list              | 5.21 us                                                | 5.29 us: 1.01x slower                                  |
| deepcopy_memo              | 40.2 us                                                | 40.7 us: 1.01x slower                                  |
| scimark_lu                 | 116 ms                                                 | 118 ms: 1.01x slower                                   |
| deepcopy                   | 365 us                                                 | 371 us: 1.02x slower                                   |
| dask                       | 365 ms                                                 | 372 ms: 1.02x slower                                   |
| sqlalchemy_imperative      | 18.3 ms                                                | 18.7 ms: 1.02x slower                                  |
| pickle_dict                | 34.6 us                                                | 35.5 us: 1.03x slower                                  |
| fannkuch                   | 405 ms                                                 | 417 ms: 1.03x slower                                   |
| regex_effbot               | 3.51 ms                                                | 3.61 ms: 1.03x slower                                  |
| create_gc_cycles           | 1.43 ms                                                | 1.48 ms: 1.03x slower                                  |
| meteor_contest             | 109 ms                                                 | 112 ms: 1.03x slower                                   |
| django_template            | 33.5 ms                                                | 34.6 ms: 1.03x slower                                  |
| aiohttp                    | 1.12 ms                                                | 1.15 ms: 1.03x slower                                  |
| telco                      | 6.86 ms                                                | 7.10 ms: 1.04x slower                                  |
| gunicorn                   | 1.20 ms                                                | 1.24 ms: 1.04x slower                                  |
| regex_dna                  | 205 ms                                                 | 212 ms: 1.04x slower                                   |
| 2to3                       | 264 ms                                                 | 274 ms: 1.04x slower                                   |
| pprint_safe_repr           | 747 ms                                                 | 776 ms: 1.04x slower                                   |
| logging_simple             | 6.22 us                                                | 6.46 us: 1.04x slower                                  |
| docutils                   | 2.66 sec                                               | 2.77 sec: 1.04x slower                                 |
| deepcopy_reduce            | 3.22 us                                                | 3.35 us: 1.04x slower                                  |
| pathlib                    | 18.5 ms                                                | 19.3 ms: 1.04x slower                                  |
| sqlalchemy_declarative     | 140 ms                                                 | 147 ms: 1.05x slower                                   |
| tornado_http               | 98.1 ms                                                | 103 ms: 1.05x slower                                   |
| regex_compile              | 141 ms                                                 | 148 ms: 1.05x slower                                   |
| pickle                     | 11.0 us                                                | 11.6 us: 1.06x slower                                  |
| dulwich_log                | 64.6 ms                                                | 68.5 ms: 1.06x slower                                  |
| logging_format             | 6.81 us                                                | 7.23 us: 1.06x slower                                  |
| spectral_norm              | 108 ms                                                 | 115 ms: 1.06x slower                                   |
| scimark_monte_carlo        | 70.7 ms                                                | 75.1 ms: 1.06x slower                                  |
| scimark_sor                | 121 ms                                                 | 129 ms: 1.06x slower                                   |
| crypto_pyaes               | 76.7 ms                                                | 81.9 ms: 1.07x slower                                  |
| float                      | 78.9 ms                                                | 84.7 ms: 1.07x slower                                  |
| xml_etree_process          | 56.9 ms                                                | 61.7 ms: 1.08x slower                                  |
| xml_etree_generate         | 81.1 ms                                                | 89.2 ms: 1.10x slower                                  |
| sqlite_synth               | 2.57 us                                                | 2.83 us: 1.10x slower                                  |
| scimark_fft                | 345 ms                                                 | 382 ms: 1.11x slower                                   |
| chameleon                  | 6.70 ms                                                | 7.41 ms: 1.11x slower                                  |
| pickle_list                | 4.59 us                                                | 5.08 us: 1.11x slower                                  |
| pyflate                    | 434 ms                                                 | 482 ms: 1.11x slower                                   |
| python_startup             | 8.56 ms                                                | 9.55 ms: 1.12x slower                                  |
| mako                       | 10.7 ms                                                | 11.9 ms: 1.12x slower                                  |
| unpickle                   | 13.8 us                                                | 15.9 us: 1.15x slower                                  |
| python_startup_no_site     | 6.01 ms                                                | 6.94 ms: 1.15x slower                                  |
| mypy2                      | 686 ms                                                 | 830 ms: 1.21x slower                                   |
| async_generators           | 374 ms                                                 | 463 ms: 1.24x slower                                   |
| unpack_sequence            | 43.5 ns                                                | 54.0 ns: 1.24x slower                                  |
| Geometric mean             | (ref)                                                  | 1.02x faster                                           |

Benchmark hidden because not significant (7): pycparser, sympy_integrate, bench_mp_pool, sympy_sum, asyncio_websockets, json, scimark_sparse_mat_mult
Ignored benchmarks (7) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: djangocms, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 79.60% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.07x