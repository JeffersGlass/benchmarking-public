
# Results vs. 3.12.0

- fork: python
- ref: v3.11.8
- machine: linux-x86_64
- commit hash: db85d51
- commit date: 2024-02-06
- overall geometric mean: 1.01x slower \*
- HPT reliability: 93.55%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.95x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-linux-x86_64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 259 ms: 1.06x faster                                   |
| chameleon      | 7.41 ms                                                | 6.92 ms: 1.07x faster                                  |
| docutils       | 2.77 sec                                               | 2.59 sec: 1.07x faster                                 |
| tornado_http   | 103 ms                                                 | 96.1 ms: 1.07x faster                                  |
| Geometric mean | (ref)                                                  | 1.07x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-linux-x86_64-python-v3.11.8-3.11.8-db85d51 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 743 ms: 1.02x slower                                   |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 744 ms: 1.03x slower                                   |
| async_tree_memoization_tg  | 575 ms                                                 | 608 ms: 1.06x slower                                   |
| async_tree_none_tg         | 450 ms                                                 | 477 ms: 1.06x slower                                   |
| async_tree_io_tg           | 1.18 sec                                               | 1.28 sec: 1.08x slower                                 |
| async_tree_memoization     | 578 ms                                                 | 646 ms: 1.12x slower                                   |
| async_tree_none            | 472 ms                                                 | 529 ms: 1.12x slower                                   |
| async_tree_io              | 1.16 sec                                               | 1.30 sec: 1.13x slower                                 |
| Geometric mean             | (ref)                                                  | 1.08x slower                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-linux-x86_64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| float          | 84.7 ms                                                | 77.8 ms: 1.09x faster                                  |
| nbody          | 97.0 ms                                                | 95.5 ms: 1.02x faster                                  |
| pidigits       | 187 ms                                                 | 195 ms: 1.04x slower                                   |
| Geometric mean | (ref)                                                  | 1.02x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-linux-x86_64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 137 ms: 1.08x faster                                   |
| regex_effbot   | 3.61 ms                                                | 3.45 ms: 1.05x faster                                  |
| regex_dna      | 212 ms                                                 | 208 ms: 1.02x faster                                   |
| regex_v8       | 23.1 ms                                                | 22.8 ms: 1.02x faster                                  |
| Geometric mean | (ref)                                                  | 1.04x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-linux-x86_64-python-v3.11.8-3.11.8-db85d51 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| unpickle             | 15.9 us                                                | 13.4 us: 1.18x faster                                  |
| xml_etree_generate   | 89.2 ms                                                | 80.3 ms: 1.11x faster                                  |
| xml_etree_process    | 61.7 ms                                                | 56.1 ms: 1.10x faster                                  |
| json_loads           | 28.5 us                                                | 26.2 us: 1.09x faster                                  |
| pickle_list          | 5.08 us                                                | 4.73 us: 1.07x faster                                  |
| pickle_pure_python   | 324 us                                                 | 311 us: 1.04x faster                                   |
| pickle               | 11.6 us                                                | 11.3 us: 1.02x faster                                  |
| unpickle_list        | 5.29 us                                                | 5.18 us: 1.02x faster                                  |
| xml_etree_iterparse  | 107 ms                                                 | 107 ms: 1.00x slower                                   |
| pickle_dict          | 35.5 us                                                | 35.8 us: 1.01x slower                                  |
| unpickle_pure_python | 230 us                                                 | 235 us: 1.02x slower                                   |
| xml_etree_parse      | 159 ms                                                 | 165 ms: 1.03x slower                                   |
| json_dumps           | 10.4 ms                                                | 13.3 ms: 1.28x slower                                  |
| Geometric mean       | (ref)                                                  | 1.02x faster                                           |

