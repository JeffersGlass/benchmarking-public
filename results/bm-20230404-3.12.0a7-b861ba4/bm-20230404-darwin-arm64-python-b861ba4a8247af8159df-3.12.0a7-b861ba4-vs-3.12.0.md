
# Results vs. 3.12.0

- fork: python
- ref: b861ba4a8247af8159df
- machine: darwin-arm64
- commit hash: b861ba4
- commit date: 2023-04-04
- overall geometric mean: 1.03x slower \*
- HPT reliability: 99.90%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-darwin-arm64-python-b861ba4a8247af8159df-3.12.0a7-b861ba4 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 170 ms: 1.00x slower                                                  |
| chameleon      | 4.70 ms                                                | 4.73 ms: 1.01x slower                                                 |
| docutils       | 1.50 sec                                               | 1.51 sec: 1.00x slower                                                |
| Geometric mean | (ref)                                                  | 1.01x slower                                                          |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-darwin-arm64-python-b861ba4a8247af8159df-3.12.0a7-b861ba4 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 526 ms                                                 | 537 ms: 1.02x slower                                                  |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 548 ms: 1.03x slower                                                  |
| async_tree_memoization     | 312 ms                                                 | 325 ms: 1.04x slower                                                  |
| async_tree_none_tg         | 258 ms                                                 | 271 ms: 1.05x slower                                                  |
| async_tree_memoization_tg  | 323 ms                                                 | 343 ms: 1.06x slower                                                  |
| async_tree_io_tg           | 669 ms                                                 | 721 ms: 1.08x slower                                                  |
| async_tree_none            | 266 ms                                                 | 288 ms: 1.08x slower                                                  |
| async_tree_io              | 668 ms                                                 | 740 ms: 1.11x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.06x slower                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-darwin-arm64-python-b861ba4a8247af8159df-3.12.0a7-b861ba4 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| nbody          | 68.8 ms                                                | 64.0 ms: 1.08x faster                                                 |
| float          | 55.8 ms                                                | 54.3 ms: 1.03x faster                                                 |
| Geometric mean | (ref)                                                  | 1.03x faster                                                          |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-darwin-arm64-python-b861ba4a8247af8159df-3.12.0a7-b861ba4 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_effbot   | 2.64 ms                                                | 2.46 ms: 1.08x faster                                                 |
| regex_v8       | 16.0 ms                                                | 15.2 ms: 1.05x faster                                                 |
| regex_dna      | 154 ms                                                 | 148 ms: 1.04x faster                                                  |
| regex_compile  | 77.9 ms                                                | 78.7 ms: 1.01x slower                                                 |
| Geometric mean | (ref)                                                  | 1.04x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-darwin-arm64-python-b861ba4a8247af8159df-3.12.0a7-b861ba4 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| xml_etree_generate   | 55.8 ms                                                | 49.6 ms: 1.12x faster                                                 |
| unpickle_list        | 3.02 us                                                | 2.70 us: 1.12x faster                                                 |
| json_loads           | 17.2 us                                                | 15.8 us: 1.09x faster                                                 |
| unpickle             | 9.12 us                                                | 8.39 us: 1.09x faster                                                 |
| xml_etree_parse      | 106 ms                                                 | 98.6 ms: 1.08x faster                                                 |
| pickle_list          | 2.89 us                                                | 2.76 us: 1.05x faster                                                 |
| pickle_dict          | 18.1 us                                                | 17.3 us: 1.04x faster                                                 |
| json_dumps           | 6.22 ms                                                | 6.01 ms: 1.03x faster                                                 |
| xml_etree_process    | 39.7 ms                                                | 39.0 ms: 1.02x faster                                                 |
| pickle               | 7.23 us                                                | 7.16 us: 1.01x faster                                                 |
| xml_etree_iterparse  | 74.0 ms                                                | 73.5 ms: 1.01x faster                                                 |
| tomli_loads          | 1.39 sec                                               | 1.43 sec: 1.03x slower                                                |
| pickle_pure_python   | 200 us                                                 | 206 us: 1.03x slower                                                  |
| unpickle_pure_python | 151 us                                                 | 158 us: 1.05x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.04x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-darwin-arm64-python-b861ba4a8247af8159df-3.12.0a7-b861ba4 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup_no_site | 9.37 ms                                                | 9.57 ms: 1.02x slower                                                 |
| python_startup         | 11.4 ms                                                | 11.8 ms: 1.03x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.03x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-darwin-arm64-python-b861ba4a8247af8159df-3.12.0a7-b861ba4 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 7.71 ms                                                | 7.17 ms: 1.08x faster                                                 |
| django_template | 22.3 ms                                                | 22.2 ms: 1.01x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.04x faster                                                          |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-darwin-arm64-python-b861ba4a8247af8159df-3.12.0a7-b861ba4 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_generators           | 304 ms                                                 | 260 ms: 1.17x faster                                                  |
| sqlite_synth               | 1.57 us                                                | 1.34 us: 1.17x faster                                                 |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 2.72 ms: 1.15x faster                                                 |
| xml_etree_generate         | 55.8 ms                                                | 49.6 ms: 1.12x faster                                                 |
| telco                      | 3.68 ms                                                | 3.27 ms: 1.12x faster                                                 |
| unpickle_list              | 3.02 us                                                | 2.70 us: 1.12x faster                                                 |
| scimark_fft                | 195 ms                                                 | 177 ms: 1.10x faster                                                  |
| json                       | 3.09 ms                                                | 2.80 ms: 1.10x faster                                                 |
| json_loads                 | 17.2 us                                                | 15.8 us: 1.09x faster                                                 |
| unpickle                   | 9.12 us                                                | 8.39 us: 1.09x faster                                                 |
| xml_etree_parse            | 106 ms                                                 | 98.6 ms: 1.08x faster                                                 |
| nbody                      | 68.8 ms                                                | 64.0 ms: 1.08x faster                                                 |
| mako                       | 7.71 ms                                                | 7.17 ms: 1.08x faster                                                 |
| regex_effbot               | 2.64 ms                                                | 2.46 ms: 1.08x faster                                                 |
| regex_v8                   | 16.0 ms                                                | 15.2 ms: 1.05x faster                                                 |
| pickle_list                | 2.89 us                                                | 2.76 us: 1.05x faster                                                 |
| pickle_dict                | 18.1 us                                                | 17.3 us: 1.04x faster                                                 |
| regex_dna                  | 154 ms                                                 | 148 ms: 1.04x faster                                                  |
| json_dumps                 | 6.22 ms                                                | 6.01 ms: 1.03x faster                                                 |
| sqlglot_optimize           | 34.0 ms                                                | 33.0 ms: 1.03x faster                                                 |
| sqlglot_normalize          | 186 ms                                                 | 181 ms: 1.03x faster                                                  |
| float                      | 55.8 ms                                                | 54.3 ms: 1.03x faster                                                 |
| nqueens                    | 62.4 ms                                                | 61.1 ms: 1.02x faster                                                 |
| dulwich_log                | 29.8 ms                                                | 29.3 ms: 1.02x faster                                                 |
| xml_etree_process          | 39.7 ms                                                | 39.0 ms: 1.02x faster                                                 |
| deepcopy_reduce            | 2.07 us                                                | 2.04 us: 1.02x faster                                                 |
| bench_thread_pool          | 504 us                                                 | 498 us: 1.01x faster                                                  |
| pickle                     | 7.23 us                                                | 7.16 us: 1.01x faster                                                 |
| xml_etree_iterparse        | 74.0 ms                                                | 73.5 ms: 1.01x faster                                                 |
| django_template            | 22.3 ms                                                | 22.2 ms: 1.01x faster                                                 |
| create_gc_cycles           | 701 us                                                 | 698 us: 1.00x faster                                                  |
| asyncio_websockets         | 409 ms                                                 | 408 ms: 1.00x faster                                                  |
| 2to3                       | 169 ms                                                 | 170 ms: 1.00x slower                                                  |
| docutils                   | 1.50 sec                                               | 1.51 sec: 1.00x slower                                                |
| sqlalchemy_declarative     | 62.3 ms                                                | 62.6 ms: 1.00x slower                                                 |
| deepcopy                   | 235 us                                                 | 236 us: 1.00x slower                                                  |
| meteor_contest             | 71.7 ms                                                | 72.3 ms: 1.01x slower                                                 |
| chameleon                  | 4.70 ms                                                | 4.73 ms: 1.01x slower                                                 |
| deepcopy_memo              | 27.7 us                                                | 27.9 us: 1.01x slower                                                 |
| crypto_pyaes               | 51.9 ms                                                | 52.4 ms: 1.01x slower                                                 |
| regex_compile              | 77.9 ms                                                | 78.7 ms: 1.01x slower                                                 |
| hexiom                     | 4.54 ms                                                | 4.60 ms: 1.01x slower                                                 |
| pprint_safe_repr           | 497 ms                                                 | 505 ms: 1.02x slower                                                  |
| logging_silent             | 76.4 ns                                                | 77.7 ns: 1.02x slower                                                 |
| python_startup_no_site     | 9.37 ms                                                | 9.57 ms: 1.02x slower                                                 |
| pprint_pformat             | 1.01 sec                                               | 1.03 sec: 1.02x slower                                                |
| sympy_expand               | 241 ms                                                 | 246 ms: 1.02x slower                                                  |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 537 ms: 1.02x slower                                                  |
| mdp                        | 1.58 sec                                               | 1.62 sec: 1.02x slower                                                |
| deltablue                  | 2.71 ms                                                | 2.77 ms: 1.02x slower                                                 |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 548 ms: 1.03x slower                                                  |
| tomli_loads                | 1.39 sec                                               | 1.43 sec: 1.03x slower                                                |
| pickle_pure_python         | 200 us                                                 | 206 us: 1.03x slower                                                  |
| sympy_str                  | 148 ms                                                 | 152 ms: 1.03x slower                                                  |
| python_startup             | 11.4 ms                                                | 11.8 ms: 1.03x slower                                                 |
| sympy_integrate            | 11.4 ms                                                | 11.8 ms: 1.04x slower                                                 |
| scimark_sor                | 87.4 ms                                                | 90.7 ms: 1.04x slower                                                 |
| async_tree_memoization     | 312 ms                                                 | 325 ms: 1.04x slower                                                  |
| fannkuch                   | 248 ms                                                 | 260 ms: 1.04x slower                                                  |
| unpickle_pure_python       | 151 us                                                 | 158 us: 1.05x slower                                                  |
| pyflate                    | 316 ms                                                 | 332 ms: 1.05x slower                                                  |
| async_tree_none_tg         | 258 ms                                                 | 271 ms: 1.05x slower                                                  |
| raytrace                   | 212 ms                                                 | 223 ms: 1.05x slower                                                  |
| spectral_norm              | 76.4 ms                                                | 80.5 ms: 1.05x slower                                                 |
| logging_format             | 3.98 us                                                | 4.21 us: 1.06x slower                                                 |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.31 sec: 1.06x slower                                                |
| async_tree_memoization_tg  | 323 ms                                                 | 343 ms: 1.06x slower                                                  |
| logging_simple             | 3.69 us                                                | 3.93 us: 1.07x slower                                                 |
| unpack_sequence            | 31.5 ns                                                | 33.6 ns: 1.07x slower                                                 |
| sqlalchemy_imperative      | 6.68 ms                                                | 7.13 ms: 1.07x slower                                                 |
| async_tree_io_tg           | 669 ms                                                 | 721 ms: 1.08x slower                                                  |
| async_tree_none            | 266 ms                                                 | 288 ms: 1.08x slower                                                  |
| richards                   | 32.1 ms                                                | 35.3 ms: 1.10x slower                                                 |
| sympy_sum                  | 77.6 ms                                                | 85.9 ms: 1.11x slower                                                 |
| async_tree_io              | 668 ms                                                 | 740 ms: 1.11x slower                                                  |
| coroutines                 | 19.2 ms                                                | 21.4 ms: 1.11x slower                                                 |
| scimark_lu                 | 76.0 ms                                                | 84.7 ms: 1.12x slower                                                 |
| chaos                      | 42.5 ms                                                | 48.1 ms: 1.13x slower                                                 |
| scimark_monte_carlo        | 45.0 ms                                                | 51.1 ms: 1.14x slower                                                 |
| generators                 | 31.1 ms                                                | 35.4 ms: 1.14x slower                                                 |
| go                         | 102 ms                                                 | 117 ms: 1.15x slower                                                  |
| comprehensions             | 14.5 us                                                | 17.0 us: 1.17x slower                                                 |
| richards_super             | 36.0 ms                                                | 42.3 ms: 1.17x slower                                                 |
| sqlglot_transpile          | 1.02 ms                                                | 1.24 ms: 1.21x slower                                                 |
| sqlglot_parse              | 848 us                                                 | 1.07 ms: 1.26x slower                                                 |
| typing_runtime_protocols   | 93.0 us                                                | 392 us: 4.21x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.03x slower                                                          |

Benchmark hidden because not significant (8): asyncio_tcp, pycparser, pidigits, gc_traversal, dask, pathlib, bench_mp_pool, tornado_http
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, coverage, gunicorn, mypy2
Ignored benchmarks (4) of results/bm-20230404-3.12.0a7-b861ba4/bm-20230404-darwin-arm64-python-b861ba4a8247af8159df-3.12.0a7-b861ba4.json: genshi_text, genshi_xml, html5lib, thrift


# HPT report

- Reliability score: 99.90% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.98x