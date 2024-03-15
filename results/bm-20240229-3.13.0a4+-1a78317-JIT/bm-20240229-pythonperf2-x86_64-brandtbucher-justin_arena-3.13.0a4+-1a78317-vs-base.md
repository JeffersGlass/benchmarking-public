# Results vs. base

- fork: brandtbucher
- ref: justin_arena
- machine: linux-x86_64
- commit hash: 1a78317
- commit date: 2024-02-29
- overall geometric mean: 1.00x faster
- HPT reliability: 65.59%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 306 ms                                                                       | 307 ms: 1.00x slower                                                       |
| chameleon      | 7.45 ms                                                                      | 7.60 ms: 1.02x slower                                                      |
| docutils       | 2.91 sec                                                                     | 2.91 sec: 1.00x faster                                                     |
| mdp            | 2.59 sec                                                                     | 2.58 sec: 1.01x faster                                                     |
| Geometric mean | (ref)                                                                        | 1.00x slower                                                               |

Benchmark hidden because not significant (2): html5lib, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_io_tg           | 1.09 sec                                                                     | 1.09 sec: 1.01x slower                                                     |
| async_tree_io              | 1.08 sec                                                                     | 1.09 sec: 1.01x slower                                                     |
| async_tree_cpu_io_mixed_tg | 709 ms                                                                       | 718 ms: 1.01x slower                                                       |
| async_tree_none            | 438 ms                                                                       | 445 ms: 1.02x slower                                                       |
| async_tree_none_tg         | 438 ms                                                                       | 447 ms: 1.02x slower                                                       |
| async_tree_memoization_tg  | 559 ms                                                                       | 572 ms: 1.02x slower                                                       |
| Geometric mean             | (ref)                                                                        | 1.01x slower                                                               |

Benchmark hidden because not significant (2): async_tree_memoization, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| nbody          | 105 ms                                                                       | 98.5 ms: 1.07x faster                                                      |
| float          | 77.6 ms                                                                      | 78.1 ms: 1.01x slower                                                      |
| Geometric mean | (ref)                                                                        | 1.02x faster                                                               |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                                       | 146 ms: 1.01x faster                                                       |
| regex_v8       | 25.4 ms                                                                      | 25.2 ms: 1.01x faster                                                      |
| regex_dna      | 235 ms                                                                       | 238 ms: 1.01x slower                                                       |
| regex_effbot   | 3.46 ms                                                                      | 3.56 ms: 1.03x slower                                                      |
| Geometric mean | (ref)                                                                        | 1.01x slower                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|---------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| unpickle_list       | 4.72 us                                                                      | 4.64 us: 1.02x faster                                                      |
| xml_etree_generate  | 84.3 ms                                                                      | 83.2 ms: 1.01x faster                                                      |
| pickle_pure_python  | 311 us                                                                       | 308 us: 1.01x faster                                                       |
| xml_etree_parse     | 144 ms                                                                       | 143 ms: 1.01x faster                                                       |
| unpickle            | 15.2 us                                                                      | 15.1 us: 1.01x faster                                                      |
| xml_etree_iterparse | 102 ms                                                                       | 102 ms: 1.01x faster                                                       |
| json_loads          | 25.0 us                                                                      | 24.8 us: 1.01x faster                                                      |
| pickle              | 10.4 us                                                                      | 10.3 us: 1.01x faster                                                      |
| pickle_dict         | 30.5 us                                                                      | 31.0 us: 1.02x slower                                                      |
| tomli_loads         | 2.13 sec                                                                     | 2.17 sec: 1.02x slower                                                     |
| json_dumps          | 10.6 ms                                                                      | 10.8 ms: 1.02x slower                                                      |
| pickle_list         | 4.21 us                                                                      | 4.30 us: 1.02x slower                                                      |
| Geometric mean      | (ref)                                                                        | 1.00x faster                                                               |

Benchmark hidden because not significant (3): mypy2, unpickle_pure_python, xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup_no_site | 14.0 ms                                                                      | 13.9 ms: 1.01x faster                                                      |
| python_startup         | 15.5 ms                                                                      | 15.4 ms: 1.01x faster                                                      |
| Geometric mean         | (ref)                                                                        | 1.01x faster                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|-----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako            | 9.93 ms                                                                      | 9.85 ms: 1.01x faster                                                      |
| genshi_xml      | 60.1 ms                                                                      | 60.7 ms: 1.01x slower                                                      |
| django_template | 38.2 ms                                                                      | 38.9 ms: 1.02x slower                                                      |
| genshi_text     | 28.5 ms                                                                      | 29.6 ms: 1.04x slower                                                      |
| Geometric mean  | (ref)                                                                        | 1.02x slower                                                               |

