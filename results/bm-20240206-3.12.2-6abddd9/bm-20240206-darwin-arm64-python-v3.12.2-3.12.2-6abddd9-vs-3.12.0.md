
# Results vs. 3.12.0

- fork: python
- ref: v3.12.2
- machine: darwin-arm64
- commit hash: 6abddd9
- commit date: 2024-02-06
- overall geometric mean: 1.00x slower \*
- HPT reliability: 94.24%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.97x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-darwin-arm64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 168 ms: 1.01x faster                                   |
| docutils       | 1.50 sec                                               | 1.49 sec: 1.01x faster                                 |
| Geometric mean | (ref)                                                  | 1.00x faster                                           |

Benchmark hidden because not significant (2): chameleon, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-darwin-arm64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_io  | 668 ms                                                 | 665 ms: 1.00x faster                                   |
| Geometric mean | (ref)                                                  | 1.00x faster                                           |

Benchmark hidden because not significant (7): async_tree_none, async_tree_memoization, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed, async_tree_io_tg, async_tree_none_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-darwin-arm64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| nbody          | 68.8 ms                                                | 68.5 ms: 1.00x faster                                  |
| float          | 55.8 ms                                                | 56.0 ms: 1.00x slower                                  |
| Geometric mean | (ref)                                                  | 1.00x faster                                           |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-darwin-arm64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 77.9 ms                                                | 75.8 ms: 1.03x faster                                  |
| regex_dna      | 154 ms                                                 | 158 ms: 1.02x slower                                   |
| regex_v8       | 16.0 ms                                                | 16.9 ms: 1.06x slower                                  |
| regex_effbot   | 2.64 ms                                                | 2.83 ms: 1.07x slower                                  |
| Geometric mean | (ref)                                                  | 1.03x slower                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-darwin-arm64-python-v3.12.2-3.12.2-6abddd9 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| xml_etree_process    | 39.7 ms                                                | 39.3 ms: 1.01x faster                                  |
| unpickle_pure_python | 151 us                                                 | 149 us: 1.01x faster                                   |
| json_loads           | 17.2 us                                                | 17.1 us: 1.01x faster                                  |
| xml_etree_generate   | 55.8 ms                                                | 55.4 ms: 1.01x faster                                  |
| pickle_pure_python   | 200 us                                                 | 200 us: 1.00x slower                                   |
| json_dumps           | 6.22 ms                                                | 6.24 ms: 1.00x slower                                  |
| pickle_dict          | 18.1 us                                                | 18.1 us: 1.00x slower                                  |
| pickle               | 7.23 us                                                | 7.28 us: 1.01x slower                                  |
| pickle_list          | 2.89 us                                                | 2.93 us: 1.02x slower                                  |
| unpickle_list        | 3.02 us                                                | 3.08 us: 1.02x slower                                  |
| Geometric mean       | (ref)                                                  | 1.00x slower                                           |

Benchmark hidden because not significant (4): xml_etree_iterparse, xml_etree_parse, tomli_loads, unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-darwin-arm64-python-v3.12.2-3.12.2-6abddd9 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 12.1 ms: 1.06x slower                                  |
| python_startup_no_site | 9.37 ms                                                | 10.1 ms: 1.08x slower                                  |
| Geometric mean         | (ref)                                                  | 1.07x slower                                           |

Benchmarks with tag 'template':
===============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-darwin-arm64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako           | 7.71 ms                                                | 7.73 ms: 1.00x slower                                  |
| Geometric mean | (ref)                                                  | 1.00x slower                                           |

Benchmark hidden because not significant (1): django_template

All benchmarks:
===============

