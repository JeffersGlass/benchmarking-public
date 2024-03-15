# Results vs. 3.12.0

- fork: python
- ref: f0df35eeca2ccdfd58cf
- machine: darwin-arm64
- commit hash: f0df35e
- commit date: 2024-02-29
- overall geometric mean: 1.05x slower \*
- HPT reliability: 99.83%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.83x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 187 ms: 1.11x slower                                                   |
| chameleon      | 4.70 ms                                                | 4.84 ms: 1.03x slower                                                  |
| docutils       | 1.50 sec                                               | 1.51 sec: 1.01x slower                                                 |
| Geometric mean | (ref)                                                  | 1.04x slower                                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 266 ms                                                 | 252 ms: 1.05x faster                                                   |
| async_tree_cpu_io_mixed | 526 ms                                                 | 520 ms: 1.01x faster                                                   |
| async_tree_none_tg      | 258 ms                                                 | 259 ms: 1.01x slower                                                   |
| async_tree_io           | 668 ms                                                 | 701 ms: 1.05x slower                                                   |
| async_tree_memoization  | 312 ms                                                 | 328 ms: 1.05x slower                                                   |
| Geometric mean          | (ref)                                                  | 1.00x slower                                                           |

Benchmark hidden because not significant (3): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg, async_tree_io_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| float          | 55.8 ms                                                | 52.9 ms: 1.06x faster                                                  |
| nbody          | 68.8 ms                                                | 70.0 ms: 1.02x slower                                                  |
| Geometric mean | (ref)                                                  | 1.01x faster                                                           |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_dna      | 154 ms                                                 | 145 ms: 1.06x faster                                                   |
| regex_effbot   | 2.64 ms                                                | 2.58 ms: 1.02x faster                                                  |
| regex_v8       | 16.0 ms                                                | 17.1 ms: 1.07x slower                                                  |
| regex_compile  | 77.9 ms                                                | 87.1 ms: 1.12x slower                                                  |
| Geometric mean | (ref)                                                  | 1.02x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_loads           | 17.2 us                                                | 16.9 us: 1.02x faster                                                  |
| pickle_pure_python   | 200 us                                                 | 196 us: 1.02x faster                                                   |
| tomli_loads          | 1.39 sec                                               | 1.39 sec: 1.01x faster                                                 |
| pickle_dict          | 18.1 us                                                | 18.1 us: 1.00x slower                                                  |
| pickle               | 7.23 us                                                | 7.27 us: 1.01x slower                                                  |
| unpickle             | 9.12 us                                                | 9.19 us: 1.01x slower                                                  |
| unpickle_pure_python | 151 us                                                 | 152 us: 1.01x slower                                                   |
| pickle_list          | 2.89 us                                                | 2.91 us: 1.01x slower                                                  |
| unpickle_list        | 3.02 us                                                | 3.06 us: 1.01x slower                                                  |
| xml_etree_iterparse  | 74.0 ms                                                | 75.4 ms: 1.02x slower                                                  |
| json_dumps           | 6.22 ms                                                | 6.56 ms: 1.05x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (3): xml_etree_parse, xml_etree_process, xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 17.7 ms: 1.55x slower                                                  |
| python_startup_no_site | 9.37 ms                                                | 16.4 ms: 1.75x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.65x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 7.71 ms                                                | 6.83 ms: 1.13x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 93.0 us                                                | 71.8 us: 1.30x faster                                                  |
| comprehensions           | 14.5 us                                                | 12.9 us: 1.13x faster                                                  |
| mako                     | 7.71 ms                                                | 6.83 ms: 1.13x faster                                                  |
| asyncio_tcp              | 449 ms                                                 | 399 ms: 1.13x faster                                                   |
| raytrace                 | 212 ms                                                 | 191 ms: 1.11x faster                                                   |
| crypto_pyaes             | 51.9 ms                                                | 47.3 ms: 1.10x faster                                                  |
| generators               | 31.1 ms                                                | 28.5 ms: 1.09x faster                                                  |
| regex_dna                | 154 ms                                                 | 145 ms: 1.06x faster                                                   |
| deltablue                | 2.71 ms                                                | 2.55 ms: 1.06x faster                                                  |
| logging_simple           | 3.69 us                                                | 3.49 us: 1.06x faster                                                  |
| logging_format           | 3.98 us                                                | 3.77 us: 1.06x faster                                                  |
| chaos                    | 42.5 ms                                                | 40.3 ms: 1.06x faster                                                  |
| float                    | 55.8 ms                                                | 52.9 ms: 1.06x faster                                                  |
| async_tree_none          | 266 ms                                                 | 252 ms: 1.05x faster                                                   |
| logging_silent           | 76.4 ns                                                | 72.5 ns: 1.05x faster                                                  |
| deepcopy_memo            | 27.7 us                                                | 26.6 us: 1.04x faster                                                  |
| json                     | 3.09 ms                                                | 2.97 ms: 1.04x faster                                                  |
| deepcopy_reduce          | 2.07 us                                                | 2.00 us: 1.04x faster                                                  |
| coroutines               | 19.2 ms                                                | 18.7 ms: 1.03x faster                                                  |
| regex_effbot             | 2.64 ms                                                | 2.58 ms: 1.02x faster                                                  |
| json_loads               | 17.2 us                                                | 16.9 us: 1.02x faster                                                  |
| pickle_pure_python       | 200 us                                                 | 196 us: 1.02x faster                                                   |
| sqlglot_parse            | 848 us                                                 | 834 us: 1.02x faster                                                   |
| sympy_str                | 148 ms                                                 | 145 ms: 1.02x faster                                                   |
| deepcopy                 | 235 us                                                 | 231 us: 1.02x faster                                                   |
| async_tree_cpu_io_mixed  | 526 ms                                                 | 520 ms: 1.01x faster                                                   |
| sqlglot_normalize        | 186 ms                                                 | 184 ms: 1.01x faster                                                   |
| sympy_sum                | 77.6 ms                                                | 77.1 ms: 1.01x faster                                                  |
| tomli_loads              | 1.39 sec                                               | 1.39 sec: 1.01x faster                                                 |
| asyncio_websockets       | 409 ms                                                 | 408 ms: 1.00x faster                                                   |
| pickle_dict              | 18.1 us                                                | 18.1 us: 1.00x slower                                                  |
| sqlglot_transpile        | 1.02 ms                                                | 1.03 ms: 1.00x slower                                                  |
| gc_traversal             | 2.40 ms                                                | 2.41 ms: 1.00x slower                                                  |
| async_tree_none_tg       | 258 ms                                                 | 259 ms: 1.01x slower                                                   |
| pickle                   | 7.23 us                                                | 7.27 us: 1.01x slower                                                  |
| unpickle                 | 9.12 us                                                | 9.19 us: 1.01x slower                                                  |
| unpickle_pure_python     | 151 us                                                 | 152 us: 1.01x slower                                                   |
| docutils                 | 1.50 sec                                               | 1.51 sec: 1.01x slower                                                 |
| pickle_list              | 2.89 us                                                | 2.91 us: 1.01x slower                                                  |
| sympy_integrate          | 11.4 ms                                                | 11.5 ms: 1.01x slower                                                  |
| unpickle_list            | 3.02 us                                                | 3.06 us: 1.01x slower                                                  |
| create_gc_cycles         | 701 us                                                 | 713 us: 1.02x slower                                                   |
| nbody                    | 68.8 ms                                                | 70.0 ms: 1.02x slower                                                  |
| xml_etree_iterparse      | 74.0 ms                                                | 75.4 ms: 1.02x slower                                                  |
| bench_thread_pool        | 504 us                                                 | 514 us: 1.02x slower                                                   |
| nqueens                  | 62.4 ms                                                | 63.7 ms: 1.02x slower                                                  |
| scimark_fft              | 195 ms                                                 | 199 ms: 1.02x slower                                                   |
| async_generators         | 304 ms                                                 | 311 ms: 1.02x slower                                                   |
| sqlite_synth             | 1.57 us                                                | 1.61 us: 1.02x slower                                                  |
| scimark_monte_carlo      | 45.0 ms                                                | 46.1 ms: 1.02x slower                                                  |
| sympy_expand             | 241 ms                                                 | 248 ms: 1.03x slower                                                   |
| chameleon                | 4.70 ms                                                | 4.84 ms: 1.03x slower                                                  |
| mdp                      | 1.58 sec                                               | 1.63 sec: 1.03x slower                                                 |
| meteor_contest           | 71.7 ms                                                | 74.1 ms: 1.03x slower                                                  |
| dulwich_log              | 29.8 ms                                                | 30.9 ms: 1.03x slower                                                  |
| pprint_safe_repr         | 497 ms                                                 | 517 ms: 1.04x slower                                                   |
| sqlglot_optimize         | 34.0 ms                                                | 35.5 ms: 1.04x slower                                                  |
| pathlib                  | 24.2 ms                                                | 25.4 ms: 1.05x slower                                                  |
| async_tree_io            | 668 ms                                                 | 701 ms: 1.05x slower                                                   |
| async_tree_memoization   | 312 ms                                                 | 328 ms: 1.05x slower                                                   |
| pprint_pformat           | 1.01 sec                                               | 1.06 sec: 1.05x slower                                                 |
| json_dumps               | 6.22 ms                                                | 6.56 ms: 1.05x slower                                                  |
| asyncio_tcp_ssl          | 1.24 sec                                               | 1.32 sec: 1.06x slower                                                 |
| spectral_norm            | 76.4 ms                                                | 81.7 ms: 1.07x slower                                                  |
| regex_v8                 | 16.0 ms                                                | 17.1 ms: 1.07x slower                                                  |
| pycparser                | 677 ms                                                 | 727 ms: 1.07x slower                                                   |
| pyflate                  | 316 ms                                                 | 346 ms: 1.10x slower                                                   |
| 2to3                     | 169 ms                                                 | 187 ms: 1.11x slower                                                   |
| regex_compile            | 77.9 ms                                                | 87.1 ms: 1.12x slower                                                  |
| scimark_lu               | 76.0 ms                                                | 85.6 ms: 1.13x slower                                                  |
| go                       | 102 ms                                                 | 116 ms: 1.14x slower                                                   |
| bench_mp_pool            | 44.9 ms                                                | 52.2 ms: 1.16x slower                                                  |
| hexiom                   | 4.54 ms                                                | 5.33 ms: 1.17x slower                                                  |
| richards_super           | 36.0 ms                                                | 43.4 ms: 1.20x slower                                                  |
| telco                    | 3.68 ms                                                | 4.48 ms: 1.22x slower                                                  |
| coverage                 | 38.9 ms                                                | 47.7 ms: 1.23x slower                                                  |
| richards                 | 32.1 ms                                                | 40.4 ms: 1.26x slower                                                  |
| fannkuch                 | 248 ms                                                 | 325 ms: 1.31x slower                                                   |
| scimark_sor              | 87.4 ms                                                | 115 ms: 1.31x slower                                                   |
| mypy2                    | 380 ms                                                 | 537 ms: 1.41x slower                                                   |
| python_startup           | 11.4 ms                                                | 17.7 ms: 1.55x slower                                                  |
| python_startup_no_site   | 9.37 ms                                                | 16.4 ms: 1.75x slower                                                  |
| unpack_sequence          | 31.5 ns                                                | 114 ns: 3.61x slower                                                   |
| Geometric mean           | (ref)                                                  | 1.05x slower                                                           |

Benchmark hidden because not significant (9): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg, pidigits, scimark_sparse_mat_mult, async_tree_io_tg, xml_etree_parse, xml_etree_process, tornado_http, xml_etree_generate
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.83% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.83x