# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_arena
- machine: darwin-arm64
- commit hash: 1a78317
- commit date: 2024-02-29
- overall geometric mean: 1.04x slower \*
- HPT reliability: 98.14%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.82x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 186 ms: 1.10x slower                                                 |
| chameleon      | 4.70 ms                                                | 4.82 ms: 1.03x slower                                                |
| docutils       | 1.50 sec                                               | 1.52 sec: 1.01x slower                                               |
| Geometric mean | (ref)                                                  | 1.03x slower                                                         |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none         | 266 ms                                                 | 252 ms: 1.06x faster                                                 |
| async_tree_cpu_io_mixed | 526 ms                                                 | 520 ms: 1.01x faster                                                 |
| async_tree_io_tg        | 669 ms                                                 | 665 ms: 1.01x faster                                                 |
| async_tree_io           | 668 ms                                                 | 697 ms: 1.04x slower                                                 |
| async_tree_memoization  | 312 ms                                                 | 326 ms: 1.04x slower                                                 |
| Geometric mean          | (ref)                                                  | 1.00x slower                                                         |

Benchmark hidden because not significant (3): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg, async_tree_none_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| float          | 55.8 ms                                                | 53.0 ms: 1.05x faster                                                |
| pidigits       | 282 ms                                                 | 281 ms: 1.00x faster                                                 |
| nbody          | 68.8 ms                                                | 70.7 ms: 1.03x slower                                                |
| Geometric mean | (ref)                                                  | 1.01x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_dna      | 154 ms                                                 | 152 ms: 1.02x faster                                                 |
| regex_effbot   | 2.64 ms                                                | 2.63 ms: 1.01x faster                                                |
| regex_v8       | 16.0 ms                                                | 17.2 ms: 1.08x slower                                                |
| regex_compile  | 77.9 ms                                                | 87.8 ms: 1.13x slower                                                |
| Geometric mean | (ref)                                                  | 1.04x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| pickle_pure_python   | 200 us                                                 | 196 us: 1.02x faster                                                 |
| xml_etree_process    | 39.7 ms                                                | 39.2 ms: 1.01x faster                                                |
| tomli_loads          | 1.39 sec                                               | 1.38 sec: 1.01x faster                                               |
| json_loads           | 17.2 us                                                | 17.1 us: 1.01x faster                                                |
| xml_etree_generate   | 55.8 ms                                                | 55.4 ms: 1.01x faster                                                |
| xml_etree_parse      | 106 ms                                                 | 106 ms: 1.01x faster                                                 |
| unpickle_pure_python | 151 us                                                 | 150 us: 1.00x faster                                                 |
| pickle_dict          | 18.1 us                                                | 18.1 us: 1.00x slower                                                |
| pickle               | 7.23 us                                                | 7.26 us: 1.00x slower                                                |
| xml_etree_iterparse  | 74.0 ms                                                | 74.9 ms: 1.01x slower                                                |
| pickle_list          | 2.89 us                                                | 2.96 us: 1.03x slower                                                |
| unpickle_list        | 3.02 us                                                | 3.13 us: 1.04x slower                                                |
| json_dumps           | 6.22 ms                                                | 6.53 ms: 1.05x slower                                                |
| Geometric mean       | (ref)                                                  | 1.00x slower                                                         |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 18.0 ms: 1.58x slower                                                |
| python_startup_no_site | 9.37 ms                                                | 16.4 ms: 1.75x slower                                                |
| Geometric mean         | (ref)                                                  | 1.66x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|-----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako            | 7.71 ms                                                | 6.82 ms: 1.13x faster                                                |
| django_template | 22.3 ms                                                | 21.8 ms: 1.03x faster                                                |
| Geometric mean  | (ref)                                                  | 1.08x faster                                                         |

All benchmarks:
===============

