
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_relax
- machine: darwin-arm64
- commit hash: ff044c0
- commit date: 2024-02-21
- overall geometric mean: 1.04x slower \*
- HPT reliability: 99.37%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.83x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 185 ms: 1.09x slower                                                 |
| chameleon      | 4.70 ms                                                | 4.89 ms: 1.04x slower                                                |
| docutils       | 1.50 sec                                               | 1.51 sec: 1.01x slower                                               |
| Geometric mean | (ref)                                                  | 1.04x slower                                                         |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none         | 266 ms                                                 | 252 ms: 1.05x faster                                                 |
| async_tree_cpu_io_mixed | 526 ms                                                 | 521 ms: 1.01x faster                                                 |
| async_tree_io           | 668 ms                                                 | 701 ms: 1.05x slower                                                 |
| async_tree_memoization  | 312 ms                                                 | 328 ms: 1.05x slower                                                 |
| Geometric mean          | (ref)                                                  | 1.00x slower                                                         |

Benchmark hidden because not significant (4): async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| float          | 55.8 ms                                                | 53.2 ms: 1.05x faster                                                |
| pidigits       | 282 ms                                                 | 282 ms: 1.00x slower                                                 |
| nbody          | 68.8 ms                                                | 69.9 ms: 1.02x slower                                                |
| Geometric mean | (ref)                                                  | 1.01x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_effbot   | 2.64 ms                                                | 2.56 ms: 1.03x faster                                                |
| regex_dna      | 154 ms                                                 | 152 ms: 1.02x faster                                                 |
| regex_v8       | 16.0 ms                                                | 17.1 ms: 1.07x slower                                                |
| regex_compile  | 77.9 ms                                                | 84.7 ms: 1.09x slower                                                |
| Geometric mean | (ref)                                                  | 1.03x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| tomli_loads          | 1.39 sec                                               | 1.37 sec: 1.02x faster                                               |
| xml_etree_process    | 39.7 ms                                                | 38.9 ms: 1.02x faster                                                |
| pickle_pure_python   | 200 us                                                 | 197 us: 1.02x faster                                                 |
| unpickle_pure_python | 151 us                                                 | 149 us: 1.01x faster                                                 |
| json_loads           | 17.2 us                                                | 17.1 us: 1.01x faster                                                |
| xml_etree_generate   | 55.8 ms                                                | 55.6 ms: 1.00x faster                                                |
| unpickle             | 9.12 us                                                | 9.09 us: 1.00x faster                                                |
| pickle_dict          | 18.1 us                                                | 18.1 us: 1.01x slower                                                |
| unpickle_list        | 3.02 us                                                | 3.04 us: 1.01x slower                                                |
| xml_etree_iterparse  | 74.0 ms                                                | 74.7 ms: 1.01x slower                                                |
| pickle_list          | 2.89 us                                                | 2.98 us: 1.03x slower                                                |
| json_dumps           | 6.22 ms                                                | 6.50 ms: 1.05x slower                                                |
| Geometric mean       | (ref)                                                  | 1.00x slower                                                         |

Benchmark hidden because not significant (2): xml_etree_parse, pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 18.0 ms: 1.57x slower                                                |
| python_startup_no_site | 9.37 ms                                                | 16.5 ms: 1.75x slower                                                |
| Geometric mean         | (ref)                                                  | 1.66x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 7.71 ms                                                | 6.85 ms: 1.13x faster                                                |

All benchmarks:
===============

