
# Results vs. 3.11.0

- fork: python
- ref: 2e91dba437fe5c56c6f8
- machine: darwin-arm64
- commit hash: 2e91dba
- commit date: 2021-12-08
- overall geometric mean: 1.07x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 1.03x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20211208-darwin-arm64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 155 ms: 1.01x slower                                                  |
| chameleon      | 4.30 ms                                                | 4.65 ms: 1.08x slower                                                 |
| docutils       | 1.43 sec                                               | 1.48 sec: 1.03x slower                                                |
| html5lib       | 33.0 ms                                                | 33.6 ms: 1.02x slower                                                 |
| tornado_http   | 69.1 ms                                                | 76.9 ms: 1.11x slower                                                 |
| Geometric mean | (ref)                                                  | 1.05x slower                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20211208-darwin-arm64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_none         | 282 ms                                                 | 288 ms: 1.02x slower                                                  |
| async_tree_cpu_io_mixed | 519 ms                                                 | 558 ms: 1.08x slower                                                  |
| async_tree_memoization  | 336 ms                                                 | 374 ms: 1.11x slower                                                  |
| async_tree_io           | 697 ms                                                 | 816 ms: 1.17x slower                                                  |
| Geometric mean          | (ref)                                                  | 1.09x slower                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20211208-darwin-arm64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 282 ms: 1.00x slower                                                  |
| float          | 50.8 ms                                                | 51.6 ms: 1.02x slower                                                 |
| nbody          | 61.7 ms                                                | 64.4 ms: 1.04x slower                                                 |
| Geometric mean | (ref)                                                  | 1.02x slower                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20211208-darwin-arm64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 72.8 ms                                                | 72.7 ms: 1.00x faster                                                 |
| regex_effbot   | 2.43 ms                                                | 2.45 ms: 1.01x slower                                                 |
| regex_v8       | 15.1 ms                                                | 16.6 ms: 1.10x slower                                                 |
| regex_dna      | 148 ms                                                 | 173 ms: 1.17x slower                                                  |
| Geometric mean | (ref)                                                  | 1.07x slower                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20211208-darwin-arm64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| xml_etree_parse      | 100 ms                                                 | 96.7 ms: 1.04x faster                                                 |
| pickle_dict          | 17.1 us                                                | 16.8 us: 1.01x faster                                                 |
| json_dumps           | 7.53 ms                                                | 7.46 ms: 1.01x faster                                                 |
| pickle_list          | 2.70 us                                                | 2.67 us: 1.01x faster                                                 |
| json_loads           | 15.3 us                                                | 15.3 us: 1.00x faster                                                 |
| xml_etree_iterparse  | 68.3 ms                                                | 69.6 ms: 1.02x slower                                                 |
| unpickle_list        | 2.69 us                                                | 2.75 us: 1.03x slower                                                 |
| xml_etree_generate   | 45.8 ms                                                | 47.3 ms: 1.03x slower                                                 |
| unpickle             | 8.29 us                                                | 8.57 us: 1.03x slower                                                 |
| xml_etree_process    | 33.6 ms                                                | 35.1 ms: 1.05x slower                                                 |
| pickle               | 6.98 us                                                | 7.39 us: 1.06x slower                                                 |
| pickle_pure_python   | 191 us                                                 | 203 us: 1.06x slower                                                  |
| unpickle_pure_python | 149 us                                                 | 158 us: 1.06x slower                                                  |
| tomli_loads          | 1.27 sec                                               | 1.36 sec: 1.07x slower                                                |
| Geometric mean       | (ref)                                                  | 1.02x slower                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20211208-darwin-arm64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup_no_site | 8.57 ms                                                | 9.02 ms: 1.05x slower                                                 |
| python_startup         | 10.8 ms                                                | 14.9 ms: 1.38x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.21x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20211208-darwin-arm64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 7.93 ms                                                | 8.07 ms: 1.02x slower                                                 |
| genshi_text     | 14.4 ms                                                | 14.8 ms: 1.03x slower                                                 |
| genshi_xml      | 28.5 ms                                                | 29.4 ms: 1.03x slower                                                 |
| django_template | 20.1 ms                                                | 20.8 ms: 1.03x slower                                                 |
| Geometric mean  | (ref)                                                  | 1.03x slower                                                          |

All benchmarks:
===============