| Benchmark                | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-darwin-arm64-python-v3.12.2-3.12.2-6abddd9 |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| typing_runtime_protocols | 93.0 us                                                | 74.1 us: 1.25x faster                                  |
| regex_compile            | 77.9 ms                                                | 75.8 ms: 1.03x faster                                  |
| json                     | 3.09 ms                                                | 3.04 ms: 1.02x faster                                  |
| dulwich_log              | 29.8 ms                                                | 29.4 ms: 1.01x faster                                  |
| async_generators         | 304 ms                                                 | 300 ms: 1.01x faster                                   |
| sympy_integrate          | 11.4 ms                                                | 11.2 ms: 1.01x faster                                  |
| sympy_sum                | 77.6 ms                                                | 76.6 ms: 1.01x faster                                  |
| bench_thread_pool        | 504 us                                                 | 498 us: 1.01x faster                                   |
| sympy_str                | 148 ms                                                 | 146 ms: 1.01x faster                                   |
| comprehensions           | 14.5 us                                                | 14.4 us: 1.01x faster                                  |
| xml_etree_process        | 39.7 ms                                                | 39.3 ms: 1.01x faster                                  |
| unpickle_pure_python     | 151 us                                                 | 149 us: 1.01x faster                                   |
| deepcopy                 | 235 us                                                 | 233 us: 1.01x faster                                   |
| json_loads               | 17.2 us                                                | 17.1 us: 1.01x faster                                  |
| xml_etree_generate       | 55.8 ms                                                | 55.4 ms: 1.01x faster                                  |
| nqueens                  | 62.4 ms                                                | 61.9 ms: 1.01x faster                                  |
| coroutines               | 19.2 ms                                                | 19.1 ms: 1.01x faster                                  |
| create_gc_cycles         | 701 us                                                 | 696 us: 1.01x faster                                   |
| 2to3                     | 169 ms                                                 | 168 ms: 1.01x faster                                   |
| hexiom                   | 4.54 ms                                                | 4.51 ms: 1.01x faster                                  |
| docutils                 | 1.50 sec                                               | 1.49 sec: 1.01x faster                                 |
| coverage                 | 38.9 ms                                                | 38.6 ms: 1.01x faster                                  |
| async_tree_io            | 668 ms                                                 | 665 ms: 1.00x faster                                   |
| nbody                    | 68.8 ms                                                | 68.5 ms: 1.00x faster                                  |
| sqlalchemy_imperative    | 6.68 ms                                                | 6.65 ms: 1.00x faster                                  |
| sympy_expand             | 241 ms                                                 | 240 ms: 1.00x faster                                   |
| gc_traversal             | 2.40 ms                                                | 2.39 ms: 1.00x faster                                  |
| asyncio_websockets       | 409 ms                                                 | 408 ms: 1.00x faster                                   |
| sqlalchemy_declarative   | 62.3 ms                                                | 62.2 ms: 1.00x faster                                  |
| mdp                      | 1.58 sec                                               | 1.58 sec: 1.00x slower                                 |
| deltablue                | 2.71 ms                                                | 2.71 ms: 1.00x slower                                  |
| pickle_pure_python       | 200 us                                                 | 200 us: 1.00x slower                                   |
| telco                    | 3.68 ms                                                | 3.69 ms: 1.00x slower                                  |
| sqlglot_optimize         | 34.0 ms                                                | 34.1 ms: 1.00x slower                                  |
| logging_simple           | 3.69 us                                                | 3.69 us: 1.00x slower                                  |
| scimark_monte_carlo      | 45.0 ms                                                | 45.1 ms: 1.00x slower                                  |
| json_dumps               | 6.22 ms                                                | 6.24 ms: 1.00x slower                                  |
| go                       | 102 ms                                                 | 102 ms: 1.00x slower                                   |
| mako                     | 7.71 ms                                                | 7.73 ms: 1.00x slower                                  |
| meteor_contest           | 71.7 ms                                                | 72.0 ms: 1.00x slower                                  |
| pprint_safe_repr         | 497 ms                                                 | 499 ms: 1.00x slower                                   |
| float                    | 55.8 ms                                                | 56.0 ms: 1.00x slower                                  |
| pickle_dict              | 18.1 us                                                | 18.1 us: 1.00x slower                                  |
| logging_format           | 3.98 us                                                | 4.00 us: 1.00x slower                                  |
| sqlite_synth             | 1.57 us                                                | 1.58 us: 1.00x slower                                  |
| pprint_pformat           | 1.01 sec                                               | 1.02 sec: 1.00x slower                                 |
| spectral_norm            | 76.4 ms                                                | 76.8 ms: 1.01x slower                                  |
| scimark_fft              | 195 ms                                                 | 196 ms: 1.01x slower                                   |
| deepcopy_memo            | 27.7 us                                                | 27.9 us: 1.01x slower                                  |
| pickle                   | 7.23 us                                                | 7.28 us: 1.01x slower                                  |
| logging_silent           | 76.4 ns                                                | 77.0 ns: 1.01x slower                                  |
| scimark_sor              | 87.4 ms                                                | 88.1 ms: 1.01x slower                                  |
| chaos                    | 42.5 ms                                                | 42.9 ms: 1.01x slower                                  |
| generators               | 31.1 ms                                                | 31.3 ms: 1.01x slower                                  |
| richards_super           | 36.0 ms                                                | 36.4 ms: 1.01x slower                                  |
| richards                 | 32.1 ms                                                | 32.5 ms: 1.01x slower                                  |
| unpack_sequence          | 31.5 ns                                                | 31.9 ns: 1.01x slower                                  |
| pickle_list              | 2.89 us                                                | 2.93 us: 1.02x slower                                  |
| unpickle_list            | 3.02 us                                                | 3.08 us: 1.02x slower                                  |
| regex_dna                | 154 ms                                                 | 158 ms: 1.02x slower                                   |
| aiohttp                  | 1.08 ms                                                | 1.11 ms: 1.03x slower                                  |
| gunicorn                 | 1.15 ms                                                | 1.20 ms: 1.05x slower                                  |
| regex_v8                 | 16.0 ms                                                | 16.9 ms: 1.06x slower                                  |
| python_startup           | 11.4 ms                                                | 12.1 ms: 1.06x slower                                  |
| regex_effbot             | 2.64 ms                                                | 2.83 ms: 1.07x slower                                  |
| python_startup_no_site   | 9.37 ms                                                | 10.1 ms: 1.08x slower                                  |
| asyncio_tcp_ssl          | 1.24 sec                                               | 1.39 sec: 1.12x slower                                 |
| mypy2                    | 380 ms                                                 | 470 ms: 1.24x slower                                   |
| Geometric mean           | (ref)                                                  | 1.00x slower                                           |

Benchmark hidden because not significant (30): asyncio_tcp, dask, bench_mp_pool, pathlib, async_tree_none, pycparser, xml_etree_iterparse, chameleon, async_tree_memoization, async_tree_cpu_io_mixed_tg, xml_etree_parse, tomli_loads, async_tree_cpu_io_mixed, async_tree_io_tg, crypto_pyaes, sqlglot_parse, raytrace, pidigits, sqlglot_normalize, fannkuch, scimark_sparse_mat_mult, pyflate, scimark_lu, django_template, unpickle, async_tree_none_tg, async_tree_memoization_tg, sqlglot_transpile, deepcopy_reduce, tornado_http


# HPT report

- Reliability score: 94.24% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.97x