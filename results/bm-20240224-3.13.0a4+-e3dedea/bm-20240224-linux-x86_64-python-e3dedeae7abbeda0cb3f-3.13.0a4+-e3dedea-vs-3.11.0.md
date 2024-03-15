
# Results vs. 3.11.0

- fork: python
- ref: e3dedeae7abbeda0cb3f
- machine: linux-x86_64
- commit hash: e3dedea
- commit date: 2024-02-24
- overall geometric mean: 1.08x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 263 ms: 1.01x faster                                                   |
| docutils       | 2.66 sec                                               | 2.58 sec: 1.03x faster                                                 |
| tornado_http   | 98.1 ms                                                | 94.5 ms: 1.04x faster                                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                                           |

Benchmark hidden because not significant (1): chameleon

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 433 ms: 1.22x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 556 ms: 1.15x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 444 ms: 1.11x faster                                                   |
| async_tree_memoization_tg  | 626 ms                                                 | 570 ms: 1.10x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.17 sec: 1.10x faster                                                 |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                                 |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 703 ms: 1.07x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 719 ms: 1.06x faster                                                   |
| Geometric mean             | (ref)                                                  | 1.11x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 88.7 ms: 1.08x faster                                                  |
| pidigits       | 194 ms                                                 | 188 ms: 1.03x faster                                                   |
| float          | 78.9 ms                                                | 80.1 ms: 1.01x slower                                                  |
| Geometric mean | (ref)                                                  | 1.03x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 130 ms: 1.08x faster                                                   |
| regex_effbot   | 3.51 ms                                                | 3.49 ms: 1.00x faster                                                  |
| regex_dna      | 205 ms                                                 | 214 ms: 1.04x slower                                                   |
| regex_v8       | 22.9 ms                                                | 24.6 ms: 1.07x slower                                                  |
| Geometric mean | (ref)                                                  | 1.01x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                  |
| unpickle_pure_python | 242 us                                                 | 211 us: 1.15x faster                                                   |
| pickle_pure_python   | 320 us                                                 | 289 us: 1.11x faster                                                   |
| tomli_loads          | 2.30 sec                                               | 2.14 sec: 1.08x faster                                                 |
| json_loads           | 29.2 us                                                | 27.4 us: 1.06x faster                                                  |
| unpickle_list        | 5.21 us                                                | 4.98 us: 1.05x faster                                                  |
| xml_etree_parse      | 164 ms                                                 | 157 ms: 1.05x faster                                                   |
| xml_etree_iterparse  | 108 ms                                                 | 105 ms: 1.03x faster                                                   |
| xml_etree_process    | 56.9 ms                                                | 57.9 ms: 1.02x slower                                                  |
| pickle_dict          | 34.6 us                                                | 35.8 us: 1.03x slower                                                  |
| xml_etree_generate   | 81.1 ms                                                | 84.3 ms: 1.04x slower                                                  |
| unpickle             | 13.8 us                                                | 14.9 us: 1.08x slower                                                  |
| pickle               | 11.0 us                                                | 12.1 us: 1.10x slower                                                  |
| pickle_list          | 4.59 us                                                | 5.21 us: 1.14x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                  |
| python_startup_no_site | 6.01 ms                                                | 8.73 ms: 1.45x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.31x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 10.7 ms: 1.01x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 111 us: 4.69x faster                                                   |
| generators                 | 74.9 ms                                                | 29.2 ms: 2.56x faster                                                  |
| asyncio_tcp                | 875 ms                                                 | 484 ms: 1.81x faster                                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.79 sec: 1.74x faster                                                 |
| comprehensions             | 23.6 us                                                | 16.2 us: 1.46x faster                                                  |
| json_dumps                 | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                  |
| deltablue                  | 3.92 ms                                                | 3.13 ms: 1.25x faster                                                  |
| coroutines                 | 27.0 ms                                                | 22.0 ms: 1.23x faster                                                  |
| chaos                      | 71.9 ms                                                | 58.5 ms: 1.23x faster                                                  |
| async_tree_none            | 528 ms                                                 | 433 ms: 1.22x faster                                                   |
| raytrace                   | 309 ms                                                 | 257 ms: 1.20x faster                                                   |
| richards_super             | 61.9 ms                                                | 52.5 ms: 1.18x faster                                                  |
| sqlglot_parse              | 1.43 ms                                                | 1.24 ms: 1.15x faster                                                  |
| hexiom                     | 6.89 ms                                                | 5.99 ms: 1.15x faster                                                  |
| async_tree_memoization     | 639 ms                                                 | 556 ms: 1.15x faster                                                   |
| unpickle_pure_python       | 242 us                                                 | 211 us: 1.15x faster                                                   |
| sympy_sum                  | 169 ms                                                 | 147 ms: 1.15x faster                                                   |
| logging_silent             | 111 ns                                                 | 97.0 ns: 1.15x faster                                                  |
| sqlglot_transpile          | 1.75 ms                                                | 1.56 ms: 1.12x faster                                                  |
| sympy_str                  | 297 ms                                                 | 268 ms: 1.11x faster                                                   |
| deepcopy_memo              | 40.2 us                                                | 36.2 us: 1.11x faster                                                  |
| logging_simple             | 6.22 us                                                | 5.61 us: 1.11x faster                                                  |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.54 ms: 1.11x faster                                                  |
| pickle_pure_python         | 320 us                                                 | 289 us: 1.11x faster                                                   |
| logging_format             | 6.81 us                                                | 6.16 us: 1.11x faster                                                  |
| async_tree_none_tg         | 491 ms                                                 | 444 ms: 1.11x faster                                                   |
| mdp                        | 2.77 sec                                               | 2.52 sec: 1.10x faster                                                 |
| sympy_integrate            | 21.5 ms                                                | 19.5 ms: 1.10x faster                                                  |
| async_tree_memoization_tg  | 626 ms                                                 | 570 ms: 1.10x faster                                                   |
| nqueens                    | 87.9 ms                                                | 80.0 ms: 1.10x faster                                                  |
| go                         | 149 ms                                                 | 135 ms: 1.10x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.17 sec: 1.10x faster                                                 |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                                 |
| crypto_pyaes               | 76.7 ms                                                | 70.5 ms: 1.09x faster                                                  |
| regex_compile              | 141 ms                                                 | 130 ms: 1.08x faster                                                   |
| deepcopy                   | 365 us                                                 | 337 us: 1.08x faster                                                   |
| nbody                      | 96.0 ms                                                | 88.7 ms: 1.08x faster                                                  |
| sympy_expand               | 484 ms                                                 | 449 ms: 1.08x faster                                                   |
| deepcopy_reduce            | 3.22 us                                                | 2.98 us: 1.08x faster                                                  |
| tomli_loads                | 2.30 sec                                               | 2.14 sec: 1.08x faster                                                 |
| richards                   | 49.8 ms                                                | 46.3 ms: 1.07x faster                                                  |
| scimark_monte_carlo        | 70.7 ms                                                | 66.0 ms: 1.07x faster                                                  |
| sqlglot_normalize          | 113 ms                                                 | 105 ms: 1.07x faster                                                   |
| pprint_pformat             | 1.55 sec                                               | 1.46 sec: 1.07x faster                                                 |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 703 ms: 1.07x faster                                                   |
| fannkuch                   | 405 ms                                                 | 381 ms: 1.06x faster                                                   |
| json_loads                 | 29.2 us                                                | 27.4 us: 1.06x faster                                                  |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 719 ms: 1.06x faster                                                   |
| json                       | 5.24 ms                                                | 4.98 ms: 1.05x faster                                                  |
| unpickle_list              | 5.21 us                                                | 4.98 us: 1.05x faster                                                  |
| gc_traversal               | 4.01 ms                                                | 3.83 ms: 1.05x faster                                                  |
| xml_etree_parse            | 164 ms                                                 | 157 ms: 1.05x faster                                                   |
| sqlglot_optimize           | 55.3 ms                                                | 53.0 ms: 1.04x faster                                                  |
| pprint_safe_repr           | 747 ms                                                 | 720 ms: 1.04x faster                                                   |
| tornado_http               | 98.1 ms                                                | 94.5 ms: 1.04x faster                                                  |
| scimark_lu                 | 116 ms                                                 | 112 ms: 1.03x faster                                                   |
| pidigits                   | 194 ms                                                 | 188 ms: 1.03x faster                                                   |
| docutils                   | 2.66 sec                                               | 2.58 sec: 1.03x faster                                                 |
| pycparser                  | 1.19 sec                                               | 1.15 sec: 1.03x faster                                                 |
| xml_etree_iterparse        | 108 ms                                                 | 105 ms: 1.03x faster                                                   |
| bench_thread_pool          | 834 us                                                 | 813 us: 1.03x faster                                                   |
| pathlib                    | 18.5 ms                                                | 18.1 ms: 1.03x faster                                                  |
| meteor_contest             | 109 ms                                                 | 107 ms: 1.02x faster                                                   |
| 2to3                       | 264 ms                                                 | 263 ms: 1.01x faster                                                   |
| regex_effbot               | 3.51 ms                                                | 3.49 ms: 1.00x faster                                                  |
| mako                       | 10.7 ms                                                | 10.7 ms: 1.01x slower                                                  |
| scimark_sor                | 121 ms                                                 | 122 ms: 1.01x slower                                                   |
| dulwich_log                | 64.6 ms                                                | 65.2 ms: 1.01x slower                                                  |
| float                      | 78.9 ms                                                | 80.1 ms: 1.01x slower                                                  |
| xml_etree_process          | 56.9 ms                                                | 57.9 ms: 1.02x slower                                                  |
| scimark_fft                | 345 ms                                                 | 352 ms: 1.02x slower                                                   |
| pickle_dict                | 34.6 us                                                | 35.8 us: 1.03x slower                                                  |
| create_gc_cycles           | 1.43 ms                                                | 1.49 ms: 1.04x slower                                                  |
| xml_etree_generate         | 81.1 ms                                                | 84.3 ms: 1.04x slower                                                  |
| regex_dna                  | 205 ms                                                 | 214 ms: 1.04x slower                                                   |
| pyflate                    | 434 ms                                                 | 458 ms: 1.06x slower                                                   |
| regex_v8                   | 22.9 ms                                                | 24.6 ms: 1.07x slower                                                  |
| unpickle                   | 13.8 us                                                | 14.9 us: 1.08x slower                                                  |
| sqlite_synth               | 2.57 us                                                | 2.81 us: 1.09x slower                                                  |
| pickle                     | 11.0 us                                                | 12.1 us: 1.10x slower                                                  |
| pickle_list                | 4.59 us                                                | 5.21 us: 1.14x slower                                                  |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                  |
| coverage                   | 78.8 ms                                                | 94.4 ms: 1.20x slower                                                  |
| async_generators           | 374 ms                                                 | 449 ms: 1.20x slower                                                   |
| telco                      | 6.86 ms                                                | 8.34 ms: 1.22x slower                                                  |
| mypy2                      | 686 ms                                                 | 843 ms: 1.23x slower                                                   |
| unpack_sequence            | 43.5 ns                                                | 55.0 ns: 1.27x slower                                                  |
| python_startup_no_site     | 6.01 ms                                                | 8.73 ms: 1.45x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                           |

Benchmark hidden because not significant (4): chameleon, bench_mp_pool, asyncio_websockets, spectral_norm
Ignored benchmarks (13) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.04x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: 0.99x