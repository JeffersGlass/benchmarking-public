
# Results vs. 3.12.0

- fork: python
- ref: 3d5d3f7af6498effbc60
- machine: darwin-arm64
- commit hash: 3d5d3f7
- commit date: 2023-01-10
- overall geometric mean: 1.02x faster \*
- HPT reliability: 99.96%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.94x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 158 ms: 1.08x faster                                                  |
| chameleon      | 4.70 ms                                                | 4.21 ms: 1.12x faster                                                 |
| docutils       | 1.50 sec                                               | 1.41 sec: 1.06x faster                                                |
| Geometric mean | (ref)                                                  | 1.09x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 526 ms                                                 | 521 ms: 1.01x faster                                                  |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 543 ms: 1.02x slower                                                  |
| async_tree_none_tg         | 258 ms                                                 | 266 ms: 1.03x slower                                                  |
| async_tree_memoization     | 312 ms                                                 | 322 ms: 1.03x slower                                                  |
| async_tree_memoization_tg  | 323 ms                                                 | 340 ms: 1.05x slower                                                  |
| async_tree_none            | 266 ms                                                 | 280 ms: 1.05x slower                                                  |
| async_tree_io_tg           | 669 ms                                                 | 710 ms: 1.06x slower                                                  |
| async_tree_io              | 668 ms                                                 | 728 ms: 1.09x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.04x slower                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| nbody          | 68.8 ms                                                | 67.7 ms: 1.02x faster                                                 |
| pidigits       | 282 ms                                                 | 280 ms: 1.01x faster                                                  |
| float          | 55.8 ms                                                | 55.5 ms: 1.01x faster                                                 |
| Geometric mean | (ref)                                                  | 1.01x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_effbot   | 2.64 ms                                                | 2.44 ms: 1.08x faster                                                 |
| regex_compile  | 77.9 ms                                                | 72.1 ms: 1.08x faster                                                 |
| regex_v8       | 16.0 ms                                                | 15.0 ms: 1.07x faster                                                 |
| regex_dna      | 154 ms                                                 | 147 ms: 1.05x faster                                                  |
| Geometric mean | (ref)                                                  | 1.07x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| xml_etree_generate   | 55.8 ms                                                | 46.9 ms: 1.19x faster                                                 |
| xml_etree_process    | 39.7 ms                                                | 33.8 ms: 1.17x faster                                                 |
| json_loads           | 17.2 us                                                | 15.5 us: 1.11x faster                                                 |
| xml_etree_parse      | 106 ms                                                 | 96.4 ms: 1.10x faster                                                 |
| unpickle_pure_python | 151 us                                                 | 137 us: 1.10x faster                                                  |
| tomli_loads          | 1.39 sec                                               | 1.28 sec: 1.09x faster                                                |
| unpickle             | 9.12 us                                                | 8.43 us: 1.08x faster                                                 |
| unpickle_list        | 3.02 us                                                | 2.81 us: 1.07x faster                                                 |
| pickle_list          | 2.89 us                                                | 2.70 us: 1.07x faster                                                 |
| json_dumps           | 6.22 ms                                                | 5.84 ms: 1.06x faster                                                 |
| pickle_dict          | 18.1 us                                                | 17.0 us: 1.06x faster                                                 |
| xml_etree_iterparse  | 74.0 ms                                                | 70.0 ms: 1.06x faster                                                 |
| pickle_pure_python   | 200 us                                                 | 190 us: 1.05x faster                                                  |
| pickle               | 7.23 us                                                | 6.98 us: 1.04x faster                                                 |
| Geometric mean       | (ref)                                                  | 1.09x faster                                                          |

Benchmarks with tag 'startup':
==============================

