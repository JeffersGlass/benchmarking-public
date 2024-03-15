
# Results vs. 3.12.0

- fork: python
- ref: b905fad83819ec9102ec
- machine: darwin-arm64
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.01x slower
- HPT reliability: 99.14%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.15x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 174 ms: 1.03x slower                                                   |
| chameleon      | 4.70 ms                                                | 4.89 ms: 1.04x slower                                                  |
| docutils       | 1.50 sec                                               | 1.48 sec: 1.02x faster                                                 |
| Geometric mean | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 266 ms                                                 | 252 ms: 1.06x faster                                                   |
| async_tree_cpu_io_mixed | 526 ms                                                 | 519 ms: 1.01x faster                                                   |
| async_tree_io_tg        | 669 ms                                                 | 665 ms: 1.01x faster                                                   |
| async_tree_none_tg      | 258 ms                                                 | 259 ms: 1.01x slower                                                   |
| async_tree_io           | 668 ms                                                 | 696 ms: 1.04x slower                                                   |
| async_tree_memoization  | 312 ms                                                 | 327 ms: 1.05x slower                                                   |
| Geometric mean          | (ref)                                                  | 1.00x slower                                                           |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 282 ms                                                 | 283 ms: 1.00x slower                                                   |
| nbody          | 68.8 ms                                                | 76.8 ms: 1.12x slower                                                  |
| Geometric mean | (ref)                                                  | 1.04x slower                                                           |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 2.64 ms                                                | 2.55 ms: 1.03x faster                                                  |
| regex_compile  | 77.9 ms                                                | 76.3 ms: 1.02x faster                                                  |
| regex_dna      | 154 ms                                                 | 152 ms: 1.02x faster                                                   |
| regex_v8       | 16.0 ms                                                | 17.1 ms: 1.07x slower                                                  |
| Geometric mean | (ref)                                                  | 1.00x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_loads           | 17.2 us                                                | 16.9 us: 1.02x faster                                                  |
| pickle_pure_python   | 200 us                                                 | 197 us: 1.02x faster                                                   |
| unpickle             | 9.12 us                                                | 9.02 us: 1.01x faster                                                  |
| xml_etree_process    | 39.7 ms                                                | 39.6 ms: 1.00x faster                                                  |
| tomli_loads          | 1.39 sec                                               | 1.40 sec: 1.00x slower                                                 |
| xml_etree_generate   | 55.8 ms                                                | 56.2 ms: 1.01x slower                                                  |
| pickle               | 7.23 us                                                | 7.31 us: 1.01x slower                                                  |
| xml_etree_parse      | 106 ms                                                 | 108 ms: 1.01x slower                                                   |
| pickle_dict          | 18.1 us                                                | 18.3 us: 1.01x slower                                                  |
| unpickle_list        | 3.02 us                                                | 3.08 us: 1.02x slower                                                  |
| xml_etree_iterparse  | 74.0 ms                                                | 76.2 ms: 1.03x slower                                                  |
| pickle_list          | 2.89 us                                                | 2.98 us: 1.03x slower                                                  |
| json_dumps           | 6.22 ms                                                | 6.51 ms: 1.05x slower                                                  |
| unpickle_pure_python | 151 us                                                 | 158 us: 1.05x slower                                                   |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 13.2 ms: 1.15x slower                                                  |
| python_startup_no_site | 9.37 ms                                                | 11.8 ms: 1.26x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.21x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 7.71 ms                                                | 7.94 ms: 1.03x slower                                                  |

All benchmarks:
===============

