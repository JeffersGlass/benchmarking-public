
# Results vs. 3.11.0

- fork: python
- ref: 3c67ec394faac79d2608
- machine: darwin-arm64
- commit hash: 3c67ec3
- commit date: 2023-02-07
- overall geometric mean: 1.06x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x slower
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 166 ms: 1.08x slower                                                  |
| chameleon      | 4.30 ms                                                | 4.69 ms: 1.09x slower                                                 |
| docutils       | 1.43 sec                                               | 1.48 sec: 1.04x slower                                                |
| html5lib       | 33.0 ms                                                | 34.6 ms: 1.05x slower                                                 |
| tornado_http   | 69.1 ms                                                | 72.3 ms: 1.05x slower                                                 |
| Geometric mean | (ref)                                                  | 1.06x slower                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 555 ms: 1.01x slower                                                  |
| async_tree_none_tg         | 276 ms                                                 | 281 ms: 1.02x slower                                                  |
| async_tree_io_tg           | 724 ms                                                 | 739 ms: 1.02x slower                                                  |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 533 ms: 1.03x slower                                                  |
| async_tree_none            | 282 ms                                                 | 290 ms: 1.03x slower                                                  |
| async_tree_io              | 697 ms                                                 | 753 ms: 1.08x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.02x slower                                                          |

