
# Results vs. 3.12.0

- fork: python
- ref: 3ddfa55df48a67a5972f
- machine: darwin-arm64
- commit hash: 3ddfa55
- commit date: 2022-03-07
- overall geometric mean: 1.08x slower \*
- HPT reliability: 99.77%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220307-darwin-arm64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 164 ms: 1.03x faster                                                  |
| chameleon      | 4.70 ms                                                | 4.55 ms: 1.03x faster                                                 |
| docutils       | 1.50 sec                                               | 1.47 sec: 1.02x faster                                                |
| tornado_http   | 69.3 ms                                                | 73.8 ms: 1.07x slower                                                 |
| Geometric mean | (ref)                                                  | 1.01x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220307-darwin-arm64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 526 ms                                                 | 533 ms: 1.01x slower                                                  |
| async_tree_io              | 668 ms                                                 | 704 ms: 1.05x slower                                                  |
| async_tree_none            | 266 ms                                                 | 287 ms: 1.08x slower                                                  |
| async_tree_memoization     | 312 ms                                                 | 347 ms: 1.11x slower                                                  |
| async_tree_io_tg           | 669 ms                                                 | 761 ms: 1.14x slower                                                  |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 624 ms: 1.17x slower                                                  |
| async_tree_none_tg         | 258 ms                                                 | 350 ms: 1.36x slower                                                  |
| async_tree_memoization_tg  | 323 ms                                                 | 449 ms: 1.39x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.16x slower                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220307-darwin-arm64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| float          | 55.8 ms                                                | 54.8 ms: 1.02x faster                                                 |
| pidigits       | 282 ms                                                 | 281 ms: 1.00x faster                                                  |
| nbody          | 68.8 ms                                                | 74.1 ms: 1.08x slower                                                 |
| Geometric mean | (ref)                                                  | 1.02x slower                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220307-darwin-arm64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_effbot   | 2.64 ms                                                | 2.45 ms: 1.08x faster                                                 |
| regex_compile  | 77.9 ms                                                | 76.7 ms: 1.02x faster                                                 |
| regex_v8       | 16.0 ms                                                | 17.5 ms: 1.10x slower                                                 |
| regex_dna      | 154 ms                                                 | 177 ms: 1.15x slower                                                  |
| Geometric mean | (ref)                                                  | 1.04x slower                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220307-darwin-arm64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| json_loads           | 17.2 us                                                | 14.9 us: 1.16x faster                                                 |
| xml_etree_generate   | 55.8 ms                                                | 48.7 ms: 1.15x faster                                                 |
| pickle_list          | 2.89 us                                                | 2.61 us: 1.10x faster                                                 |
| unpickle_list        | 3.02 us                                                | 2.74 us: 1.10x faster                                                 |
| unpickle             | 9.12 us                                                | 8.29 us: 1.10x faster                                                 |
| xml_etree_parse      | 106 ms                                                 | 97.5 ms: 1.09x faster                                                 |
| xml_etree_process    | 39.7 ms                                                | 36.5 ms: 1.09x faster                                                 |
| xml_etree_iterparse  | 74.0 ms                                                | 69.4 ms: 1.07x faster                                                 |
| pickle_dict          | 18.1 us                                                | 17.3 us: 1.05x faster                                                 |
| tomli_loads          | 1.39 sec                                               | 1.44 sec: 1.03x slower                                                |
| pickle_pure_python   | 200 us                                                 | 214 us: 1.07x slower                                                  |
| unpickle_pure_python | 151 us                                                 | 167 us: 1.11x slower                                                  |
| json_dumps           | 6.22 ms                                                | 7.66 ms: 1.23x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                          |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220307-darwin-arm64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup_no_site | 9.37 ms                                                | 9.28 ms: 1.01x faster                                                 |
| python_startup         | 11.4 ms                                                | 14.8 ms: 1.30x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.13x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220307-darwin-arm64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 7.71 ms                                                | 7.33 ms: 1.05x faster                                                 |
| django_template | 22.3 ms                                                | 21.6 ms: 1.04x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.04x faster                                                          |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220307-darwin-arm64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_generators           | 304 ms                                                 | 194 ms: 1.57x faster                                                  |
| sqlite_synth               | 1.57 us                                                | 1.25 us: 1.26x faster                                                 |
| logging_format             | 3.98 us                                                | 3.43 us: 1.16x faster                                                 |
| json_loads                 | 17.2 us                                                | 14.9 us: 1.16x faster                                                 |
| logging_simple             | 3.69 us                                                | 3.21 us: 1.15x faster                                                 |
| xml_etree_generate         | 55.8 ms                                                | 48.7 ms: 1.15x faster                                                 |
| json                       | 3.09 ms                                                | 2.71 ms: 1.14x faster                                                 |
| pickle_list                | 2.89 us                                                | 2.61 us: 1.10x faster                                                 |
| unpickle_list              | 3.02 us                                                | 2.74 us: 1.10x faster                                                 |
| telco                      | 3.68 ms                                                | 3.34 ms: 1.10x faster                                                 |
| unpickle                   | 9.12 us                                                | 8.29 us: 1.10x faster                                                 |
| sqlglot_normalize          | 186 ms                                                 | 170 ms: 1.09x faster                                                  |
| xml_etree_parse            | 106 ms                                                 | 97.5 ms: 1.09x faster                                                 |
| xml_etree_process          | 39.7 ms                                                | 36.5 ms: 1.09x faster                                                 |
| regex_effbot               | 2.64 ms                                                | 2.45 ms: 1.08x faster                                                 |
| nqueens                    | 62.4 ms                                                | 58.5 ms: 1.07x faster                                                 |
| xml_etree_iterparse        | 74.0 ms                                                | 69.4 ms: 1.07x faster                                                 |
| coroutines                 | 19.2 ms                                                | 18.1 ms: 1.07x faster                                                 |
| deepcopy_reduce            | 2.07 us                                                | 1.95 us: 1.06x faster                                                 |
| sqlglot_optimize           | 34.0 ms                                                | 32.2 ms: 1.06x faster                                                 |
| mako                       | 7.71 ms                                                | 7.33 ms: 1.05x faster                                                 |
| bench_mp_pool              | 44.9 ms                                                | 42.8 ms: 1.05x faster                                                 |
| pathlib                    | 24.2 ms                                                | 23.1 ms: 1.05x faster                                                 |
| pickle_dict                | 18.1 us                                                | 17.3 us: 1.05x faster                                                 |
| django_template            | 22.3 ms                                                | 21.6 ms: 1.04x faster                                                 |
| chameleon                  | 4.70 ms                                                | 4.55 ms: 1.03x faster                                                 |
| 2to3                       | 169 ms                                                 | 164 ms: 1.03x faster                                                  |
| docutils                   | 1.50 sec                                               | 1.47 sec: 1.02x faster                                                |
| deepcopy                   | 235 us                                                 | 229 us: 1.02x faster                                                  |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 3.07 ms: 1.02x faster                                                 |
| float                      | 55.8 ms                                                | 54.8 ms: 1.02x faster                                                 |
| regex_compile              | 77.9 ms                                                | 76.7 ms: 1.02x faster                                                 |
| spectral_norm              | 76.4 ms                                                | 75.5 ms: 1.01x faster                                                 |
| python_startup_no_site     | 9.37 ms                                                | 9.28 ms: 1.01x faster                                                 |
| scimark_monte_carlo        | 45.0 ms                                                | 44.6 ms: 1.01x faster                                                 |
| generators                 | 31.1 ms                                                | 30.8 ms: 1.01x faster                                                 |
| deepcopy_memo              | 27.7 us                                                | 27.5 us: 1.01x faster                                                 |
| scimark_fft                | 195 ms                                                 | 194 ms: 1.01x faster                                                  |
| scimark_lu                 | 76.0 ms                                                | 75.5 ms: 1.01x faster                                                 |
| pidigits                   | 282 ms                                                 | 281 ms: 1.00x faster                                                  |
| gc_traversal               | 2.40 ms                                                | 2.40 ms: 1.00x faster                                                 |
| pyflate                    | 316 ms                                                 | 316 ms: 1.00x slower                                                  |
| dulwich_log                | 29.8 ms                                                | 30.0 ms: 1.00x slower                                                 |
| raytrace                   | 212 ms                                                 | 214 ms: 1.01x slower                                                  |
| bench_thread_pool          | 504 us                                                 | 510 us: 1.01x slower                                                  |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 533 ms: 1.01x slower                                                  |
| scimark_sor                | 87.4 ms                                                | 88.7 ms: 1.02x slower                                                 |
| sympy_str                  | 148 ms                                                 | 150 ms: 1.02x slower                                                  |
| sympy_expand               | 241 ms                                                 | 247 ms: 1.02x slower                                                  |
| sqlalchemy_declarative     | 62.3 ms                                                | 63.8 ms: 1.02x slower                                                 |
| create_gc_cycles           | 701 us                                                 | 720 us: 1.03x slower                                                  |
| tomli_loads                | 1.39 sec                                               | 1.44 sec: 1.03x slower                                                |
| sympy_integrate            | 11.4 ms                                                | 11.7 ms: 1.03x slower                                                 |
| meteor_contest             | 71.7 ms                                                | 74.1 ms: 1.03x slower                                                 |
| aiohttp                    | 1.08 ms                                                | 1.12 ms: 1.04x slower                                                 |
| logging_silent             | 76.4 ns                                                | 80.3 ns: 1.05x slower                                                 |
| pycparser                  | 677 ms                                                 | 711 ms: 1.05x slower                                                  |
| hexiom                     | 4.54 ms                                                | 4.78 ms: 1.05x slower                                                 |
| async_tree_io              | 668 ms                                                 | 704 ms: 1.05x slower                                                  |
| sympy_sum                  | 77.6 ms                                                | 82.0 ms: 1.06x slower                                                 |
| gunicorn                   | 1.15 ms                                                | 1.21 ms: 1.06x slower                                                 |
| fannkuch                   | 248 ms                                                 | 264 ms: 1.06x slower                                                  |
| tornado_http               | 69.3 ms                                                | 73.8 ms: 1.07x slower                                                 |
| crypto_pyaes               | 51.9 ms                                                | 55.4 ms: 1.07x slower                                                 |
| pickle_pure_python         | 200 us                                                 | 214 us: 1.07x slower                                                  |
| nbody                      | 68.8 ms                                                | 74.1 ms: 1.08x slower                                                 |
| async_tree_none            | 266 ms                                                 | 287 ms: 1.08x slower                                                  |
| pprint_safe_repr           | 497 ms                                                 | 538 ms: 1.08x slower                                                  |
| richards                   | 32.1 ms                                                | 34.9 ms: 1.09x slower                                                 |
| pprint_pformat             | 1.01 sec                                               | 1.10 sec: 1.09x slower                                                |
| regex_v8                   | 16.0 ms                                                | 17.5 ms: 1.10x slower                                                 |
| go                         | 102 ms                                                 | 112 ms: 1.10x slower                                                  |
| unpickle_pure_python       | 151 us                                                 | 167 us: 1.11x slower                                                  |
| chaos                      | 42.5 ms                                                | 47.2 ms: 1.11x slower                                                 |
| async_tree_memoization     | 312 ms                                                 | 347 ms: 1.11x slower                                                  |
| deltablue                  | 2.71 ms                                                | 3.03 ms: 1.12x slower                                                 |
| mdp                        | 1.58 sec                                               | 1.80 sec: 1.14x slower                                                |
| async_tree_io_tg           | 669 ms                                                 | 761 ms: 1.14x slower                                                  |
| regex_dna                  | 154 ms                                                 | 177 ms: 1.15x slower                                                  |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.44 sec: 1.15x slower                                                |
| sqlalchemy_imperative      | 6.68 ms                                                | 7.72 ms: 1.16x slower                                                 |
| richards_super             | 36.0 ms                                                | 41.9 ms: 1.16x slower                                                 |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 624 ms: 1.17x slower                                                  |
| comprehensions             | 14.5 us                                                | 17.1 us: 1.17x slower                                                 |
| json_dumps                 | 6.22 ms                                                | 7.66 ms: 1.23x slower                                                 |
| python_startup             | 11.4 ms                                                | 14.8 ms: 1.30x slower                                                 |
| async_tree_none_tg         | 258 ms                                                 | 350 ms: 1.36x slower                                                  |
| sqlglot_transpile          | 1.02 ms                                                | 1.40 ms: 1.37x slower                                                 |
| dask                       | 222 ms                                                 | 308 ms: 1.39x slower                                                  |
| async_tree_memoization_tg  | 323 ms                                                 | 449 ms: 1.39x slower                                                  |
| sqlglot_parse              | 848 us                                                 | 1.23 ms: 1.45x slower                                                 |
| asyncio_tcp                | 449 ms                                                 | 663 ms: 1.48x slower                                                  |
| unpack_sequence            | 31.5 ns                                                | 93.6 ns: 2.98x slower                                                 |
| typing_runtime_protocols   | 93.0 us                                                | 330 us: 3.55x slower                                                  |
| coverage                   | 38.9 ms                                                | 328 ms: 8.43x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.08x slower                                                          |

Benchmark hidden because not significant (1): pickle
Ignored benchmarks (2) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: asyncio_websockets, mypy2
Ignored benchmarks (6) of results/bm-20220307-3.11.0a6-3ddfa55/bm-20220307-darwin-arm64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 99.77% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.01x