
# Results vs. 3.12.0

- fork: python
- ref: 1ae7ceba29771baf8f2e
- machine: darwin-arm64
- commit hash: 1ae7ceb
- commit date: 2024-01-04
- overall geometric mean: 1.01x slower
- HPT reliability: 99.13%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 173 ms: 1.02x slower                                                   |
| chameleon      | 4.70 ms                                                | 4.81 ms: 1.03x slower                                                  |
| docutils       | 1.50 sec                                               | 1.49 sec: 1.01x faster                                                 |
| Geometric mean | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none        | 266 ms                                                 | 250 ms: 1.06x faster                                                   |
| async_tree_io_tg       | 669 ms                                                 | 672 ms: 1.00x slower                                                   |
| async_tree_none_tg     | 258 ms                                                 | 259 ms: 1.01x slower                                                   |
| async_tree_memoization | 312 ms                                                 | 328 ms: 1.05x slower                                                   |
| async_tree_io          | 668 ms                                                 | 709 ms: 1.06x slower                                                   |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (3): async_tree_cpu_io_mixed, async_tree_memoization_tg, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 282 ms                                                 | 283 ms: 1.00x slower                                                   |
| float          | 55.8 ms                                                | 57.9 ms: 1.04x slower                                                  |
| nbody          | 68.8 ms                                                | 79.0 ms: 1.15x slower                                                  |
| Geometric mean | (ref)                                                  | 1.06x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 2.64 ms                                                | 2.49 ms: 1.06x faster                                                  |
| regex_compile  | 77.9 ms                                                | 73.9 ms: 1.05x faster                                                  |
| regex_dna      | 154 ms                                                 | 148 ms: 1.04x faster                                                   |
| regex_v8       | 16.0 ms                                                | 16.9 ms: 1.06x slower                                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 200 us                                                 | 198 us: 1.01x faster                                                   |
| pickle_dict          | 18.1 us                                                | 17.9 us: 1.01x faster                                                  |
| xml_etree_process    | 39.7 ms                                                | 40.0 ms: 1.01x slower                                                  |
| xml_etree_generate   | 55.8 ms                                                | 56.7 ms: 1.02x slower                                                  |
| unpickle             | 9.12 us                                                | 9.33 us: 1.02x slower                                                  |
| xml_etree_iterparse  | 74.0 ms                                                | 76.1 ms: 1.03x slower                                                  |
| pickle               | 7.23 us                                                | 7.49 us: 1.04x slower                                                  |
| unpickle_list        | 3.02 us                                                | 3.15 us: 1.04x slower                                                  |
| unpickle_pure_python | 151 us                                                 | 157 us: 1.05x slower                                                   |
| json_dumps           | 6.22 ms                                                | 6.60 ms: 1.06x slower                                                  |
| tomli_loads          | 1.39 sec                                               | 1.58 sec: 1.13x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.03x slower                                                           |