Benchmark hidden because not significant (1): tomli_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-linux-x86_64-python-v3.11.8-3.11.8-db85d51 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup_no_site | 6.94 ms                                                | 6.00 ms: 1.16x faster                                  |
| python_startup         | 9.55 ms                                                | 8.56 ms: 1.12x faster                                  |
| Geometric mean         | (ref)                                                  | 1.14x faster                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-linux-x86_64-python-v3.11.8-3.11.8-db85d51 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako            | 11.9 ms                                                | 10.8 ms: 1.10x faster                                  |
| django_template | 34.6 ms                                                | 33.0 ms: 1.05x faster                                  |
| Geometric mean  | (ref)                                                  | 1.07x faster                                           |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-linux-x86_64-python-v3.11.8-3.11.8-db85d51 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_generators           | 463 ms                                                 | 361 ms: 1.28x faster                                   |
| mypy2                      | 830 ms                                                 | 678 ms: 1.23x faster                                   |
| unpickle                   | 15.9 us                                                | 13.4 us: 1.18x faster                                  |
| unpack_sequence            | 54.0 ns                                                | 46.5 ns: 1.16x faster                                  |
| python_startup_no_site     | 6.94 ms                                                | 6.00 ms: 1.16x faster                                  |
| pyflate                    | 482 ms                                                 | 422 ms: 1.14x faster                                   |
| python_startup             | 9.55 ms                                                | 8.56 ms: 1.12x faster                                  |
| xml_etree_generate         | 89.2 ms                                                | 80.3 ms: 1.11x faster                                  |
| xml_etree_process          | 61.7 ms                                                | 56.1 ms: 1.10x faster                                  |
| sqlite_synth               | 2.83 us                                                | 2.58 us: 1.10x faster                                  |
| mako                       | 11.9 ms                                                | 10.8 ms: 1.10x faster                                  |
| scimark_fft                | 382 ms                                                 | 349 ms: 1.10x faster                                   |
| logging_format             | 7.23 us                                                | 6.63 us: 1.09x faster                                  |
| float                      | 84.7 ms                                                | 77.8 ms: 1.09x faster                                  |
| json_loads                 | 28.5 us                                                | 26.2 us: 1.09x faster                                  |
| json                       | 5.26 ms                                                | 4.84 ms: 1.09x faster                                  |
| regex_compile              | 148 ms                                                 | 137 ms: 1.08x faster                                   |
| deepcopy_reduce            | 3.35 us                                                | 3.09 us: 1.08x faster                                  |
| crypto_pyaes               | 81.9 ms                                                | 76.0 ms: 1.08x faster                                  |
| pickle_list                | 5.08 us                                                | 4.73 us: 1.07x faster                                  |
| scimark_sor                | 129 ms                                                 | 120 ms: 1.07x faster                                   |
| chameleon                  | 7.41 ms                                                | 6.92 ms: 1.07x faster                                  |
| docutils                   | 2.77 sec                                               | 2.59 sec: 1.07x faster                                 |
| tornado_http               | 103 ms                                                 | 96.1 ms: 1.07x faster                                  |
| dulwich_log                | 68.5 ms                                                | 64.3 ms: 1.07x faster                                  |
| spectral_norm              | 115 ms                                                 | 108 ms: 1.07x faster                                   |
| deepcopy                   | 371 us                                                 | 349 us: 1.06x faster                                   |
| logging_simple             | 6.46 us                                                | 6.07 us: 1.06x faster                                  |
| scimark_monte_carlo        | 75.1 ms                                                | 70.6 ms: 1.06x faster                                  |
| gunicorn                   | 1.24 ms                                                | 1.17 ms: 1.06x faster                                  |
| 2to3                       | 274 ms                                                 | 259 ms: 1.06x faster                                   |
| pprint_safe_repr           | 776 ms                                                 | 736 ms: 1.05x faster                                   |
| meteor_contest             | 112 ms                                                 | 107 ms: 1.05x faster                                   |
| pathlib                    | 19.3 ms                                                | 18.4 ms: 1.05x faster                                  |
| aiohttp                    | 1.15 ms                                                | 1.09 ms: 1.05x faster                                  |
| deepcopy_memo              | 40.7 us                                                | 38.8 us: 1.05x faster                                  |
| sqlalchemy_declarative     | 147 ms                                                 | 140 ms: 1.05x faster                                   |
| django_template            | 34.6 ms                                                | 33.0 ms: 1.05x faster                                  |
| regex_effbot               | 3.61 ms                                                | 3.45 ms: 1.05x faster                                  |
| fannkuch                   | 417 ms                                                 | 400 ms: 1.04x faster                                   |
| raytrace                   | 312 ms                                                 | 299 ms: 1.04x faster                                   |
| sqlalchemy_imperative      | 18.7 ms                                                | 17.9 ms: 1.04x faster                                  |
| pickle_pure_python         | 324 us                                                 | 311 us: 1.04x faster                                   |
| telco                      | 7.10 ms                                                | 6.83 ms: 1.04x faster                                  |
| pycparser                  | 1.18 sec                                               | 1.14 sec: 1.04x faster                                 |
| pprint_pformat             | 1.57 sec                                               | 1.52 sec: 1.03x faster                                 |
| sympy_integrate            | 21.4 ms                                                | 20.8 ms: 1.03x faster                                  |
| dask                       | 372 ms                                                 | 361 ms: 1.03x faster                                   |
| logging_silent             | 104 ns                                                 | 102 ns: 1.03x faster                                   |
| scimark_lu                 | 118 ms                                                 | 115 ms: 1.02x faster                                   |
| sympy_str                  | 300 ms                                                 | 292 ms: 1.02x faster                                   |
| create_gc_cycles           | 1.48 ms                                                | 1.44 ms: 1.02x faster                                  |
| pickle                     | 11.6 us                                                | 11.3 us: 1.02x faster                                  |
| bench_thread_pool          | 842 us                                                 | 824 us: 1.02x faster                                   |
| unpickle_list              | 5.29 us                                                | 5.18 us: 1.02x faster                                  |
| sympy_sum                  | 169 ms                                                 | 166 ms: 1.02x faster                                   |
| regex_dna                  | 212 ms                                                 | 208 ms: 1.02x faster                                   |
| nbody                      | 97.0 ms                                                | 95.5 ms: 1.02x faster                                  |
| regex_v8                   | 23.1 ms                                                | 22.8 ms: 1.02x faster                                  |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 5.00 ms: 1.01x faster                                  |
| gc_traversal               | 3.79 ms                                                | 3.76 ms: 1.01x faster                                  |
| sqlglot_optimize           | 54.8 ms                                                | 54.5 ms: 1.01x faster                                  |
| xml_etree_iterparse        | 107 ms                                                 | 107 ms: 1.00x slower                                   |
| pickle_dict                | 35.5 us                                                | 35.8 us: 1.01x slower                                  |
| sqlglot_normalize          | 110 ms                                                 | 111 ms: 1.01x slower                                   |
| richards                   | 45.8 ms                                                | 46.4 ms: 1.01x slower                                  |
| sqlglot_transpile          | 1.68 ms                                                | 1.71 ms: 1.02x slower                                  |
| go                         | 139 ms                                                 | 142 ms: 1.02x slower                                   |
| sympy_expand               | 478 ms                                                 | 488 ms: 1.02x slower                                   |
| unpickle_pure_python       | 230 us                                                 | 235 us: 1.02x slower                                   |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 743 ms: 1.02x slower                                   |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 744 ms: 1.03x slower                                   |
| hexiom                     | 6.41 ms                                                | 6.58 ms: 1.03x slower                                  |
| sqlglot_parse              | 1.36 ms                                                | 1.40 ms: 1.03x slower                                  |
| xml_etree_parse            | 159 ms                                                 | 165 ms: 1.03x slower                                   |
| comprehensions             | 21.8 us                                                | 22.6 us: 1.04x slower                                  |
| nqueens                    | 83.3 ms                                                | 86.5 ms: 1.04x slower                                  |
| pidigits                   | 187 ms                                                 | 195 ms: 1.04x slower                                   |
| async_tree_memoization_tg  | 575 ms                                                 | 608 ms: 1.06x slower                                   |
| async_tree_none_tg         | 450 ms                                                 | 477 ms: 1.06x slower                                   |
| chaos                      | 67.0 ms                                                | 71.1 ms: 1.06x slower                                  |
| mdp                        | 2.63 sec                                               | 2.82 sec: 1.07x slower                                 |
| async_tree_io_tg           | 1.18 sec                                               | 1.28 sec: 1.08x slower                                 |
| coverage                   | 72.7 ms                                                | 78.9 ms: 1.08x slower                                  |
| async_tree_memoization     | 578 ms                                                 | 646 ms: 1.12x slower                                   |
| async_tree_none            | 472 ms                                                 | 529 ms: 1.12x slower                                   |
| async_tree_io              | 1.16 sec                                               | 1.30 sec: 1.13x slower                                 |
| richards_super             | 51.5 ms                                                | 58.1 ms: 1.13x slower                                  |
| coroutines                 | 23.2 ms                                                | 26.4 ms: 1.14x slower                                  |
| json_dumps                 | 10.4 ms                                                | 13.3 ms: 1.28x slower                                  |
| asyncio_tcp_ssl            | 1.79 sec                                               | 3.12 sec: 1.75x slower                                 |
| asyncio_tcp                | 491 ms                                                 | 909 ms: 1.85x slower                                   |
| generators                 | 31.2 ms                                                | 75.9 ms: 2.43x slower                                  |
| typing_runtime_protocols   | 158 us                                                 | 514 us: 3.26x slower                                   |
| Geometric mean             | (ref)                                                  | 1.01x slower                                           |

Benchmark hidden because not significant (4): asyncio_websockets, tomli_loads, bench_mp_pool, deltablue
Ignored benchmarks (7) of results/bm-20240206-3.11.8-db85d51/bm-20240206-linux-x86_64-python-v3.11.8-3.11.8-db85d51.json: djangocms, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 93.55% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.95x