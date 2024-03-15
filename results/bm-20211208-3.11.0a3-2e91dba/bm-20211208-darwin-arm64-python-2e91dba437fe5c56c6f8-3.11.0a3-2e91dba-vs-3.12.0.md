
# Results vs. 3.12.0

- fork: python
- ref: 2e91dba437fe5c56c6f8
- machine: darwin-arm64
- commit hash: 2e91dba
- commit date: 2021-12-08
- overall geometric mean: 1.03x slower \*
- HPT reliability: 71.73%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.97x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211208-darwin-arm64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 155 ms: 1.09x faster                                                  |
| chameleon      | 4.70 ms                                                | 4.65 ms: 1.01x faster                                                 |
| docutils       | 1.50 sec                                               | 1.48 sec: 1.02x faster                                                |
| tornado_http   | 69.3 ms                                                | 76.9 ms: 1.11x slower                                                 |
| Geometric mean | (ref)                                                  | 1.00x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211208-darwin-arm64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 526 ms                                                 | 558 ms: 1.06x slower                                                  |
| async_tree_none         | 266 ms                                                 | 288 ms: 1.08x slower                                                  |
| async_tree_memoization  | 312 ms                                                 | 374 ms: 1.20x slower                                                  |
| async_tree_io           | 668 ms                                                 | 816 ms: 1.22x slower                                                  |
| Geometric mean          | (ref)                                                  | 1.14x slower                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211208-darwin-arm64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| float          | 55.8 ms                                                | 51.6 ms: 1.08x faster                                                 |
| nbody          | 68.8 ms                                                | 64.4 ms: 1.07x faster                                                 |
| Geometric mean | (ref)                                                  | 1.05x faster                                                          |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211208-darwin-arm64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_effbot   | 2.64 ms                                                | 2.45 ms: 1.08x faster                                                 |
| regex_compile  | 77.9 ms                                                | 72.7 ms: 1.07x faster                                                 |
| regex_v8       | 16.0 ms                                                | 16.6 ms: 1.04x slower                                                 |
| regex_dna      | 154 ms                                                 | 173 ms: 1.12x slower                                                  |
| Geometric mean | (ref)                                                  | 1.00x slower                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211208-darwin-arm64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| xml_etree_generate   | 55.8 ms                                                | 47.3 ms: 1.18x faster                                                 |
| xml_etree_process    | 39.7 ms                                                | 35.1 ms: 1.13x faster                                                 |
| json_loads           | 17.2 us                                                | 15.3 us: 1.13x faster                                                 |
| xml_etree_parse      | 106 ms                                                 | 96.7 ms: 1.10x faster                                                 |
| unpickle_list        | 3.02 us                                                | 2.75 us: 1.10x faster                                                 |
| pickle_list          | 2.89 us                                                | 2.67 us: 1.08x faster                                                 |
| pickle_dict          | 18.1 us                                                | 16.8 us: 1.07x faster                                                 |
| xml_etree_iterparse  | 74.0 ms                                                | 69.6 ms: 1.06x faster                                                 |
| unpickle             | 9.12 us                                                | 8.57 us: 1.06x faster                                                 |
| tomli_loads          | 1.39 sec                                               | 1.36 sec: 1.03x faster                                                |
| pickle_pure_python   | 200 us                                                 | 203 us: 1.02x slower                                                  |
| pickle               | 7.23 us                                                | 7.39 us: 1.02x slower                                                 |
| unpickle_pure_python | 151 us                                                 | 158 us: 1.05x slower                                                  |
| json_dumps           | 6.22 ms                                                | 7.46 ms: 1.20x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.05x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211208-darwin-arm64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup_no_site | 9.37 ms                                                | 9.02 ms: 1.04x faster                                                 |
| python_startup         | 11.4 ms                                                | 14.9 ms: 1.30x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.12x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211208-darwin-arm64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| django_template | 22.3 ms                                                | 20.8 ms: 1.08x faster                                                 |
| mako            | 7.71 ms                                                | 8.07 ms: 1.05x slower                                                 |
| Geometric mean  | (ref)                                                  | 1.01x faster                                                          |

All benchmarks:
===============

