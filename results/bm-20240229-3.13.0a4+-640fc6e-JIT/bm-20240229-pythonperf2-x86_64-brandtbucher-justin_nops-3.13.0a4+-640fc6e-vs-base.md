# Results vs. base

- fork: brandtbucher
- ref: justin_nops
- machine: linux-x86_64
- commit hash: 640fc6e
- commit date: 2024-02-29
- overall geometric mean: 1.01x slower
- HPT reliability: 99.99%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:----------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 306 ms                                                                       | 308 ms: 1.01x slower                                                      |
| mdp            | 2.59 sec                                                                     | 2.58 sec: 1.01x faster                                                    |
| Geometric mean | (ref)                                                                        | 1.00x slower                                                              |

Benchmark hidden because not significant (4): chameleon, docutils, html5lib, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|--------------------|:----------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_none_tg | 438 ms                                                                       | 435 ms: 1.01x faster                                                      |
| async_tree_io      | 1.08 sec                                                                     | 1.10 sec: 1.01x slower                                                    |
| Geometric mean     | (ref)                                                                        | 1.00x slower                                                              |

Benchmark hidden because not significant (6): async_tree_memoization_tg, async_tree_memoization, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_cpu_io_mixed, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:----------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| nbody          | 105 ms                                                                       | 99.1 ms: 1.06x faster                                                     |
| pidigits       | 261 ms                                                                       | 262 ms: 1.00x slower                                                      |
| float          | 77.6 ms                                                                      | 79.0 ms: 1.02x slower                                                     |
| Geometric mean | (ref)                                                                        | 1.01x faster                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:----------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_v8       | 25.4 ms                                                                      | 25.0 ms: 1.02x faster                                                     |
| regex_dna      | 235 ms                                                                       | 238 ms: 1.01x slower                                                      |
| regex_effbot   | 3.46 ms                                                                      | 3.56 ms: 1.03x slower                                                     |
| Geometric mean | (ref)                                                                        | 1.01x slower                                                              |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------|:----------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| unpickle_list        | 4.72 us                                                                      | 4.63 us: 1.02x faster                                                     |
| xml_etree_generate   | 84.3 ms                                                                      | 83.5 ms: 1.01x faster                                                     |
| unpickle             | 15.2 us                                                                      | 15.2 us: 1.01x faster                                                     |
| json_dumps           | 10.6 ms                                                                      | 10.6 ms: 1.00x slower                                                     |
| json_loads           | 25.0 us                                                                      | 25.1 us: 1.01x slower                                                     |
| pickle               | 10.4 us                                                                      | 10.6 us: 1.02x slower                                                     |
| pickle_pure_python   | 311 us                                                                       | 319 us: 1.03x slower                                                      |
| unpickle_pure_python | 230 us                                                                       | 238 us: 1.03x slower                                                      |
| pickle_list          | 4.21 us                                                                      | 4.38 us: 1.04x slower                                                     |
| tomli_loads          | 2.13 sec                                                                     | 2.22 sec: 1.04x slower                                                    |
| pickle_dict          | 30.5 us                                                                      | 32.9 us: 1.08x slower                                                     |
| Geometric mean       | (ref)                                                                        | 1.01x slower                                                              |

Benchmark hidden because not significant (4): xml_etree_iterparse, xml_etree_parse, mypy2, xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|------------------------|:----------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup_no_site | 14.0 ms                                                                      | 14.0 ms: 1.00x faster                                                     |
| Geometric mean         | (ref)                                                                        | 1.00x faster                                                              |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|-----------------|:----------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| genshi_text     | 28.5 ms                                                                      | 28.8 ms: 1.01x slower                                                     |
| mako            | 9.93 ms                                                                      | 10.1 ms: 1.01x slower                                                     |
| genshi_xml      | 60.1 ms                                                                      | 61.8 ms: 1.03x slower                                                     |
| django_template | 38.2 ms                                                                      | 40.3 ms: 1.05x slower                                                     |
| Geometric mean  | (ref)                                                                        | 1.03x slower                                                              |

