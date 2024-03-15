
# Results vs. 3.11.0

- fork: python
- ref: v3.12.1
- machine: darwin-arm64
- commit hash: 2305ca5
- commit date: 2023-12-07
- overall geometric mean: 1.02x slower
- HPT reliability: 99.93%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 167 ms: 1.08x slower                                   |
| chameleon      | 4.30 ms                                                | 4.50 ms: 1.05x slower                                  |
| docutils       | 1.43 sec                                               | 1.48 sec: 1.04x slower                                 |
| Geometric mean | (ref)                                                  | 1.04x slower                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_memoization_tg  | 352 ms                                                 | 317 ms: 1.11x faster                                   |
| async_tree_io_tg           | 724 ms                                                 | 660 ms: 1.10x faster                                   |
| async_tree_memoization     | 336 ms                                                 | 306 ms: 1.10x faster                                   |
| async_tree_none_tg         | 276 ms                                                 | 252 ms: 1.09x faster                                   |
| async_tree_none            | 282 ms                                                 | 260 ms: 1.08x faster                                   |
| async_tree_io              | 697 ms                                                 | 655 ms: 1.07x faster                                   |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 531 ms: 1.03x faster                                   |
| Geometric mean             | (ref)                                                  | 1.07x faster                                           |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 283 ms: 1.01x slower                                   |
| float          | 50.8 ms                                                | 56.5 ms: 1.11x slower                                  |
| nbody          | 61.7 ms                                                | 69.1 ms: 1.12x slower                                  |
| Geometric mean | (ref)                                                  | 1.08x slower                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 72.8 ms                                                | 73.7 ms: 1.01x slower                                  |
| regex_dna      | 148 ms                                                 | 152 ms: 1.03x slower                                   |
| regex_v8       | 15.1 ms                                                | 16.3 ms: 1.08x slower                                  |
| regex_effbot   | 2.43 ms                                                | 2.69 ms: 1.11x slower                                  |
| Geometric mean | (ref)                                                  | 1.06x slower                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.31 ms: 1.19x faster                                  |
| unpickle_pure_python | 149 us                                                 | 142 us: 1.04x faster                                   |
| pickle_pure_python   | 191 us                                                 | 188 us: 1.02x faster                                   |
| pickle               | 6.98 us                                                | 7.27 us: 1.04x slower                                  |
| pickle_dict          | 17.1 us                                                | 18.0 us: 1.05x slower                                  |
| pickle_list          | 2.70 us                                                | 2.85 us: 1.06x slower                                  |
| xml_etree_parse      | 100 ms                                                 | 107 ms: 1.07x slower                                   |
| xml_etree_iterparse  | 68.3 ms                                                | 74.0 ms: 1.08x slower                                  |
| tomli_loads          | 1.27 sec                                               | 1.40 sec: 1.10x slower                                 |
| unpickle             | 8.29 us                                                | 9.24 us: 1.11x slower                                  |
| json_loads           | 15.3 us                                                | 17.2 us: 1.12x slower                                  |
| xml_etree_process    | 33.6 ms                                                | 38.7 ms: 1.15x slower                                  |
| unpickle_list        | 2.69 us                                                | 3.25 us: 1.21x slower                                  |
| xml_etree_generate   | 45.8 ms                                                | 55.8 ms: 1.22x slower                                  |
| Geometric mean       | (ref)                                                  | 1.07x slower                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 12.9 ms: 1.20x slower                                  |
| python_startup_no_site | 8.57 ms                                                | 11.0 ms: 1.28x slower                                  |
| Geometric mean         | (ref)                                                  | 1.24x slower                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako            | 7.93 ms                                                | 7.59 ms: 1.05x faster                                  |
| django_template | 20.1 ms                                                | 21.2 ms: 1.05x slower                                  |
| Geometric mean  | (ref)                                                  | 1.00x slower                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| typing_runtime_protocols   | 301 us                                                 | 72.5 us: 4.15x faster                                  |
| asyncio_tcp                | 643 ms                                                 | 418 ms: 1.54x faster                                   |
| json_dumps                 | 7.53 ms                                                | 6.31 ms: 1.19x faster                                  |
| generators                 | 30.3 ms                                                | 25.9 ms: 1.17x faster                                  |
| unpack_sequence            | 33.6 ns                                                | 29.0 ns: 1.16x faster                                  |
| deltablue                  | 2.75 ms                                                | 2.40 ms: 1.15x faster                                  |
| chaos                      | 47.4 ms                                                | 41.8 ms: 1.14x faster                                  |
| go                         | 105 ms                                                 | 94.3 ms: 1.12x faster                                  |
| async_tree_memoization_tg  | 352 ms                                                 | 317 ms: 1.11x faster                                   |
| coverage                   | 43.9 ms                                                | 39.6 ms: 1.11x faster                                  |
| richards_super             | 37.3 ms                                                | 33.8 ms: 1.10x faster                                  |
| async_tree_io_tg           | 724 ms                                                 | 660 ms: 1.10x faster                                   |
| async_tree_memoization     | 336 ms                                                 | 306 ms: 1.10x faster                                   |
| async_tree_none_tg         | 276 ms                                                 | 252 ms: 1.09x faster                                   |
| hexiom                     | 4.58 ms                                                | 4.23 ms: 1.08x faster                                  |
| async_tree_none            | 282 ms                                                 | 260 ms: 1.08x faster                                   |
| sqlglot_parse              | 890 us                                                 | 823 us: 1.08x faster                                   |
| async_tree_io              | 697 ms                                                 | 655 ms: 1.07x faster                                   |
| sqlglot_transpile          | 1.05 ms                                                | 995 us: 1.06x faster                                   |
| mako                       | 7.93 ms                                                | 7.59 ms: 1.05x faster                                  |
| unpickle_pure_python       | 149 us                                                 | 142 us: 1.04x faster                                   |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 531 ms: 1.03x faster                                   |
| deepcopy_memo              | 25.7 us                                                | 24.9 us: 1.03x faster                                  |
| sympy_sum                  | 80.2 ms                                                | 77.8 ms: 1.03x faster                                  |
| richards                   | 31.1 ms                                                | 30.2 ms: 1.03x faster                                  |
| create_gc_cycles           | 711 us                                                 | 693 us: 1.03x faster                                   |
| pickle_pure_python         | 191 us                                                 | 188 us: 1.02x faster                                   |
| sympy_integrate            | 11.3 ms                                                | 11.1 ms: 1.02x faster                                  |
| sqlalchemy_imperative      | 6.98 ms                                                | 6.93 ms: 1.01x faster                                  |
| scimark_monte_carlo        | 43.5 ms                                                | 43.2 ms: 1.01x faster                                  |
| raytrace                   | 206 ms                                                 | 206 ms: 1.00x slower                                   |
| gc_traversal               | 2.38 ms                                                | 2.40 ms: 1.01x slower                                  |
| pidigits                   | 280 ms                                                 | 283 ms: 1.01x slower                                   |
| regex_compile              | 72.8 ms                                                | 73.7 ms: 1.01x slower                                  |
| dask                       | 219 ms                                                 | 222 ms: 1.01x slower                                   |
| comprehensions             | 14.4 us                                                | 14.7 us: 1.01x slower                                  |
| pycparser                  | 659 ms                                                 | 670 ms: 1.02x slower                                   |
| logging_silent             | 66.5 ns                                                | 67.7 ns: 1.02x slower                                  |
| dulwich_log                | 28.6 ms                                                | 29.1 ms: 1.02x slower                                  |
| meteor_contest             | 71.1 ms                                                | 72.5 ms: 1.02x slower                                  |
| pprint_pformat             | 979 ms                                                 | 999 ms: 1.02x slower                                   |
| regex_dna                  | 148 ms                                                 | 152 ms: 1.03x slower                                   |
| pprint_safe_repr           | 478 ms                                                 | 492 ms: 1.03x slower                                   |
| sympy_str                  | 144 ms                                                 | 148 ms: 1.03x slower                                   |
| docutils                   | 1.43 sec                                               | 1.48 sec: 1.04x slower                                 |
| deepcopy                   | 215 us                                                 | 224 us: 1.04x slower                                   |
| pickle                     | 6.98 us                                                | 7.27 us: 1.04x slower                                  |
| chameleon                  | 4.30 ms                                                | 4.50 ms: 1.05x slower                                  |
| logging_simple             | 3.41 us                                                | 3.57 us: 1.05x slower                                  |
| logging_format             | 3.67 us                                                | 3.86 us: 1.05x slower                                  |
| django_template            | 20.1 ms                                                | 21.2 ms: 1.05x slower                                  |
| pathlib                    | 23.2 ms                                                | 24.5 ms: 1.05x slower                                  |
| pickle_dict                | 17.1 us                                                | 18.0 us: 1.05x slower                                  |
| scimark_lu                 | 67.7 ms                                                | 71.5 ms: 1.06x slower                                  |
| pickle_list                | 2.70 us                                                | 2.85 us: 1.06x slower                                  |
| bench_thread_pool          | 465 us                                                 | 497 us: 1.07x slower                                   |
| xml_etree_parse            | 100 ms                                                 | 107 ms: 1.07x slower                                   |
| scimark_sor                | 79.2 ms                                                | 85.1 ms: 1.07x slower                                  |
| sympy_expand               | 229 ms                                                 | 247 ms: 1.08x slower                                   |
| regex_v8                   | 15.1 ms                                                | 16.3 ms: 1.08x slower                                  |
| json                       | 2.75 ms                                                | 2.97 ms: 1.08x slower                                  |
| nqueens                    | 55.9 ms                                                | 60.4 ms: 1.08x slower                                  |
| 2to3                       | 154 ms                                                 | 167 ms: 1.08x slower                                   |
| xml_etree_iterparse        | 68.3 ms                                                | 74.0 ms: 1.08x slower                                  |
| crypto_pyaes               | 47.5 ms                                                | 51.5 ms: 1.09x slower                                  |
| pyflate                    | 284 ms                                                 | 309 ms: 1.09x slower                                   |
| sqlalchemy_declarative     | 59.3 ms                                                | 64.7 ms: 1.09x slower                                  |
| mdp                        | 1.48 sec                                               | 1.62 sec: 1.09x slower                                 |
| tomli_loads                | 1.27 sec                                               | 1.40 sec: 1.10x slower                                 |
| fannkuch                   | 240 ms                                                 | 265 ms: 1.10x slower                                   |
| regex_effbot               | 2.43 ms                                                | 2.69 ms: 1.11x slower                                  |
| coroutines                 | 17.2 ms                                                | 19.1 ms: 1.11x slower                                  |
| float                      | 50.8 ms                                                | 56.5 ms: 1.11x slower                                  |
| unpickle                   | 8.29 us                                                | 9.24 us: 1.11x slower                                  |
| bench_mp_pool              | 41.0 ms                                                | 45.8 ms: 1.12x slower                                  |
| nbody                      | 61.7 ms                                                | 69.1 ms: 1.12x slower                                  |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 3.15 ms: 1.12x slower                                  |
| deepcopy_reduce            | 1.79 us                                                | 2.01 us: 1.12x slower                                  |
| aiohttp                    | 1.02 ms                                                | 1.15 ms: 1.12x slower                                  |
| json_loads                 | 15.3 us                                                | 17.2 us: 1.12x slower                                  |
| sqlglot_normalize          | 162 ms                                                 | 184 ms: 1.14x slower                                   |
| spectral_norm              | 65.7 ms                                                | 75.0 ms: 1.14x slower                                  |
| gunicorn                   | 1.10 ms                                                | 1.26 ms: 1.15x slower                                  |
| sqlglot_optimize           | 29.6 ms                                                | 34.0 ms: 1.15x slower                                  |
| xml_etree_process          | 33.6 ms                                                | 38.7 ms: 1.15x slower                                  |
| scimark_fft                | 173 ms                                                 | 200 ms: 1.16x slower                                   |
| python_startup             | 10.8 ms                                                | 12.9 ms: 1.20x slower                                  |
| telco                      | 3.17 ms                                                | 3.82 ms: 1.21x slower                                  |
| unpickle_list              | 2.69 us                                                | 3.25 us: 1.21x slower                                  |
| xml_etree_generate         | 45.8 ms                                                | 55.8 ms: 1.22x slower                                  |
| mypy2                      | 372 ms                                                 | 469 ms: 1.26x slower                                   |
| sqlite_synth               | 1.26 us                                                | 1.61 us: 1.28x slower                                  |
| python_startup_no_site     | 8.57 ms                                                | 11.0 ms: 1.28x slower                                  |
| async_generators           | 192 ms                                                 | 303 ms: 1.58x slower                                   |
| Geometric mean             | (ref)                                                  | 1.02x slower                                           |

Benchmark hidden because not significant (4): tornado_http, asyncio_tcp_ssl, asyncio_websockets, async_tree_cpu_io_mixed
Ignored benchmarks (6) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 99.93% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x