
# Results vs. 3.12.0

- fork: python
- ref: v3.11.0
- machine: linux-x86_64
- commit hash: deaf509
- commit date: 2022-10-24
- overall geometric mean: 1.02x slower
- HPT reliability: 79.60%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.95x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 264 ms: 1.04x faster                                   |
| chameleon      | 7.41 ms                                                | 6.70 ms: 1.11x faster                                  |
| docutils       | 2.77 sec                                               | 2.66 sec: 1.04x faster                                 |
| tornado_http   | 103 ms                                                 | 98.1 ms: 1.05x faster                                  |
| Geometric mean | (ref)                                                  | 1.06x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 726 ms                                                 | 749 ms: 1.03x slower                                   |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 761 ms: 1.05x slower                                   |
| async_tree_memoization_tg  | 575 ms                                                 | 626 ms: 1.09x slower                                   |
| async_tree_none_tg         | 450 ms                                                 | 491 ms: 1.09x slower                                   |
| async_tree_io_tg           | 1.18 sec                                               | 1.29 sec: 1.09x slower                                 |
| async_tree_memoization     | 578 ms                                                 | 639 ms: 1.11x slower                                   |
| async_tree_io              | 1.16 sec                                               | 1.29 sec: 1.11x slower                                 |
| async_tree_none            | 472 ms                                                 | 528 ms: 1.12x slower                                   |
| Geometric mean             | (ref)                                                  | 1.09x slower                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| float          | 84.7 ms                                                | 78.9 ms: 1.07x faster                                  |
| nbody          | 97.0 ms                                                | 96.0 ms: 1.01x faster                                  |
| pidigits       | 187 ms                                                 | 194 ms: 1.04x slower                                   |
| Geometric mean | (ref)                                                  | 1.02x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 141 ms: 1.05x faster                                   |
| regex_dna      | 212 ms                                                 | 205 ms: 1.04x faster                                   |
| regex_effbot   | 3.61 ms                                                | 3.51 ms: 1.03x faster                                  |
| regex_v8       | 23.1 ms                                                | 22.9 ms: 1.01x faster                                  |
| Geometric mean | (ref)                                                  | 1.03x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| unpickle             | 15.9 us                                                | 13.8 us: 1.15x faster                                  |
| pickle_list          | 5.08 us                                                | 4.59 us: 1.11x faster                                  |
| xml_etree_generate   | 89.2 ms                                                | 81.1 ms: 1.10x faster                                  |
| xml_etree_process    | 61.7 ms                                                | 56.9 ms: 1.08x faster                                  |
| pickle               | 11.6 us                                                | 11.0 us: 1.06x faster                                  |
| pickle_dict          | 35.5 us                                                | 34.6 us: 1.03x faster                                  |
| unpickle_list        | 5.29 us                                                | 5.21 us: 1.01x faster                                  |
| pickle_pure_python   | 324 us                                                 | 320 us: 1.01x faster                                   |
| tomli_loads          | 2.33 sec                                               | 2.30 sec: 1.01x faster                                 |
| xml_etree_iterparse  | 107 ms                                                 | 108 ms: 1.01x slower                                   |
| json_loads           | 28.5 us                                                | 29.2 us: 1.02x slower                                  |
| xml_etree_parse      | 159 ms                                                 | 164 ms: 1.03x slower                                   |
| unpickle_pure_python | 230 us                                                 | 242 us: 1.05x slower                                   |
| json_dumps           | 10.4 ms                                                | 13.3 ms: 1.28x slower                                  |
| Geometric mean       | (ref)                                                  | 1.01x faster                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup_no_site | 6.94 ms                                                | 6.01 ms: 1.15x faster                                  |
| python_startup         | 9.55 ms                                                | 8.56 ms: 1.12x faster                                  |
| Geometric mean         | (ref)                                                  | 1.13x faster                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako            | 11.9 ms                                                | 10.7 ms: 1.12x faster                                  |
| django_template | 34.6 ms                                                | 33.5 ms: 1.03x faster                                  |
| Geometric mean  | (ref)                                                  | 1.07x faster                                           |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| unpack_sequence            | 54.0 ns                                                | 43.5 ns: 1.24x faster                                  |
| async_generators           | 463 ms                                                 | 374 ms: 1.24x faster                                   |
| mypy2                      | 830 ms                                                 | 686 ms: 1.21x faster                                   |
| python_startup_no_site     | 6.94 ms                                                | 6.01 ms: 1.15x faster                                  |
| unpickle                   | 15.9 us                                                | 13.8 us: 1.15x faster                                  |
| mako                       | 11.9 ms                                                | 10.7 ms: 1.12x faster                                  |
| python_startup             | 9.55 ms                                                | 8.56 ms: 1.12x faster                                  |
| pyflate                    | 482 ms                                                 | 434 ms: 1.11x faster                                   |
| pickle_list                | 5.08 us                                                | 4.59 us: 1.11x faster                                  |
| chameleon                  | 7.41 ms                                                | 6.70 ms: 1.11x faster                                  |
| scimark_fft                | 382 ms                                                 | 345 ms: 1.11x faster                                   |
| sqlite_synth               | 2.83 us                                                | 2.57 us: 1.10x faster                                  |
| xml_etree_generate         | 89.2 ms                                                | 81.1 ms: 1.10x faster                                  |
| xml_etree_process          | 61.7 ms                                                | 56.9 ms: 1.08x faster                                  |
| float                      | 84.7 ms                                                | 78.9 ms: 1.07x faster                                  |
| crypto_pyaes               | 81.9 ms                                                | 76.7 ms: 1.07x faster                                  |
| scimark_sor                | 129 ms                                                 | 121 ms: 1.06x faster                                   |
| scimark_monte_carlo        | 75.1 ms                                                | 70.7 ms: 1.06x faster                                  |
| spectral_norm              | 115 ms                                                 | 108 ms: 1.06x faster                                   |
| logging_format             | 7.23 us                                                | 6.81 us: 1.06x faster                                  |
| dulwich_log                | 68.5 ms                                                | 64.6 ms: 1.06x faster                                  |
| pickle                     | 11.6 us                                                | 11.0 us: 1.06x faster                                  |
| regex_compile              | 148 ms                                                 | 141 ms: 1.05x faster                                   |
| tornado_http               | 103 ms                                                 | 98.1 ms: 1.05x faster                                  |
| sqlalchemy_declarative     | 147 ms                                                 | 140 ms: 1.05x faster                                   |
| pathlib                    | 19.3 ms                                                | 18.5 ms: 1.04x faster                                  |
| deepcopy_reduce            | 3.35 us                                                | 3.22 us: 1.04x faster                                  |
| docutils                   | 2.77 sec                                               | 2.66 sec: 1.04x faster                                 |
| logging_simple             | 6.46 us                                                | 6.22 us: 1.04x faster                                  |
| pprint_safe_repr           | 776 ms                                                 | 747 ms: 1.04x faster                                   |
| 2to3                       | 274 ms                                                 | 264 ms: 1.04x faster                                   |
| regex_dna                  | 212 ms                                                 | 205 ms: 1.04x faster                                   |
| gunicorn                   | 1.24 ms                                                | 1.20 ms: 1.04x faster                                  |
| telco                      | 7.10 ms                                                | 6.86 ms: 1.04x faster                                  |
| aiohttp                    | 1.15 ms                                                | 1.12 ms: 1.03x faster                                  |
| django_template            | 34.6 ms                                                | 33.5 ms: 1.03x faster                                  |
| meteor_contest             | 112 ms                                                 | 109 ms: 1.03x faster                                   |
| create_gc_cycles           | 1.48 ms                                                | 1.43 ms: 1.03x faster                                  |
| regex_effbot               | 3.61 ms                                                | 3.51 ms: 1.03x faster                                  |
| fannkuch                   | 417 ms                                                 | 405 ms: 1.03x faster                                   |
| pickle_dict                | 35.5 us                                                | 34.6 us: 1.03x faster                                  |
| sqlalchemy_imperative      | 18.7 ms                                                | 18.3 ms: 1.02x faster                                  |
| dask                       | 372 ms                                                 | 365 ms: 1.02x faster                                   |
| deepcopy                   | 371 us                                                 | 365 us: 1.02x faster                                   |
| scimark_lu                 | 118 ms                                                 | 116 ms: 1.01x faster                                   |
| deepcopy_memo              | 40.7 us                                                | 40.2 us: 1.01x faster                                  |
| unpickle_list              | 5.29 us                                                | 5.21 us: 1.01x faster                                  |
| pickle_pure_python         | 324 us                                                 | 320 us: 1.01x faster                                   |
| raytrace                   | 312 ms                                                 | 309 ms: 1.01x faster                                   |
| tomli_loads                | 2.33 sec                                               | 2.30 sec: 1.01x faster                                 |
| regex_v8                   | 23.1 ms                                                | 22.9 ms: 1.01x faster                                  |
| nbody                      | 97.0 ms                                                | 96.0 ms: 1.01x faster                                  |
| pprint_pformat             | 1.57 sec                                               | 1.55 sec: 1.01x faster                                 |
| bench_thread_pool          | 842 us                                                 | 834 us: 1.01x faster                                   |
| sympy_str                  | 300 ms                                                 | 297 ms: 1.01x faster                                   |
| sqlglot_optimize           | 54.8 ms                                                | 55.3 ms: 1.01x slower                                  |
| xml_etree_iterparse        | 107 ms                                                 | 108 ms: 1.01x slower                                   |
| sympy_expand               | 478 ms                                                 | 484 ms: 1.01x slower                                   |
| sqlglot_normalize          | 110 ms                                                 | 113 ms: 1.02x slower                                   |
| json_loads                 | 28.5 us                                                | 29.2 us: 1.02x slower                                  |
| xml_etree_parse            | 159 ms                                                 | 164 ms: 1.03x slower                                   |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 749 ms: 1.03x slower                                   |
| pidigits                   | 187 ms                                                 | 194 ms: 1.04x slower                                   |
| sqlglot_transpile          | 1.68 ms                                                | 1.75 ms: 1.04x slower                                  |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 761 ms: 1.05x slower                                   |
| unpickle_pure_python       | 230 us                                                 | 242 us: 1.05x slower                                   |
| sqlglot_parse              | 1.36 ms                                                | 1.43 ms: 1.05x slower                                  |
| mdp                        | 2.63 sec                                               | 2.77 sec: 1.05x slower                                 |
| nqueens                    | 83.3 ms                                                | 87.9 ms: 1.06x slower                                  |
| deltablue                  | 3.72 ms                                                | 3.92 ms: 1.06x slower                                  |
| gc_traversal               | 3.79 ms                                                | 4.01 ms: 1.06x slower                                  |
| logging_silent             | 104 ns                                                 | 111 ns: 1.06x slower                                   |
| go                         | 139 ms                                                 | 149 ms: 1.07x slower                                   |
| chaos                      | 67.0 ms                                                | 71.9 ms: 1.07x slower                                  |
| hexiom                     | 6.41 ms                                                | 6.89 ms: 1.07x slower                                  |
| coverage                   | 72.7 ms                                                | 78.8 ms: 1.08x slower                                  |
| comprehensions             | 21.8 us                                                | 23.6 us: 1.08x slower                                  |
| richards                   | 45.8 ms                                                | 49.8 ms: 1.09x slower                                  |
| async_tree_memoization_tg  | 575 ms                                                 | 626 ms: 1.09x slower                                   |
| async_tree_none_tg         | 450 ms                                                 | 491 ms: 1.09x slower                                   |
| async_tree_io_tg           | 1.18 sec                                               | 1.29 sec: 1.09x slower                                 |
| async_tree_memoization     | 578 ms                                                 | 639 ms: 1.11x slower                                   |
| async_tree_io              | 1.16 sec                                               | 1.29 sec: 1.11x slower                                 |
| async_tree_none            | 472 ms                                                 | 528 ms: 1.12x slower                                   |
| coroutines                 | 23.2 ms                                                | 27.0 ms: 1.17x slower                                  |
| richards_super             | 51.5 ms                                                | 61.9 ms: 1.20x slower                                  |
| json_dumps                 | 10.4 ms                                                | 13.3 ms: 1.28x slower                                  |
| asyncio_tcp_ssl            | 1.79 sec                                               | 3.11 sec: 1.74x slower                                 |
| asyncio_tcp                | 491 ms                                                 | 875 ms: 1.78x slower                                   |
| generators                 | 31.2 ms                                                | 74.9 ms: 2.40x slower                                  |
| typing_runtime_protocols   | 158 us                                                 | 520 us: 3.29x slower                                   |
| Geometric mean             | (ref)                                                  | 1.02x slower                                           |

Benchmark hidden because not significant (7): scimark_sparse_mat_mult, json, asyncio_websockets, sympy_sum, bench_mp_pool, sympy_integrate, pycparser
Ignored benchmarks (7) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: djangocms, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 79.60% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.95x