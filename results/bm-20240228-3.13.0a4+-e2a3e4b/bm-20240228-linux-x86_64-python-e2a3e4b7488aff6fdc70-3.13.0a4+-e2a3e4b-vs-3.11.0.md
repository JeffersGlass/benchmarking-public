# Results vs. 3.11.0

- fork: python
- ref: e2a3e4b7488aff6fdc70
- machine: linux-x86_64
- commit hash: e2a3e4b
- commit date: 2024-02-28
- overall geometric mean: 1.08x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 261 ms: 1.01x faster                                                   |
| chameleon      | 6.70 ms                                                | 6.82 ms: 1.02x slower                                                  |
| docutils       | 2.66 sec                                               | 2.56 sec: 1.04x faster                                                 |
| tornado_http   | 98.1 ms                                                | 94.7 ms: 1.03x faster                                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 431 ms: 1.23x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 555 ms: 1.15x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 442 ms: 1.11x faster                                                   |
| async_tree_memoization_tg  | 626 ms                                                 | 566 ms: 1.11x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.16 sec: 1.10x faster                                                 |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                                 |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 699 ms: 1.07x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 715 ms: 1.06x faster                                                   |
| Geometric mean             | (ref)                                                  | 1.11x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 86.5 ms: 1.11x faster                                                  |
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                                   |
| Geometric mean | (ref)                                                  | 1.05x faster                                                           |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 131 ms: 1.08x faster                                                   |
| regex_effbot   | 3.51 ms                                                | 3.73 ms: 1.06x slower                                                  |
| regex_dna      | 205 ms                                                 | 219 ms: 1.07x slower                                                   |
| regex_v8       | 22.9 ms                                                | 24.8 ms: 1.08x slower                                                  |
| Geometric mean | (ref)                                                  | 1.03x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.3 ms: 1.29x faster                                                  |
| unpickle_pure_python | 242 us                                                 | 212 us: 1.14x faster                                                   |
| pickle_pure_python   | 320 us                                                 | 292 us: 1.09x faster                                                   |
| json_loads           | 29.2 us                                                | 27.1 us: 1.08x faster                                                  |
| tomli_loads          | 2.30 sec                                               | 2.15 sec: 1.07x faster                                                 |
| unpickle_list        | 5.21 us                                                | 4.92 us: 1.06x faster                                                  |
| xml_etree_parse      | 164 ms                                                 | 156 ms: 1.05x faster                                                   |
| xml_etree_iterparse  | 108 ms                                                 | 104 ms: 1.04x faster                                                   |
| pickle_dict          | 34.6 us                                                | 35.1 us: 1.01x slower                                                  |
| xml_etree_process    | 56.9 ms                                                | 57.8 ms: 1.02x slower                                                  |
| xml_etree_generate   | 81.1 ms                                                | 84.7 ms: 1.04x slower                                                  |
| pickle               | 11.0 us                                                | 11.7 us: 1.07x slower                                                  |
| unpickle             | 13.8 us                                                | 15.6 us: 1.13x slower                                                  |
| pickle_list          | 4.59 us                                                | 5.29 us: 1.15x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                  |
| python_startup_no_site | 6.01 ms                                                | 8.81 ms: 1.47x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.32x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.0 ms: 1.03x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 110 us: 4.70x faster                                                   |
| generators                 | 74.9 ms                                                | 29.4 ms: 2.55x faster                                                  |
| asyncio_tcp                | 875 ms                                                 | 483 ms: 1.81x faster                                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.79 sec: 1.74x faster                                                 |
| comprehensions             | 23.6 us                                                | 16.1 us: 1.47x faster                                                  |
| json_dumps                 | 13.3 ms                                                | 10.3 ms: 1.29x faster                                                  |
| deltablue                  | 3.92 ms                                                | 3.15 ms: 1.25x faster                                                  |
| async_tree_none            | 528 ms                                                 | 431 ms: 1.23x faster                                                   |
| coroutines                 | 27.0 ms                                                | 22.3 ms: 1.21x faster                                                  |
| chaos                      | 71.9 ms                                                | 59.8 ms: 1.20x faster                                                  |
| raytrace                   | 309 ms                                                 | 260 ms: 1.19x faster                                                   |
| hexiom                     | 6.89 ms                                                | 5.86 ms: 1.17x faster                                                  |
| logging_silent             | 111 ns                                                 | 95.1 ns: 1.17x faster                                                  |
| async_tree_memoization     | 639 ms                                                 | 555 ms: 1.15x faster                                                   |
| sympy_sum                  | 169 ms                                                 | 147 ms: 1.15x faster                                                   |
| sqlglot_parse              | 1.43 ms                                                | 1.24 ms: 1.15x faster                                                  |
| richards_super             | 61.9 ms                                                | 53.8 ms: 1.15x faster                                                  |
| unpickle_pure_python       | 242 us                                                 | 212 us: 1.14x faster                                                   |
| nqueens                    | 87.9 ms                                                | 77.5 ms: 1.13x faster                                                  |
| sqlglot_transpile          | 1.75 ms                                                | 1.56 ms: 1.12x faster                                                  |
| sympy_str                  | 297 ms                                                 | 266 ms: 1.12x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 442 ms: 1.11x faster                                                   |
| nbody                      | 96.0 ms                                                | 86.5 ms: 1.11x faster                                                  |
| async_tree_memoization_tg  | 626 ms                                                 | 566 ms: 1.11x faster                                                   |
| sympy_integrate            | 21.5 ms                                                | 19.4 ms: 1.11x faster                                                  |
| async_tree_io              | 1.29 sec                                               | 1.16 sec: 1.10x faster                                                 |
| logging_simple             | 6.22 us                                                | 5.64 us: 1.10x faster                                                  |
| go                         | 149 ms                                                 | 135 ms: 1.10x faster                                                   |
| crypto_pyaes               | 76.7 ms                                                | 69.9 ms: 1.10x faster                                                  |
| pickle_pure_python         | 320 us                                                 | 292 us: 1.09x faster                                                   |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.60 ms: 1.09x faster                                                  |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                                 |
| logging_format             | 6.81 us                                                | 6.24 us: 1.09x faster                                                  |
| regex_compile              | 141 ms                                                 | 131 ms: 1.08x faster                                                   |
| sqlglot_normalize          | 113 ms                                                 | 104 ms: 1.08x faster                                                   |
| fannkuch                   | 405 ms                                                 | 376 ms: 1.08x faster                                                   |
| json_loads                 | 29.2 us                                                | 27.1 us: 1.08x faster                                                  |
| tomli_loads                | 2.30 sec                                               | 2.15 sec: 1.07x faster                                                 |
| sympy_expand               | 484 ms                                                 | 452 ms: 1.07x faster                                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 699 ms: 1.07x faster                                                   |
| deepcopy_memo              | 40.2 us                                                | 37.5 us: 1.07x faster                                                  |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 715 ms: 1.06x faster                                                   |
| unpickle_list              | 5.21 us                                                | 4.92 us: 1.06x faster                                                  |
| json                       | 5.24 ms                                                | 4.96 ms: 1.06x faster                                                  |
| deepcopy_reduce            | 3.22 us                                                | 3.04 us: 1.06x faster                                                  |
| pprint_pformat             | 1.55 sec                                               | 1.47 sec: 1.06x faster                                                 |
| xml_etree_parse            | 164 ms                                                 | 156 ms: 1.05x faster                                                   |
| deepcopy                   | 365 us                                                 | 347 us: 1.05x faster                                                   |
| richards                   | 49.8 ms                                                | 47.5 ms: 1.05x faster                                                  |
| sqlglot_optimize           | 55.3 ms                                                | 52.8 ms: 1.05x faster                                                  |
| scimark_monte_carlo        | 70.7 ms                                                | 67.5 ms: 1.05x faster                                                  |
| pprint_safe_repr           | 747 ms                                                 | 715 ms: 1.04x faster                                                   |
| xml_etree_iterparse        | 108 ms                                                 | 104 ms: 1.04x faster                                                   |
| docutils                   | 2.66 sec                                               | 2.56 sec: 1.04x faster                                                 |
| meteor_contest             | 109 ms                                                 | 105 ms: 1.04x faster                                                   |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                                   |
| pathlib                    | 18.5 ms                                                | 17.9 ms: 1.04x faster                                                  |
| mdp                        | 2.77 sec                                               | 2.68 sec: 1.04x faster                                                 |
| tornado_http               | 98.1 ms                                                | 94.7 ms: 1.03x faster                                                  |
| pycparser                  | 1.19 sec                                               | 1.15 sec: 1.03x faster                                                 |
| scimark_lu                 | 116 ms                                                 | 113 ms: 1.03x faster                                                   |
| bench_thread_pool          | 834 us                                                 | 814 us: 1.03x faster                                                   |
| unpack_sequence            | 43.5 ns                                                | 42.5 ns: 1.02x faster                                                  |
| scimark_sor                | 121 ms                                                 | 120 ms: 1.01x faster                                                   |
| 2to3                       | 264 ms                                                 | 261 ms: 1.01x faster                                                   |
| gc_traversal               | 4.01 ms                                                | 4.00 ms: 1.00x faster                                                  |
| dulwich_log                | 64.6 ms                                                | 65.0 ms: 1.01x slower                                                  |
| pickle_dict                | 34.6 us                                                | 35.1 us: 1.01x slower                                                  |
| xml_etree_process          | 56.9 ms                                                | 57.8 ms: 1.02x slower                                                  |
| asyncio_websockets         | 550 ms                                                 | 560 ms: 1.02x slower                                                   |
| chameleon                  | 6.70 ms                                                | 6.82 ms: 1.02x slower                                                  |
| pyflate                    | 434 ms                                                 | 442 ms: 1.02x slower                                                   |
| scimark_fft                | 345 ms                                                 | 353 ms: 1.02x slower                                                   |
| mako                       | 10.7 ms                                                | 11.0 ms: 1.03x slower                                                  |
| create_gc_cycles           | 1.43 ms                                                | 1.48 ms: 1.03x slower                                                  |
| xml_etree_generate         | 81.1 ms                                                | 84.7 ms: 1.04x slower                                                  |
| regex_effbot               | 3.51 ms                                                | 3.73 ms: 1.06x slower                                                  |
| pickle                     | 11.0 us                                                | 11.7 us: 1.07x slower                                                  |
| regex_dna                  | 205 ms                                                 | 219 ms: 1.07x slower                                                   |
| regex_v8                   | 22.9 ms                                                | 24.8 ms: 1.08x slower                                                  |
| sqlite_synth               | 2.57 us                                                | 2.83 us: 1.10x slower                                                  |
| unpickle                   | 13.8 us                                                | 15.6 us: 1.13x slower                                                  |
| pickle_list                | 4.59 us                                                | 5.29 us: 1.15x slower                                                  |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                  |
| async_generators           | 374 ms                                                 | 445 ms: 1.19x slower                                                   |
| coverage                   | 78.8 ms                                                | 95.2 ms: 1.21x slower                                                  |
| telco                      | 6.86 ms                                                | 8.34 ms: 1.22x slower                                                  |
| mypy2                      | 686 ms                                                 | 839 ms: 1.22x slower                                                   |
| python_startup_no_site     | 6.01 ms                                                | 8.81 ms: 1.47x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                           |

Benchmark hidden because not significant (3): bench_mp_pool, float, spectral_norm
Ignored benchmarks (13) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.04x
- 95% likely to have a speedup of 1.04x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: 0.99x