| Benchmark                | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20211208-darwin-arm64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|--------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| generators               | 30.3 ms                                                | 26.6 ms: 1.14x faster                                                 |
| unpack_sequence          | 33.6 ns                                                | 31.0 ns: 1.08x faster                                                 |
| logging_simple           | 3.41 us                                                | 3.19 us: 1.07x faster                                                 |
| logging_format           | 3.67 us                                                | 3.49 us: 1.05x faster                                                 |
| pylint                   | 253 ms                                                 | 241 ms: 1.05x faster                                                  |
| hexiom                   | 4.58 ms                                                | 4.41 ms: 1.04x faster                                                 |
| xml_etree_parse          | 100 ms                                                 | 96.7 ms: 1.04x faster                                                 |
| pprint_safe_repr         | 478 ms                                                 | 465 ms: 1.03x faster                                                  |
| pprint_pformat           | 979 ms                                                 | 952 ms: 1.03x faster                                                  |
| chaos                    | 47.4 ms                                                | 46.4 ms: 1.02x faster                                                 |
| pickle_dict              | 17.1 us                                                | 16.8 us: 1.01x faster                                                 |
| coroutines               | 17.2 ms                                                | 16.9 ms: 1.01x faster                                                 |
| json_dumps               | 7.53 ms                                                | 7.46 ms: 1.01x faster                                                 |
| pickle_list              | 2.70 us                                                | 2.67 us: 1.01x faster                                                 |
| nqueens                  | 55.9 ms                                                | 55.5 ms: 1.01x faster                                                 |
| async_generators         | 192 ms                                                 | 191 ms: 1.01x faster                                                  |
| scimark_monte_carlo      | 43.5 ms                                                | 43.2 ms: 1.01x faster                                                 |
| json_loads               | 15.3 us                                                | 15.3 us: 1.00x faster                                                 |
| regex_compile            | 72.8 ms                                                | 72.7 ms: 1.00x faster                                                 |
| sympy_integrate          | 11.3 ms                                                | 11.3 ms: 1.00x slower                                                 |
| pidigits                 | 280 ms                                                 | 282 ms: 1.00x slower                                                  |
| gc_traversal             | 2.38 ms                                                | 2.40 ms: 1.01x slower                                                 |
| 2to3                     | 154 ms                                                 | 155 ms: 1.01x slower                                                  |
| meteor_contest           | 71.1 ms                                                | 71.7 ms: 1.01x slower                                                 |
| regex_effbot             | 2.43 ms                                                | 2.45 ms: 1.01x slower                                                 |
| deepcopy_memo            | 25.7 us                                                | 26.0 us: 1.01x slower                                                 |
| sqlglot_normalize        | 162 ms                                                 | 164 ms: 1.02x slower                                                  |
| float                    | 50.8 ms                                                | 51.6 ms: 1.02x slower                                                 |
| mako                     | 7.93 ms                                                | 8.07 ms: 1.02x slower                                                 |
| xml_etree_iterparse      | 68.3 ms                                                | 69.6 ms: 1.02x slower                                                 |
| html5lib                 | 33.0 ms                                                | 33.6 ms: 1.02x slower                                                 |
| async_tree_none          | 282 ms                                                 | 288 ms: 1.02x slower                                                  |
| unpickle_list            | 2.69 us                                                | 2.75 us: 1.03x slower                                                 |
| genshi_text              | 14.4 ms                                                | 14.8 ms: 1.03x slower                                                 |
| sympy_sum                | 80.2 ms                                                | 82.2 ms: 1.03x slower                                                 |
| create_gc_cycles         | 711 us                                                 | 729 us: 1.03x slower                                                  |
| genshi_xml               | 28.5 ms                                                | 29.4 ms: 1.03x slower                                                 |
| django_template          | 20.1 ms                                                | 20.8 ms: 1.03x slower                                                 |
| xml_etree_generate       | 45.8 ms                                                | 47.3 ms: 1.03x slower                                                 |
| fannkuch                 | 240 ms                                                 | 247 ms: 1.03x slower                                                  |
| flaskblogging            | 2.35 ms                                                | 2.43 ms: 1.03x slower                                                 |
| dulwich_log              | 28.6 ms                                                | 29.6 ms: 1.03x slower                                                 |
| docutils                 | 1.43 sec                                               | 1.48 sec: 1.03x slower                                                |
| unpickle                 | 8.29 us                                                | 8.57 us: 1.03x slower                                                 |
| json                     | 2.75 ms                                                | 2.86 ms: 1.04x slower                                                 |
| deepcopy                 | 215 us                                                 | 224 us: 1.04x slower                                                  |
| nbody                    | 61.7 ms                                                | 64.4 ms: 1.04x slower                                                 |
| telco                    | 3.17 ms                                                | 3.31 ms: 1.05x slower                                                 |
| xml_etree_process        | 33.6 ms                                                | 35.1 ms: 1.05x slower                                                 |
| sympy_str                | 144 ms                                                 | 151 ms: 1.05x slower                                                  |
| sqlite_synth             | 1.26 us                                                | 1.32 us: 1.05x slower                                                 |
| python_startup_no_site   | 8.57 ms                                                | 9.02 ms: 1.05x slower                                                 |
| scimark_lu               | 67.7 ms                                                | 71.4 ms: 1.05x slower                                                 |
| deepcopy_reduce          | 1.79 us                                                | 1.89 us: 1.05x slower                                                 |
| sqlalchemy_declarative   | 59.3 ms                                                | 62.6 ms: 1.06x slower                                                 |
| pickle                   | 6.98 us                                                | 7.39 us: 1.06x slower                                                 |
| pickle_pure_python       | 191 us                                                 | 203 us: 1.06x slower                                                  |
| raytrace                 | 206 ms                                                 | 218 ms: 1.06x slower                                                  |
| unpickle_pure_python     | 149 us                                                 | 158 us: 1.06x slower                                                  |
| sqlglot_optimize         | 29.6 ms                                                | 31.6 ms: 1.07x slower                                                 |
| pycparser                | 659 ms                                                 | 702 ms: 1.07x slower                                                  |
| sqlalchemy_imperative    | 6.98 ms                                                | 7.43 ms: 1.07x slower                                                 |
| tomli_loads              | 1.27 sec                                               | 1.36 sec: 1.07x slower                                                |
| sympy_expand             | 229 ms                                                 | 244 ms: 1.07x slower                                                  |
| scimark_fft              | 173 ms                                                 | 184 ms: 1.07x slower                                                  |
| scimark_sparse_mat_mult  | 2.81 ms                                                | 3.01 ms: 1.07x slower                                                 |
| bench_thread_pool        | 465 us                                                 | 498 us: 1.07x slower                                                  |
| richards                 | 31.1 ms                                                | 33.2 ms: 1.07x slower                                                 |
| thrift                   | 410 us                                                 | 440 us: 1.07x slower                                                  |
| go                       | 105 ms                                                 | 113 ms: 1.07x slower                                                  |
| async_tree_cpu_io_mixed  | 519 ms                                                 | 558 ms: 1.08x slower                                                  |
| deltablue                | 2.75 ms                                                | 2.96 ms: 1.08x slower                                                 |
| scimark_sor              | 79.2 ms                                                | 85.3 ms: 1.08x slower                                                 |
| typing_runtime_protocols | 301 us                                                 | 325 us: 1.08x slower                                                  |
| chameleon                | 4.30 ms                                                | 4.65 ms: 1.08x slower                                                 |
| spectral_norm            | 65.7 ms                                                | 71.6 ms: 1.09x slower                                                 |
| regex_v8                 | 15.1 ms                                                | 16.6 ms: 1.10x slower                                                 |
| async_tree_memoization   | 336 ms                                                 | 374 ms: 1.11x slower                                                  |
| tornado_http             | 69.1 ms                                                | 76.9 ms: 1.11x slower                                                 |
| logging_silent           | 66.5 ns                                                | 74.3 ns: 1.12x slower                                                 |
| gunicorn                 | 1.10 ms                                                | 1.23 ms: 1.12x slower                                                 |
| pyflate                  | 284 ms                                                 | 322 ms: 1.14x slower                                                  |
| comprehensions           | 14.4 us                                                | 16.5 us: 1.14x slower                                                 |
| richards_super           | 37.3 ms                                                | 42.7 ms: 1.15x slower                                                 |
| regex_dna                | 148 ms                                                 | 173 ms: 1.17x slower                                                  |
| async_tree_io            | 697 ms                                                 | 816 ms: 1.17x slower                                                  |
| crypto_pyaes             | 47.5 ms                                                | 56.0 ms: 1.18x slower                                                 |
| mdp                      | 1.48 sec                                               | 1.76 sec: 1.18x slower                                                |
| sqlglot_transpile        | 1.05 ms                                                | 1.35 ms: 1.29x slower                                                 |
| sqlglot_parse            | 890 us                                                 | 1.19 ms: 1.33x slower                                                 |
| dask                     | 219 ms                                                 | 302 ms: 1.38x slower                                                  |
| python_startup           | 10.8 ms                                                | 14.9 ms: 1.38x slower                                                 |
| coverage                 | 43.9 ms                                                | 303 ms: 6.90x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.07x slower                                                          |

Benchmark hidden because not significant (2): pathlib, bench_mp_pool
Ignored benchmarks (9) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, mypy2


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.03x
- 95% likely to have a slowdown of 1.03x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 1.03x