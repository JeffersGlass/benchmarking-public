
# Results vs. 3.11.0

- fork: python
- ref: a2bb8ad14409c7ecb8de
- machine: linux-x86_64
- commit hash: a2bb8ad
- commit date: 2024-02-20
- overall geometric mean: 1.02x slower \*
- HPT reliability: 99.87%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240220-linux-x86_64-python-a2bb8ad14409c7ecb8de-3.13.0a4+-a2bb8ad |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 292 ms: 1.11x slower                                                   |
| chameleon      | 6.70 ms                                                | 7.23 ms: 1.08x slower                                                  |
| docutils       | 2.66 sec                                               | 2.81 sec: 1.06x slower                                                 |
| tornado_http   | 98.1 ms                                                | 99.1 ms: 1.01x slower                                                  |
| Geometric mean | (ref)                                                  | 1.06x slower                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240220-linux-x86_64-python-a2bb8ad14409c7ecb8de-3.13.0a4+-a2bb8ad |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 451 ms: 1.17x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 579 ms: 1.10x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 459 ms: 1.07x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.06x faster                                                 |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 594 ms: 1.05x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 736 ms: 1.03x faster                                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 727 ms: 1.03x faster                                                   |
| Geometric mean             | (ref)                                                  | 1.07x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240220-linux-x86_64-python-a2bb8ad14409c7ecb8de-3.13.0a4+-a2bb8ad |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 189 ms: 1.03x faster                                                   |
| float          | 78.9 ms                                                | 90.8 ms: 1.15x slower                                                  |
| nbody          | 96.0 ms                                                | 114 ms: 1.19x slower                                                   |
| Geometric mean | (ref)                                                  | 1.10x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240220-linux-x86_64-python-a2bb8ad14409c7ecb8de-3.13.0a4+-a2bb8ad |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.85 ms: 1.10x slower                                                  |
| regex_dna      | 205 ms                                                 | 230 ms: 1.12x slower                                                   |
| regex_v8       | 22.9 ms                                                | 25.9 ms: 1.13x slower                                                  |
| regex_compile  | 141 ms                                                 | 172 ms: 1.22x slower                                                   |
| Geometric mean | (ref)                                                  | 1.14x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240220-linux-x86_64-python-a2bb8ad14409c7ecb8de-3.13.0a4+-a2bb8ad |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.6 ms: 1.26x faster                                                  |
| pickle_pure_python   | 320 us                                                 | 301 us: 1.06x faster                                                   |
| json_loads           | 29.2 us                                                | 27.5 us: 1.06x faster                                                  |
| unpickle_list        | 5.21 us                                                | 4.96 us: 1.05x faster                                                  |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                                   |
| xml_etree_iterparse  | 108 ms                                                 | 111 ms: 1.03x slower                                                   |
| pickle               | 11.0 us                                                | 11.7 us: 1.06x slower                                                  |
| xml_etree_process    | 56.9 ms                                                | 60.9 ms: 1.07x slower                                                  |
| xml_etree_generate   | 81.1 ms                                                | 89.1 ms: 1.10x slower                                                  |
| unpickle_pure_python | 242 us                                                 | 271 us: 1.12x slower                                                   |
| unpickle             | 13.8 us                                                | 15.6 us: 1.13x slower                                                  |
| pickle_list          | 4.59 us                                                | 5.23 us: 1.14x slower                                                  |
| tomli_loads          | 2.30 sec                                               | 2.63 sec: 1.14x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.02x slower                                                           |

