# Results vs. 3.11.0

- fork: mdboom
- ref: estimate_too_short
- machine: linux-x86_64
- commit hash: c3a9b5a
- commit date: 2024-03-14
- overall geometric mean: 1.03x faster
- HPT reliability: 89.92%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.24x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 280 ms: 1.06x slower                                                 |
| chameleon      | 6.70 ms                                                | 7.00 ms: 1.05x slower                                                |
| docutils       | 2.66 sec                                               | 2.72 sec: 1.02x slower                                               |
| html5lib       | 64.8 ms                                                | 67.6 ms: 1.04x slower                                                |
| Geometric mean | (ref)                                                  | 1.03x slower                                                         |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 445 ms: 1.19x faster                                                 |
| async_tree_memoization     | 639 ms                                                 | 574 ms: 1.11x faster                                                 |
| async_tree_none_tg         | 491 ms                                                 | 458 ms: 1.07x faster                                                 |
| async_tree_io              | 1.29 sec                                               | 1.20 sec: 1.07x faster                                               |
| async_tree_memoization_tg  | 626 ms                                                 | 587 ms: 1.07x faster                                                 |
| async_tree_io_tg           | 1.29 sec                                               | 1.23 sec: 1.06x faster                                               |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 724 ms: 1.03x faster                                                 |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 740 ms: 1.03x faster                                                 |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 93.1 ms: 1.03x faster                                                |
| pidigits       | 194 ms                                                 | 189 ms: 1.03x faster                                                 |
| float          | 78.9 ms                                                | 81.3 ms: 1.03x slower                                                |
| Geometric mean | (ref)                                                  | 1.01x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 142 ms: 1.01x slower                                                 |
| regex_effbot   | 3.51 ms                                                | 3.83 ms: 1.09x slower                                                |
| regex_dna      | 205 ms                                                 | 224 ms: 1.10x slower                                                 |
| regex_v8       | 22.9 ms                                                | 25.7 ms: 1.12x slower                                                |
| Geometric mean | (ref)                                                  | 1.08x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                |
| tomli_loads          | 2.30 sec                                               | 2.05 sec: 1.12x faster                                               |
| unpickle_list        | 5.21 us                                                | 4.88 us: 1.07x faster                                                |
| pickle_pure_python   | 320 us                                                 | 304 us: 1.05x faster                                                 |
| json_loads           | 29.2 us                                                | 28.1 us: 1.04x faster                                                |
| xml_etree_parse      | 164 ms                                                 | 159 ms: 1.03x faster                                                 |
| unpickle_pure_python | 242 us                                                 | 237 us: 1.02x faster                                                 |
| xml_etree_iterparse  | 108 ms                                                 | 107 ms: 1.01x faster                                                 |
| pickle_dict          | 34.6 us                                                | 34.6 us: 1.00x slower                                                |
| xml_etree_process    | 56.9 ms                                                | 59.7 ms: 1.05x slower                                                |
| pickle               | 11.0 us                                                | 11.6 us: 1.06x slower                                                |
| xml_etree_generate   | 81.1 ms                                                | 86.9 ms: 1.07x slower                                                |
| unpickle             | 13.8 us                                                | 15.0 us: 1.08x slower                                                |
| pickle_list          | 4.59 us                                                | 5.10 us: 1.11x slower                                                |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                         |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 12.6 ms: 1.47x slower                                                |
| python_startup_no_site | 6.01 ms                                                | 11.2 ms: 1.86x slower                                                |
| Geometric mean         | (ref)                                                  | 1.65x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|-----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| django_template | 33.5 ms                                                | 33.9 ms: 1.01x slower                                                |
| mako            | 10.7 ms                                                | 10.9 ms: 1.02x slower                                                |
| genshi_text     | 22.5 ms                                                | 23.7 ms: 1.05x slower                                                |
| Geometric mean  | (ref)                                                  | 1.02x slower                                                         |