| Benchmark                | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 93.0 us                                                | 72.0 us: 1.29x faster                                                  |
| raytrace                 | 212 ms                                                 | 177 ms: 1.20x faster                                                   |
| comprehensions           | 14.5 us                                                | 12.7 us: 1.14x faster                                                  |
| unpack_sequence          | 31.5 ns                                                | 28.2 ns: 1.11x faster                                                  |
| generators               | 31.1 ms                                                | 27.9 ms: 1.11x faster                                                  |
| logging_silent           | 76.4 ns                                                | 70.7 ns: 1.08x faster                                                  |
| deltablue                | 2.71 ms                                                | 2.51 ms: 1.08x faster                                                  |
| deepcopy_memo            | 27.7 us                                                | 25.9 us: 1.07x faster                                                  |
| sqlglot_parse            | 848 us                                                 | 799 us: 1.06x faster                                                   |
| logging_simple           | 3.69 us                                                | 3.48 us: 1.06x faster                                                  |
| async_tree_none          | 266 ms                                                 | 252 ms: 1.06x faster                                                   |
| crypto_pyaes             | 51.9 ms                                                | 49.2 ms: 1.05x faster                                                  |
| json                     | 3.09 ms                                                | 2.94 ms: 1.05x faster                                                  |
| logging_format           | 3.98 us                                                | 3.82 us: 1.04x faster                                                  |
| sqlglot_transpile        | 1.02 ms                                                | 982 us: 1.04x faster                                                   |
| sympy_str                | 148 ms                                                 | 142 ms: 1.04x faster                                                   |
| regex_effbot             | 2.64 ms                                                | 2.55 ms: 1.03x faster                                                  |
| deepcopy_reduce          | 2.07 us                                                | 2.00 us: 1.03x faster                                                  |
| deepcopy                 | 235 us                                                 | 227 us: 1.03x faster                                                   |
| regex_compile            | 77.9 ms                                                | 76.3 ms: 1.02x faster                                                  |
| sympy_sum                | 77.6 ms                                                | 76.1 ms: 1.02x faster                                                  |
| json_loads               | 17.2 us                                                | 16.9 us: 1.02x faster                                                  |
| scimark_lu               | 76.0 ms                                                | 74.6 ms: 1.02x faster                                                  |
| regex_dna                | 154 ms                                                 | 152 ms: 1.02x faster                                                   |
| docutils                 | 1.50 sec                                               | 1.48 sec: 1.02x faster                                                 |
| pickle_pure_python       | 200 us                                                 | 197 us: 1.02x faster                                                   |
| async_tree_cpu_io_mixed  | 526 ms                                                 | 519 ms: 1.01x faster                                                   |
| unpickle                 | 9.12 us                                                | 9.02 us: 1.01x faster                                                  |
| chaos                    | 42.5 ms                                                | 42.2 ms: 1.01x faster                                                  |
| sympy_integrate          | 11.4 ms                                                | 11.3 ms: 1.01x faster                                                  |
| coroutines               | 19.2 ms                                                | 19.1 ms: 1.01x faster                                                  |
| async_tree_io_tg         | 669 ms                                                 | 665 ms: 1.01x faster                                                   |
| sqlglot_normalize        | 186 ms                                                 | 185 ms: 1.00x faster                                                   |
| xml_etree_process        | 39.7 ms                                                | 39.6 ms: 1.00x faster                                                  |
| dulwich_log              | 29.8 ms                                                | 29.9 ms: 1.00x slower                                                  |
| richards                 | 32.1 ms                                                | 32.2 ms: 1.00x slower                                                  |
| richards_super           | 36.0 ms                                                | 36.1 ms: 1.00x slower                                                  |
| sympy_expand             | 241 ms                                                 | 242 ms: 1.00x slower                                                   |
| tomli_loads              | 1.39 sec                                               | 1.40 sec: 1.00x slower                                                 |
| pidigits                 | 282 ms                                                 | 283 ms: 1.00x slower                                                   |
| create_gc_cycles         | 701 us                                                 | 705 us: 1.01x slower                                                   |
| xml_etree_generate       | 55.8 ms                                                | 56.2 ms: 1.01x slower                                                  |
| nqueens                  | 62.4 ms                                                | 62.8 ms: 1.01x slower                                                  |
| async_tree_none_tg       | 258 ms                                                 | 259 ms: 1.01x slower                                                   |
| pickle                   | 7.23 us                                                | 7.31 us: 1.01x slower                                                  |
| xml_etree_parse          | 106 ms                                                 | 108 ms: 1.01x slower                                                   |
| asyncio_tcp_ssl          | 1.24 sec                                               | 1.26 sec: 1.01x slower                                                 |
| pickle_dict              | 18.1 us                                                | 18.3 us: 1.01x slower                                                  |
| dask                     | 222 ms                                                 | 225 ms: 1.01x slower                                                   |
| unpickle_list            | 3.02 us                                                | 3.08 us: 1.02x slower                                                  |
| sqlite_synth             | 1.57 us                                                | 1.60 us: 1.02x slower                                                  |
| sqlglot_optimize         | 34.0 ms                                                | 34.8 ms: 1.02x slower                                                  |
| mdp                      | 1.58 sec                                               | 1.62 sec: 1.02x slower                                                 |
| 2to3                     | 169 ms                                                 | 174 ms: 1.03x slower                                                   |
| mako                     | 7.71 ms                                                | 7.94 ms: 1.03x slower                                                  |
| xml_etree_iterparse      | 74.0 ms                                                | 76.2 ms: 1.03x slower                                                  |
| pycparser                | 677 ms                                                 | 699 ms: 1.03x slower                                                   |
| meteor_contest           | 71.7 ms                                                | 74.1 ms: 1.03x slower                                                  |
| pickle_list              | 2.89 us                                                | 2.98 us: 1.03x slower                                                  |
| pyflate                  | 316 ms                                                 | 327 ms: 1.04x slower                                                   |
| pprint_safe_repr         | 497 ms                                                 | 516 ms: 1.04x slower                                                   |
| bench_mp_pool            | 44.9 ms                                                | 46.7 ms: 1.04x slower                                                  |
| chameleon                | 4.70 ms                                                | 4.89 ms: 1.04x slower                                                  |
| async_tree_io            | 668 ms                                                 | 696 ms: 1.04x slower                                                   |
| pprint_pformat           | 1.01 sec                                               | 1.06 sec: 1.05x slower                                                 |
| json_dumps               | 6.22 ms                                                | 6.51 ms: 1.05x slower                                                  |
| async_tree_memoization   | 312 ms                                                 | 327 ms: 1.05x slower                                                   |
| unpickle_pure_python     | 151 us                                                 | 158 us: 1.05x slower                                                   |
| scimark_sparse_mat_mult  | 3.14 ms                                                | 3.34 ms: 1.07x slower                                                  |
| regex_v8                 | 16.0 ms                                                | 17.1 ms: 1.07x slower                                                  |
| spectral_norm            | 76.4 ms                                                | 82.9 ms: 1.09x slower                                                  |
| go                       | 102 ms                                                 | 110 ms: 1.09x slower                                                   |
| scimark_monte_carlo      | 45.0 ms                                                | 49.2 ms: 1.09x slower                                                  |
| nbody                    | 68.8 ms                                                | 76.8 ms: 1.12x slower                                                  |
| scimark_fft              | 195 ms                                                 | 218 ms: 1.12x slower                                                   |
| fannkuch                 | 248 ms                                                 | 278 ms: 1.12x slower                                                   |
| hexiom                   | 4.54 ms                                                | 5.09 ms: 1.12x slower                                                  |
| python_startup           | 11.4 ms                                                | 13.2 ms: 1.15x slower                                                  |
| scimark_sor              | 87.4 ms                                                | 106 ms: 1.21x slower                                                   |
| coverage                 | 38.9 ms                                                | 47.3 ms: 1.22x slower                                                  |
| telco                    | 3.68 ms                                                | 4.53 ms: 1.23x slower                                                  |
| python_startup_no_site   | 9.37 ms                                                | 11.8 ms: 1.26x slower                                                  |
| mypy2                    | 380 ms                                                 | 526 ms: 1.39x slower                                                   |
| Geometric mean           | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (10): asyncio_tcp, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg, bench_thread_pool, gc_traversal, async_generators, asyncio_websockets, tornado_http, float, pathlib
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.14% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.15x