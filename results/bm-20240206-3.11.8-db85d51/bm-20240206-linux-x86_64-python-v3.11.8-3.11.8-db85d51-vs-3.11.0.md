
# Results vs. 3.11.0

- fork: python
- ref: v3.11.8
- machine: linux-x86_64
- commit hash: db85d51
- commit date: 2024-02-06
- overall geometric mean: 1.01x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-linux-x86_64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 259 ms: 1.02x faster                                   |
| chameleon      | 6.70 ms                                                | 6.92 ms: 1.03x slower                                  |
| docutils       | 2.66 sec                                               | 2.59 sec: 1.03x faster                                 |
| tornado_http   | 98.1 ms                                                | 96.1 ms: 1.02x faster                                  |
| Geometric mean | (ref)                                                  | 1.01x faster                                           |

Benchmark hidden because not significant (1): html5lib

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-linux-x86_64-python-v3.11.8-3.11.8-db85d51 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_memoization_tg  | 626 ms                                                 | 608 ms: 1.03x faster                                   |
| async_tree_none_tg         | 491 ms                                                 | 477 ms: 1.03x faster                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 743 ms: 1.02x faster                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.28 sec: 1.01x faster                                 |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 744 ms: 1.01x faster                                   |
| async_tree_io              | 1.29 sec                                               | 1.30 sec: 1.01x slower                                 |
| async_tree_memoization     | 639 ms                                                 | 646 ms: 1.01x slower                                   |
| Geometric mean             | (ref)                                                  | 1.01x faster                                           |

Benchmark hidden because not significant (1): async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-linux-x86_64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| float          | 78.9 ms                                                | 77.8 ms: 1.02x faster                                  |
| pidigits       | 194 ms                                                 | 195 ms: 1.01x slower                                   |
| Geometric mean | (ref)                                                  | 1.00x faster                                           |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-linux-x86_64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 137 ms: 1.03x faster                                   |
| regex_effbot   | 3.51 ms                                                | 3.45 ms: 1.02x faster                                  |
| regex_v8       | 22.9 ms                                                | 22.8 ms: 1.00x faster                                  |
| regex_dna      | 205 ms                                                 | 208 ms: 1.02x slower                                   |
| Geometric mean | (ref)                                                  | 1.01x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-linux-x86_64-python-v3.11.8-3.11.8-db85d51 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| json_loads           | 29.2 us                                                | 26.2 us: 1.11x faster                                  |
| unpickle             | 13.8 us                                                | 13.4 us: 1.03x faster                                  |
| pickle_pure_python   | 320 us                                                 | 311 us: 1.03x faster                                   |
| unpickle_pure_python | 242 us                                                 | 235 us: 1.03x faster                                   |
| xml_etree_process    | 56.9 ms                                                | 56.1 ms: 1.01x faster                                  |
| xml_etree_generate   | 81.1 ms                                                | 80.3 ms: 1.01x faster                                  |
| unpickle_list        | 5.21 us                                                | 5.18 us: 1.01x faster                                  |
| xml_etree_iterparse  | 108 ms                                                 | 107 ms: 1.01x faster                                   |
| tomli_loads          | 2.30 sec                                               | 2.33 sec: 1.01x slower                                 |
| pickle_list          | 4.59 us                                                | 4.73 us: 1.03x slower                                  |
| pickle               | 11.0 us                                                | 11.3 us: 1.03x slower                                  |
| pickle_dict          | 34.6 us                                                | 35.8 us: 1.03x slower                                  |
| Geometric mean       | (ref)                                                  | 1.01x faster                                           |

