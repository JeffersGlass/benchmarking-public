# Results vs. 3.12.0

- fork: python
- ref: e7ba6e9dbe5433b4a0bc
- machine: darwin-arm64
- commit hash: e7ba6e9
- commit date: 2024-03-05
- overall geometric mean: 1.05x slower \*
- HPT reliability: 98.37%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.82x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 189 ms: 1.12x slower                                                   |
| chameleon      | 4.70 ms                                                | 4.83 ms: 1.03x slower                                                  |
| docutils       | 1.50 sec                                               | 1.53 sec: 1.02x slower                                                 |
| Geometric mean | (ref)                                                  | 1.04x slower                                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 266 ms                                                 | 251 ms: 1.06x faster                                                   |
| async_tree_cpu_io_mixed | 526 ms                                                 | 519 ms: 1.01x faster                                                   |
| async_tree_memoization  | 312 ms                                                 | 327 ms: 1.05x slower                                                   |
| async_tree_io           | 668 ms                                                 | 701 ms: 1.05x slower                                                   |
| Geometric mean          | (ref)                                                  | 1.00x slower                                                           |

Benchmark hidden because not significant (4): async_tree_memoization_tg, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_none_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| float          | 55.8 ms                                                | 53.4 ms: 1.05x faster                                                  |
| nbody          | 68.8 ms                                                | 70.7 ms: 1.03x slower                                                  |
| Geometric mean | (ref)                                                  | 1.01x faster                                                           |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_dna      | 154 ms                                                 | 152 ms: 1.01x faster                                                   |
| regex_effbot   | 2.64 ms                                                | 2.62 ms: 1.01x faster                                                  |
| regex_v8       | 16.0 ms                                                | 17.2 ms: 1.08x slower                                                  |
| regex_compile  | 77.9 ms                                                | 86.4 ms: 1.11x slower                                                  |
| Geometric mean | (ref)                                                  | 1.04x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|---------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| xml_etree_process   | 39.7 ms                                                | 38.8 ms: 1.02x faster                                                  |
| tomli_loads         | 1.39 sec                                               | 1.37 sec: 1.02x faster                                                 |
| pickle_pure_python  | 200 us                                                 | 197 us: 1.01x faster                                                   |
| json_loads          | 17.2 us                                                | 17.0 us: 1.01x faster                                                  |
| pickle_dict         | 18.1 us                                                | 18.1 us: 1.01x slower                                                  |
| xml_etree_iterparse | 74.0 ms                                                | 74.6 ms: 1.01x slower                                                  |
| pickle              | 7.23 us                                                | 7.34 us: 1.02x slower                                                  |
| unpickle            | 9.12 us                                                | 9.27 us: 1.02x slower                                                  |
| pickle_list         | 2.89 us                                                | 2.95 us: 1.02x slower                                                  |
| unpickle_list       | 3.02 us                                                | 3.11 us: 1.03x slower                                                  |
| json_dumps          | 6.22 ms                                                | 6.47 ms: 1.04x slower                                                  |
| Geometric mean      | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (3): xml_etree_parse, unpickle_pure_python, xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 18.7 ms: 1.64x slower                                                  |
| python_startup_no_site | 9.37 ms                                                | 17.0 ms: 1.81x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.73x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako            | 7.71 ms                                                | 6.82 ms: 1.13x faster                                                  |
| django_template | 22.3 ms                                                | 21.8 ms: 1.02x faster                                                  |
| Geometric mean  | (ref)                                                  | 1.08x faster                                                           |

All benchmarks:
===============

