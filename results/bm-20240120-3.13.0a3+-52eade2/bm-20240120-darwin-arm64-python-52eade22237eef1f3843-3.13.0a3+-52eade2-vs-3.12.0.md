
# Results vs. 3.12.0

- fork: python
- ref: 52eade22237eef1f3843
- machine: darwin-arm64
- commit hash: 52eade2
- commit date: 2024-01-20
- overall geometric mean: 1.00x slower
- HPT reliability: 69.01%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| chameleon      | 4.70 ms                                                | 4.89 ms: 1.04x slower                                                  |
| docutils       | 1.50 sec                                               | 1.46 sec: 1.03x faster                                                 |
| Geometric mean | (ref)                                                  | 1.00x slower                                                           |

Benchmark hidden because not significant (2): 2to3, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 266 ms                                                 | 252 ms: 1.05x faster                                                   |
| async_tree_cpu_io_mixed | 526 ms                                                 | 520 ms: 1.01x faster                                                   |
| async_tree_none_tg      | 258 ms                                                 | 261 ms: 1.01x slower                                                   |
| async_tree_io_tg        | 669 ms                                                 | 679 ms: 1.01x slower                                                   |
| async_tree_io           | 668 ms                                                 | 704 ms: 1.05x slower                                                   |
| async_tree_memoization  | 312 ms                                                 | 331 ms: 1.06x slower                                                   |
| Geometric mean          | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 282 ms                                                 | 283 ms: 1.00x slower                                                   |
| float          | 55.8 ms                                                | 56.9 ms: 1.02x slower                                                  |
| nbody          | 68.8 ms                                                | 75.5 ms: 1.10x slower                                                  |
| Geometric mean | (ref)                                                  | 1.04x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 77.9 ms                                                | 73.9 ms: 1.05x faster                                                  |
| regex_dna      | 154 ms                                                 | 155 ms: 1.01x slower                                                   |
| regex_effbot   | 2.64 ms                                                | 2.74 ms: 1.04x slower                                                  |
| regex_v8       | 16.0 ms                                                | 17.8 ms: 1.12x slower                                                  |
| Geometric mean | (ref)                                                  | 1.03x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 200 us                                                 | 197 us: 1.01x faster                                                   |
| xml_etree_process    | 39.7 ms                                                | 39.4 ms: 1.01x faster                                                  |
| json_loads           | 17.2 us                                                | 17.2 us: 1.00x faster                                                  |
| pickle_dict          | 18.1 us                                                | 18.1 us: 1.00x slower                                                  |
| xml_etree_generate   | 55.8 ms                                                | 56.2 ms: 1.01x slower                                                  |
| unpickle             | 9.12 us                                                | 9.17 us: 1.01x slower                                                  |
| unpickle_list        | 3.02 us                                                | 3.06 us: 1.01x slower                                                  |
| pickle_list          | 2.89 us                                                | 2.94 us: 1.02x slower                                                  |
| unpickle_pure_python | 151 us                                                 | 154 us: 1.02x slower                                                   |
| xml_etree_iterparse  | 74.0 ms                                                | 75.8 ms: 1.02x slower                                                  |
| pickle               | 7.23 us                                                | 7.40 us: 1.02x slower                                                  |
| json_dumps           | 6.22 ms                                                | 6.59 ms: 1.06x slower                                                  |
| tomli_loads          | 1.39 sec                                               | 1.55 sec: 1.11x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.02x slower                                                           |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 12.5 ms: 1.10x slower                                                  |
| python_startup_no_site | 9.37 ms                                                | 11.1 ms: 1.18x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.14x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 7.71 ms                                                | 7.62 ms: 1.01x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 93.0 us                                                | 71.3 us: 1.30x faster                                                  |
| raytrace                 | 212 ms                                                 | 171 ms: 1.24x faster                                                   |
| comprehensions           | 14.5 us                                                | 12.1 us: 1.20x faster                                                  |
| unpack_sequence          | 31.5 ns                                                | 28.4 ns: 1.11x faster                                                  |
| deltablue                | 2.71 ms                                                | 2.45 ms: 1.11x faster                                                  |
| generators               | 31.1 ms                                                | 28.5 ms: 1.09x faster                                                  |
| logging_silent           | 76.4 ns                                                | 70.5 ns: 1.08x faster                                                  |
| deepcopy_memo            | 27.7 us                                                | 25.7 us: 1.08x faster                                                  |
| sqlglot_parse            | 848 us                                                 | 790 us: 1.07x faster                                                   |
| sympy_sum                | 77.6 ms                                                | 72.6 ms: 1.07x faster                                                  |
| crypto_pyaes             | 51.9 ms                                                | 48.6 ms: 1.07x faster                                                  |
| chaos                    | 42.5 ms                                                | 39.9 ms: 1.07x faster                                                  |
| sympy_integrate          | 11.4 ms                                                | 10.7 ms: 1.07x faster                                                  |
| logging_format           | 3.98 us                                                | 3.74 us: 1.06x faster                                                  |
| logging_simple           | 3.69 us                                                | 3.47 us: 1.06x faster                                                  |
| sympy_str                | 148 ms                                                 | 139 ms: 1.06x faster                                                   |
| sqlglot_transpile        | 1.02 ms                                                | 967 us: 1.06x faster                                                   |
| async_tree_none          | 266 ms                                                 | 252 ms: 1.05x faster                                                   |
| regex_compile            | 77.9 ms                                                | 73.9 ms: 1.05x faster                                                  |
| deepcopy_reduce          | 2.07 us                                                | 1.98 us: 1.05x faster                                                  |
| deepcopy                 | 235 us                                                 | 225 us: 1.04x faster                                                   |
| json                     | 3.09 ms                                                | 2.96 ms: 1.04x faster                                                  |
| nqueens                  | 62.4 ms                                                | 60.3 ms: 1.03x faster                                                  |
| coroutines               | 19.2 ms                                                | 18.7 ms: 1.03x faster                                                  |
| async_generators         | 304 ms                                                 | 296 ms: 1.03x faster                                                   |
| docutils                 | 1.50 sec                                               | 1.46 sec: 1.03x faster                                                 |
| scimark_lu               | 76.0 ms                                                | 74.2 ms: 1.02x faster                                                  |
| sqlglot_normalize        | 186 ms                                                 | 182 ms: 1.02x faster                                                   |
| bench_mp_pool            | 44.9 ms                                                | 44.1 ms: 1.02x faster                                                  |
| pickle_pure_python       | 200 us                                                 | 197 us: 1.01x faster                                                   |
| mdp                      | 1.58 sec                                               | 1.56 sec: 1.01x faster                                                 |
| mako                     | 7.71 ms                                                | 7.62 ms: 1.01x faster                                                  |
| async_tree_cpu_io_mixed  | 526 ms                                                 | 520 ms: 1.01x faster                                                   |
| dulwich_log              | 29.8 ms                                                | 29.6 ms: 1.01x faster                                                  |
| sympy_expand             | 241 ms                                                 | 240 ms: 1.01x faster                                                   |
| sqlglot_optimize         | 34.0 ms                                                | 33.8 ms: 1.01x faster                                                  |
| xml_etree_process        | 39.7 ms                                                | 39.4 ms: 1.01x faster                                                  |
| json_loads               | 17.2 us                                                | 17.2 us: 1.00x faster                                                  |
| scimark_sparse_mat_mult  | 3.14 ms                                                | 3.12 ms: 1.00x faster                                                  |
| hexiom                   | 4.54 ms                                                | 4.53 ms: 1.00x faster                                                  |
| asyncio_websockets       | 409 ms                                                 | 409 ms: 1.00x faster                                                   |
| pidigits                 | 282 ms                                                 | 283 ms: 1.00x slower                                                   |
| pickle_dict              | 18.1 us                                                | 18.1 us: 1.00x slower                                                  |
| xml_etree_generate       | 55.8 ms                                                | 56.2 ms: 1.01x slower                                                  |
| unpickle                 | 9.12 us                                                | 9.17 us: 1.01x slower                                                  |
| create_gc_cycles         | 701 us                                                 | 706 us: 1.01x slower                                                   |
| regex_dna                | 154 ms                                                 | 155 ms: 1.01x slower                                                   |
| meteor_contest           | 71.7 ms                                                | 72.3 ms: 1.01x slower                                                  |
| async_tree_none_tg       | 258 ms                                                 | 261 ms: 1.01x slower                                                   |
| unpickle_list            | 3.02 us                                                | 3.06 us: 1.01x slower                                                  |
| async_tree_io_tg         | 669 ms                                                 | 679 ms: 1.01x slower                                                   |
| sqlite_synth             | 1.57 us                                                | 1.59 us: 1.01x slower                                                  |
| float                    | 55.8 ms                                                | 56.9 ms: 1.02x slower                                                  |
| pickle_list              | 2.89 us                                                | 2.94 us: 1.02x slower                                                  |
| unpickle_pure_python     | 151 us                                                 | 154 us: 1.02x slower                                                   |
| xml_etree_iterparse      | 74.0 ms                                                | 75.8 ms: 1.02x slower                                                  |
| pickle                   | 7.23 us                                                | 7.40 us: 1.02x slower                                                  |
| richards_super           | 36.0 ms                                                | 37.0 ms: 1.03x slower                                                  |
| pycparser                | 677 ms                                                 | 697 ms: 1.03x slower                                                   |
| richards                 | 32.1 ms                                                | 33.2 ms: 1.03x slower                                                  |
| regex_effbot             | 2.64 ms                                                | 2.74 ms: 1.04x slower                                                  |
| pprint_safe_repr         | 497 ms                                                 | 517 ms: 1.04x slower                                                   |
| pprint_pformat           | 1.01 sec                                               | 1.05 sec: 1.04x slower                                                 |
| go                       | 102 ms                                                 | 106 ms: 1.04x slower                                                   |
| chameleon                | 4.70 ms                                                | 4.89 ms: 1.04x slower                                                  |
| scimark_monte_carlo      | 45.0 ms                                                | 47.2 ms: 1.05x slower                                                  |
| pathlib                  | 24.2 ms                                                | 25.4 ms: 1.05x slower                                                  |
| scimark_fft              | 195 ms                                                 | 205 ms: 1.05x slower                                                   |
| asyncio_tcp_ssl          | 1.24 sec                                               | 1.31 sec: 1.05x slower                                                 |
| async_tree_io            | 668 ms                                                 | 704 ms: 1.05x slower                                                   |
| async_tree_memoization   | 312 ms                                                 | 331 ms: 1.06x slower                                                   |
| json_dumps               | 6.22 ms                                                | 6.59 ms: 1.06x slower                                                  |
| pyflate                  | 316 ms                                                 | 342 ms: 1.08x slower                                                   |
| nbody                    | 68.8 ms                                                | 75.5 ms: 1.10x slower                                                  |
| python_startup           | 11.4 ms                                                | 12.5 ms: 1.10x slower                                                  |
| fannkuch                 | 248 ms                                                 | 273 ms: 1.10x slower                                                   |
| tomli_loads              | 1.39 sec                                               | 1.55 sec: 1.11x slower                                                 |
| regex_v8                 | 16.0 ms                                                | 17.8 ms: 1.12x slower                                                  |
| python_startup_no_site   | 9.37 ms                                                | 11.1 ms: 1.18x slower                                                  |
| scimark_sor              | 87.4 ms                                                | 105 ms: 1.20x slower                                                   |
| coverage                 | 38.9 ms                                                | 47.5 ms: 1.22x slower                                                  |
| telco                    | 3.68 ms                                                | 4.55 ms: 1.24x slower                                                  |
| mypy2                    | 380 ms                                                 | 518 ms: 1.36x slower                                                   |
| Geometric mean           | (ref)                                                  | 1.00x slower                                                           |

Benchmark hidden because not significant (10): asyncio_tcp, tornado_http, spectral_norm, bench_thread_pool, async_tree_cpu_io_mixed_tg, gc_traversal, 2to3, xml_etree_parse, async_tree_memoization_tg, dask
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 69.01% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x