| Benchmark                | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211208-darwin-arm64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|--------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_generators         | 304 ms                                                 | 191 ms: 1.59x faster                                                  |
| sqlite_synth             | 1.57 us                                                | 1.32 us: 1.19x faster                                                 |
| xml_etree_generate       | 55.8 ms                                                | 47.3 ms: 1.18x faster                                                 |
| generators               | 31.1 ms                                                | 26.6 ms: 1.17x faster                                                 |
| logging_simple           | 3.69 us                                                | 3.19 us: 1.16x faster                                                 |
| logging_format           | 3.98 us                                                | 3.49 us: 1.14x faster                                                 |
| coroutines               | 19.2 ms                                                | 16.9 ms: 1.14x faster                                                 |
| sqlglot_normalize        | 186 ms                                                 | 164 ms: 1.13x faster                                                  |
| xml_etree_process        | 39.7 ms                                                | 35.1 ms: 1.13x faster                                                 |
| json_loads               | 17.2 us                                                | 15.3 us: 1.13x faster                                                 |
| nqueens                  | 62.4 ms                                                | 55.5 ms: 1.12x faster                                                 |
| telco                    | 3.68 ms                                                | 3.31 ms: 1.11x faster                                                 |
| xml_etree_parse          | 106 ms                                                 | 96.7 ms: 1.10x faster                                                 |
| unpickle_list            | 3.02 us                                                | 2.75 us: 1.10x faster                                                 |
| deepcopy_reduce          | 2.07 us                                                | 1.89 us: 1.09x faster                                                 |
| 2to3                     | 169 ms                                                 | 155 ms: 1.09x faster                                                  |
| bench_mp_pool            | 44.9 ms                                                | 41.4 ms: 1.08x faster                                                 |
| pickle_list              | 2.89 us                                                | 2.67 us: 1.08x faster                                                 |
| float                    | 55.8 ms                                                | 51.6 ms: 1.08x faster                                                 |
| sqlglot_optimize         | 34.0 ms                                                | 31.6 ms: 1.08x faster                                                 |
| json                     | 3.09 ms                                                | 2.86 ms: 1.08x faster                                                 |
| regex_effbot             | 2.64 ms                                                | 2.45 ms: 1.08x faster                                                 |
| django_template          | 22.3 ms                                                | 20.8 ms: 1.08x faster                                                 |
| pickle_dict              | 18.1 us                                                | 16.8 us: 1.07x faster                                                 |
| regex_compile            | 77.9 ms                                                | 72.7 ms: 1.07x faster                                                 |
| pprint_safe_repr         | 497 ms                                                 | 465 ms: 1.07x faster                                                  |
| nbody                    | 68.8 ms                                                | 64.4 ms: 1.07x faster                                                 |
| spectral_norm            | 76.4 ms                                                | 71.6 ms: 1.07x faster                                                 |
| xml_etree_iterparse      | 74.0 ms                                                | 69.6 ms: 1.06x faster                                                 |
| deepcopy_memo            | 27.7 us                                                | 26.0 us: 1.06x faster                                                 |
| scimark_lu               | 76.0 ms                                                | 71.4 ms: 1.06x faster                                                 |
| unpickle                 | 9.12 us                                                | 8.57 us: 1.06x faster                                                 |
| pprint_pformat           | 1.01 sec                                               | 952 ms: 1.06x faster                                                  |
| scimark_fft              | 195 ms                                                 | 184 ms: 1.06x faster                                                  |
| deepcopy                 | 235 us                                                 | 224 us: 1.05x faster                                                  |
| scimark_sparse_mat_mult  | 3.14 ms                                                | 3.01 ms: 1.04x faster                                                 |
| scimark_monte_carlo      | 45.0 ms                                                | 43.2 ms: 1.04x faster                                                 |
| python_startup_no_site   | 9.37 ms                                                | 9.02 ms: 1.04x faster                                                 |
| pathlib                  | 24.2 ms                                                | 23.3 ms: 1.04x faster                                                 |
| hexiom                   | 4.54 ms                                                | 4.41 ms: 1.03x faster                                                 |
| logging_silent           | 76.4 ns                                                | 74.3 ns: 1.03x faster                                                 |
| tomli_loads              | 1.39 sec                                               | 1.36 sec: 1.03x faster                                                |
| scimark_sor              | 87.4 ms                                                | 85.3 ms: 1.02x faster                                                 |
| docutils                 | 1.50 sec                                               | 1.48 sec: 1.02x faster                                                |
| unpack_sequence          | 31.5 ns                                                | 31.0 ns: 1.01x faster                                                 |
| bench_thread_pool        | 504 us                                                 | 498 us: 1.01x faster                                                  |
| chameleon                | 4.70 ms                                                | 4.65 ms: 1.01x faster                                                 |
| dulwich_log              | 29.8 ms                                                | 29.6 ms: 1.01x faster                                                 |
| sympy_integrate          | 11.4 ms                                                | 11.3 ms: 1.01x faster                                                 |
| fannkuch                 | 248 ms                                                 | 247 ms: 1.00x faster                                                  |
| gc_traversal             | 2.40 ms                                                | 2.40 ms: 1.00x faster                                                 |
| sqlalchemy_declarative   | 62.3 ms                                                | 62.6 ms: 1.00x slower                                                 |
| sympy_expand             | 241 ms                                                 | 244 ms: 1.01x slower                                                  |
| pickle_pure_python       | 200 us                                                 | 203 us: 1.02x slower                                                  |
| sympy_str                | 148 ms                                                 | 151 ms: 1.02x slower                                                  |
| pyflate                  | 316 ms                                                 | 322 ms: 1.02x slower                                                  |
| pickle                   | 7.23 us                                                | 7.39 us: 1.02x slower                                                 |
| raytrace                 | 212 ms                                                 | 218 ms: 1.03x slower                                                  |
| richards                 | 32.1 ms                                                | 33.2 ms: 1.03x slower                                                 |
| pycparser                | 677 ms                                                 | 702 ms: 1.04x slower                                                  |
| create_gc_cycles         | 701 us                                                 | 729 us: 1.04x slower                                                  |
| regex_v8                 | 16.0 ms                                                | 16.6 ms: 1.04x slower                                                 |
| mako                     | 7.71 ms                                                | 8.07 ms: 1.05x slower                                                 |
| unpickle_pure_python     | 151 us                                                 | 158 us: 1.05x slower                                                  |
| sympy_sum                | 77.6 ms                                                | 82.2 ms: 1.06x slower                                                 |
| async_tree_cpu_io_mixed  | 526 ms                                                 | 558 ms: 1.06x slower                                                  |
| gunicorn                 | 1.15 ms                                                | 1.23 ms: 1.07x slower                                                 |
| crypto_pyaes             | 51.9 ms                                                | 56.0 ms: 1.08x slower                                                 |
| async_tree_none          | 266 ms                                                 | 288 ms: 1.08x slower                                                  |
| chaos                    | 42.5 ms                                                | 46.4 ms: 1.09x slower                                                 |
| deltablue                | 2.71 ms                                                | 2.96 ms: 1.09x slower                                                 |
| tornado_http             | 69.3 ms                                                | 76.9 ms: 1.11x slower                                                 |
| mdp                      | 1.58 sec                                               | 1.76 sec: 1.11x slower                                                |
| sqlalchemy_imperative    | 6.68 ms                                                | 7.43 ms: 1.11x slower                                                 |
| go                       | 102 ms                                                 | 113 ms: 1.12x slower                                                  |
| regex_dna                | 154 ms                                                 | 173 ms: 1.12x slower                                                  |
| comprehensions           | 14.5 us                                                | 16.5 us: 1.14x slower                                                 |
| richards_super           | 36.0 ms                                                | 42.7 ms: 1.19x slower                                                 |
| async_tree_memoization   | 312 ms                                                 | 374 ms: 1.20x slower                                                  |
| json_dumps               | 6.22 ms                                                | 7.46 ms: 1.20x slower                                                 |
| async_tree_io            | 668 ms                                                 | 816 ms: 1.22x slower                                                  |
| python_startup           | 11.4 ms                                                | 14.9 ms: 1.30x slower                                                 |
| sqlglot_transpile        | 1.02 ms                                                | 1.35 ms: 1.33x slower                                                 |
| dask                     | 222 ms                                                 | 302 ms: 1.36x slower                                                  |
| sqlglot_parse            | 848 us                                                 | 1.19 ms: 1.40x slower                                                 |
| typing_runtime_protocols | 93.0 us                                                | 325 us: 3.49x slower                                                  |
| coverage                 | 38.9 ms                                                | 303 ms: 7.79x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.03x slower                                                          |

Benchmark hidden because not significant (2): meteor_contest, pidigits
Ignored benchmarks (9) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, mypy2
Ignored benchmarks (6) of results/bm-20211208-3.11.0a3-2e91dba/bm-20211208-darwin-arm64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 71.73% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.97x