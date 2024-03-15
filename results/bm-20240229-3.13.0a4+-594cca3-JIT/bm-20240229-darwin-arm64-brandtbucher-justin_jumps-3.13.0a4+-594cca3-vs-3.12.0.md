# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_jumps
- machine: darwin-arm64
- commit hash: 594cca3
- commit date: 2024-02-29
- overall geometric mean: 1.05x slower \*
- HPT reliability: 99.95%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.83x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 188 ms: 1.11x slower                                                 |
| chameleon      | 4.70 ms                                                | 4.85 ms: 1.03x slower                                                |
| docutils       | 1.50 sec                                               | 1.53 sec: 1.02x slower                                               |
| Geometric mean | (ref)                                                  | 1.04x slower                                                         |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none        | 266 ms                                                 | 251 ms: 1.06x faster                                                 |
| async_tree_none_tg     | 258 ms                                                 | 259 ms: 1.01x slower                                                 |
| async_tree_memoization | 312 ms                                                 | 327 ms: 1.05x slower                                                 |
| async_tree_io          | 668 ms                                                 | 701 ms: 1.05x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.00x slower                                                         |

Benchmark hidden because not significant (4): async_tree_cpu_io_mixed, async_tree_memoization_tg, async_tree_cpu_io_mixed_tg, async_tree_io_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| float          | 55.8 ms                                                | 53.0 ms: 1.05x faster                                                |
| pidigits       | 282 ms                                                 | 282 ms: 1.00x slower                                                 |
| nbody          | 68.8 ms                                                | 70.6 ms: 1.03x slower                                                |
| Geometric mean | (ref)                                                  | 1.01x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_dna      | 154 ms                                                 | 152 ms: 1.01x faster                                                 |
| regex_effbot   | 2.64 ms                                                | 2.63 ms: 1.01x faster                                                |
| regex_v8       | 16.0 ms                                                | 17.2 ms: 1.08x slower                                                |
| regex_compile  | 77.9 ms                                                | 86.7 ms: 1.11x slower                                                |
| Geometric mean | (ref)                                                  | 1.04x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| json_loads           | 17.2 us                                                | 16.9 us: 1.02x faster                                                |
| pickle_pure_python   | 200 us                                                 | 197 us: 1.02x faster                                                 |
| xml_etree_process    | 39.7 ms                                                | 39.0 ms: 1.02x faster                                                |
| tomli_loads          | 1.39 sec                                               | 1.38 sec: 1.01x faster                                               |
| pickle               | 7.23 us                                                | 7.25 us: 1.00x slower                                                |
| unpickle             | 9.12 us                                                | 9.15 us: 1.00x slower                                                |
| unpickle_pure_python | 151 us                                                 | 152 us: 1.01x slower                                                 |
| xml_etree_parse      | 106 ms                                                 | 108 ms: 1.01x slower                                                 |
| pickle_dict          | 18.1 us                                                | 18.3 us: 1.01x slower                                                |
| xml_etree_iterparse  | 74.0 ms                                                | 75.0 ms: 1.01x slower                                                |
| unpickle_list        | 3.02 us                                                | 3.07 us: 1.02x slower                                                |
| pickle_list          | 2.89 us                                                | 2.96 us: 1.02x slower                                                |
| xml_etree_generate   | 55.8 ms                                                | 57.8 ms: 1.03x slower                                                |
| json_dumps           | 6.22 ms                                                | 6.54 ms: 1.05x slower                                                |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                         |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 17.3 ms: 1.52x slower                                                |
| python_startup_no_site | 9.37 ms                                                | 15.9 ms: 1.69x slower                                                |
| Geometric mean         | (ref)                                                  | 1.60x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 7.71 ms                                                | 6.85 ms: 1.13x faster                                                |

All benchmarks:
===============