Benchmark hidden because not significant (3): pickle_list, json_loads, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 13.4 ms: 1.17x slower                                                  |
| python_startup_no_site | 9.37 ms                                                | 12.0 ms: 1.28x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.22x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 7.71 ms                                                | 7.61 ms: 1.01x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 93.0 us                                                | 73.6 us: 1.26x faster                                                  |
| generators               | 31.1 ms                                                | 24.8 ms: 1.25x faster                                                  |
| raytrace                 | 212 ms                                                 | 174 ms: 1.22x faster                                                   |
| comprehensions           | 14.5 us                                                | 12.2 us: 1.19x faster                                                  |
| unpack_sequence          | 31.5 ns                                                | 26.6 ns: 1.18x faster                                                  |
| deepcopy_memo            | 27.7 us                                                | 24.9 us: 1.11x faster                                                  |
| deltablue                | 2.71 ms                                                | 2.47 ms: 1.10x faster                                                  |
| coroutines               | 19.2 ms                                                | 17.8 ms: 1.08x faster                                                  |
| crypto_pyaes             | 51.9 ms                                                | 48.2 ms: 1.08x faster                                                  |
| logging_silent           | 76.4 ns                                                | 71.1 ns: 1.07x faster                                                  |
| chaos                    | 42.5 ms                                                | 40.0 ms: 1.06x faster                                                  |
| async_tree_none          | 266 ms                                                 | 250 ms: 1.06x faster                                                   |
| regex_effbot             | 2.64 ms                                                | 2.49 ms: 1.06x faster                                                  |
| regex_compile            | 77.9 ms                                                | 73.9 ms: 1.05x faster                                                  |
| logging_simple           | 3.69 us                                                | 3.53 us: 1.04x faster                                                  |
| regex_dna                | 154 ms                                                 | 148 ms: 1.04x faster                                                   |
| sqlglot_parse            | 848 us                                                 | 818 us: 1.04x faster                                                   |
| logging_format           | 3.98 us                                                | 3.84 us: 1.04x faster                                                  |
| sympy_integrate          | 11.4 ms                                                | 11.0 ms: 1.03x faster                                                  |
| sympy_sum                | 77.6 ms                                                | 75.1 ms: 1.03x faster                                                  |
| spectral_norm            | 76.4 ms                                                | 74.0 ms: 1.03x faster                                                  |
| deepcopy                 | 235 us                                                 | 229 us: 1.03x faster                                                   |
| nqueens                  | 62.4 ms                                                | 61.0 ms: 1.02x faster                                                  |
| sqlglot_transpile        | 1.02 ms                                                | 1000 us: 1.02x faster                                                  |
| sympy_str                | 148 ms                                                 | 145 ms: 1.02x faster                                                   |
| json                     | 3.09 ms                                                | 3.03 ms: 1.02x faster                                                  |
| mako                     | 7.71 ms                                                | 7.61 ms: 1.01x faster                                                  |
| hexiom                   | 4.54 ms                                                | 4.49 ms: 1.01x faster                                                  |
| pickle_pure_python       | 200 us                                                 | 198 us: 1.01x faster                                                   |
| dulwich_log              | 29.8 ms                                                | 29.6 ms: 1.01x faster                                                  |
| pickle_dict              | 18.1 us                                                | 17.9 us: 1.01x faster                                                  |
| docutils                 | 1.50 sec                                               | 1.49 sec: 1.01x faster                                                 |
| async_generators         | 304 ms                                                 | 302 ms: 1.01x faster                                                   |
| deepcopy_reduce          | 2.07 us                                                | 2.06 us: 1.01x faster                                                  |
| pidigits                 | 282 ms                                                 | 283 ms: 1.00x slower                                                   |
| async_tree_io_tg         | 669 ms                                                 | 672 ms: 1.00x slower                                                   |
| sqlglot_normalize        | 186 ms                                                 | 187 ms: 1.01x slower                                                   |
| async_tree_none_tg       | 258 ms                                                 | 259 ms: 1.01x slower                                                   |
| xml_etree_process        | 39.7 ms                                                | 40.0 ms: 1.01x slower                                                  |
| xml_etree_generate       | 55.8 ms                                                | 56.7 ms: 1.02x slower                                                  |
| pathlib                  | 24.2 ms                                                | 24.6 ms: 1.02x slower                                                  |
| bench_mp_pool            | 44.9 ms                                                | 45.6 ms: 1.02x slower                                                  |
| asyncio_tcp_ssl          | 1.24 sec                                               | 1.27 sec: 1.02x slower                                                 |
| bench_thread_pool        | 504 us                                                 | 514 us: 1.02x slower                                                   |
| dask                     | 222 ms                                                 | 227 ms: 1.02x slower                                                   |
| 2to3                     | 169 ms                                                 | 173 ms: 1.02x slower                                                   |
| unpickle                 | 9.12 us                                                | 9.33 us: 1.02x slower                                                  |
| chameleon                | 4.70 ms                                                | 4.81 ms: 1.03x slower                                                  |
| sqlglot_optimize         | 34.0 ms                                                | 34.9 ms: 1.03x slower                                                  |
| xml_etree_iterparse      | 74.0 ms                                                | 76.1 ms: 1.03x slower                                                  |
| go                       | 102 ms                                                 | 104 ms: 1.03x slower                                                   |
| meteor_contest           | 71.7 ms                                                | 74.0 ms: 1.03x slower                                                  |
| mdp                      | 1.58 sec                                               | 1.63 sec: 1.03x slower                                                 |
| pickle                   | 7.23 us                                                | 7.49 us: 1.04x slower                                                  |
| pycparser                | 677 ms                                                 | 702 ms: 1.04x slower                                                   |
| float                    | 55.8 ms                                                | 57.9 ms: 1.04x slower                                                  |
| sympy_expand             | 241 ms                                                 | 251 ms: 1.04x slower                                                   |
| richards_super           | 36.0 ms                                                | 37.5 ms: 1.04x slower                                                  |
| unpickle_list            | 3.02 us                                                | 3.15 us: 1.04x slower                                                  |
| unpickle_pure_python     | 151 us                                                 | 157 us: 1.05x slower                                                   |
| async_tree_memoization   | 312 ms                                                 | 328 ms: 1.05x slower                                                   |
| scimark_fft              | 195 ms                                                 | 205 ms: 1.05x slower                                                   |
| sqlite_synth             | 1.57 us                                                | 1.66 us: 1.06x slower                                                  |
| richards                 | 32.1 ms                                                | 34.0 ms: 1.06x slower                                                  |
| regex_v8                 | 16.0 ms                                                | 16.9 ms: 1.06x slower                                                  |
| pprint_pformat           | 1.01 sec                                               | 1.07 sec: 1.06x slower                                                 |
| scimark_monte_carlo      | 45.0 ms                                                | 47.7 ms: 1.06x slower                                                  |
| json_dumps               | 6.22 ms                                                | 6.60 ms: 1.06x slower                                                  |
| async_tree_io            | 668 ms                                                 | 709 ms: 1.06x slower                                                   |
| pprint_safe_repr         | 497 ms                                                 | 529 ms: 1.06x slower                                                   |
| pyflate                  | 316 ms                                                 | 343 ms: 1.09x slower                                                   |
| tomli_loads              | 1.39 sec                                               | 1.58 sec: 1.13x slower                                                 |
| nbody                    | 68.8 ms                                                | 79.0 ms: 1.15x slower                                                  |
| python_startup           | 11.4 ms                                                | 13.4 ms: 1.17x slower                                                  |
| fannkuch                 | 248 ms                                                 | 295 ms: 1.19x slower                                                   |
| scimark_sor              | 87.4 ms                                                | 107 ms: 1.22x slower                                                   |
| coverage                 | 38.9 ms                                                | 49.3 ms: 1.27x slower                                                  |
| python_startup_no_site   | 9.37 ms                                                | 12.0 ms: 1.28x slower                                                  |
| telco                    | 3.68 ms                                                | 4.74 ms: 1.29x slower                                                  |
| mypy2                    | 380 ms                                                 | 521 ms: 1.37x slower                                                   |
| Geometric mean           | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (13): asyncio_tcp, async_tree_cpu_io_mixed, async_tree_memoization_tg, pickle_list, scimark_lu, asyncio_websockets, scimark_sparse_mat_mult, gc_traversal, async_tree_cpu_io_mixed_tg, json_loads, create_gc_cycles, tornado_http, xml_etree_parse
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.13% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x