Benchmark hidden because not significant (2): async_tree_memoization_tg, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 281 ms: 1.00x slower                                                  |
| nbody          | 61.7 ms                                                | 68.5 ms: 1.11x slower                                                 |
| float          | 50.8 ms                                                | 57.5 ms: 1.13x slower                                                 |
| Geometric mean | (ref)                                                  | 1.08x slower                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_dna      | 148 ms                                                 | 147 ms: 1.01x faster                                                  |
| regex_effbot   | 2.43 ms                                                | 2.45 ms: 1.01x slower                                                 |
| regex_v8       | 15.1 ms                                                | 15.3 ms: 1.01x slower                                                 |
| regex_compile  | 72.8 ms                                                | 76.0 ms: 1.04x slower                                                 |
| Geometric mean | (ref)                                                  | 1.01x slower                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.08 ms: 1.24x faster                                                 |
| xml_etree_parse      | 100 ms                                                 | 95.0 ms: 1.06x faster                                                 |
| pickle_dict          | 17.1 us                                                | 16.8 us: 1.01x faster                                                 |
| pickle_list          | 2.70 us                                                | 2.72 us: 1.01x slower                                                 |
| pickle               | 6.98 us                                                | 7.09 us: 1.02x slower                                                 |
| json_loads           | 15.3 us                                                | 15.7 us: 1.02x slower                                                 |
| unpickle             | 8.29 us                                                | 8.50 us: 1.02x slower                                                 |
| xml_etree_iterparse  | 68.3 ms                                                | 71.9 ms: 1.05x slower                                                 |
| xml_etree_generate   | 45.8 ms                                                | 48.7 ms: 1.06x slower                                                 |
| unpickle_list        | 2.69 us                                                | 2.85 us: 1.06x slower                                                 |
| tomli_loads          | 1.27 sec                                               | 1.38 sec: 1.08x slower                                                |
| unpickle_pure_python | 149 us                                                 | 161 us: 1.08x slower                                                  |
| xml_etree_process    | 33.6 ms                                                | 37.1 ms: 1.10x slower                                                 |
| pickle_pure_python   | 191 us                                                 | 214 us: 1.12x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.02x slower                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 11.8 ms: 1.10x slower                                                 |
| python_startup_no_site | 8.57 ms                                                | 9.55 ms: 1.11x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.11x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 7.93 ms                                                | 6.94 ms: 1.14x faster                                                 |
| genshi_xml      | 28.5 ms                                                | 30.7 ms: 1.08x slower                                                 |
| django_template | 20.1 ms                                                | 22.5 ms: 1.12x slower                                                 |
| genshi_text     | 14.4 ms                                                | 16.3 ms: 1.13x slower                                                 |
| Geometric mean  | (ref)                                                  | 1.04x slower                                                          |

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| asyncio_tcp                | 643 ms                                                 | 437 ms: 1.47x faster                                                  |
| json_dumps                 | 7.53 ms                                                | 6.08 ms: 1.24x faster                                                 |
| mako                       | 7.93 ms                                                | 6.94 ms: 1.14x faster                                                 |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.28 sec: 1.09x faster                                                |
| xml_etree_parse            | 100 ms                                                 | 95.0 ms: 1.06x faster                                                 |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 2.70 ms: 1.04x faster                                                 |
| create_gc_cycles           | 711 us                                                 | 687 us: 1.03x faster                                                  |
| pickle_dict                | 17.1 us                                                | 16.8 us: 1.01x faster                                                 |
| regex_dna                  | 148 ms                                                 | 147 ms: 1.01x faster                                                  |
| gc_traversal               | 2.38 ms                                                | 2.39 ms: 1.00x slower                                                 |
| pidigits                   | 280 ms                                                 | 281 ms: 1.00x slower                                                  |
| telco                      | 3.17 ms                                                | 3.18 ms: 1.00x slower                                                 |
| regex_effbot               | 2.43 ms                                                | 2.45 ms: 1.01x slower                                                 |
| hexiom                     | 4.58 ms                                                | 4.61 ms: 1.01x slower                                                 |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 555 ms: 1.01x slower                                                  |
| pickle_list                | 2.70 us                                                | 2.72 us: 1.01x slower                                                 |
| regex_v8                   | 15.1 ms                                                | 15.3 ms: 1.01x slower                                                 |
| json                       | 2.75 ms                                                | 2.79 ms: 1.01x slower                                                 |
| pycparser                  | 659 ms                                                 | 670 ms: 1.02x slower                                                  |
| async_tree_none_tg         | 276 ms                                                 | 281 ms: 1.02x slower                                                  |
| pickle                     | 6.98 us                                                | 7.09 us: 1.02x slower                                                 |
| deltablue                  | 2.75 ms                                                | 2.81 ms: 1.02x slower                                                 |
| async_tree_io_tg           | 724 ms                                                 | 739 ms: 1.02x slower                                                  |
| dulwich_log                | 28.6 ms                                                | 29.2 ms: 1.02x slower                                                 |
| chaos                      | 47.4 ms                                                | 48.4 ms: 1.02x slower                                                 |
| json_loads                 | 15.3 us                                                | 15.7 us: 1.02x slower                                                 |
| sympy_integrate            | 11.3 ms                                                | 11.5 ms: 1.02x slower                                                 |
| unpickle                   | 8.29 us                                                | 8.50 us: 1.02x slower                                                 |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 533 ms: 1.03x slower                                                  |
| sympy_sum                  | 80.2 ms                                                | 82.4 ms: 1.03x slower                                                 |
| fannkuch                   | 240 ms                                                 | 246 ms: 1.03x slower                                                  |
| sympy_str                  | 144 ms                                                 | 148 ms: 1.03x slower                                                  |
| async_tree_none            | 282 ms                                                 | 290 ms: 1.03x slower                                                  |
| docutils                   | 1.43 sec                                               | 1.48 sec: 1.04x slower                                                |
| regex_compile              | 72.8 ms                                                | 76.0 ms: 1.04x slower                                                 |
| tornado_http               | 69.1 ms                                                | 72.3 ms: 1.05x slower                                                 |
| sqlalchemy_imperative      | 6.98 ms                                                | 7.32 ms: 1.05x slower                                                 |
| html5lib                   | 33.0 ms                                                | 34.6 ms: 1.05x slower                                                 |
| xml_etree_iterparse        | 68.3 ms                                                | 71.9 ms: 1.05x slower                                                 |
| sqlalchemy_declarative     | 59.3 ms                                                | 62.6 ms: 1.06x slower                                                 |
| typing_runtime_protocols   | 301 us                                                 | 319 us: 1.06x slower                                                  |
| xml_etree_generate         | 45.8 ms                                                | 48.7 ms: 1.06x slower                                                 |
| scimark_fft                | 173 ms                                                 | 183 ms: 1.06x slower                                                  |
| unpickle_list              | 2.69 us                                                | 2.85 us: 1.06x slower                                                 |
| bench_thread_pool          | 465 us                                                 | 495 us: 1.06x slower                                                  |
| bench_mp_pool              | 41.0 ms                                                | 43.7 ms: 1.07x slower                                                 |
| sympy_expand               | 229 ms                                                 | 245 ms: 1.07x slower                                                  |
| nqueens                    | 55.9 ms                                                | 59.9 ms: 1.07x slower                                                 |
| go                         | 105 ms                                                 | 113 ms: 1.08x slower                                                  |
| genshi_xml                 | 28.5 ms                                                | 30.7 ms: 1.08x slower                                                 |
| 2to3                       | 154 ms                                                 | 166 ms: 1.08x slower                                                  |
| richards                   | 31.1 ms                                                | 33.5 ms: 1.08x slower                                                 |
| thrift                     | 410 us                                                 | 443 us: 1.08x slower                                                  |
| async_tree_io              | 697 ms                                                 | 753 ms: 1.08x slower                                                  |
| tomli_loads                | 1.27 sec                                               | 1.38 sec: 1.08x slower                                                |
| unpickle_pure_python       | 149 us                                                 | 161 us: 1.08x slower                                                  |
| richards_super             | 37.3 ms                                                | 40.4 ms: 1.08x slower                                                 |
| crypto_pyaes               | 47.5 ms                                                | 51.6 ms: 1.09x slower                                                 |
| meteor_contest             | 71.1 ms                                                | 77.2 ms: 1.09x slower                                                 |
| async_generators           | 192 ms                                                 | 209 ms: 1.09x slower                                                  |
| chameleon                  | 4.30 ms                                                | 4.69 ms: 1.09x slower                                                 |
| pprint_pformat             | 979 ms                                                 | 1.07 sec: 1.10x slower                                                |
| python_startup             | 10.8 ms                                                | 11.8 ms: 1.10x slower                                                 |
| pprint_safe_repr           | 478 ms                                                 | 524 ms: 1.10x slower                                                  |
| xml_etree_process          | 33.6 ms                                                | 37.1 ms: 1.10x slower                                                 |
| nbody                      | 61.7 ms                                                | 68.5 ms: 1.11x slower                                                 |
| deepcopy_memo              | 25.7 us                                                | 28.6 us: 1.11x slower                                                 |
| raytrace                   | 206 ms                                                 | 229 ms: 1.11x slower                                                  |
| sqlite_synth               | 1.26 us                                                | 1.40 us: 1.11x slower                                                 |
| python_startup_no_site     | 8.57 ms                                                | 9.55 ms: 1.11x slower                                                 |
| sqlglot_optimize           | 29.6 ms                                                | 33.1 ms: 1.12x slower                                                 |
| pickle_pure_python         | 191 us                                                 | 214 us: 1.12x slower                                                  |
| django_template            | 20.1 ms                                                | 22.5 ms: 1.12x slower                                                 |
| sqlglot_normalize          | 162 ms                                                 | 181 ms: 1.12x slower                                                  |
| float                      | 50.8 ms                                                | 57.5 ms: 1.13x slower                                                 |
| genshi_text                | 14.4 ms                                                | 16.3 ms: 1.13x slower                                                 |
| deepcopy                   | 215 us                                                 | 246 us: 1.14x slower                                                  |
| pyflate                    | 284 ms                                                 | 324 ms: 1.14x slower                                                  |
| logging_simple             | 3.41 us                                                | 3.89 us: 1.14x slower                                                 |
| logging_format             | 3.67 us                                                | 4.21 us: 1.14x slower                                                 |
| scimark_sor                | 79.2 ms                                                | 90.7 ms: 1.15x slower                                                 |
| sqlglot_transpile          | 1.05 ms                                                | 1.23 ms: 1.17x slower                                                 |
| mdp                        | 1.48 sec                                               | 1.76 sec: 1.18x slower                                                |
| sqlglot_parse              | 890 us                                                 | 1.05 ms: 1.18x slower                                                 |
| deepcopy_reduce            | 1.79 us                                                | 2.15 us: 1.20x slower                                                 |
| coroutines                 | 17.2 ms                                                | 20.6 ms: 1.20x slower                                                 |
| scimark_monte_carlo        | 43.5 ms                                                | 52.9 ms: 1.22x slower                                                 |
| scimark_lu                 | 67.7 ms                                                | 83.3 ms: 1.23x slower                                                 |
| spectral_norm              | 65.7 ms                                                | 81.8 ms: 1.24x slower                                                 |
| logging_silent             | 66.5 ns                                                | 83.0 ns: 1.25x slower                                                 |
| generators                 | 30.3 ms                                                | 38.6 ms: 1.27x slower                                                 |
| dask                       | 219 ms                                                 | 327 ms: 1.49x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.06x slower                                                          |

Benchmark hidden because not significant (6): unpack_sequence, async_tree_memoization_tg, pathlib, async_tree_memoization, asyncio_websockets, comprehensions
Ignored benchmarks (6) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, coverage, flaskblogging, gunicorn, mypy2, pylint


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.04x
- 95% likely to have a slowdown of 1.04x
- 99% likely to have a slowdown of 1.03x


# Memory

- memory change: 0.98x