| Benchmark                | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols | 93.0 us                                                | 72.1 us: 1.29x faster                                                |
| mako                     | 7.71 ms                                                | 6.85 ms: 1.13x faster                                                |
| comprehensions           | 14.5 us                                                | 13.0 us: 1.12x faster                                                |
| raytrace                 | 212 ms                                                 | 192 ms: 1.10x faster                                                 |
| asyncio_tcp              | 449 ms                                                 | 407 ms: 1.10x faster                                                 |
| crypto_pyaes             | 51.9 ms                                                | 47.4 ms: 1.09x faster                                                |
| generators               | 31.1 ms                                                | 28.4 ms: 1.09x faster                                                |
| deltablue                | 2.71 ms                                                | 2.54 ms: 1.07x faster                                                |
| async_tree_none          | 266 ms                                                 | 251 ms: 1.06x faster                                                 |
| logging_simple           | 3.69 us                                                | 3.49 us: 1.05x faster                                                |
| float                    | 55.8 ms                                                | 53.0 ms: 1.05x faster                                                |
| logging_silent           | 76.4 ns                                                | 72.6 ns: 1.05x faster                                                |
| chaos                    | 42.5 ms                                                | 40.4 ms: 1.05x faster                                                |
| logging_format           | 3.98 us                                                | 3.79 us: 1.05x faster                                                |
| json                     | 3.09 ms                                                | 2.96 ms: 1.04x faster                                                |
| deepcopy_memo            | 27.7 us                                                | 26.6 us: 1.04x faster                                                |
| deepcopy_reduce          | 2.07 us                                                | 2.00 us: 1.03x faster                                                |
| coroutines               | 19.2 ms                                                | 18.6 ms: 1.03x faster                                                |
| deepcopy                 | 235 us                                                 | 228 us: 1.03x faster                                                 |
| json_loads               | 17.2 us                                                | 16.9 us: 1.02x faster                                                |
| pickle_pure_python       | 200 us                                                 | 197 us: 1.02x faster                                                 |
| xml_etree_process        | 39.7 ms                                                | 39.0 ms: 1.02x faster                                                |
| sqlglot_parse            | 848 us                                                 | 836 us: 1.01x faster                                                 |
| sympy_str                | 148 ms                                                 | 146 ms: 1.01x faster                                                 |
| regex_dna                | 154 ms                                                 | 152 ms: 1.01x faster                                                 |
| sqlglot_normalize        | 186 ms                                                 | 184 ms: 1.01x faster                                                 |
| tomli_loads              | 1.39 sec                                               | 1.38 sec: 1.01x faster                                               |
| regex_effbot             | 2.64 ms                                                | 2.63 ms: 1.01x faster                                                |
| pidigits                 | 282 ms                                                 | 282 ms: 1.00x slower                                                 |
| gc_traversal             | 2.40 ms                                                | 2.41 ms: 1.00x slower                                                |
| pickle                   | 7.23 us                                                | 7.25 us: 1.00x slower                                                |
| unpickle                 | 9.12 us                                                | 9.15 us: 1.00x slower                                                |
| sqlglot_transpile        | 1.02 ms                                                | 1.03 ms: 1.00x slower                                                |
| async_tree_none_tg       | 258 ms                                                 | 259 ms: 1.01x slower                                                 |
| unpickle_pure_python     | 151 us                                                 | 152 us: 1.01x slower                                                 |
| bench_thread_pool        | 504 us                                                 | 510 us: 1.01x slower                                                 |
| sqlite_synth             | 1.57 us                                                | 1.59 us: 1.01x slower                                                |
| xml_etree_parse          | 106 ms                                                 | 108 ms: 1.01x slower                                                 |
| pickle_dict              | 18.1 us                                                | 18.3 us: 1.01x slower                                                |
| xml_etree_iterparse      | 74.0 ms                                                | 75.0 ms: 1.01x slower                                                |
| sympy_integrate          | 11.4 ms                                                | 11.5 ms: 1.01x slower                                                |
| create_gc_cycles         | 701 us                                                 | 712 us: 1.02x slower                                                 |
| unpickle_list            | 3.02 us                                                | 3.07 us: 1.02x slower                                                |
| async_generators         | 304 ms                                                 | 309 ms: 1.02x slower                                                 |
| docutils                 | 1.50 sec                                               | 1.53 sec: 1.02x slower                                               |
| scimark_monte_carlo      | 45.0 ms                                                | 46.0 ms: 1.02x slower                                                |
| sympy_expand             | 241 ms                                                 | 247 ms: 1.02x slower                                                 |
| pickle_list              | 2.89 us                                                | 2.96 us: 1.02x slower                                                |
| nbody                    | 68.8 ms                                                | 70.6 ms: 1.03x slower                                                |
| scimark_fft              | 195 ms                                                 | 201 ms: 1.03x slower                                                 |
| chameleon                | 4.70 ms                                                | 4.85 ms: 1.03x slower                                                |
| mdp                      | 1.58 sec                                               | 1.64 sec: 1.03x slower                                               |
| xml_etree_generate       | 55.8 ms                                                | 57.8 ms: 1.03x slower                                                |
| meteor_contest           | 71.7 ms                                                | 74.5 ms: 1.04x slower                                                |
| pathlib                  | 24.2 ms                                                | 25.2 ms: 1.04x slower                                                |
| pprint_safe_repr         | 497 ms                                                 | 517 ms: 1.04x slower                                                 |
| nqueens                  | 62.4 ms                                                | 65.0 ms: 1.04x slower                                                |
| dulwich_log              | 29.8 ms                                                | 31.1 ms: 1.04x slower                                                |
| sqlglot_optimize         | 34.0 ms                                                | 35.6 ms: 1.05x slower                                                |
| pprint_pformat           | 1.01 sec                                               | 1.06 sec: 1.05x slower                                               |
| async_tree_memoization   | 312 ms                                                 | 327 ms: 1.05x slower                                                 |
| async_tree_io            | 668 ms                                                 | 701 ms: 1.05x slower                                                 |
| spectral_norm            | 76.4 ms                                                | 80.2 ms: 1.05x slower                                                |
| json_dumps               | 6.22 ms                                                | 6.54 ms: 1.05x slower                                                |
| asyncio_tcp_ssl          | 1.24 sec                                               | 1.31 sec: 1.06x slower                                               |
| pycparser                | 677 ms                                                 | 724 ms: 1.07x slower                                                 |
| regex_v8                 | 16.0 ms                                                | 17.2 ms: 1.08x slower                                                |
| pyflate                  | 316 ms                                                 | 346 ms: 1.10x slower                                                 |
| 2to3                     | 169 ms                                                 | 188 ms: 1.11x slower                                                 |
| regex_compile            | 77.9 ms                                                | 86.7 ms: 1.11x slower                                                |
| scimark_lu               | 76.0 ms                                                | 85.7 ms: 1.13x slower                                                |
| go                       | 102 ms                                                 | 116 ms: 1.14x slower                                                 |
| bench_mp_pool            | 44.9 ms                                                | 52.0 ms: 1.16x slower                                                |
| hexiom                   | 4.54 ms                                                | 5.32 ms: 1.17x slower                                                |
| richards_super           | 36.0 ms                                                | 43.8 ms: 1.21x slower                                                |
| telco                    | 3.68 ms                                                | 4.48 ms: 1.22x slower                                                |
| richards                 | 32.1 ms                                                | 39.8 ms: 1.24x slower                                                |
| coverage                 | 38.9 ms                                                | 48.5 ms: 1.25x slower                                                |
| fannkuch                 | 248 ms                                                 | 316 ms: 1.27x slower                                                 |
| scimark_sor              | 87.4 ms                                                | 116 ms: 1.33x slower                                                 |
| python_startup           | 11.4 ms                                                | 17.3 ms: 1.52x slower                                                |
| mypy2                    | 380 ms                                                 | 587 ms: 1.54x slower                                                 |
| python_startup_no_site   | 9.37 ms                                                | 15.9 ms: 1.69x slower                                                |
| unpack_sequence          | 31.5 ns                                                | 113 ns: 3.60x slower                                                 |
| Geometric mean           | (ref)                                                  | 1.05x slower                                                         |

Benchmark hidden because not significant (8): async_tree_cpu_io_mixed, sympy_sum, async_tree_memoization_tg, async_tree_cpu_io_mixed_tg, async_tree_io_tg, asyncio_websockets, scimark_sparse_mat_mult, tornado_http
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.95% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.83x