| Benchmark                | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols | 93.0 us                                                | 71.5 us: 1.30x faster                                                |
| comprehensions           | 14.5 us                                                | 12.7 us: 1.15x faster                                                |
| asyncio_tcp              | 449 ms                                                 | 396 ms: 1.13x faster                                                 |
| mako                     | 7.71 ms                                                | 6.82 ms: 1.13x faster                                                |
| raytrace                 | 212 ms                                                 | 192 ms: 1.11x faster                                                 |
| crypto_pyaes             | 51.9 ms                                                | 47.2 ms: 1.10x faster                                                |
| generators               | 31.1 ms                                                | 28.4 ms: 1.09x faster                                                |
| deltablue                | 2.71 ms                                                | 2.52 ms: 1.07x faster                                                |
| logging_simple           | 3.69 us                                                | 3.48 us: 1.06x faster                                                |
| chaos                    | 42.5 ms                                                | 40.2 ms: 1.06x faster                                                |
| deepcopy_memo            | 27.7 us                                                | 26.2 us: 1.06x faster                                                |
| async_tree_none          | 266 ms                                                 | 252 ms: 1.06x faster                                                 |
| logging_silent           | 76.4 ns                                                | 72.5 ns: 1.05x faster                                                |
| logging_format           | 3.98 us                                                | 3.78 us: 1.05x faster                                                |
| float                    | 55.8 ms                                                | 53.0 ms: 1.05x faster                                                |
| coroutines               | 19.2 ms                                                | 18.3 ms: 1.05x faster                                                |
| deepcopy_reduce          | 2.07 us                                                | 1.97 us: 1.05x faster                                                |
| json                     | 3.09 ms                                                | 2.95 ms: 1.05x faster                                                |
| aiohttp                  | 1.08 ms                                                | 1.05 ms: 1.03x faster                                                |
| deepcopy                 | 235 us                                                 | 228 us: 1.03x faster                                                 |
| django_template          | 22.3 ms                                                | 21.8 ms: 1.03x faster                                                |
| sympy_str                | 148 ms                                                 | 144 ms: 1.03x faster                                                 |
| gunicorn                 | 1.15 ms                                                | 1.13 ms: 1.02x faster                                                |
| pickle_pure_python       | 200 us                                                 | 196 us: 1.02x faster                                                 |
| sqlglot_normalize        | 186 ms                                                 | 183 ms: 1.02x faster                                                 |
| sympy_sum                | 77.6 ms                                                | 76.4 ms: 1.02x faster                                                |
| regex_dna                | 154 ms                                                 | 152 ms: 1.02x faster                                                 |
| xml_etree_process        | 39.7 ms                                                | 39.2 ms: 1.01x faster                                                |
| tomli_loads              | 1.39 sec                                               | 1.38 sec: 1.01x faster                                               |
| async_tree_cpu_io_mixed  | 526 ms                                                 | 520 ms: 1.01x faster                                                 |
| json_loads               | 17.2 us                                                | 17.1 us: 1.01x faster                                                |
| xml_etree_generate       | 55.8 ms                                                | 55.4 ms: 1.01x faster                                                |
| xml_etree_parse          | 106 ms                                                 | 106 ms: 1.01x faster                                                 |
| async_tree_io_tg         | 669 ms                                                 | 665 ms: 1.01x faster                                                 |
| regex_effbot             | 2.64 ms                                                | 2.63 ms: 1.01x faster                                                |
| sqlglot_parse            | 848 us                                                 | 843 us: 1.01x faster                                                 |
| unpickle_pure_python     | 151 us                                                 | 150 us: 1.00x faster                                                 |
| asyncio_websockets       | 409 ms                                                 | 408 ms: 1.00x faster                                                 |
| pidigits                 | 282 ms                                                 | 281 ms: 1.00x faster                                                 |
| gc_traversal             | 2.40 ms                                                | 2.41 ms: 1.00x slower                                                |
| pickle_dict              | 18.1 us                                                | 18.1 us: 1.00x slower                                                |
| pickle                   | 7.23 us                                                | 7.26 us: 1.00x slower                                                |
| sqlglot_transpile        | 1.02 ms                                                | 1.03 ms: 1.01x slower                                                |
| scimark_sparse_mat_mult  | 3.14 ms                                                | 3.17 ms: 1.01x slower                                                |
| xml_etree_iterparse      | 74.0 ms                                                | 74.9 ms: 1.01x slower                                                |
| docutils                 | 1.50 sec                                               | 1.52 sec: 1.01x slower                                               |
| create_gc_cycles         | 701 us                                                 | 711 us: 1.01x slower                                                 |
| nqueens                  | 62.4 ms                                                | 63.4 ms: 1.02x slower                                                |
| sympy_expand             | 241 ms                                                 | 245 ms: 1.02x slower                                                 |
| bench_thread_pool        | 504 us                                                 | 512 us: 1.02x slower                                                 |
| sqlite_synth             | 1.57 us                                                | 1.60 us: 1.02x slower                                                |
| pprint_safe_repr         | 497 ms                                                 | 507 ms: 1.02x slower                                                 |
| scimark_fft              | 195 ms                                                 | 200 ms: 1.02x slower                                                 |
| async_generators         | 304 ms                                                 | 311 ms: 1.02x slower                                                 |
| pathlib                  | 24.2 ms                                                | 24.8 ms: 1.02x slower                                                |
| scimark_monte_carlo      | 45.0 ms                                                | 46.1 ms: 1.02x slower                                                |
| pickle_list              | 2.89 us                                                | 2.96 us: 1.03x slower                                                |
| mdp                      | 1.58 sec                                               | 1.62 sec: 1.03x slower                                               |
| nbody                    | 68.8 ms                                                | 70.7 ms: 1.03x slower                                                |
| chameleon                | 4.70 ms                                                | 4.82 ms: 1.03x slower                                                |
| pprint_pformat           | 1.01 sec                                               | 1.04 sec: 1.03x slower                                               |
| dulwich_log              | 29.8 ms                                                | 30.9 ms: 1.04x slower                                                |
| unpickle_list            | 3.02 us                                                | 3.13 us: 1.04x slower                                                |
| sqlglot_optimize         | 34.0 ms                                                | 35.4 ms: 1.04x slower                                                |
| pycparser                | 677 ms                                                 | 706 ms: 1.04x slower                                                 |
| async_tree_io            | 668 ms                                                 | 697 ms: 1.04x slower                                                 |
| async_tree_memoization   | 312 ms                                                 | 326 ms: 1.04x slower                                                 |
| asyncio_tcp_ssl          | 1.24 sec                                               | 1.30 sec: 1.05x slower                                               |
| meteor_contest           | 71.7 ms                                                | 75.3 ms: 1.05x slower                                                |
| json_dumps               | 6.22 ms                                                | 6.53 ms: 1.05x slower                                                |
| regex_v8                 | 16.0 ms                                                | 17.2 ms: 1.08x slower                                                |
| pyflate                  | 316 ms                                                 | 345 ms: 1.09x slower                                                 |
| 2to3                     | 169 ms                                                 | 186 ms: 1.10x slower                                                 |
| scimark_lu               | 76.0 ms                                                | 85.0 ms: 1.12x slower                                                |
| go                       | 102 ms                                                 | 114 ms: 1.12x slower                                                 |
| regex_compile            | 77.9 ms                                                | 87.8 ms: 1.13x slower                                                |
| richards_super           | 36.0 ms                                                | 40.8 ms: 1.13x slower                                                |
| richards                 | 32.1 ms                                                | 37.0 ms: 1.15x slower                                                |
| hexiom                   | 4.54 ms                                                | 5.29 ms: 1.16x slower                                                |
| bench_mp_pool            | 44.9 ms                                                | 53.0 ms: 1.18x slower                                                |
| coverage                 | 38.9 ms                                                | 47.5 ms: 1.22x slower                                                |
| telco                    | 3.68 ms                                                | 4.54 ms: 1.23x slower                                                |
| fannkuch                 | 248 ms                                                 | 313 ms: 1.26x slower                                                 |
| scimark_sor              | 87.4 ms                                                | 114 ms: 1.31x slower                                                 |
| mypy2                    | 380 ms                                                 | 535 ms: 1.41x slower                                                 |
| dask                     | 222 ms                                                 | 334 ms: 1.50x slower                                                 |
| python_startup           | 11.4 ms                                                | 18.0 ms: 1.58x slower                                                |
| python_startup_no_site   | 9.37 ms                                                | 16.4 ms: 1.75x slower                                                |
| unpack_sequence          | 31.5 ns                                                | 112 ns: 3.57x slower                                                 |
| Geometric mean           | (ref)                                                  | 1.04x slower                                                         |

Benchmark hidden because not significant (7): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg, unpickle, async_tree_none_tg, sympy_integrate, tornado_http, spectral_norm
Ignored benchmarks (2) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (5) of results/bm-20240229-3.13.0a4+-1a78317-JIT/bm-20240229-darwin-arm64-brandtbucher-justin_arena-3.13.0a4+-1a78317.json: genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 98.14% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.82x