Benchmark hidden because not significant (1): pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240220-linux-x86_64-python-a2bb8ad14409c7ecb8de-3.13.0a4+-a2bb8ad |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                  |
| python_startup_no_site | 6.01 ms                                                | 8.85 ms: 1.47x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.33x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240220-linux-x86_64-python-a2bb8ad14409c7ecb8de-3.13.0a4+-a2bb8ad |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 13.0 ms: 1.22x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240220-linux-x86_64-python-a2bb8ad14409c7ecb8de-3.13.0a4+-a2bb8ad |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 113 us: 4.58x faster                                                   |
| generators                 | 74.9 ms                                                | 29.7 ms: 2.52x faster                                                  |
| asyncio_tcp                | 875 ms                                                 | 493 ms: 1.78x faster                                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.81 sec: 1.72x faster                                                 |
| json_dumps                 | 13.3 ms                                                | 10.6 ms: 1.26x faster                                                  |
| async_tree_none            | 528 ms                                                 | 451 ms: 1.17x faster                                                   |
| coroutines                 | 27.0 ms                                                | 23.1 ms: 1.17x faster                                                  |
| comprehensions             | 23.6 us                                                | 20.7 us: 1.14x faster                                                  |
| async_tree_memoization     | 639 ms                                                 | 579 ms: 1.10x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 459 ms: 1.07x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.06x faster                                                 |
| pickle_pure_python         | 320 us                                                 | 301 us: 1.06x faster                                                   |
| json_loads                 | 29.2 us                                                | 27.5 us: 1.06x faster                                                  |
| logging_silent             | 111 ns                                                 | 105 ns: 1.06x faster                                                   |
| deltablue                  | 3.92 ms                                                | 3.70 ms: 1.06x faster                                                  |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 594 ms: 1.05x faster                                                   |
| unpickle_list              | 5.21 us                                                | 4.96 us: 1.05x faster                                                  |
| xml_etree_parse            | 164 ms                                                 | 158 ms: 1.04x faster                                                   |
| sympy_sum                  | 169 ms                                                 | 163 ms: 1.04x faster                                                   |
| gc_traversal               | 4.01 ms                                                | 3.87 ms: 1.03x faster                                                  |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 736 ms: 1.03x faster                                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 727 ms: 1.03x faster                                                   |
| pidigits                   | 194 ms                                                 | 189 ms: 1.03x faster                                                   |
| deepcopy                   | 365 us                                                 | 356 us: 1.03x faster                                                   |
| deepcopy_reduce            | 3.22 us                                                | 3.14 us: 1.02x faster                                                  |
| json                       | 5.24 ms                                                | 5.14 ms: 1.02x faster                                                  |
| sympy_integrate            | 21.5 ms                                                | 21.1 ms: 1.02x faster                                                  |
| sqlglot_parse              | 1.43 ms                                                | 1.41 ms: 1.02x faster                                                  |
| logging_simple             | 6.22 us                                                | 6.16 us: 1.01x faster                                                  |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                                   |
| sqlglot_normalize          | 113 ms                                                 | 113 ms: 1.01x slower                                                   |
| tornado_http               | 98.1 ms                                                | 99.1 ms: 1.01x slower                                                  |
| pathlib                    | 18.5 ms                                                | 18.9 ms: 1.02x slower                                                  |
| deepcopy_memo              | 40.2 us                                                | 41.0 us: 1.02x slower                                                  |
| mdp                        | 2.77 sec                                               | 2.84 sec: 1.02x slower                                                 |
| bench_thread_pool          | 834 us                                                 | 856 us: 1.03x slower                                                   |
| xml_etree_iterparse        | 108 ms                                                 | 111 ms: 1.03x slower                                                   |
| logging_format             | 6.81 us                                                | 7.00 us: 1.03x slower                                                  |
| chaos                      | 71.9 ms                                                | 74.4 ms: 1.04x slower                                                  |
| sympy_expand               | 484 ms                                                 | 502 ms: 1.04x slower                                                   |
| richards_super             | 61.9 ms                                                | 64.2 ms: 1.04x slower                                                  |
| meteor_contest             | 109 ms                                                 | 115 ms: 1.05x slower                                                   |
| docutils                   | 2.66 sec                                               | 2.81 sec: 1.06x slower                                                 |
| create_gc_cycles           | 1.43 ms                                                | 1.52 ms: 1.06x slower                                                  |
| pickle                     | 11.0 us                                                | 11.7 us: 1.06x slower                                                  |
| xml_etree_process          | 56.9 ms                                                | 60.9 ms: 1.07x slower                                                  |
| chameleon                  | 6.70 ms                                                | 7.23 ms: 1.08x slower                                                  |
| sqlglot_optimize           | 55.3 ms                                                | 60.2 ms: 1.09x slower                                                  |
| crypto_pyaes               | 76.7 ms                                                | 83.8 ms: 1.09x slower                                                  |
| regex_effbot               | 3.51 ms                                                | 3.85 ms: 1.10x slower                                                  |
| xml_etree_generate         | 81.1 ms                                                | 89.1 ms: 1.10x slower                                                  |
| raytrace                   | 309 ms                                                 | 339 ms: 1.10x slower                                                   |
| 2to3                       | 264 ms                                                 | 292 ms: 1.11x slower                                                   |
| nqueens                    | 87.9 ms                                                | 97.8 ms: 1.11x slower                                                  |
| dulwich_log                | 64.6 ms                                                | 72.0 ms: 1.11x slower                                                  |
| pycparser                  | 1.19 sec                                               | 1.32 sec: 1.12x slower                                                 |
| sqlite_synth               | 2.57 us                                                | 2.88 us: 1.12x slower                                                  |
| unpickle_pure_python       | 242 us                                                 | 271 us: 1.12x slower                                                   |
| regex_dna                  | 205 ms                                                 | 230 ms: 1.12x slower                                                   |
| unpickle                   | 13.8 us                                                | 15.6 us: 1.13x slower                                                  |
| pprint_safe_repr           | 747 ms                                                 | 844 ms: 1.13x slower                                                   |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.68 ms: 1.13x slower                                                  |
| regex_v8                   | 22.9 ms                                                | 25.9 ms: 1.13x slower                                                  |
| pprint_pformat             | 1.55 sec                                               | 1.76 sec: 1.13x slower                                                 |
| pickle_list                | 4.59 us                                                | 5.23 us: 1.14x slower                                                  |
| tomli_loads                | 2.30 sec                                               | 2.63 sec: 1.14x slower                                                 |
| float                      | 78.9 ms                                                | 90.8 ms: 1.15x slower                                                  |
| fannkuch                   | 405 ms                                                 | 468 ms: 1.15x slower                                                   |
| richards                   | 49.8 ms                                                | 57.6 ms: 1.16x slower                                                  |
| scimark_sor                | 121 ms                                                 | 141 ms: 1.16x slower                                                   |
| go                         | 149 ms                                                 | 173 ms: 1.17x slower                                                   |
| nbody                      | 96.0 ms                                                | 114 ms: 1.19x slower                                                   |
| scimark_monte_carlo        | 70.7 ms                                                | 84.3 ms: 1.19x slower                                                  |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                  |
| regex_compile              | 141 ms                                                 | 172 ms: 1.22x slower                                                   |
| mako                       | 10.7 ms                                                | 13.0 ms: 1.22x slower                                                  |
| spectral_norm              | 108 ms                                                 | 132 ms: 1.22x slower                                                   |
| scimark_fft                | 345 ms                                                 | 424 ms: 1.23x slower                                                   |
| coverage                   | 78.8 ms                                                | 97.0 ms: 1.23x slower                                                  |
| async_generators           | 374 ms                                                 | 465 ms: 1.24x slower                                                   |
| telco                      | 6.86 ms                                                | 8.72 ms: 1.27x slower                                                  |
| unpack_sequence            | 43.5 ns                                                | 55.8 ns: 1.28x slower                                                  |
| hexiom                     | 6.89 ms                                                | 8.93 ms: 1.30x slower                                                  |
| pyflate                    | 434 ms                                                 | 565 ms: 1.30x slower                                                   |
| mypy2                      | 686 ms                                                 | 894 ms: 1.30x slower                                                   |
| scimark_lu                 | 116 ms                                                 | 154 ms: 1.32x slower                                                   |
| python_startup_no_site     | 6.01 ms                                                | 8.85 ms: 1.47x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.02x slower                                                           |

Benchmark hidden because not significant (5): sqlglot_transpile, sympy_str, pickle_dict, bench_mp_pool, dask
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.87% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x