Benchmark hidden because not significant (1): genshi_xml

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 109 us: 4.76x faster                                                 |
| generators                 | 74.9 ms                                                | 29.6 ms: 2.53x faster                                                |
| asyncio_tcp                | 875 ms                                                 | 510 ms: 1.72x faster                                                 |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.85 sec: 1.68x faster                                               |
| pylint                     | 476 ms                                                 | 321 ms: 1.48x faster                                                 |
| comprehensions             | 23.6 us                                                | 17.2 us: 1.37x faster                                                |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                |
| coroutines                 | 27.0 ms                                                | 22.0 ms: 1.23x faster                                                |
| richards_super             | 61.9 ms                                                | 52.0 ms: 1.19x faster                                                |
| async_tree_none            | 528 ms                                                 | 445 ms: 1.19x faster                                                 |
| chaos                      | 71.9 ms                                                | 63.6 ms: 1.13x faster                                                |
| tomli_loads                | 2.30 sec                                               | 2.05 sec: 1.12x faster                                               |
| gc_traversal               | 4.01 ms                                                | 3.59 ms: 1.12x faster                                                |
| async_tree_memoization     | 639 ms                                                 | 574 ms: 1.11x faster                                                 |
| sqlglot_parse              | 1.43 ms                                                | 1.31 ms: 1.09x faster                                                |
| logging_silent             | 111 ns                                                 | 102 ns: 1.09x faster                                                 |
| richards                   | 49.8 ms                                                | 45.9 ms: 1.08x faster                                                |
| raytrace                   | 309 ms                                                 | 286 ms: 1.08x faster                                                 |
| nqueens                    | 87.9 ms                                                | 81.8 ms: 1.07x faster                                                |
| async_tree_none_tg         | 491 ms                                                 | 458 ms: 1.07x faster                                                 |
| djangocms                  | 33.5 us                                                | 31.3 us: 1.07x faster                                                |
| deepcopy_reduce            | 3.22 us                                                | 3.01 us: 1.07x faster                                                |
| deepcopy_memo              | 40.2 us                                                | 37.5 us: 1.07x faster                                                |
| deepcopy                   | 365 us                                                 | 342 us: 1.07x faster                                                 |
| async_tree_io              | 1.29 sec                                               | 1.20 sec: 1.07x faster                                               |
| unpickle_list              | 5.21 us                                                | 4.88 us: 1.07x faster                                                |
| async_tree_memoization_tg  | 626 ms                                                 | 587 ms: 1.07x faster                                                 |
| sqlglot_transpile          | 1.75 ms                                                | 1.64 ms: 1.07x faster                                                |
| logging_simple             | 6.22 us                                                | 5.86 us: 1.06x faster                                                |
| async_tree_io_tg           | 1.29 sec                                               | 1.23 sec: 1.06x faster                                               |
| pickle_pure_python         | 320 us                                                 | 304 us: 1.05x faster                                                 |
| sqlglot_normalize          | 113 ms                                                 | 107 ms: 1.05x faster                                                 |
| sympy_sum                  | 169 ms                                                 | 160 ms: 1.05x faster                                                 |
| sympy_str                  | 297 ms                                                 | 283 ms: 1.05x faster                                                 |
| deltablue                  | 3.92 ms                                                | 3.75 ms: 1.05x faster                                                |
| logging_format             | 6.81 us                                                | 6.53 us: 1.04x faster                                                |
| json_loads                 | 29.2 us                                                | 28.1 us: 1.04x faster                                                |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 724 ms: 1.03x faster                                                 |
| xml_etree_parse            | 164 ms                                                 | 159 ms: 1.03x faster                                                 |
| nbody                      | 96.0 ms                                                | 93.1 ms: 1.03x faster                                                |
| sympy_integrate            | 21.5 ms                                                | 20.8 ms: 1.03x faster                                                |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 740 ms: 1.03x faster                                                 |
| pidigits                   | 194 ms                                                 | 189 ms: 1.03x faster                                                 |
| hexiom                     | 6.89 ms                                                | 6.74 ms: 1.02x faster                                                |
| unpickle_pure_python       | 242 us                                                 | 237 us: 1.02x faster                                                 |
| json                       | 5.24 ms                                                | 5.14 ms: 1.02x faster                                                |
| crypto_pyaes               | 76.7 ms                                                | 75.5 ms: 1.02x faster                                                |
| pprint_pformat             | 1.55 sec                                               | 1.53 sec: 1.01x faster                                               |
| mdp                        | 2.77 sec                                               | 2.74 sec: 1.01x faster                                               |
| xml_etree_iterparse        | 108 ms                                                 | 107 ms: 1.01x faster                                                 |
| fannkuch                   | 405 ms                                                 | 401 ms: 1.01x faster                                                 |
| pathlib                    | 18.5 ms                                                | 18.4 ms: 1.01x faster                                                |
| pickle_dict                | 34.6 us                                                | 34.6 us: 1.00x slower                                                |
| regex_compile              | 141 ms                                                 | 142 ms: 1.01x slower                                                 |
| django_template            | 33.5 ms                                                | 33.9 ms: 1.01x slower                                                |
| meteor_contest             | 109 ms                                                 | 110 ms: 1.01x slower                                                 |
| sqlglot_optimize           | 55.3 ms                                                | 56.2 ms: 1.02x slower                                                |
| thrift                     | 784 us                                                 | 798 us: 1.02x slower                                                 |
| mako                       | 10.7 ms                                                | 10.9 ms: 1.02x slower                                                |
| docutils                   | 2.66 sec                                               | 2.72 sec: 1.02x slower                                               |
| dask                       | 365 ms                                                 | 373 ms: 1.02x slower                                                 |
| pycparser                  | 1.19 sec                                               | 1.21 sec: 1.02x slower                                               |
| asyncio_websockets         | 550 ms                                                 | 563 ms: 1.02x slower                                                 |
| bench_thread_pool          | 834 us                                                 | 857 us: 1.03x slower                                                 |
| float                      | 78.9 ms                                                | 81.3 ms: 1.03x slower                                                |
| spectral_norm              | 108 ms                                                 | 111 ms: 1.03x slower                                                 |
| html5lib                   | 64.8 ms                                                | 67.6 ms: 1.04x slower                                                |
| chameleon                  | 6.70 ms                                                | 7.00 ms: 1.05x slower                                                |
| go                         | 149 ms                                                 | 156 ms: 1.05x slower                                                 |
| xml_etree_process          | 56.9 ms                                                | 59.7 ms: 1.05x slower                                                |
| genshi_text                | 22.5 ms                                                | 23.7 ms: 1.05x slower                                                |
| pickle                     | 11.0 us                                                | 11.6 us: 1.06x slower                                                |
| 2to3                       | 264 ms                                                 | 280 ms: 1.06x slower                                                 |
| create_gc_cycles           | 1.43 ms                                                | 1.52 ms: 1.06x slower                                                |
| xml_etree_generate         | 81.1 ms                                                | 86.9 ms: 1.07x slower                                                |
| dulwich_log                | 64.6 ms                                                | 69.4 ms: 1.07x slower                                                |
| aiohttp                    | 1.12 ms                                                | 1.20 ms: 1.07x slower                                                |
| gunicorn                   | 1.20 ms                                                | 1.29 ms: 1.07x slower                                                |
| unpickle                   | 13.8 us                                                | 15.0 us: 1.08x slower                                                |
| regex_effbot               | 3.51 ms                                                | 3.83 ms: 1.09x slower                                                |
| regex_dna                  | 205 ms                                                 | 224 ms: 1.10x slower                                                 |
| bench_mp_pool              | 24.0 ms                                                | 26.4 ms: 1.10x slower                                                |
| pickle_list                | 4.59 us                                                | 5.10 us: 1.11x slower                                                |
| scimark_lu                 | 116 ms                                                 | 130 ms: 1.12x slower                                                 |
| regex_v8                   | 22.9 ms                                                | 25.7 ms: 1.12x slower                                                |
| sqlite_synth               | 2.57 us                                                | 2.89 us: 1.12x slower                                                |
| scimark_sor                | 121 ms                                                 | 138 ms: 1.13x slower                                                 |
| pyflate                    | 434 ms                                                 | 492 ms: 1.13x slower                                                 |
| telco                      | 6.86 ms                                                | 8.33 ms: 1.22x slower                                                |
| coverage                   | 78.8 ms                                                | 96.0 ms: 1.22x slower                                                |
| async_generators           | 374 ms                                                 | 469 ms: 1.25x slower                                                 |
| mypy2                      | 686 ms                                                 | 897 ms: 1.31x slower                                                 |
| python_startup             | 8.56 ms                                                | 12.6 ms: 1.47x slower                                                |
| python_startup_no_site     | 6.01 ms                                                | 11.2 ms: 1.86x slower                                                |
| unpack_sequence            | 43.5 ns                                                | 92.9 ns: 2.14x slower                                                |
| Geometric mean             | (ref)                                                  | 1.03x faster                                                         |

Benchmark hidden because not significant (7): scimark_sparse_mat_mult, sympy_expand, scimark_monte_carlo, pprint_safe_repr, genshi_xml, scimark_fft, tornado_http
Ignored benchmarks (3) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 89.92% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.24x