| Benchmark                | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols | 93.0 us                                                | 71.7 us: 1.30x faster                                                |
| comprehensions           | 14.5 us                                                | 12.6 us: 1.15x faster                                                |
| mako                     | 7.71 ms                                                | 6.85 ms: 1.13x faster                                                |
| raytrace                 | 212 ms                                                 | 191 ms: 1.11x faster                                                 |
| asyncio_tcp              | 449 ms                                                 | 413 ms: 1.09x faster                                                 |
| generators               | 31.1 ms                                                | 28.6 ms: 1.09x faster                                                |
| crypto_pyaes             | 51.9 ms                                                | 47.8 ms: 1.08x faster                                                |
| logging_silent           | 76.4 ns                                                | 70.7 ns: 1.08x faster                                                |
| deltablue                | 2.71 ms                                                | 2.55 ms: 1.06x faster                                                |
| chaos                    | 42.5 ms                                                | 40.2 ms: 1.06x faster                                                |
| logging_simple           | 3.69 us                                                | 3.49 us: 1.06x faster                                                |
| logging_format           | 3.98 us                                                | 3.78 us: 1.05x faster                                                |
| async_tree_none          | 266 ms                                                 | 252 ms: 1.05x faster                                                 |
| deepcopy_memo            | 27.7 us                                                | 26.3 us: 1.05x faster                                                |
| float                    | 55.8 ms                                                | 53.2 ms: 1.05x faster                                                |
| json                     | 3.09 ms                                                | 2.95 ms: 1.05x faster                                                |
| deepcopy_reduce          | 2.07 us                                                | 1.99 us: 1.04x faster                                                |
| coroutines               | 19.2 ms                                                | 18.5 ms: 1.04x faster                                                |
| deepcopy                 | 235 us                                                 | 226 us: 1.04x faster                                                 |
| spectral_norm            | 76.4 ms                                                | 74.0 ms: 1.03x faster                                                |
| regex_effbot             | 2.64 ms                                                | 2.56 ms: 1.03x faster                                                |
| sympy_str                | 148 ms                                                 | 144 ms: 1.03x faster                                                 |
| sqlglot_parse            | 848 us                                                 | 827 us: 1.03x faster                                                 |
| tomli_loads              | 1.39 sec                                               | 1.37 sec: 1.02x faster                                               |
| xml_etree_process        | 39.7 ms                                                | 38.9 ms: 1.02x faster                                                |
| regex_dna                | 154 ms                                                 | 152 ms: 1.02x faster                                                 |
| pickle_pure_python       | 200 us                                                 | 197 us: 1.02x faster                                                 |
| sympy_sum                | 77.6 ms                                                | 76.6 ms: 1.01x faster                                                |
| unpickle_pure_python     | 151 us                                                 | 149 us: 1.01x faster                                                 |
| json_loads               | 17.2 us                                                | 17.1 us: 1.01x faster                                                |
| async_tree_cpu_io_mixed  | 526 ms                                                 | 521 ms: 1.01x faster                                                 |
| sqlglot_normalize        | 186 ms                                                 | 184 ms: 1.01x faster                                                 |
| sqlglot_transpile        | 1.02 ms                                                | 1.01 ms: 1.01x faster                                                |
| xml_etree_generate       | 55.8 ms                                                | 55.6 ms: 1.00x faster                                                |
| unpickle                 | 9.12 us                                                | 9.09 us: 1.00x faster                                                |
| asyncio_websockets       | 409 ms                                                 | 408 ms: 1.00x faster                                                 |
| pidigits                 | 282 ms                                                 | 282 ms: 1.00x slower                                                 |
| pickle_dict              | 18.1 us                                                | 18.1 us: 1.01x slower                                                |
| docutils                 | 1.50 sec                                               | 1.51 sec: 1.01x slower                                               |
| sympy_integrate          | 11.4 ms                                                | 11.5 ms: 1.01x slower                                                |
| unpickle_list            | 3.02 us                                                | 3.04 us: 1.01x slower                                                |
| xml_etree_iterparse      | 74.0 ms                                                | 74.7 ms: 1.01x slower                                                |
| sqlite_synth             | 1.57 us                                                | 1.59 us: 1.01x slower                                                |
| gc_traversal             | 2.40 ms                                                | 2.43 ms: 1.01x slower                                                |
| nbody                    | 68.8 ms                                                | 69.9 ms: 1.02x slower                                                |
| sympy_expand             | 241 ms                                                 | 246 ms: 1.02x slower                                                 |
| async_generators         | 304 ms                                                 | 310 ms: 1.02x slower                                                 |
| scimark_fft              | 195 ms                                                 | 200 ms: 1.02x slower                                                 |
| scimark_monte_carlo      | 45.0 ms                                                | 46.1 ms: 1.02x slower                                                |
| bench_thread_pool        | 504 us                                                 | 517 us: 1.03x slower                                                 |
| dulwich_log              | 29.8 ms                                                | 30.6 ms: 1.03x slower                                                |
| pprint_safe_repr         | 497 ms                                                 | 512 ms: 1.03x slower                                                 |
| create_gc_cycles         | 701 us                                                 | 723 us: 1.03x slower                                                 |
| meteor_contest           | 71.7 ms                                                | 74.0 ms: 1.03x slower                                                |
| pickle_list              | 2.89 us                                                | 2.98 us: 1.03x slower                                                |
| nqueens                  | 62.4 ms                                                | 64.5 ms: 1.03x slower                                                |
| mdp                      | 1.58 sec                                               | 1.63 sec: 1.03x slower                                               |
| pprint_pformat           | 1.01 sec                                               | 1.05 sec: 1.04x slower                                               |
| chameleon                | 4.70 ms                                                | 4.89 ms: 1.04x slower                                                |
| sqlglot_optimize         | 34.0 ms                                                | 35.5 ms: 1.04x slower                                                |
| asyncio_tcp_ssl          | 1.24 sec                                               | 1.30 sec: 1.05x slower                                               |
| json_dumps               | 6.22 ms                                                | 6.50 ms: 1.05x slower                                                |
| async_tree_io            | 668 ms                                                 | 701 ms: 1.05x slower                                                 |
| async_tree_memoization   | 312 ms                                                 | 328 ms: 1.05x slower                                                 |
| regex_v8                 | 16.0 ms                                                | 17.1 ms: 1.07x slower                                                |
| pyflate                  | 316 ms                                                 | 339 ms: 1.07x slower                                                 |
| pycparser                | 677 ms                                                 | 732 ms: 1.08x slower                                                 |
| regex_compile            | 77.9 ms                                                | 84.7 ms: 1.09x slower                                                |
| 2to3                     | 169 ms                                                 | 185 ms: 1.09x slower                                                 |
| go                       | 102 ms                                                 | 115 ms: 1.13x slower                                                 |
| scimark_lu               | 76.0 ms                                                | 86.7 ms: 1.14x slower                                                |
| hexiom                   | 4.54 ms                                                | 5.27 ms: 1.16x slower                                                |
| bench_mp_pool            | 44.9 ms                                                | 53.3 ms: 1.19x slower                                                |
| richards_super           | 36.0 ms                                                | 43.3 ms: 1.20x slower                                                |
| richards                 | 32.1 ms                                                | 39.4 ms: 1.22x slower                                                |
| coverage                 | 38.9 ms                                                | 47.9 ms: 1.23x slower                                                |
| telco                    | 3.68 ms                                                | 4.55 ms: 1.24x slower                                                |
| fannkuch                 | 248 ms                                                 | 311 ms: 1.25x slower                                                 |
| scimark_sor              | 87.4 ms                                                | 116 ms: 1.33x slower                                                 |
| python_startup           | 11.4 ms                                                | 18.0 ms: 1.57x slower                                                |
| mypy2                    | 380 ms                                                 | 603 ms: 1.59x slower                                                 |
| python_startup_no_site   | 9.37 ms                                                | 16.5 ms: 1.75x slower                                                |
| unpack_sequence          | 31.5 ns                                                | 115 ns: 3.64x slower                                                 |
| Geometric mean           | (ref)                                                  | 1.04x slower                                                         |

Benchmark hidden because not significant (9): async_tree_cpu_io_mixed_tg, xml_etree_parse, async_tree_io_tg, async_tree_memoization_tg, scimark_sparse_mat_mult, async_tree_none_tg, pickle, tornado_http, pathlib
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.37% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.83x