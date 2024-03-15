
# Results vs. 3.11.0

- fork: python
- ref: v3.13.0a2
- machine: darwin-arm64
- commit hash: 9c4347e
- commit date: 2023-11-22
- overall geometric mean: 1.09x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x slower
- Memory change: 1.04x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-darwin-arm64-python-v3.13.0a2-3.13.0a2-9c4347e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 179 ms: 1.16x slower                                       |
| chameleon      | 4.30 ms                                                | 4.93 ms: 1.15x slower                                      |
| docutils       | 1.43 sec                                               | 1.51 sec: 1.05x slower                                     |
| Geometric mean | (ref)                                                  | 1.10x slower                                               |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-darwin-arm64-python-v3.13.0a2-3.13.0a2-9c4347e |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| async_tree_none         | 282 ms                                                 | 263 ms: 1.07x faster                                       |
| async_tree_io_tg        | 724 ms                                                 | 703 ms: 1.03x faster                                       |
| async_tree_none_tg      | 276 ms                                                 | 277 ms: 1.00x slower                                       |
| async_tree_cpu_io_mixed | 519 ms                                                 | 532 ms: 1.02x slower                                       |
| async_tree_io           | 697 ms                                                 | 719 ms: 1.03x slower                                       |
| Geometric mean          | (ref)                                                  | 1.01x faster                                               |

Benchmark hidden because not significant (3): async_tree_memoization_tg, async_tree_cpu_io_mixed_tg, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-darwin-arm64-python-v3.13.0a2-3.13.0a2-9c4347e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 284 ms: 1.01x slower                                       |
| float          | 50.8 ms                                                | 68.2 ms: 1.34x slower                                      |
| nbody          | 61.7 ms                                                | 86.3 ms: 1.40x slower                                      |
| Geometric mean | (ref)                                                  | 1.24x slower                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-darwin-arm64-python-v3.13.0a2-3.13.0a2-9c4347e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| regex_dna      | 148 ms                                                 | 155 ms: 1.05x slower                                       |
| regex_effbot   | 2.43 ms                                                | 2.56 ms: 1.06x slower                                      |
| regex_v8       | 15.1 ms                                                | 17.4 ms: 1.15x slower                                      |
| regex_compile  | 72.8 ms                                                | 85.5 ms: 1.17x slower                                      |
| Geometric mean | (ref)                                                  | 1.10x slower                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-darwin-arm64-python-v3.13.0a2-3.13.0a2-9c4347e |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.61 ms: 1.14x faster                                      |
| pickle_pure_python   | 191 us                                                 | 201 us: 1.05x slower                                       |
| pickle               | 6.98 us                                                | 7.36 us: 1.05x slower                                      |
| pickle_dict          | 17.1 us                                                | 18.1 us: 1.06x slower                                      |
| xml_etree_parse      | 100 ms                                                 | 107 ms: 1.07x slower                                       |
| unpickle             | 8.29 us                                                | 8.99 us: 1.08x slower                                      |
| pickle_list          | 2.70 us                                                | 2.93 us: 1.09x slower                                      |
| unpickle_list        | 2.69 us                                                | 2.98 us: 1.11x slower                                      |
| json_loads           | 15.3 us                                                | 17.1 us: 1.11x slower                                      |
| unpickle_pure_python | 149 us                                                 | 168 us: 1.13x slower                                       |
| xml_etree_iterparse  | 68.3 ms                                                | 81.1 ms: 1.19x slower                                      |
| xml_etree_process    | 33.6 ms                                                | 41.2 ms: 1.23x slower                                      |
| xml_etree_generate   | 45.8 ms                                                | 59.6 ms: 1.30x slower                                      |
| tomli_loads          | 1.27 sec                                               | 1.67 sec: 1.31x slower                                     |
| Geometric mean       | (ref)                                                  | 1.11x slower                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-darwin-arm64-python-v3.13.0a2-3.13.0a2-9c4347e |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 12.7 ms: 1.18x slower                                      |
| python_startup_no_site | 8.57 ms                                                | 11.4 ms: 1.33x slower                                      |
| Geometric mean         | (ref)                                                  | 1.25x slower                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-darwin-arm64-python-v3.13.0a2-3.13.0a2-9c4347e |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------:|
| mako      | 7.93 ms                                                | 9.60 ms: 1.21x slower                                      |

All benchmarks:
===============

