
# Results vs. 3.12.0

- fork: python
- ref: v3.11.7
- machine: darwin-arm64
- commit hash: fa7a6f2
- commit date: 2023-12-04
- overall geometric mean: 1.01x faster
- HPT reliability: 99.01%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.97x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 153 ms: 1.11x faster                                   |
| chameleon      | 4.70 ms                                                | 4.36 ms: 1.08x faster                                  |
| docutils       | 1.50 sec                                               | 1.41 sec: 1.07x faster                                 |
| Geometric mean | (ref)                                                  | 1.06x faster                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 526 ms                                                 | 516 ms: 1.02x faster                                   |
| async_tree_memoization     | 312 ms                                                 | 315 ms: 1.01x slower                                   |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 542 ms: 1.02x slower                                   |
| async_tree_memoization_tg  | 323 ms                                                 | 334 ms: 1.04x slower                                   |
| async_tree_io              | 668 ms                                                 | 697 ms: 1.04x slower                                   |
| async_tree_io_tg           | 669 ms                                                 | 700 ms: 1.05x slower                                   |
| async_tree_none_tg         | 258 ms                                                 | 271 ms: 1.05x slower                                   |
| async_tree_none            | 266 ms                                                 | 282 ms: 1.06x slower                                   |
| Geometric mean             | (ref)                                                  | 1.03x slower                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| float          | 55.8 ms                                                | 53.5 ms: 1.04x faster                                  |
| Geometric mean | (ref)                                                  | 1.01x faster                                           |

Benchmark hidden because not significant (2): pidigits, nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 77.9 ms                                                | 72.8 ms: 1.07x faster                                  |
| regex_v8       | 16.0 ms                                                | 15.7 ms: 1.01x faster                                  |
| regex_dna      | 154 ms                                                 | 152 ms: 1.01x faster                                   |
| regex_effbot   | 2.64 ms                                                | 2.61 ms: 1.01x faster                                  |
| Geometric mean | (ref)                                                  | 1.03x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2 |
|---------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| xml_etree_generate  | 55.8 ms                                                | 47.2 ms: 1.18x faster                                  |
| xml_etree_process   | 39.7 ms                                                | 34.4 ms: 1.15x faster                                  |
| json_loads          | 17.2 us                                                | 15.4 us: 1.12x faster                                  |
| unpickle            | 9.12 us                                                | 8.32 us: 1.10x faster                                  |
| xml_etree_parse     | 106 ms                                                 | 97.1 ms: 1.09x faster                                  |
| xml_etree_iterparse | 74.0 ms                                                | 67.8 ms: 1.09x faster                                  |
| unpickle_list       | 3.02 us                                                | 2.78 us: 1.09x faster                                  |
| pickle_list         | 2.89 us                                                | 2.69 us: 1.07x faster                                  |
| pickle_dict         | 18.1 us                                                | 17.0 us: 1.06x faster                                  |
| tomli_loads         | 1.39 sec                                               | 1.32 sec: 1.06x faster                                 |
| pickle_pure_python  | 200 us                                                 | 193 us: 1.04x faster                                   |
| pickle              | 7.23 us                                                | 7.26 us: 1.01x slower                                  |
| json_dumps          | 6.22 ms                                                | 7.60 ms: 1.22x slower                                  |
| Geometric mean      | (ref)                                                  | 1.06x faster                                           |