| Benchmark                | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 93.0 us                                                | 72.1 us: 1.29x faster                                                  |
| comprehensions           | 14.5 us                                                | 12.7 us: 1.14x faster                                                  |
| mako                     | 7.71 ms                                                | 6.82 ms: 1.13x faster                                                  |
| raytrace                 | 212 ms                                                 | 192 ms: 1.10x faster                                                   |
| generators               | 31.1 ms                                                | 28.4 ms: 1.09x faster                                                  |
| crypto_pyaes             | 51.9 ms                                                | 47.7 ms: 1.09x faster                                                  |
| asyncio_tcp              | 449 ms                                                 | 414 ms: 1.08x faster                                                   |
| deltablue                | 2.71 ms                                                | 2.54 ms: 1.06x faster                                                  |
| logging_simple           | 3.69 us                                                | 3.47 us: 1.06x faster                                                  |
| async_tree_none          | 266 ms                                                 | 251 ms: 1.06x faster                                                   |
| logging_format           | 3.98 us                                                | 3.77 us: 1.06x faster                                                  |
| deepcopy_memo            | 27.7 us                                                | 26.2 us: 1.06x faster                                                  |
| chaos                    | 42.5 ms                                                | 40.5 ms: 1.05x faster                                                  |
| coroutines               | 19.2 ms                                                | 18.3 ms: 1.05x faster                                                  |
| logging_silent           | 76.4 ns                                                | 73.0 ns: 1.05x faster                                                  |
| deepcopy_reduce          | 2.07 us                                                | 1.98 us: 1.05x faster                                                  |
| float                    | 55.8 ms                                                | 53.4 ms: 1.05x faster                                                  |
| json                     | 3.09 ms                                                | 2.98 ms: 1.04x faster                                                  |
| gunicorn                 | 1.15 ms                                                | 1.11 ms: 1.03x faster                                                  |
| sympy_str                | 148 ms                                                 | 144 ms: 1.02x faster                                                   |
| django_template          | 22.3 ms                                                | 21.8 ms: 1.02x faster                                                  |
| aiohttp                  | 1.08 ms                                                | 1.05 ms: 1.02x faster                                                  |
| spectral_norm            | 76.4 ms                                                | 74.6 ms: 1.02x faster                                                  |
| xml_etree_process        | 39.7 ms                                                | 38.8 ms: 1.02x faster                                                  |
| deepcopy                 | 235 us                                                 | 231 us: 1.02x faster                                                   |
| sympy_sum                | 77.6 ms                                                | 76.3 ms: 1.02x faster                                                  |
| tomli_loads              | 1.39 sec                                               | 1.37 sec: 1.02x faster                                                 |
| sqlglot_parse            | 848 us                                                 | 835 us: 1.01x faster                                                   |
| regex_dna                | 154 ms                                                 | 152 ms: 1.01x faster                                                   |
| pickle_pure_python       | 200 us                                                 | 197 us: 1.01x faster                                                   |
| async_tree_cpu_io_mixed  | 526 ms                                                 | 519 ms: 1.01x faster                                                   |
| json_loads               | 17.2 us                                                | 17.0 us: 1.01x faster                                                  |
| sqlglot_normalize        | 186 ms                                                 | 184 ms: 1.01x faster                                                   |
| regex_effbot             | 2.64 ms                                                | 2.62 ms: 1.01x faster                                                  |
| asyncio_websockets       | 409 ms                                                 | 408 ms: 1.00x faster                                                   |
| scimark_sparse_mat_mult  | 3.14 ms                                                | 3.14 ms: 1.00x slower                                                  |
| gc_traversal             | 2.40 ms                                                | 2.41 ms: 1.00x slower                                                  |
| sqlglot_transpile        | 1.02 ms                                                | 1.03 ms: 1.00x slower                                                  |
| sympy_integrate          | 11.4 ms                                                | 11.4 ms: 1.00x slower                                                  |
| pickle_dict              | 18.1 us                                                | 18.1 us: 1.01x slower                                                  |
| sqlite_synth             | 1.57 us                                                | 1.58 us: 1.01x slower                                                  |
| xml_etree_iterparse      | 74.0 ms                                                | 74.6 ms: 1.01x slower                                                  |
| scimark_monte_carlo      | 45.0 ms                                                | 45.7 ms: 1.01x slower                                                  |
| pickle                   | 7.23 us                                                | 7.34 us: 1.02x slower                                                  |
| unpickle                 | 9.12 us                                                | 9.27 us: 1.02x slower                                                  |
| sympy_expand             | 241 ms                                                 | 245 ms: 1.02x slower                                                   |
| docutils                 | 1.50 sec                                               | 1.53 sec: 1.02x slower                                                 |
| create_gc_cycles         | 701 us                                                 | 714 us: 1.02x slower                                                   |
| nqueens                  | 62.4 ms                                                | 63.7 ms: 1.02x slower                                                  |
| scimark_fft              | 195 ms                                                 | 199 ms: 1.02x slower                                                   |
| pickle_list              | 2.89 us                                                | 2.95 us: 1.02x slower                                                  |
| bench_thread_pool        | 504 us                                                 | 516 us: 1.02x slower                                                   |
| mdp                      | 1.58 sec                                               | 1.62 sec: 1.02x slower                                                 |
| async_generators         | 304 ms                                                 | 312 ms: 1.03x slower                                                   |
| nbody                    | 68.8 ms                                                | 70.7 ms: 1.03x slower                                                  |
| chameleon                | 4.70 ms                                                | 4.83 ms: 1.03x slower                                                  |
| unpickle_list            | 3.02 us                                                | 3.11 us: 1.03x slower                                                  |
| dulwich_log              | 29.8 ms                                                | 30.8 ms: 1.03x slower                                                  |
| pprint_safe_repr         | 497 ms                                                 | 516 ms: 1.04x slower                                                   |
| pathlib                  | 24.2 ms                                                | 25.2 ms: 1.04x slower                                                  |
| sqlglot_optimize         | 34.0 ms                                                | 35.4 ms: 1.04x slower                                                  |
| json_dumps               | 6.22 ms                                                | 6.47 ms: 1.04x slower                                                  |
| async_tree_memoization   | 312 ms                                                 | 327 ms: 1.05x slower                                                   |
| asyncio_tcp_ssl          | 1.24 sec                                               | 1.30 sec: 1.05x slower                                                 |
| async_tree_io            | 668 ms                                                 | 701 ms: 1.05x slower                                                   |
| pprint_pformat           | 1.01 sec                                               | 1.06 sec: 1.05x slower                                                 |
| meteor_contest           | 71.7 ms                                                | 75.4 ms: 1.05x slower                                                  |
| regex_v8                 | 16.0 ms                                                | 17.2 ms: 1.08x slower                                                  |
| pycparser                | 677 ms                                                 | 735 ms: 1.09x slower                                                   |
| pyflate                  | 316 ms                                                 | 344 ms: 1.09x slower                                                   |
| regex_compile            | 77.9 ms                                                | 86.4 ms: 1.11x slower                                                  |
| 2to3                     | 169 ms                                                 | 189 ms: 1.12x slower                                                   |
| scimark_lu               | 76.0 ms                                                | 85.8 ms: 1.13x slower                                                  |
| go                       | 102 ms                                                 | 117 ms: 1.15x slower                                                   |
| hexiom                   | 4.54 ms                                                | 5.26 ms: 1.16x slower                                                  |
| richards_super           | 36.0 ms                                                | 42.7 ms: 1.19x slower                                                  |
| bench_mp_pool            | 44.9 ms                                                | 53.4 ms: 1.19x slower                                                  |
| telco                    | 3.68 ms                                                | 4.46 ms: 1.21x slower                                                  |
| richards                 | 32.1 ms                                                | 39.1 ms: 1.22x slower                                                  |
| coverage                 | 38.9 ms                                                | 47.5 ms: 1.22x slower                                                  |
| fannkuch                 | 248 ms                                                 | 312 ms: 1.26x slower                                                   |
| scimark_sor              | 87.4 ms                                                | 112 ms: 1.28x slower                                                   |
| mypy2                    | 380 ms                                                 | 540 ms: 1.42x slower                                                   |
| dask                     | 222 ms                                                 | 334 ms: 1.50x slower                                                   |
| python_startup           | 11.4 ms                                                | 18.7 ms: 1.64x slower                                                  |
| python_startup_no_site   | 9.37 ms                                                | 17.0 ms: 1.81x slower                                                  |
| unpack_sequence          | 31.5 ns                                                | 113 ns: 3.60x slower                                                   |
| Geometric mean           | (ref)                                                  | 1.05x slower                                                           |

Benchmark hidden because not significant (9): async_tree_memoization_tg, async_tree_cpu_io_mixed_tg, xml_etree_parse, async_tree_io_tg, async_tree_none_tg, pidigits, unpickle_pure_python, xml_etree_generate, tornado_http
Ignored benchmarks (2) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (5) of results/bm-20240305-3.13.0a4+-e7ba6e9-JIT/bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9.json: genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 98.37% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.82x