| Benchmark                | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-darwin-arm64-python-v3.13.0a2-3.13.0a2-9c4347e |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| typing_runtime_protocols | 301 us                                                 | 77.1 us: 3.90x faster                                      |
| asyncio_tcp              | 643 ms                                                 | 435 ms: 1.48x faster                                       |
| unpack_sequence          | 33.6 ns                                                | 28.2 ns: 1.19x faster                                      |
| json_dumps               | 7.53 ms                                                | 6.61 ms: 1.14x faster                                      |
| generators               | 30.3 ms                                                | 28.0 ms: 1.08x faster                                      |
| async_tree_none          | 282 ms                                                 | 263 ms: 1.07x faster                                       |
| asyncio_tcp_ssl          | 1.40 sec                                               | 1.30 sec: 1.07x faster                                     |
| sqlglot_parse            | 890 us                                                 | 838 us: 1.06x faster                                       |
| raytrace                 | 206 ms                                                 | 195 ms: 1.06x faster                                       |
| sqlglot_transpile        | 1.05 ms                                                | 1.02 ms: 1.03x faster                                      |
| async_tree_io_tg         | 724 ms                                                 | 703 ms: 1.03x faster                                       |
| create_gc_cycles         | 711 us                                                 | 704 us: 1.01x faster                                       |
| chaos                    | 47.4 ms                                                | 47.5 ms: 1.00x slower                                      |
| async_tree_none_tg       | 276 ms                                                 | 277 ms: 1.00x slower                                       |
| gc_traversal             | 2.38 ms                                                | 2.40 ms: 1.01x slower                                      |
| richards_super           | 37.3 ms                                                | 37.7 ms: 1.01x slower                                      |
| pidigits                 | 280 ms                                                 | 284 ms: 1.01x slower                                       |
| async_tree_cpu_io_mixed  | 519 ms                                                 | 532 ms: 1.02x slower                                       |
| async_tree_io            | 697 ms                                                 | 719 ms: 1.03x slower                                       |
| deepcopy_memo            | 25.7 us                                                | 26.7 us: 1.04x slower                                      |
| sympy_str                | 144 ms                                                 | 149 ms: 1.04x slower                                       |
| sympy_integrate          | 11.3 ms                                                | 11.7 ms: 1.04x slower                                      |
| deepcopy                 | 215 us                                                 | 224 us: 1.04x slower                                       |
| pickle_pure_python       | 191 us                                                 | 201 us: 1.05x slower                                       |
| regex_dna                | 148 ms                                                 | 155 ms: 1.05x slower                                       |
| dask                     | 219 ms                                                 | 230 ms: 1.05x slower                                       |
| dulwich_log              | 28.6 ms                                                | 30.1 ms: 1.05x slower                                      |
| docutils                 | 1.43 sec                                               | 1.51 sec: 1.05x slower                                     |
| pickle                   | 6.98 us                                                | 7.36 us: 1.05x slower                                      |
| regex_effbot             | 2.43 ms                                                | 2.56 ms: 1.06x slower                                      |
| logging_simple           | 3.41 us                                                | 3.60 us: 1.06x slower                                      |
| pickle_dict              | 17.1 us                                                | 18.1 us: 1.06x slower                                      |
| go                       | 105 ms                                                 | 112 ms: 1.06x slower                                       |
| logging_format           | 3.67 us                                                | 3.90 us: 1.06x slower                                      |
| sympy_expand             | 229 ms                                                 | 243 ms: 1.06x slower                                       |
| xml_etree_parse          | 100 ms                                                 | 107 ms: 1.07x slower                                       |
| pycparser                | 659 ms                                                 | 706 ms: 1.07x slower                                       |
| richards                 | 31.1 ms                                                | 33.6 ms: 1.08x slower                                      |
| coroutines               | 17.2 ms                                                | 18.6 ms: 1.08x slower                                      |
| logging_silent           | 66.5 ns                                                | 72.1 ns: 1.08x slower                                      |
| unpickle                 | 8.29 us                                                | 8.99 us: 1.08x slower                                      |
| json                     | 2.75 ms                                                | 2.99 ms: 1.09x slower                                      |
| pickle_list              | 2.70 us                                                | 2.93 us: 1.09x slower                                      |
| comprehensions           | 14.4 us                                                | 15.7 us: 1.09x slower                                      |
| pathlib                  | 23.2 ms                                                | 25.3 ms: 1.09x slower                                      |
| deepcopy_reduce          | 1.79 us                                                | 1.95 us: 1.09x slower                                      |
| coverage                 | 43.9 ms                                                | 47.9 ms: 1.09x slower                                      |
| bench_mp_pool            | 41.0 ms                                                | 44.8 ms: 1.09x slower                                      |
| mdp                      | 1.48 sec                                               | 1.63 sec: 1.10x slower                                     |
| meteor_contest           | 71.1 ms                                                | 78.7 ms: 1.11x slower                                      |
| unpickle_list            | 2.69 us                                                | 2.98 us: 1.11x slower                                      |
| json_loads               | 15.3 us                                                | 17.1 us: 1.11x slower                                      |
| scimark_lu               | 67.7 ms                                                | 76.1 ms: 1.12x slower                                      |
| bench_thread_pool        | 465 us                                                 | 523 us: 1.12x slower                                       |
| unpickle_pure_python     | 149 us                                                 | 168 us: 1.13x slower                                       |
| chameleon                | 4.30 ms                                                | 4.93 ms: 1.15x slower                                      |
| regex_v8                 | 15.1 ms                                                | 17.4 ms: 1.15x slower                                      |
| crypto_pyaes             | 47.5 ms                                                | 54.5 ms: 1.15x slower                                      |
| 2to3                     | 154 ms                                                 | 179 ms: 1.16x slower                                       |
| pprint_safe_repr         | 478 ms                                                 | 561 ms: 1.17x slower                                       |
| regex_compile            | 72.8 ms                                                | 85.5 ms: 1.17x slower                                      |
| python_startup           | 10.8 ms                                                | 12.7 ms: 1.18x slower                                      |
| sqlglot_normalize        | 162 ms                                                 | 191 ms: 1.18x slower                                       |
| pprint_pformat           | 979 ms                                                 | 1.15 sec: 1.18x slower                                     |
| xml_etree_iterparse      | 68.3 ms                                                | 81.1 ms: 1.19x slower                                      |
| mako                     | 7.93 ms                                                | 9.60 ms: 1.21x slower                                      |
| sqlglot_optimize         | 29.6 ms                                                | 35.9 ms: 1.21x slower                                      |
| xml_etree_process        | 33.6 ms                                                | 41.2 ms: 1.23x slower                                      |
| nqueens                  | 55.9 ms                                                | 69.7 ms: 1.25x slower                                      |
| pyflate                  | 284 ms                                                 | 369 ms: 1.30x slower                                       |
| xml_etree_generate       | 45.8 ms                                                | 59.6 ms: 1.30x slower                                      |
| deltablue                | 2.75 ms                                                | 3.59 ms: 1.31x slower                                      |
| sqlite_synth             | 1.26 us                                                | 1.64 us: 1.31x slower                                      |
| tomli_loads              | 1.27 sec                                               | 1.67 sec: 1.31x slower                                     |
| python_startup_no_site   | 8.57 ms                                                | 11.4 ms: 1.33x slower                                      |
| scimark_monte_carlo      | 43.5 ms                                                | 57.9 ms: 1.33x slower                                      |
| scimark_sor              | 79.2 ms                                                | 106 ms: 1.34x slower                                       |
| float                    | 50.8 ms                                                | 68.2 ms: 1.34x slower                                      |
| fannkuch                 | 240 ms                                                 | 324 ms: 1.35x slower                                       |
| hexiom                   | 4.58 ms                                                | 6.21 ms: 1.36x slower                                      |
| nbody                    | 61.7 ms                                                | 86.3 ms: 1.40x slower                                      |
| scimark_fft              | 173 ms                                                 | 246 ms: 1.43x slower                                       |
| mypy2                    | 372 ms                                                 | 532 ms: 1.43x slower                                       |
| scimark_sparse_mat_mult  | 2.81 ms                                                | 4.04 ms: 1.44x slower                                      |
| telco                    | 3.17 ms                                                | 4.63 ms: 1.46x slower                                      |
| spectral_norm            | 65.7 ms                                                | 102 ms: 1.56x slower                                       |
| async_generators         | 192 ms                                                 | 301 ms: 1.57x slower                                       |
| Geometric mean           | (ref)                                                  | 1.09x slower                                               |

Benchmark hidden because not significant (6): async_tree_memoization_tg, async_tree_cpu_io_mixed_tg, sympy_sum, asyncio_websockets, async_tree_memoization, tornado_http
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.06x
- 95% likely to have a slowdown of 1.06x
- 99% likely to have a slowdown of 1.05x


# Memory

- memory change: 1.04x