Benchmark hidden because not significant (2): python_startup, python_startup_no_site

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| django_template | 22.3 ms                                                | 20.8 ms: 1.07x faster                                                 |
| mako            | 7.71 ms                                                | 7.76 ms: 1.01x slower                                                 |
| Geometric mean  | (ref)                                                  | 1.03x faster                                                          |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_generators           | 304 ms                                                 | 200 ms: 1.52x faster                                                  |
| logging_silent             | 76.4 ns                                                | 63.9 ns: 1.20x faster                                                 |
| xml_etree_generate         | 55.8 ms                                                | 46.9 ms: 1.19x faster                                                 |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 2.66 ms: 1.18x faster                                                 |
| xml_etree_process          | 39.7 ms                                                | 33.8 ms: 1.17x faster                                                 |
| sqlite_synth               | 1.57 us                                                | 1.36 us: 1.15x faster                                                 |
| telco                      | 3.68 ms                                                | 3.22 ms: 1.14x faster                                                 |
| sqlglot_optimize           | 34.0 ms                                                | 30.0 ms: 1.14x faster                                                 |
| scimark_lu                 | 76.0 ms                                                | 67.3 ms: 1.13x faster                                                 |
| sqlglot_normalize          | 186 ms                                                 | 165 ms: 1.13x faster                                                  |
| chameleon                  | 4.70 ms                                                | 4.21 ms: 1.12x faster                                                 |
| json_loads                 | 17.2 us                                                | 15.5 us: 1.11x faster                                                 |
| json                       | 3.09 ms                                                | 2.79 ms: 1.11x faster                                                 |
| logging_format             | 3.98 us                                                | 3.60 us: 1.11x faster                                                 |
| xml_etree_parse            | 106 ms                                                 | 96.4 ms: 1.10x faster                                                 |
| logging_simple             | 3.69 us                                                | 3.34 us: 1.10x faster                                                 |
| coroutines                 | 19.2 ms                                                | 17.5 ms: 1.10x faster                                                 |
| unpickle_pure_python       | 151 us                                                 | 137 us: 1.10x faster                                                  |
| bench_thread_pool          | 504 us                                                 | 460 us: 1.10x faster                                                  |
| nqueens                    | 62.4 ms                                                | 57.2 ms: 1.09x faster                                                 |
| tomli_loads                | 1.39 sec                                               | 1.28 sec: 1.09x faster                                                |
| spectral_norm              | 76.4 ms                                                | 70.6 ms: 1.08x faster                                                 |
| regex_effbot               | 2.64 ms                                                | 2.44 ms: 1.08x faster                                                 |
| unpickle                   | 9.12 us                                                | 8.43 us: 1.08x faster                                                 |
| regex_compile              | 77.9 ms                                                | 72.1 ms: 1.08x faster                                                 |
| deltablue                  | 2.71 ms                                                | 2.51 ms: 1.08x faster                                                 |
| richards                   | 32.1 ms                                                | 29.8 ms: 1.08x faster                                                 |
| 2to3                       | 169 ms                                                 | 158 ms: 1.08x faster                                                  |
| unpickle_list              | 3.02 us                                                | 2.81 us: 1.07x faster                                                 |
| django_template            | 22.3 ms                                                | 20.8 ms: 1.07x faster                                                 |
| scimark_fft                | 195 ms                                                 | 182 ms: 1.07x faster                                                  |
| pickle_list                | 2.89 us                                                | 2.70 us: 1.07x faster                                                 |
| regex_v8                   | 16.0 ms                                                | 15.0 ms: 1.07x faster                                                 |
| deepcopy_reduce            | 2.07 us                                                | 1.94 us: 1.07x faster                                                 |
| json_dumps                 | 6.22 ms                                                | 5.84 ms: 1.06x faster                                                 |
| docutils                   | 1.50 sec                                               | 1.41 sec: 1.06x faster                                                |
| pickle_dict                | 18.1 us                                                | 17.0 us: 1.06x faster                                                 |
| xml_etree_iterparse        | 74.0 ms                                                | 70.0 ms: 1.06x faster                                                 |
| dulwich_log                | 29.8 ms                                                | 28.2 ms: 1.06x faster                                                 |
| bench_mp_pool              | 44.9 ms                                                | 42.5 ms: 1.06x faster                                                 |
| pycparser                  | 677 ms                                                 | 643 ms: 1.05x faster                                                  |
| pickle_pure_python         | 200 us                                                 | 190 us: 1.05x faster                                                  |
| regex_dna                  | 154 ms                                                 | 147 ms: 1.05x faster                                                  |
| pyflate                    | 316 ms                                                 | 301 ms: 1.05x faster                                                  |
| scimark_sor                | 87.4 ms                                                | 83.4 ms: 1.05x faster                                                 |
| sympy_expand               | 241 ms                                                 | 230 ms: 1.05x faster                                                  |
| pathlib                    | 24.2 ms                                                | 23.1 ms: 1.05x faster                                                 |
| unpack_sequence            | 31.5 ns                                                | 30.2 ns: 1.04x faster                                                 |
| pprint_safe_repr           | 497 ms                                                 | 480 ms: 1.04x faster                                                  |
| pickle                     | 7.23 us                                                | 6.98 us: 1.04x faster                                                 |
| pprint_pformat             | 1.01 sec                                               | 977 ms: 1.03x faster                                                  |
| deepcopy                   | 235 us                                                 | 227 us: 1.03x faster                                                  |
| crypto_pyaes               | 51.9 ms                                                | 50.4 ms: 1.03x faster                                                 |
| sympy_str                  | 148 ms                                                 | 144 ms: 1.03x faster                                                  |
| sympy_integrate            | 11.4 ms                                                | 11.1 ms: 1.03x faster                                                 |
| create_gc_cycles           | 701 us                                                 | 686 us: 1.02x faster                                                  |
| fannkuch                   | 248 ms                                                 | 244 ms: 1.02x faster                                                  |
| raytrace                   | 212 ms                                                 | 208 ms: 1.02x faster                                                  |
| nbody                      | 68.8 ms                                                | 67.7 ms: 1.02x faster                                                 |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 521 ms: 1.01x faster                                                  |
| meteor_contest             | 71.7 ms                                                | 71.1 ms: 1.01x faster                                                 |
| gc_traversal               | 2.40 ms                                                | 2.38 ms: 1.01x faster                                                 |
| pidigits                   | 282 ms                                                 | 280 ms: 1.01x faster                                                  |
| float                      | 55.8 ms                                                | 55.5 ms: 1.01x faster                                                 |
| asyncio_websockets         | 409 ms                                                 | 408 ms: 1.00x faster                                                  |
| deepcopy_memo              | 27.7 us                                                | 27.7 us: 1.00x slower                                                 |
| mako                       | 7.71 ms                                                | 7.76 ms: 1.01x slower                                                 |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.26 sec: 1.01x slower                                                |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 543 ms: 1.02x slower                                                  |
| hexiom                     | 4.54 ms                                                | 4.66 ms: 1.03x slower                                                 |
| async_tree_none_tg         | 258 ms                                                 | 266 ms: 1.03x slower                                                  |
| async_tree_memoization     | 312 ms                                                 | 322 ms: 1.03x slower                                                  |
| scimark_monte_carlo        | 45.0 ms                                                | 46.8 ms: 1.04x slower                                                 |
| go                         | 102 ms                                                 | 106 ms: 1.04x slower                                                  |
| sympy_sum                  | 77.6 ms                                                | 81.7 ms: 1.05x slower                                                 |
| async_tree_memoization_tg  | 323 ms                                                 | 340 ms: 1.05x slower                                                  |
| async_tree_none            | 266 ms                                                 | 280 ms: 1.05x slower                                                  |
| async_tree_io_tg           | 669 ms                                                 | 710 ms: 1.06x slower                                                  |
| mdp                        | 1.58 sec                                               | 1.70 sec: 1.07x slower                                                |
| async_tree_io              | 668 ms                                                 | 728 ms: 1.09x slower                                                  |
| sqlglot_transpile          | 1.02 ms                                                | 1.15 ms: 1.12x slower                                                 |
| generators                 | 31.1 ms                                                | 35.1 ms: 1.13x slower                                                 |
| comprehensions             | 14.5 us                                                | 16.6 us: 1.14x slower                                                 |
| sqlglot_parse              | 848 us                                                 | 985 us: 1.16x slower                                                  |
| chaos                      | 42.5 ms                                                | 49.5 ms: 1.16x slower                                                 |
| dask                       | 222 ms                                                 | 309 ms: 1.39x slower                                                  |
| typing_runtime_protocols   | 93.0 us                                                | 320 us: 3.45x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.02x faster                                                          |

Benchmark hidden because not significant (4): asyncio_tcp, richards_super, python_startup, python_startup_no_site
Ignored benchmarks (7) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, coverage, gunicorn, mypy2, sqlalchemy_declarative, sqlalchemy_imperative, tornado_http
Ignored benchmarks (4) of results/bm-20230110-3.12.0a4-3d5d3f7/bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7.json: genshi_text, genshi_xml, html5lib, thrift


# HPT report

- Reliability score: 99.96% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.94x