Benchmark hidden because not significant (2): json_dumps, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-linux-x86_64-python-v3.11.8-3.11.8-db85d51 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup_no_site | 6.01 ms                                                | 6.00 ms: 1.00x faster                                  |
| python_startup         | 8.56 ms                                                | 8.56 ms: 1.00x faster                                  |
| Geometric mean         | (ref)                                                  | 1.00x faster                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-linux-x86_64-python-v3.11.8-3.11.8-db85d51 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| genshi_text     | 22.5 ms                                                | 22.2 ms: 1.02x faster                                  |
| django_template | 33.5 ms                                                | 33.0 ms: 1.02x faster                                  |
| genshi_xml      | 53.4 ms                                                | 52.8 ms: 1.01x faster                                  |
| mako            | 10.7 ms                                                | 10.8 ms: 1.02x slower                                  |
| Geometric mean  | (ref)                                                  | 1.01x faster                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-linux-x86_64-python-v3.11.8-3.11.8-db85d51 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| json_loads                 | 29.2 us                                                | 26.2 us: 1.11x faster                                  |
| logging_silent             | 111 ns                                                 | 102 ns: 1.09x faster                                   |
| json                       | 5.24 ms                                                | 4.84 ms: 1.08x faster                                  |
| richards                   | 49.8 ms                                                | 46.4 ms: 1.07x faster                                  |
| gc_traversal               | 4.01 ms                                                | 3.76 ms: 1.07x faster                                  |
| richards_super             | 61.9 ms                                                | 58.1 ms: 1.06x faster                                  |
| deltablue                  | 3.92 ms                                                | 3.72 ms: 1.05x faster                                  |
| deepcopy                   | 365 us                                                 | 349 us: 1.05x faster                                   |
| hexiom                     | 6.89 ms                                                | 6.58 ms: 1.05x faster                                  |
| comprehensions             | 23.6 us                                                | 22.6 us: 1.04x faster                                  |
| pycparser                  | 1.19 sec                                               | 1.14 sec: 1.04x faster                                 |
| go                         | 149 ms                                                 | 142 ms: 1.04x faster                                   |
| deepcopy_reduce            | 3.22 us                                                | 3.09 us: 1.04x faster                                  |
| async_generators           | 374 ms                                                 | 361 ms: 1.04x faster                                   |
| deepcopy_memo              | 40.2 us                                                | 38.8 us: 1.03x faster                                  |
| sympy_integrate            | 21.5 ms                                                | 20.8 ms: 1.03x faster                                  |
| raytrace                   | 309 ms                                                 | 299 ms: 1.03x faster                                   |
| unpickle                   | 13.8 us                                                | 13.4 us: 1.03x faster                                  |
| async_tree_memoization_tg  | 626 ms                                                 | 608 ms: 1.03x faster                                   |
| regex_compile              | 141 ms                                                 | 137 ms: 1.03x faster                                   |
| async_tree_none_tg         | 491 ms                                                 | 477 ms: 1.03x faster                                   |
| pickle_pure_python         | 320 us                                                 | 311 us: 1.03x faster                                   |
| pylint                     | 476 ms                                                 | 462 ms: 1.03x faster                                   |
| docutils                   | 2.66 sec                                               | 2.59 sec: 1.03x faster                                 |
| pyflate                    | 434 ms                                                 | 422 ms: 1.03x faster                                   |
| unpickle_pure_python       | 242 us                                                 | 235 us: 1.03x faster                                   |
| logging_format             | 6.81 us                                                | 6.63 us: 1.03x faster                                  |
| logging_simple             | 6.22 us                                                | 6.07 us: 1.02x faster                                  |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 743 ms: 1.02x faster                                   |
| pprint_pformat             | 1.55 sec                                               | 1.52 sec: 1.02x faster                                 |
| coroutines                 | 27.0 ms                                                | 26.4 ms: 1.02x faster                                  |
| sqlalchemy_imperative      | 18.3 ms                                                | 17.9 ms: 1.02x faster                                  |
| sqlglot_transpile          | 1.75 ms                                                | 1.71 ms: 1.02x faster                                  |
| gunicorn                   | 1.20 ms                                                | 1.17 ms: 1.02x faster                                  |
| sqlglot_parse              | 1.43 ms                                                | 1.40 ms: 1.02x faster                                  |
| meteor_contest             | 109 ms                                                 | 107 ms: 1.02x faster                                   |
| tornado_http               | 98.1 ms                                                | 96.1 ms: 1.02x faster                                  |
| 2to3                       | 264 ms                                                 | 259 ms: 1.02x faster                                   |
| aiohttp                    | 1.12 ms                                                | 1.09 ms: 1.02x faster                                  |
| djangocms                  | 33.5 us                                                | 32.9 us: 1.02x faster                                  |
| sympy_sum                  | 169 ms                                                 | 166 ms: 1.02x faster                                   |
| genshi_text                | 22.5 ms                                                | 22.2 ms: 1.02x faster                                  |
| regex_effbot               | 3.51 ms                                                | 3.45 ms: 1.02x faster                                  |
| sympy_str                  | 297 ms                                                 | 292 ms: 1.02x faster                                   |
| nqueens                    | 87.9 ms                                                | 86.5 ms: 1.02x faster                                  |
| django_template            | 33.5 ms                                                | 33.0 ms: 1.02x faster                                  |
| pprint_safe_repr           | 747 ms                                                 | 736 ms: 1.02x faster                                   |
| float                      | 78.9 ms                                                | 77.8 ms: 1.02x faster                                  |
| sqlglot_optimize           | 55.3 ms                                                | 54.5 ms: 1.01x faster                                  |
| xml_etree_process          | 56.9 ms                                                | 56.1 ms: 1.01x faster                                  |
| fannkuch                   | 405 ms                                                 | 400 ms: 1.01x faster                                   |
| sqlglot_normalize          | 113 ms                                                 | 111 ms: 1.01x faster                                   |
| bench_thread_pool          | 834 us                                                 | 824 us: 1.01x faster                                   |
| dask                       | 365 ms                                                 | 361 ms: 1.01x faster                                   |
| genshi_xml                 | 53.4 ms                                                | 52.8 ms: 1.01x faster                                  |
| mypy2                      | 686 ms                                                 | 678 ms: 1.01x faster                                   |
| chaos                      | 71.9 ms                                                | 71.1 ms: 1.01x faster                                  |
| typing_runtime_protocols   | 520 us                                                 | 514 us: 1.01x faster                                   |
| scimark_lu                 | 116 ms                                                 | 115 ms: 1.01x faster                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.28 sec: 1.01x faster                                 |
| xml_etree_generate         | 81.1 ms                                                | 80.3 ms: 1.01x faster                                  |
| crypto_pyaes               | 76.7 ms                                                | 76.0 ms: 1.01x faster                                  |
| scimark_sor                | 121 ms                                                 | 120 ms: 1.01x faster                                   |
| flaskblogging              | 7.28 ms                                                | 7.23 ms: 1.01x faster                                  |
| unpickle_list              | 5.21 us                                                | 5.18 us: 1.01x faster                                  |
| xml_etree_iterparse        | 108 ms                                                 | 107 ms: 1.01x faster                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 744 ms: 1.01x faster                                   |
| pathlib                    | 18.5 ms                                                | 18.4 ms: 1.01x faster                                  |
| dulwich_log                | 64.6 ms                                                | 64.3 ms: 1.00x faster                                  |
| regex_v8                   | 22.9 ms                                                | 22.8 ms: 1.00x faster                                  |
| python_startup_no_site     | 6.01 ms                                                | 6.00 ms: 1.00x faster                                  |
| python_startup             | 8.56 ms                                                | 8.56 ms: 1.00x faster                                  |
| asyncio_tcp_ssl            | 3.11 sec                                               | 3.12 sec: 1.00x slower                                 |
| create_gc_cycles           | 1.43 ms                                                | 1.44 ms: 1.01x slower                                  |
| pidigits                   | 194 ms                                                 | 195 ms: 1.01x slower                                   |
| sympy_expand               | 484 ms                                                 | 488 ms: 1.01x slower                                   |
| scimark_fft                | 345 ms                                                 | 349 ms: 1.01x slower                                   |
| tomli_loads                | 2.30 sec                                               | 2.33 sec: 1.01x slower                                 |
| async_tree_io              | 1.29 sec                                               | 1.30 sec: 1.01x slower                                 |
| async_tree_memoization     | 639 ms                                                 | 646 ms: 1.01x slower                                   |
| generators                 | 74.9 ms                                                | 75.9 ms: 1.01x slower                                  |
| mako                       | 10.7 ms                                                | 10.8 ms: 1.02x slower                                  |
| mdp                        | 2.77 sec                                               | 2.82 sec: 1.02x slower                                 |
| regex_dna                  | 205 ms                                                 | 208 ms: 1.02x slower                                   |
| pickle_list                | 4.59 us                                                | 4.73 us: 1.03x slower                                  |
| pickle                     | 11.0 us                                                | 11.3 us: 1.03x slower                                  |
| chameleon                  | 6.70 ms                                                | 6.92 ms: 1.03x slower                                  |
| pickle_dict                | 34.6 us                                                | 35.8 us: 1.03x slower                                  |
| asyncio_tcp                | 875 ms                                                 | 909 ms: 1.04x slower                                   |
| unpack_sequence            | 43.5 ns                                                | 46.5 ns: 1.07x slower                                  |
| Geometric mean             | (ref)                                                  | 1.01x faster                                           |

Benchmark hidden because not significant (15): html5lib, nbody, scimark_sparse_mat_mult, telco, spectral_norm, sqlalchemy_declarative, json_dumps, thrift, scimark_monte_carlo, bench_mp_pool, asyncio_websockets, async_tree_none, coverage, xml_etree_parse, sqlite_synth


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x