All benchmarks:
===============

| Benchmark                  | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| nbody                      | 105 ms                                                                       | 98.5 ms: 1.07x faster                                                      |
| gc_traversal               | 3.67 ms                                                                      | 3.47 ms: 1.06x faster                                                      |
| pycparser                  | 1.35 sec                                                                     | 1.28 sec: 1.05x faster                                                     |
| logging_simple             | 6.69 us                                                                      | 6.42 us: 1.04x faster                                                      |
| logging_format             | 7.34 us                                                                      | 7.12 us: 1.03x faster                                                      |
| generators                 | 34.0 ms                                                                      | 33.0 ms: 1.03x faster                                                      |
| chaos                      | 68.3 ms                                                                      | 66.8 ms: 1.02x faster                                                      |
| unpack_sequence            | 61.9 ns                                                                      | 60.5 ns: 1.02x faster                                                      |
| fannkuch                   | 394 ms                                                                       | 386 ms: 1.02x faster                                                       |
| unpickle_list              | 4.72 us                                                                      | 4.64 us: 1.02x faster                                                      |
| sqlglot_transpile          | 1.86 ms                                                                      | 1.83 ms: 1.02x faster                                                      |
| sqlglot_parse              | 1.42 ms                                                                      | 1.40 ms: 1.02x faster                                                      |
| telco                      | 8.12 ms                                                                      | 7.99 ms: 1.02x faster                                                      |
| xml_etree_generate         | 84.3 ms                                                                      | 83.2 ms: 1.01x faster                                                      |
| crypto_pyaes               | 77.6 ms                                                                      | 76.7 ms: 1.01x faster                                                      |
| regex_compile              | 148 ms                                                                       | 146 ms: 1.01x faster                                                       |
| pprint_pformat             | 1.74 sec                                                                     | 1.72 sec: 1.01x faster                                                     |
| scimark_monte_carlo        | 77.5 ms                                                                      | 76.6 ms: 1.01x faster                                                      |
| dulwich_log                | 69.1 ms                                                                      | 68.3 ms: 1.01x faster                                                      |
| pprint_safe_repr           | 844 ms                                                                       | 835 ms: 1.01x faster                                                       |
| richards                   | 50.1 ms                                                                      | 49.6 ms: 1.01x faster                                                      |
| scimark_sparse_mat_mult    | 4.20 ms                                                                      | 4.16 ms: 1.01x faster                                                      |
| go                         | 174 ms                                                                       | 172 ms: 1.01x faster                                                       |
| hexiom                     | 7.37 ms                                                                      | 7.30 ms: 1.01x faster                                                      |
| pickle_pure_python         | 311 us                                                                       | 308 us: 1.01x faster                                                       |
| python_startup_no_site     | 14.0 ms                                                                      | 13.9 ms: 1.01x faster                                                      |
| python_startup             | 15.5 ms                                                                      | 15.4 ms: 1.01x faster                                                      |
| pathlib                    | 19.4 ms                                                                      | 19.3 ms: 1.01x faster                                                      |
| comprehensions             | 18.8 us                                                                      | 18.7 us: 1.01x faster                                                      |
| mako                       | 9.93 ms                                                                      | 9.85 ms: 1.01x faster                                                      |
| typing_runtime_protocols   | 119 us                                                                       | 118 us: 1.01x faster                                                       |
| xml_etree_parse            | 144 ms                                                                       | 143 ms: 1.01x faster                                                       |
| unpickle                   | 15.2 us                                                                      | 15.1 us: 1.01x faster                                                      |
| xml_etree_iterparse        | 102 ms                                                                       | 102 ms: 1.01x faster                                                       |
| mdp                        | 2.59 sec                                                                     | 2.58 sec: 1.01x faster                                                     |
| coverage                   | 81.9 ms                                                                      | 81.4 ms: 1.01x faster                                                      |
| deepcopy_memo              | 37.6 us                                                                      | 37.4 us: 1.01x faster                                                      |
| json_loads                 | 25.0 us                                                                      | 24.8 us: 1.01x faster                                                      |
| pickle                     | 10.4 us                                                                      | 10.3 us: 1.01x faster                                                      |
| regex_v8                   | 25.4 ms                                                                      | 25.2 ms: 1.01x faster                                                      |
| sqlite_synth               | 2.70 us                                                                      | 2.69 us: 1.00x faster                                                      |
| docutils                   | 2.91 sec                                                                     | 2.91 sec: 1.00x faster                                                     |
| asyncio_tcp_ssl            | 1.57 sec                                                                     | 1.58 sec: 1.00x slower                                                     |
| 2to3                       | 306 ms                                                                       | 307 ms: 1.00x slower                                                       |
| sqlglot_optimize           | 62.8 ms                                                                      | 63.0 ms: 1.00x slower                                                      |
| scimark_sor                | 151 ms                                                                       | 151 ms: 1.00x slower                                                       |
| float                      | 77.6 ms                                                                      | 78.1 ms: 1.01x slower                                                      |
| scimark_fft                | 316 ms                                                                       | 318 ms: 1.01x slower                                                       |
| asyncio_tcp                | 368 ms                                                                       | 371 ms: 1.01x slower                                                       |
| gunicorn                   | 1.07 ms                                                                      | 1.08 ms: 1.01x slower                                                      |
| sqlglot_normalize          | 119 ms                                                                       | 120 ms: 1.01x slower                                                       |
| async_tree_io_tg           | 1.09 sec                                                                     | 1.09 sec: 1.01x slower                                                     |
| thrift                     | 861 us                                                                       | 868 us: 1.01x slower                                                       |
| deltablue                  | 3.78 ms                                                                      | 3.81 ms: 1.01x slower                                                      |
| async_tree_io              | 1.08 sec                                                                     | 1.09 sec: 1.01x slower                                                     |
| async_generators           | 384 ms                                                                       | 389 ms: 1.01x slower                                                       |
| genshi_xml                 | 60.1 ms                                                                      | 60.7 ms: 1.01x slower                                                      |
| async_tree_cpu_io_mixed_tg | 709 ms                                                                       | 718 ms: 1.01x slower                                                       |
| regex_dna                  | 235 ms                                                                       | 238 ms: 1.01x slower                                                       |
| async_tree_none            | 438 ms                                                                       | 445 ms: 1.02x slower                                                       |
| pickle_dict                | 30.5 us                                                                      | 31.0 us: 1.02x slower                                                      |
| scimark_lu                 | 115 ms                                                                       | 117 ms: 1.02x slower                                                       |
| django_template            | 38.2 ms                                                                      | 38.9 ms: 1.02x slower                                                      |
| tomli_loads                | 2.13 sec                                                                     | 2.17 sec: 1.02x slower                                                     |
| json_dumps                 | 10.6 ms                                                                      | 10.8 ms: 1.02x slower                                                      |
| chameleon                  | 7.45 ms                                                                      | 7.60 ms: 1.02x slower                                                      |
| async_tree_none_tg         | 438 ms                                                                       | 447 ms: 1.02x slower                                                       |
| pickle_list                | 4.21 us                                                                      | 4.30 us: 1.02x slower                                                      |
| async_tree_memoization_tg  | 559 ms                                                                       | 572 ms: 1.02x slower                                                       |
| regex_effbot               | 3.46 ms                                                                      | 3.56 ms: 1.03x slower                                                      |
| bench_mp_pool              | 6.88 ms                                                                      | 7.08 ms: 1.03x slower                                                      |
| genshi_text                | 28.5 ms                                                                      | 29.6 ms: 1.04x slower                                                      |
| pyflate                    | 518 ms                                                                       | 538 ms: 1.04x slower                                                       |
| Geometric mean             | (ref)                                                                        | 1.00x faster                                                               |

Benchmark hidden because not significant (28): mypy2, asyncio_websockets, json, bench_thread_pool, deepcopy, html5lib, dask, sympy_expand, sympy_str, deepcopy_reduce, nqueens, pylint, unpickle_pure_python, logging_silent, richards_super, sympy_integrate, pidigits, meteor_contest, spectral_norm, create_gc_cycles, xml_etree_process, tornado_http, sympy_sum, coroutines, raytrace, aiohttp, async_tree_memoization, async_tree_cpu_io_mixed


# HPT report

- Reliability score: 65.59% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x