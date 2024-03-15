
# Results vs. 3.12.0

- fork: python
- ref: 2e49bd06c5ffab7d1540
- machine: darwin-arm64
- commit hash: 2e49bd0
- commit date: 2022-04-05
- overall geometric mean: 1.02x slower \*
- HPT reliability: 96.80%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220405-darwin-arm64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 156 ms: 1.09x faster                                                  |
| chameleon      | 4.70 ms                                                | 4.32 ms: 1.09x faster                                                 |
| docutils       | 1.50 sec                                               | 1.40 sec: 1.08x faster                                                |
| Geometric mean | (ref)                                                  | 1.06x faster                                                          |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220405-darwin-arm64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 526 ms                                                 | 516 ms: 1.02x faster                                                  |
| async_tree_io              | 668 ms                                                 | 693 ms: 1.04x slower                                                  |
| async_tree_none            | 266 ms                                                 | 277 ms: 1.04x slower                                                  |
| async_tree_io_tg           | 669 ms                                                 | 748 ms: 1.12x slower                                                  |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 611 ms: 1.15x slower                                                  |
| async_tree_memoization     | 312 ms                                                 | 361 ms: 1.16x slower                                                  |
| async_tree_none_tg         | 258 ms                                                 | 338 ms: 1.31x slower                                                  |
| async_tree_memoization_tg  | 323 ms                                                 | 436 ms: 1.35x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.14x slower                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220405-darwin-arm64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| float          | 55.8 ms                                                | 49.9 ms: 1.12x faster                                                 |
| nbody          | 68.8 ms                                                | 67.4 ms: 1.02x faster                                                 |
| pidigits       | 282 ms                                                 | 280 ms: 1.01x faster                                                  |
| Geometric mean | (ref)                                                  | 1.05x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220405-darwin-arm64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_effbot   | 2.64 ms                                                | 2.07 ms: 1.27x faster                                                 |
| regex_compile  | 77.9 ms                                                | 73.7 ms: 1.06x faster                                                 |
| regex_dna      | 154 ms                                                 | 175 ms: 1.13x slower                                                  |
| regex_v8       | 16.0 ms                                                | 19.3 ms: 1.21x slower                                                 |
| Geometric mean | (ref)                                                  | 1.01x slower                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220405-darwin-arm64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| xml_etree_generate   | 55.8 ms                                                | 47.0 ms: 1.19x faster                                                 |
| json_loads           | 17.2 us                                                | 14.9 us: 1.15x faster                                                 |
| xml_etree_process    | 39.7 ms                                                | 34.6 ms: 1.15x faster                                                 |
| xml_etree_iterparse  | 74.0 ms                                                | 67.4 ms: 1.10x faster                                                 |
| unpickle             | 9.12 us                                                | 8.31 us: 1.10x faster                                                 |
| xml_etree_parse      | 106 ms                                                 | 97.0 ms: 1.10x faster                                                 |
| pickle_list          | 2.89 us                                                | 2.66 us: 1.08x faster                                                 |
| unpickle_list        | 3.02 us                                                | 2.80 us: 1.08x faster                                                 |
| pickle_pure_python   | 200 us                                                 | 190 us: 1.05x faster                                                  |
| pickle_dict          | 18.1 us                                                | 17.4 us: 1.04x faster                                                 |
| tomli_loads          | 1.39 sec                                               | 1.36 sec: 1.02x faster                                                |
| unpickle_pure_python | 151 us                                                 | 149 us: 1.01x faster                                                  |
| pickle               | 7.23 us                                                | 7.19 us: 1.01x faster                                                 |
| json_dumps           | 6.22 ms                                                | 7.58 ms: 1.22x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.06x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220405-darwin-arm64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup_no_site | 9.37 ms                                                | 9.19 ms: 1.02x faster                                                 |
| python_startup         | 11.4 ms                                                | 11.4 ms: 1.00x faster                                                 |
| Geometric mean         | (ref)                                                  | 1.01x faster                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220405-darwin-arm64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| django_template | 22.3 ms                                                | 20.0 ms: 1.12x faster                                                 |
| mako            | 7.71 ms                                                | 7.05 ms: 1.09x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.11x faster                                                          |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220405-darwin-arm64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_generators           | 304 ms                                                 | 189 ms: 1.61x faster                                                  |
| regex_effbot               | 2.64 ms                                                | 2.07 ms: 1.27x faster                                                 |
| sqlite_synth               | 1.57 us                                                | 1.26 us: 1.24x faster                                                 |
| xml_etree_generate         | 55.8 ms                                                | 47.0 ms: 1.19x faster                                                 |
| telco                      | 3.68 ms                                                | 3.15 ms: 1.17x faster                                                 |
| json_loads                 | 17.2 us                                                | 14.9 us: 1.15x faster                                                 |
| xml_etree_process          | 39.7 ms                                                | 34.6 ms: 1.15x faster                                                 |
| deepcopy_reduce            | 2.07 us                                                | 1.83 us: 1.13x faster                                                 |
| json                       | 3.09 ms                                                | 2.75 ms: 1.12x faster                                                 |
| sqlglot_normalize          | 186 ms                                                 | 166 ms: 1.12x faster                                                  |
| nqueens                    | 62.4 ms                                                | 55.8 ms: 1.12x faster                                                 |
| float                      | 55.8 ms                                                | 49.9 ms: 1.12x faster                                                 |
| django_template            | 22.3 ms                                                | 20.0 ms: 1.12x faster                                                 |
| deepcopy_memo              | 27.7 us                                                | 24.8 us: 1.12x faster                                                 |
| logging_format             | 3.98 us                                                | 3.58 us: 1.11x faster                                                 |
| sqlglot_optimize           | 34.0 ms                                                | 30.7 ms: 1.11x faster                                                 |
| deepcopy                   | 235 us                                                 | 212 us: 1.11x faster                                                  |
| logging_simple             | 3.69 us                                                | 3.35 us: 1.10x faster                                                 |
| xml_etree_iterparse        | 74.0 ms                                                | 67.4 ms: 1.10x faster                                                 |
| unpickle                   | 9.12 us                                                | 8.31 us: 1.10x faster                                                 |
| xml_etree_parse            | 106 ms                                                 | 97.0 ms: 1.10x faster                                                 |
| mako                       | 7.71 ms                                                | 7.05 ms: 1.09x faster                                                 |
| logging_silent             | 76.4 ns                                                | 70.1 ns: 1.09x faster                                                 |
| 2to3                       | 169 ms                                                 | 156 ms: 1.09x faster                                                  |
| chameleon                  | 4.70 ms                                                | 4.32 ms: 1.09x faster                                                 |
| pickle_list                | 2.89 us                                                | 2.66 us: 1.08x faster                                                 |
| bench_mp_pool              | 44.9 ms                                                | 41.5 ms: 1.08x faster                                                 |
| unpickle_list              | 3.02 us                                                | 2.80 us: 1.08x faster                                                 |
| spectral_norm              | 76.4 ms                                                | 70.9 ms: 1.08x faster                                                 |
| docutils                   | 1.50 sec                                               | 1.40 sec: 1.08x faster                                                |
| coroutines                 | 19.2 ms                                                | 17.9 ms: 1.07x faster                                                 |
| scimark_lu                 | 76.0 ms                                                | 71.2 ms: 1.07x faster                                                 |
| pyflate                    | 316 ms                                                 | 297 ms: 1.06x faster                                                  |
| regex_compile              | 77.9 ms                                                | 73.7 ms: 1.06x faster                                                 |
| scimark_sor                | 87.4 ms                                                | 82.8 ms: 1.05x faster                                                 |
| pickle_pure_python         | 200 us                                                 | 190 us: 1.05x faster                                                  |
| pathlib                    | 24.2 ms                                                | 23.1 ms: 1.05x faster                                                 |
| scimark_fft                | 195 ms                                                 | 187 ms: 1.05x faster                                                  |
| pickle_dict                | 18.1 us                                                | 17.4 us: 1.04x faster                                                 |
| bench_thread_pool          | 504 us                                                 | 487 us: 1.03x faster                                                  |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 3.04 ms: 1.03x faster                                                 |
| generators                 | 31.1 ms                                                | 30.1 ms: 1.03x faster                                                 |
| dulwich_log                | 29.8 ms                                                | 28.9 ms: 1.03x faster                                                 |
| sympy_expand               | 241 ms                                                 | 234 ms: 1.03x faster                                                  |
| sympy_str                  | 148 ms                                                 | 144 ms: 1.03x faster                                                  |
| sqlalchemy_declarative     | 62.3 ms                                                | 60.7 ms: 1.03x faster                                                 |
| raytrace                   | 212 ms                                                 | 207 ms: 1.03x faster                                                  |
| richards                   | 32.1 ms                                                | 31.3 ms: 1.03x faster                                                 |
| tomli_loads                | 1.39 sec                                               | 1.36 sec: 1.02x faster                                                |
| nbody                      | 68.8 ms                                                | 67.4 ms: 1.02x faster                                                 |
| python_startup_no_site     | 9.37 ms                                                | 9.19 ms: 1.02x faster                                                 |
| sympy_integrate            | 11.4 ms                                                | 11.2 ms: 1.02x faster                                                 |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 516 ms: 1.02x faster                                                  |
| unpickle_pure_python       | 151 us                                                 | 149 us: 1.01x faster                                                  |
| scimark_monte_carlo        | 45.0 ms                                                | 44.6 ms: 1.01x faster                                                 |
| pprint_safe_repr           | 497 ms                                                 | 492 ms: 1.01x faster                                                  |
| pprint_pformat             | 1.01 sec                                               | 1.00 sec: 1.01x faster                                                |
| gc_traversal               | 2.40 ms                                                | 2.38 ms: 1.01x faster                                                 |
| deltablue                  | 2.71 ms                                                | 2.69 ms: 1.01x faster                                                 |
| pidigits                   | 282 ms                                                 | 280 ms: 1.01x faster                                                  |
| pickle                     | 7.23 us                                                | 7.19 us: 1.01x faster                                                 |
| asyncio_websockets         | 409 ms                                                 | 407 ms: 1.00x faster                                                  |
| python_startup             | 11.4 ms                                                | 11.4 ms: 1.00x faster                                                 |
| create_gc_cycles           | 701 us                                                 | 706 us: 1.01x slower                                                  |
| sympy_sum                  | 77.6 ms                                                | 78.2 ms: 1.01x slower                                                 |
| fannkuch                   | 248 ms                                                 | 254 ms: 1.02x slower                                                  |
| gunicorn                   | 1.15 ms                                                | 1.18 ms: 1.03x slower                                                 |
| crypto_pyaes               | 51.9 ms                                                | 53.4 ms: 1.03x slower                                                 |
| meteor_contest             | 71.7 ms                                                | 73.9 ms: 1.03x slower                                                 |
| go                         | 102 ms                                                 | 105 ms: 1.03x slower                                                  |
| async_tree_io              | 668 ms                                                 | 693 ms: 1.04x slower                                                  |
| async_tree_none            | 266 ms                                                 | 277 ms: 1.04x slower                                                  |
| richards_super             | 36.0 ms                                                | 37.9 ms: 1.05x slower                                                 |
| hexiom                     | 4.54 ms                                                | 4.85 ms: 1.07x slower                                                 |
| unpack_sequence            | 31.5 ns                                                | 33.7 ns: 1.07x slower                                                 |
| sqlalchemy_imperative      | 6.68 ms                                                | 7.31 ms: 1.09x slower                                                 |
| mdp                        | 1.58 sec                                               | 1.76 sec: 1.11x slower                                                |
| async_tree_io_tg           | 669 ms                                                 | 748 ms: 1.12x slower                                                  |
| comprehensions             | 14.5 us                                                | 16.3 us: 1.12x slower                                                 |
| regex_dna                  | 154 ms                                                 | 175 ms: 1.13x slower                                                  |
| chaos                      | 42.5 ms                                                | 48.7 ms: 1.14x slower                                                 |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 611 ms: 1.15x slower                                                  |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.43 sec: 1.15x slower                                                |
| async_tree_memoization     | 312 ms                                                 | 361 ms: 1.16x slower                                                  |
| regex_v8                   | 16.0 ms                                                | 19.3 ms: 1.21x slower                                                 |
| json_dumps                 | 6.22 ms                                                | 7.58 ms: 1.22x slower                                                 |
| sqlglot_transpile          | 1.02 ms                                                | 1.30 ms: 1.27x slower                                                 |
| async_tree_none_tg         | 258 ms                                                 | 338 ms: 1.31x slower                                                  |
| async_tree_memoization_tg  | 323 ms                                                 | 436 ms: 1.35x slower                                                  |
| sqlglot_parse              | 848 us                                                 | 1.15 ms: 1.35x slower                                                 |
| asyncio_tcp                | 449 ms                                                 | 663 ms: 1.48x slower                                                  |
| typing_runtime_protocols   | 93.0 us                                                | 323 us: 3.47x slower                                                  |
| coverage                   | 38.9 ms                                                | 392 ms: 10.09x slower                                                 |
| Geometric mean             | (ref)                                                  | 1.02x slower                                                          |

Benchmark hidden because not significant (3): pycparser, aiohttp, tornado_http
Ignored benchmarks (2) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: dask, mypy2
Ignored benchmarks (6) of results/bm-20220405-3.11.0a7-2e49bd0/bm-20220405-darwin-arm64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 96.80% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.99x