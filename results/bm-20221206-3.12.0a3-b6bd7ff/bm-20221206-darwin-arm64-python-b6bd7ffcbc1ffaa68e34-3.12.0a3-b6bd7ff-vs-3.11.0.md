
# Results vs. 3.11.0

- fork: python
- ref: b6bd7ffcbc1ffaa68e34
- machine: darwin-arm64
- commit hash: b6bd7ff
- commit date: 2022-12-06
- overall geometric mean: 1.07x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 166 ms: 1.07x slower                                                  |
| chameleon      | 4.30 ms                                                | 4.68 ms: 1.09x slower                                                 |
| docutils       | 1.43 sec                                               | 1.48 sec: 1.03x slower                                                |
| html5lib       | 33.0 ms                                                | 34.7 ms: 1.05x slower                                                 |
| Geometric mean | (ref)                                                  | 1.06x slower                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_io_tg        | 724 ms                                                 | 733 ms: 1.01x slower                                                  |
| async_tree_cpu_io_mixed | 519 ms                                                 | 539 ms: 1.04x slower                                                  |
| async_tree_none         | 282 ms                                                 | 295 ms: 1.05x slower                                                  |
| async_tree_io           | 697 ms                                                 | 758 ms: 1.09x slower                                                  |
| Geometric mean          | (ref)                                                  | 1.02x slower                                                          |

Benchmark hidden because not significant (4): async_tree_memoization, async_tree_memoization_tg, async_tree_none_tg, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 280 ms: 1.00x faster                                                  |
| nbody          | 61.7 ms                                                | 68.4 ms: 1.11x slower                                                 |
| float          | 50.8 ms                                                | 57.6 ms: 1.13x slower                                                 |
| Geometric mean | (ref)                                                  | 1.08x slower                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_dna      | 148 ms                                                 | 147 ms: 1.01x faster                                                  |
| regex_v8       | 15.1 ms                                                | 15.1 ms: 1.00x faster                                                 |
| regex_effbot   | 2.43 ms                                                | 2.45 ms: 1.01x slower                                                 |
| regex_compile  | 72.8 ms                                                | 78.1 ms: 1.07x slower                                                 |
| Geometric mean | (ref)                                                  | 1.02x slower                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.15 ms: 1.22x faster                                                 |
| xml_etree_parse      | 100 ms                                                 | 96.5 ms: 1.04x faster                                                 |
| pickle_list          | 2.70 us                                                | 2.67 us: 1.01x faster                                                 |
| pickle_dict          | 17.1 us                                                | 17.0 us: 1.00x faster                                                 |
| unpickle             | 8.29 us                                                | 8.45 us: 1.02x slower                                                 |
| pickle               | 6.98 us                                                | 7.13 us: 1.02x slower                                                 |
| unpickle_list        | 2.69 us                                                | 2.75 us: 1.02x slower                                                 |
| json_loads           | 15.3 us                                                | 15.8 us: 1.03x slower                                                 |
| xml_etree_iterparse  | 68.3 ms                                                | 70.3 ms: 1.03x slower                                                 |
| xml_etree_generate   | 45.8 ms                                                | 47.5 ms: 1.04x slower                                                 |
| unpickle_pure_python | 149 us                                                 | 160 us: 1.08x slower                                                  |
| xml_etree_process    | 33.6 ms                                                | 36.4 ms: 1.08x slower                                                 |
| pickle_pure_python   | 191 us                                                 | 213 us: 1.11x slower                                                  |
| tomli_loads          | 1.27 sec                                               | 1.51 sec: 1.18x slower                                                |
| Geometric mean       | (ref)                                                  | 1.02x slower                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 11.4 ms: 1.06x slower                                                 |
| python_startup_no_site | 8.57 ms                                                | 9.48 ms: 1.11x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.09x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 7.93 ms                                                | 7.45 ms: 1.06x faster                                                 |
| genshi_xml      | 28.5 ms                                                | 30.7 ms: 1.07x slower                                                 |
| django_template | 20.1 ms                                                | 21.9 ms: 1.09x slower                                                 |
| genshi_text     | 14.4 ms                                                | 15.9 ms: 1.10x slower                                                 |
| Geometric mean  | (ref)                                                  | 1.05x slower                                                          |

All benchmarks:
===============