Benchmark hidden because not significant (1): unpickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 11.9 ms: 1.04x slower                                  |
| python_startup_no_site | 9.37 ms                                                | 9.93 ms: 1.06x slower                                  |
| Geometric mean         | (ref)                                                  | 1.05x slower                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| django_template | 22.3 ms                                                | 19.7 ms: 1.13x faster                                  |
| mako            | 7.71 ms                                                | 8.19 ms: 1.06x slower                                  |
| Geometric mean  | (ref)                                                  | 1.03x faster                                           |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_generators           | 304 ms                                                 | 187 ms: 1.63x faster                                   |
| sqlite_synth               | 1.57 us                                                | 1.26 us: 1.25x faster                                  |
| xml_etree_generate         | 55.8 ms                                                | 47.2 ms: 1.18x faster                                  |
| telco                      | 3.68 ms                                                | 3.17 ms: 1.16x faster                                  |
| logging_silent             | 76.4 ns                                                | 66.2 ns: 1.15x faster                                  |
| xml_etree_process          | 39.7 ms                                                | 34.4 ms: 1.15x faster                                  |
| deepcopy_reduce            | 2.07 us                                                | 1.80 us: 1.15x faster                                  |
| scimark_sor                | 87.4 ms                                                | 76.4 ms: 1.14x faster                                  |
| coroutines                 | 19.2 ms                                                | 16.9 ms: 1.14x faster                                  |
| sqlglot_normalize          | 186 ms                                                 | 163 ms: 1.14x faster                                   |
| sqlglot_optimize           | 34.0 ms                                                | 30.0 ms: 1.13x faster                                  |
| django_template            | 22.3 ms                                                | 19.7 ms: 1.13x faster                                  |
| nqueens                    | 62.4 ms                                                | 55.7 ms: 1.12x faster                                  |
| json_loads                 | 17.2 us                                                | 15.4 us: 1.12x faster                                  |
| json                       | 3.09 ms                                                | 2.77 ms: 1.11x faster                                  |
| deepcopy                   | 235 us                                                 | 211 us: 1.11x faster                                   |
| 2to3                       | 169 ms                                                 | 153 ms: 1.11x faster                                   |
| scimark_lu                 | 76.0 ms                                                | 68.7 ms: 1.11x faster                                  |
| unpickle                   | 9.12 us                                                | 8.32 us: 1.10x faster                                  |
| xml_etree_parse            | 106 ms                                                 | 97.1 ms: 1.09x faster                                  |
| xml_etree_iterparse        | 74.0 ms                                                | 67.8 ms: 1.09x faster                                  |
| bench_mp_pool              | 44.9 ms                                                | 41.2 ms: 1.09x faster                                  |
| bench_thread_pool          | 504 us                                                 | 464 us: 1.09x faster                                   |
| deepcopy_memo              | 27.7 us                                                | 25.5 us: 1.09x faster                                  |
| unpickle_list              | 3.02 us                                                | 2.78 us: 1.09x faster                                  |
| spectral_norm              | 76.4 ms                                                | 70.5 ms: 1.08x faster                                  |
| crypto_pyaes               | 51.9 ms                                                | 48.0 ms: 1.08x faster                                  |
| pyflate                    | 316 ms                                                 | 292 ms: 1.08x faster                                   |
| chameleon                  | 4.70 ms                                                | 4.36 ms: 1.08x faster                                  |
| pickle_list                | 2.89 us                                                | 2.69 us: 1.07x faster                                  |
| regex_compile              | 77.9 ms                                                | 72.8 ms: 1.07x faster                                  |
| docutils                   | 1.50 sec                                               | 1.41 sec: 1.07x faster                                 |
| pickle_dict                | 18.1 us                                                | 17.0 us: 1.06x faster                                  |
| tomli_loads                | 1.39 sec                                               | 1.32 sec: 1.06x faster                                 |
| logging_simple             | 3.69 us                                                | 3.50 us: 1.05x faster                                  |
| logging_format             | 3.98 us                                                | 3.79 us: 1.05x faster                                  |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 2.99 ms: 1.05x faster                                  |
| float                      | 55.8 ms                                                | 53.5 ms: 1.04x faster                                  |
| generators                 | 31.1 ms                                                | 29.8 ms: 1.04x faster                                  |
| dulwich_log                | 29.8 ms                                                | 28.7 ms: 1.04x faster                                  |
| scimark_fft                | 195 ms                                                 | 188 ms: 1.04x faster                                   |
| pickle_pure_python         | 200 us                                                 | 193 us: 1.04x faster                                   |
| sqlalchemy_declarative     | 62.3 ms                                                | 60.4 ms: 1.03x faster                                  |
| pprint_safe_repr           | 497 ms                                                 | 483 ms: 1.03x faster                                   |
| pycparser                  | 677 ms                                                 | 659 ms: 1.03x faster                                   |
| pprint_pformat             | 1.01 sec                                               | 986 ms: 1.03x faster                                   |
| sympy_str                  | 148 ms                                                 | 144 ms: 1.03x faster                                   |
| sympy_expand               | 241 ms                                                 | 235 ms: 1.02x faster                                   |
| aiohttp                    | 1.08 ms                                                | 1.06 ms: 1.02x faster                                  |
| sympy_integrate            | 11.4 ms                                                | 11.1 ms: 1.02x faster                                  |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 516 ms: 1.02x faster                                   |
| pathlib                    | 24.2 ms                                                | 23.9 ms: 1.02x faster                                  |
| regex_v8                   | 16.0 ms                                                | 15.7 ms: 1.01x faster                                  |
| comprehensions             | 14.5 us                                                | 14.3 us: 1.01x faster                                  |
| regex_dna                  | 154 ms                                                 | 152 ms: 1.01x faster                                   |
| raytrace                   | 212 ms                                                 | 209 ms: 1.01x faster                                   |
| regex_effbot               | 2.64 ms                                                | 2.61 ms: 1.01x faster                                  |
| richards                   | 32.1 ms                                                | 31.9 ms: 1.01x faster                                  |
| asyncio_websockets         | 409 ms                                                 | 407 ms: 1.00x faster                                   |
| pickle                     | 7.23 us                                                | 7.26 us: 1.01x slower                                  |
| fannkuch                   | 248 ms                                                 | 250 ms: 1.01x slower                                   |
| meteor_contest             | 71.7 ms                                                | 72.3 ms: 1.01x slower                                  |
| async_tree_memoization     | 312 ms                                                 | 315 ms: 1.01x slower                                   |
| create_gc_cycles           | 701 us                                                 | 713 us: 1.02x slower                                   |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 542 ms: 1.02x slower                                   |
| deltablue                  | 2.71 ms                                                | 2.77 ms: 1.02x slower                                  |
| hexiom                     | 4.54 ms                                                | 4.65 ms: 1.02x slower                                  |
| sympy_sum                  | 77.6 ms                                                | 80.0 ms: 1.03x slower                                  |
| async_tree_memoization_tg  | 323 ms                                                 | 334 ms: 1.04x slower                                   |
| python_startup             | 11.4 ms                                                | 11.9 ms: 1.04x slower                                  |
| async_tree_io              | 668 ms                                                 | 697 ms: 1.04x slower                                   |
| sqlglot_transpile          | 1.02 ms                                                | 1.07 ms: 1.04x slower                                  |
| async_tree_io_tg           | 669 ms                                                 | 700 ms: 1.05x slower                                   |
| async_tree_none_tg         | 258 ms                                                 | 271 ms: 1.05x slower                                   |
| scimark_monte_carlo        | 45.0 ms                                                | 47.6 ms: 1.06x slower                                  |
| python_startup_no_site     | 9.37 ms                                                | 9.93 ms: 1.06x slower                                  |
| go                         | 102 ms                                                 | 108 ms: 1.06x slower                                   |
| async_tree_none            | 266 ms                                                 | 282 ms: 1.06x slower                                   |
| mako                       | 7.71 ms                                                | 8.19 ms: 1.06x slower                                  |
| sqlglot_parse              | 848 us                                                 | 904 us: 1.07x slower                                   |
| sqlalchemy_imperative      | 6.68 ms                                                | 7.16 ms: 1.07x slower                                  |
| richards_super             | 36.0 ms                                                | 38.8 ms: 1.08x slower                                  |
| unpack_sequence            | 31.5 ns                                                | 33.9 ns: 1.08x slower                                  |
| mdp                        | 1.58 sec                                               | 1.75 sec: 1.11x slower                                 |
| coverage                   | 38.9 ms                                                | 43.5 ms: 1.12x slower                                  |
| chaos                      | 42.5 ms                                                | 48.6 ms: 1.14x slower                                  |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.45 sec: 1.16x slower                                 |
| json_dumps                 | 6.22 ms                                                | 7.60 ms: 1.22x slower                                  |
| asyncio_tcp                | 449 ms                                                 | 659 ms: 1.47x slower                                   |
| mypy2                      | 380 ms                                                 | 583 ms: 1.53x slower                                   |
| typing_runtime_protocols   | 93.0 us                                                | 328 us: 3.53x slower                                   |
| Geometric mean             | (ref)                                                  | 1.01x faster                                           |

Benchmark hidden because not significant (7): gunicorn, dask, pidigits, gc_traversal, unpickle_pure_python, nbody, tornado_http
Ignored benchmarks (6) of results/bm-20231204-3.11.7-fa7a6f2/bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 99.01% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.97x