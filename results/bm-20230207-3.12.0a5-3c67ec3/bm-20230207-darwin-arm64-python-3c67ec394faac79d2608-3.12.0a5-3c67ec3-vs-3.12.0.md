
# Results vs. 3.12.0

- fork: python
- ref: 3c67ec394faac79d2608
- machine: darwin-arm64
- commit hash: 3c67ec3
- commit date: 2023-02-07
- overall geometric mean: 1.03x slower \*
- HPT reliability: 95.35%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.95x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 166 ms: 1.02x faster                                                  |
| docutils       | 1.50 sec                                               | 1.48 sec: 1.01x faster                                                |
| tornado_http   | 69.3 ms                                                | 72.3 ms: 1.04x slower                                                 |
| Geometric mean | (ref)                                                  | 1.00x slower                                                          |

Benchmark hidden because not significant (1): chameleon

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 526 ms                                                 | 533 ms: 1.01x slower                                                  |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 555 ms: 1.04x slower                                                  |
| async_tree_memoization     | 312 ms                                                 | 336 ms: 1.08x slower                                                  |
| async_tree_memoization_tg  | 323 ms                                                 | 351 ms: 1.09x slower                                                  |
| async_tree_none_tg         | 258 ms                                                 | 281 ms: 1.09x slower                                                  |
| async_tree_none            | 266 ms                                                 | 290 ms: 1.09x slower                                                  |
| async_tree_io_tg           | 669 ms                                                 | 739 ms: 1.10x slower                                                  |
| async_tree_io              | 668 ms                                                 | 753 ms: 1.13x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.08x slower                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| nbody          | 68.8 ms                                                | 68.5 ms: 1.00x faster                                                 |
| pidigits       | 282 ms                                                 | 281 ms: 1.00x faster                                                  |
| float          | 55.8 ms                                                | 57.5 ms: 1.03x slower                                                 |
| Geometric mean | (ref)                                                  | 1.01x slower                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_effbot   | 2.64 ms                                                | 2.45 ms: 1.08x faster                                                 |
| regex_dna      | 154 ms                                                 | 147 ms: 1.05x faster                                                  |
| regex_v8       | 16.0 ms                                                | 15.3 ms: 1.04x faster                                                 |
| regex_compile  | 77.9 ms                                                | 76.0 ms: 1.02x faster                                                 |
| Geometric mean | (ref)                                                  | 1.05x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| xml_etree_generate   | 55.8 ms                                                | 48.7 ms: 1.15x faster                                                 |
| xml_etree_parse      | 106 ms                                                 | 95.0 ms: 1.12x faster                                                 |
| json_loads           | 17.2 us                                                | 15.7 us: 1.10x faster                                                 |
| unpickle             | 9.12 us                                                | 8.50 us: 1.07x faster                                                 |
| pickle_dict          | 18.1 us                                                | 16.8 us: 1.07x faster                                                 |
| xml_etree_process    | 39.7 ms                                                | 37.1 ms: 1.07x faster                                                 |
| pickle_list          | 2.89 us                                                | 2.72 us: 1.06x faster                                                 |
| unpickle_list        | 3.02 us                                                | 2.85 us: 1.06x faster                                                 |
| xml_etree_iterparse  | 74.0 ms                                                | 71.9 ms: 1.03x faster                                                 |
| json_dumps           | 6.22 ms                                                | 6.08 ms: 1.02x faster                                                 |
| pickle               | 7.23 us                                                | 7.09 us: 1.02x faster                                                 |
| tomli_loads          | 1.39 sec                                               | 1.38 sec: 1.01x faster                                                |
| unpickle_pure_python | 151 us                                                 | 161 us: 1.07x slower                                                  |
| pickle_pure_python   | 200 us                                                 | 214 us: 1.07x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.04x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup_no_site | 9.37 ms                                                | 9.55 ms: 1.02x slower                                                 |
| python_startup         | 11.4 ms                                                | 11.8 ms: 1.03x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.03x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 7.71 ms                                                | 6.94 ms: 1.11x faster                                                 |
| django_template | 22.3 ms                                                | 22.5 ms: 1.01x slower                                                 |
| Geometric mean  | (ref)                                                  | 1.05x faster                                                          |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_generators           | 304 ms                                                 | 209 ms: 1.45x faster                                                  |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 2.70 ms: 1.16x faster                                                 |
| telco                      | 3.68 ms                                                | 3.18 ms: 1.16x faster                                                 |
| xml_etree_generate         | 55.8 ms                                                | 48.7 ms: 1.15x faster                                                 |
| sqlite_synth               | 1.57 us                                                | 1.40 us: 1.12x faster                                                 |
| xml_etree_parse            | 106 ms                                                 | 95.0 ms: 1.12x faster                                                 |
| mako                       | 7.71 ms                                                | 6.94 ms: 1.11x faster                                                 |
| json                       | 3.09 ms                                                | 2.79 ms: 1.11x faster                                                 |
| json_loads                 | 17.2 us                                                | 15.7 us: 1.10x faster                                                 |
| regex_effbot               | 2.64 ms                                                | 2.45 ms: 1.08x faster                                                 |
| unpickle                   | 9.12 us                                                | 8.50 us: 1.07x faster                                                 |
| pickle_dict                | 18.1 us                                                | 16.8 us: 1.07x faster                                                 |
| xml_etree_process          | 39.7 ms                                                | 37.1 ms: 1.07x faster                                                 |
| scimark_fft                | 195 ms                                                 | 183 ms: 1.06x faster                                                  |
| pickle_list                | 2.89 us                                                | 2.72 us: 1.06x faster                                                 |
| unpickle_list              | 3.02 us                                                | 2.85 us: 1.06x faster                                                 |
| regex_dna                  | 154 ms                                                 | 147 ms: 1.05x faster                                                  |
| pathlib                    | 24.2 ms                                                | 23.2 ms: 1.05x faster                                                 |
| regex_v8                   | 16.0 ms                                                | 15.3 ms: 1.04x faster                                                 |
| nqueens                    | 62.4 ms                                                | 59.9 ms: 1.04x faster                                                 |
| xml_etree_iterparse        | 74.0 ms                                                | 71.9 ms: 1.03x faster                                                 |
| sqlglot_optimize           | 34.0 ms                                                | 33.1 ms: 1.03x faster                                                 |
| bench_mp_pool              | 44.9 ms                                                | 43.7 ms: 1.03x faster                                                 |
| regex_compile              | 77.9 ms                                                | 76.0 ms: 1.02x faster                                                 |
| sqlglot_normalize          | 186 ms                                                 | 181 ms: 1.02x faster                                                  |
| json_dumps                 | 6.22 ms                                                | 6.08 ms: 1.02x faster                                                 |
| dulwich_log                | 29.8 ms                                                | 29.2 ms: 1.02x faster                                                 |
| create_gc_cycles           | 701 us                                                 | 687 us: 1.02x faster                                                  |
| 2to3                       | 169 ms                                                 | 166 ms: 1.02x faster                                                  |
| bench_thread_pool          | 504 us                                                 | 495 us: 1.02x faster                                                  |
| pickle                     | 7.23 us                                                | 7.09 us: 1.02x faster                                                 |
| docutils                   | 1.50 sec                                               | 1.48 sec: 1.01x faster                                                |
| tomli_loads                | 1.39 sec                                               | 1.38 sec: 1.01x faster                                                |
| pycparser                  | 677 ms                                                 | 670 ms: 1.01x faster                                                  |
| fannkuch                   | 248 ms                                                 | 246 ms: 1.01x faster                                                  |
| comprehensions             | 14.5 us                                                | 14.5 us: 1.01x faster                                                 |
| crypto_pyaes               | 51.9 ms                                                | 51.6 ms: 1.01x faster                                                 |
| gc_traversal               | 2.40 ms                                                | 2.39 ms: 1.01x faster                                                 |
| nbody                      | 68.8 ms                                                | 68.5 ms: 1.00x faster                                                 |
| pidigits                   | 282 ms                                                 | 281 ms: 1.00x faster                                                  |
| asyncio_websockets         | 409 ms                                                 | 409 ms: 1.00x faster                                                  |
| sqlalchemy_declarative     | 62.3 ms                                                | 62.6 ms: 1.00x slower                                                 |
| django_template            | 22.3 ms                                                | 22.5 ms: 1.01x slower                                                 |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 533 ms: 1.01x slower                                                  |
| sympy_integrate            | 11.4 ms                                                | 11.5 ms: 1.01x slower                                                 |
| hexiom                     | 4.54 ms                                                | 4.61 ms: 1.01x slower                                                 |
| sympy_expand               | 241 ms                                                 | 245 ms: 1.02x slower                                                  |
| python_startup_no_site     | 9.37 ms                                                | 9.55 ms: 1.02x slower                                                 |
| pyflate                    | 316 ms                                                 | 324 ms: 1.03x slower                                                  |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.28 sec: 1.03x slower                                                |
| float                      | 55.8 ms                                                | 57.5 ms: 1.03x slower                                                 |
| python_startup             | 11.4 ms                                                | 11.8 ms: 1.03x slower                                                 |
| deepcopy_memo              | 27.7 us                                                | 28.6 us: 1.03x slower                                                 |
| deltablue                  | 2.71 ms                                                | 2.81 ms: 1.04x slower                                                 |
| deepcopy_reduce            | 2.07 us                                                | 2.15 us: 1.04x slower                                                 |
| scimark_sor                | 87.4 ms                                                | 90.7 ms: 1.04x slower                                                 |
| richards                   | 32.1 ms                                                | 33.5 ms: 1.04x slower                                                 |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 555 ms: 1.04x slower                                                  |
| tornado_http               | 69.3 ms                                                | 72.3 ms: 1.04x slower                                                 |
| deepcopy                   | 235 us                                                 | 246 us: 1.05x slower                                                  |
| pprint_safe_repr           | 497 ms                                                 | 524 ms: 1.05x slower                                                  |
| logging_simple             | 3.69 us                                                | 3.89 us: 1.06x slower                                                 |
| logging_format             | 3.98 us                                                | 4.21 us: 1.06x slower                                                 |
| pprint_pformat             | 1.01 sec                                               | 1.07 sec: 1.06x slower                                                |
| unpack_sequence            | 31.5 ns                                                | 33.4 ns: 1.06x slower                                                 |
| sympy_sum                  | 77.6 ms                                                | 82.4 ms: 1.06x slower                                                 |
| unpickle_pure_python       | 151 us                                                 | 161 us: 1.07x slower                                                  |
| pickle_pure_python         | 200 us                                                 | 214 us: 1.07x slower                                                  |
| spectral_norm              | 76.4 ms                                                | 81.8 ms: 1.07x slower                                                 |
| coroutines                 | 19.2 ms                                                | 20.6 ms: 1.07x slower                                                 |
| async_tree_memoization     | 312 ms                                                 | 336 ms: 1.08x slower                                                  |
| meteor_contest             | 71.7 ms                                                | 77.2 ms: 1.08x slower                                                 |
| raytrace                   | 212 ms                                                 | 229 ms: 1.08x slower                                                  |
| logging_silent             | 76.4 ns                                                | 83.0 ns: 1.09x slower                                                 |
| async_tree_memoization_tg  | 323 ms                                                 | 351 ms: 1.09x slower                                                  |
| async_tree_none_tg         | 258 ms                                                 | 281 ms: 1.09x slower                                                  |
| async_tree_none            | 266 ms                                                 | 290 ms: 1.09x slower                                                  |
| sqlalchemy_imperative      | 6.68 ms                                                | 7.32 ms: 1.09x slower                                                 |
| scimark_lu                 | 76.0 ms                                                | 83.3 ms: 1.10x slower                                                 |
| async_tree_io_tg           | 669 ms                                                 | 739 ms: 1.10x slower                                                  |
| mdp                        | 1.58 sec                                               | 1.76 sec: 1.11x slower                                                |
| go                         | 102 ms                                                 | 113 ms: 1.12x slower                                                  |
| richards_super             | 36.0 ms                                                | 40.4 ms: 1.12x slower                                                 |
| async_tree_io              | 668 ms                                                 | 753 ms: 1.13x slower                                                  |
| chaos                      | 42.5 ms                                                | 48.4 ms: 1.14x slower                                                 |
| scimark_monte_carlo        | 45.0 ms                                                | 52.9 ms: 1.17x slower                                                 |
| sqlglot_transpile          | 1.02 ms                                                | 1.23 ms: 1.20x slower                                                 |
| generators                 | 31.1 ms                                                | 38.6 ms: 1.24x slower                                                 |
| sqlglot_parse              | 848 us                                                 | 1.05 ms: 1.24x slower                                                 |
| dask                       | 222 ms                                                 | 327 ms: 1.47x slower                                                  |
| typing_runtime_protocols   | 93.0 us                                                | 319 us: 3.43x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.03x slower                                                          |

Benchmark hidden because not significant (3): asyncio_tcp, chameleon, sympy_str
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, coverage, gunicorn, mypy2
Ignored benchmarks (4) of results/bm-20230207-3.12.0a5-3c67ec3/bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3.json: genshi_text, genshi_xml, html5lib, thrift


# HPT report

- Reliability score: 95.35% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.95x