All benchmarks:
===============

| Benchmark                | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|--------------------------|:----------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| nbody                    | 105 ms                                                                       | 99.1 ms: 1.06x faster                                                     |
| pycparser                | 1.35 sec                                                                     | 1.30 sec: 1.04x faster                                                    |
| async_generators         | 384 ms                                                                       | 377 ms: 1.02x faster                                                      |
| unpickle_list            | 4.72 us                                                                      | 4.63 us: 1.02x faster                                                     |
| coverage                 | 81.9 ms                                                                      | 80.4 ms: 1.02x faster                                                     |
| regex_v8                 | 25.4 ms                                                                      | 25.0 ms: 1.02x faster                                                     |
| unpack_sequence          | 61.9 ns                                                                      | 61.0 ns: 1.01x faster                                                     |
| xml_etree_generate       | 84.3 ms                                                                      | 83.5 ms: 1.01x faster                                                     |
| richards_super           | 56.7 ms                                                                      | 56.2 ms: 1.01x faster                                                     |
| mdp                      | 2.59 sec                                                                     | 2.58 sec: 1.01x faster                                                    |
| go                       | 174 ms                                                                       | 173 ms: 1.01x faster                                                      |
| unpickle                 | 15.2 us                                                                      | 15.2 us: 1.01x faster                                                     |
| async_tree_none_tg       | 438 ms                                                                       | 435 ms: 1.01x faster                                                      |
| scimark_sparse_mat_mult  | 4.20 ms                                                                      | 4.18 ms: 1.00x faster                                                     |
| python_startup_no_site   | 14.0 ms                                                                      | 14.0 ms: 1.00x faster                                                     |
| sympy_integrate          | 24.5 ms                                                                      | 24.5 ms: 1.00x slower                                                     |
| asyncio_tcp_ssl          | 1.57 sec                                                                     | 1.58 sec: 1.00x slower                                                    |
| pidigits                 | 261 ms                                                                       | 262 ms: 1.00x slower                                                      |
| richards                 | 50.1 ms                                                                      | 50.2 ms: 1.00x slower                                                     |
| logging_silent           | 97.1 ns                                                                      | 97.4 ns: 1.00x slower                                                     |
| sqlite_synth             | 2.70 us                                                                      | 2.71 us: 1.00x slower                                                     |
| json_dumps               | 10.6 ms                                                                      | 10.6 ms: 1.00x slower                                                     |
| sympy_str                | 302 ms                                                                       | 303 ms: 1.00x slower                                                      |
| dulwich_log              | 69.1 ms                                                                      | 69.4 ms: 1.00x slower                                                     |
| sympy_sum                | 159 ms                                                                       | 160 ms: 1.01x slower                                                      |
| sqlglot_normalize        | 119 ms                                                                       | 119 ms: 1.01x slower                                                      |
| json_loads               | 25.0 us                                                                      | 25.1 us: 1.01x slower                                                     |
| scimark_monte_carlo      | 77.5 ms                                                                      | 77.9 ms: 1.01x slower                                                     |
| logging_format           | 7.34 us                                                                      | 7.39 us: 1.01x slower                                                     |
| logging_simple           | 6.69 us                                                                      | 6.74 us: 1.01x slower                                                     |
| 2to3                     | 306 ms                                                                       | 308 ms: 1.01x slower                                                      |
| sqlglot_parse            | 1.42 ms                                                                      | 1.43 ms: 1.01x slower                                                     |
| sqlglot_optimize         | 62.8 ms                                                                      | 63.3 ms: 1.01x slower                                                     |
| hexiom                   | 7.37 ms                                                                      | 7.43 ms: 1.01x slower                                                     |
| deepcopy_reduce          | 3.34 us                                                                      | 3.37 us: 1.01x slower                                                     |
| aiohttp                  | 1.10 ms                                                                      | 1.11 ms: 1.01x slower                                                     |
| genshi_text              | 28.5 ms                                                                      | 28.8 ms: 1.01x slower                                                     |
| asyncio_tcp              | 368 ms                                                                       | 372 ms: 1.01x slower                                                      |
| bench_mp_pool            | 6.88 ms                                                                      | 6.96 ms: 1.01x slower                                                     |
| pathlib                  | 19.4 ms                                                                      | 19.6 ms: 1.01x slower                                                     |
| coroutines               | 22.3 ms                                                                      | 22.6 ms: 1.01x slower                                                     |
| meteor_contest           | 132 ms                                                                       | 133 ms: 1.01x slower                                                      |
| regex_dna                | 235 ms                                                                       | 238 ms: 1.01x slower                                                      |
| async_tree_io            | 1.08 sec                                                                     | 1.10 sec: 1.01x slower                                                    |
| mako                     | 9.93 ms                                                                      | 10.1 ms: 1.01x slower                                                     |
| nqueens                  | 101 ms                                                                       | 103 ms: 1.01x slower                                                      |
| scimark_sor              | 151 ms                                                                       | 153 ms: 1.01x slower                                                      |
| telco                    | 8.12 ms                                                                      | 8.24 ms: 1.01x slower                                                     |
| float                    | 77.6 ms                                                                      | 79.0 ms: 1.02x slower                                                     |
| pyflate                  | 518 ms                                                                       | 528 ms: 1.02x slower                                                      |
| comprehensions           | 18.8 us                                                                      | 19.2 us: 1.02x slower                                                     |
| raytrace                 | 303 ms                                                                       | 310 ms: 1.02x slower                                                      |
| fannkuch                 | 394 ms                                                                       | 402 ms: 1.02x slower                                                      |
| scimark_lu               | 115 ms                                                                       | 118 ms: 1.02x slower                                                      |
| pickle                   | 10.4 us                                                                      | 10.6 us: 1.02x slower                                                     |
| spectral_norm            | 92.4 ms                                                                      | 94.7 ms: 1.02x slower                                                     |
| pickle_pure_python       | 311 us                                                                       | 319 us: 1.03x slower                                                      |
| genshi_xml               | 60.1 ms                                                                      | 61.8 ms: 1.03x slower                                                     |
| regex_effbot             | 3.46 ms                                                                      | 3.56 ms: 1.03x slower                                                     |
| unpickle_pure_python     | 230 us                                                                       | 238 us: 1.03x slower                                                      |
| thrift                   | 861 us                                                                       | 891 us: 1.04x slower                                                      |
| typing_runtime_protocols | 119 us                                                                       | 123 us: 1.04x slower                                                      |
| scimark_fft              | 316 ms                                                                       | 327 ms: 1.04x slower                                                      |
| pickle_list              | 4.21 us                                                                      | 4.38 us: 1.04x slower                                                     |
| tomli_loads              | 2.13 sec                                                                     | 2.22 sec: 1.04x slower                                                    |
| django_template          | 38.2 ms                                                                      | 40.3 ms: 1.05x slower                                                     |
| pickle_dict              | 30.5 us                                                                      | 32.9 us: 1.08x slower                                                     |
| Geometric mean           | (ref)                                                                        | 1.01x slower                                                              |

Benchmark hidden because not significant (34): async_tree_memoization_tg, bench_thread_pool, json, xml_etree_iterparse, async_tree_memoization, xml_etree_parse, regex_compile, create_gc_cycles, crypto_pyaes, mypy2, sqlglot_transpile, docutils, deltablue, sympy_expand, async_tree_cpu_io_mixed_tg, python_startup, async_tree_io_tg, chaos, generators, dask, chameleon, pprint_pformat, gunicorn, xml_etree_process, pprint_safe_repr, gc_traversal, deepcopy, async_tree_cpu_io_mixed, deepcopy_memo, pylint, html5lib, tornado_http, asyncio_websockets, async_tree_none


# HPT report

- Reliability score: 99.99% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x