| Benchmark                | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|--------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| json_dumps               | 7.53 ms                                                | 6.15 ms: 1.22x faster                                                 |
| mako                     | 7.93 ms                                                | 7.45 ms: 1.06x faster                                                 |
| scimark_sparse_mat_mult  | 2.81 ms                                                | 2.65 ms: 1.06x faster                                                 |
| create_gc_cycles         | 711 us                                                 | 682 us: 1.04x faster                                                  |
| unpack_sequence          | 33.6 ns                                                | 32.3 ns: 1.04x faster                                                 |
| xml_etree_parse          | 100 ms                                                 | 96.5 ms: 1.04x faster                                                 |
| telco                    | 3.17 ms                                                | 3.09 ms: 1.02x faster                                                 |
| pickle_list              | 2.70 us                                                | 2.67 us: 1.01x faster                                                 |
| regex_dna                | 148 ms                                                 | 147 ms: 1.01x faster                                                  |
| pickle_dict              | 17.1 us                                                | 17.0 us: 1.00x faster                                                 |
| gc_traversal             | 2.38 ms                                                | 2.38 ms: 1.00x faster                                                 |
| pidigits                 | 280 ms                                                 | 280 ms: 1.00x faster                                                  |
| regex_v8                 | 15.1 ms                                                | 15.1 ms: 1.00x faster                                                 |
| regex_effbot             | 2.43 ms                                                | 2.45 ms: 1.01x slower                                                 |
| async_tree_io_tg         | 724 ms                                                 | 733 ms: 1.01x slower                                                  |
| unpickle                 | 8.29 us                                                | 8.45 us: 1.02x slower                                                 |
| pickle                   | 6.98 us                                                | 7.13 us: 1.02x slower                                                 |
| unpickle_list            | 2.69 us                                                | 2.75 us: 1.02x slower                                                 |
| dulwich_log              | 28.6 ms                                                | 29.4 ms: 1.03x slower                                                 |
| json_loads               | 15.3 us                                                | 15.8 us: 1.03x slower                                                 |
| asyncio_tcp              | 643 ms                                                 | 661 ms: 1.03x slower                                                  |
| xml_etree_iterparse      | 68.3 ms                                                | 70.3 ms: 1.03x slower                                                 |
| deltablue                | 2.75 ms                                                | 2.83 ms: 1.03x slower                                                 |
| docutils                 | 1.43 sec                                               | 1.48 sec: 1.03x slower                                                |
| json                     | 2.75 ms                                                | 2.85 ms: 1.04x slower                                                 |
| xml_etree_generate       | 45.8 ms                                                | 47.5 ms: 1.04x slower                                                 |
| async_tree_cpu_io_mixed  | 519 ms                                                 | 539 ms: 1.04x slower                                                  |
| pycparser                | 659 ms                                                 | 686 ms: 1.04x slower                                                  |
| bench_mp_pool            | 41.0 ms                                                | 42.6 ms: 1.04x slower                                                 |
| bench_thread_pool        | 465 us                                                 | 485 us: 1.04x slower                                                  |
| asyncio_tcp_ssl          | 1.40 sec                                               | 1.46 sec: 1.04x slower                                                |
| async_tree_none          | 282 ms                                                 | 295 ms: 1.05x slower                                                  |
| html5lib                 | 33.0 ms                                                | 34.7 ms: 1.05x slower                                                 |
| sympy_integrate          | 11.3 ms                                                | 11.9 ms: 1.05x slower                                                 |
| pprint_pformat           | 979 ms                                                 | 1.03 sec: 1.06x slower                                                |
| pprint_safe_repr         | 478 ms                                                 | 507 ms: 1.06x slower                                                  |
| sympy_sum                | 80.2 ms                                                | 85.0 ms: 1.06x slower                                                 |
| raytrace                 | 206 ms                                                 | 218 ms: 1.06x slower                                                  |
| sympy_str                | 144 ms                                                 | 153 ms: 1.06x slower                                                  |
| python_startup           | 10.8 ms                                                | 11.4 ms: 1.06x slower                                                 |
| meteor_contest           | 71.1 ms                                                | 75.9 ms: 1.07x slower                                                 |
| regex_compile            | 72.8 ms                                                | 78.1 ms: 1.07x slower                                                 |
| nqueens                  | 55.9 ms                                                | 60.0 ms: 1.07x slower                                                 |
| 2to3                     | 154 ms                                                 | 166 ms: 1.07x slower                                                  |
| genshi_xml               | 28.5 ms                                                | 30.7 ms: 1.07x slower                                                 |
| sympy_expand             | 229 ms                                                 | 246 ms: 1.08x slower                                                  |
| scimark_fft              | 173 ms                                                 | 186 ms: 1.08x slower                                                  |
| unpickle_pure_python     | 149 us                                                 | 160 us: 1.08x slower                                                  |
| async_generators         | 192 ms                                                 | 208 ms: 1.08x slower                                                  |
| crypto_pyaes             | 47.5 ms                                                | 51.5 ms: 1.08x slower                                                 |
| thrift                   | 410 us                                                 | 445 us: 1.08x slower                                                  |
| chaos                    | 47.4 ms                                                | 51.4 ms: 1.08x slower                                                 |
| xml_etree_process        | 33.6 ms                                                | 36.4 ms: 1.08x slower                                                 |
| hexiom                   | 4.58 ms                                                | 4.97 ms: 1.09x slower                                                 |
| django_template          | 20.1 ms                                                | 21.9 ms: 1.09x slower                                                 |
| async_tree_io            | 697 ms                                                 | 758 ms: 1.09x slower                                                  |
| chameleon                | 4.30 ms                                                | 4.68 ms: 1.09x slower                                                 |
| typing_runtime_protocols | 301 us                                                 | 329 us: 1.09x slower                                                  |
| genshi_text              | 14.4 ms                                                | 15.9 ms: 1.10x slower                                                 |
| python_startup_no_site   | 8.57 ms                                                | 9.48 ms: 1.11x slower                                                 |
| nbody                    | 61.7 ms                                                | 68.4 ms: 1.11x slower                                                 |
| sqlglot_normalize        | 162 ms                                                 | 180 ms: 1.11x slower                                                  |
| pickle_pure_python       | 191 us                                                 | 213 us: 1.11x slower                                                  |
| fannkuch                 | 240 ms                                                 | 267 ms: 1.11x slower                                                  |
| deepcopy                 | 215 us                                                 | 240 us: 1.11x slower                                                  |
| richards_super           | 37.3 ms                                                | 41.5 ms: 1.11x slower                                                 |
| deepcopy_memo            | 25.7 us                                                | 28.7 us: 1.11x slower                                                 |
| sqlglot_optimize         | 29.6 ms                                                | 33.1 ms: 1.12x slower                                                 |
| richards                 | 31.1 ms                                                | 34.7 ms: 1.12x slower                                                 |
| go                       | 105 ms                                                 | 118 ms: 1.12x slower                                                  |
| logging_format           | 3.67 us                                                | 4.10 us: 1.12x slower                                                 |
| logging_simple           | 3.41 us                                                | 3.81 us: 1.12x slower                                                 |
| float                    | 50.8 ms                                                | 57.6 ms: 1.13x slower                                                 |
| sqlglot_transpile        | 1.05 ms                                                | 1.19 ms: 1.14x slower                                                 |
| sqlite_synth             | 1.26 us                                                | 1.43 us: 1.14x slower                                                 |
| sqlglot_parse            | 890 us                                                 | 1.02 ms: 1.15x slower                                                 |
| deepcopy_reduce          | 1.79 us                                                | 2.09 us: 1.16x slower                                                 |
| tomli_loads              | 1.27 sec                                               | 1.51 sec: 1.18x slower                                                |
| logging_silent           | 66.5 ns                                                | 79.3 ns: 1.19x slower                                                 |
| coroutines               | 17.2 ms                                                | 20.5 ms: 1.19x slower                                                 |
| mdp                      | 1.48 sec                                               | 1.77 sec: 1.19x slower                                                |
| comprehensions           | 14.4 us                                                | 17.3 us: 1.20x slower                                                 |
| pyflate                  | 284 ms                                                 | 340 ms: 1.20x slower                                                  |
| scimark_lu               | 67.7 ms                                                | 81.7 ms: 1.21x slower                                                 |
| spectral_norm            | 65.7 ms                                                | 79.6 ms: 1.21x slower                                                 |
| generators               | 30.3 ms                                                | 37.2 ms: 1.23x slower                                                 |
| scimark_monte_carlo      | 43.5 ms                                                | 53.6 ms: 1.23x slower                                                 |
| scimark_sor              | 79.2 ms                                                | 105 ms: 1.32x slower                                                  |
| dask                     | 219 ms                                                 | 331 ms: 1.51x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.07x slower                                                          |

Benchmark hidden because not significant (6): async_tree_memoization, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, pathlib, async_tree_cpu_io_mixed_tg
Ignored benchmarks (9) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, coverage, flaskblogging, gunicorn, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, tornado_http


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.05x
- 95% likely to have a slowdown of 1.05x
- 99% likely to have a slowdown of 1.04x


# Memory

- memory change: 0.99x