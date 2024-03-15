# Results vs. base

- fork: brandtbucher
- ref: justin_nops
- machine: linux-x86_64
- commit hash: 640fc6e
- commit date: 2024-02-29
- overall geometric mean: 1.00x slower \*
- HPT reliability: 99.82%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------:|
| 2to3           | 276 ms                                                                 | 277 ms: 1.00x slower                                                |
| chameleon      | 6.81 ms                                                                | 6.76 ms: 1.01x faster                                               |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                        |

Benchmark hidden because not significant (2): docutils, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|--------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------:|
| async_tree_io_tg   | 1.20 sec                                                               | 1.20 sec: 1.01x faster                                              |
| async_tree_io      | 1.18 sec                                                               | 1.18 sec: 1.00x faster                                              |
| async_tree_none_tg | 446 ms                                                                 | 447 ms: 1.00x slower                                                |
| Geometric mean     | (ref)                                                                  | 1.00x slower                                                        |

Benchmark hidden because not significant (5): async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed, async_tree_memoization_tg, async_tree_memoization, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------:|
| pidigits       | 187 ms                                                                 | 187 ms: 1.00x slower                                                |
| float          | 78.3 ms                                                                | 80.0 ms: 1.02x slower                                               |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                        |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------:|
| regex_v8       | 25.3 ms                                                                | 24.7 ms: 1.02x faster                                               |
| regex_effbot   | 3.69 ms                                                                | 3.73 ms: 1.01x slower                                               |
| regex_dna      | 222 ms                                                                 | 229 ms: 1.03x slower                                                |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                        |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------:|
| unpickle             | 15.0 us                                                                | 14.5 us: 1.03x faster                                               |
| unpickle_list        | 4.91 us                                                                | 4.79 us: 1.02x faster                                               |
| pickle               | 11.6 us                                                                | 11.3 us: 1.02x faster                                               |
| json_dumps           | 10.4 ms                                                                | 10.2 ms: 1.01x faster                                               |
| xml_etree_generate   | 86.5 ms                                                                | 86.0 ms: 1.01x faster                                               |
| unpickle_pure_python | 236 us                                                                 | 238 us: 1.01x slower                                                |
| pickle_dict          | 33.8 us                                                                | 34.2 us: 1.01x slower                                               |
| json_loads           | 27.4 us                                                                | 27.7 us: 1.01x slower                                               |
| pickle_list          | 4.89 us                                                                | 4.98 us: 1.02x slower                                               |
| tomli_loads          | 2.01 sec                                                               | 2.07 sec: 1.03x slower                                              |
| pickle_pure_python   | 297 us                                                                 | 307 us: 1.03x slower                                                |
| Geometric mean       | (ref)                                                                  | 1.00x faster                                                        |

Benchmark hidden because not significant (3): xml_etree_parse, xml_etree_iterparse, xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|------------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------:|
| python_startup_no_site | 11.0 ms                                                                | 11.0 ms: 1.00x slower                                               |
| python_startup         | 12.3 ms                                                                | 12.3 ms: 1.00x slower                                               |
| Geometric mean         | (ref)                                                                  | 1.00x slower                                                        |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|-----------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------:|
| mako      | 11.0 ms                                                                | 11.2 ms: 1.01x slower                                               |

All benchmarks:
===============

| Benchmark                | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|--------------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------:|
| mdp                      | 2.77 sec                                                               | 2.59 sec: 1.07x faster                                              |
| unpickle                 | 15.0 us                                                                | 14.5 us: 1.03x faster                                               |
| gc_traversal             | 4.04 ms                                                                | 3.92 ms: 1.03x faster                                               |
| unpickle_list            | 4.91 us                                                                | 4.79 us: 1.02x faster                                               |
| regex_v8                 | 25.3 ms                                                                | 24.7 ms: 1.02x faster                                               |
| typing_runtime_protocols | 112 us                                                                 | 110 us: 1.02x faster                                                |
| pickle                   | 11.6 us                                                                | 11.3 us: 1.02x faster                                               |
| async_generators         | 468 ms                                                                 | 459 ms: 1.02x faster                                                |
| richards_super           | 53.1 ms                                                                | 52.3 ms: 1.02x faster                                               |
| json_dumps               | 10.4 ms                                                                | 10.2 ms: 1.01x faster                                               |
| chameleon                | 6.81 ms                                                                | 6.76 ms: 1.01x faster                                               |
| xml_etree_generate       | 86.5 ms                                                                | 86.0 ms: 1.01x faster                                               |
| pathlib                  | 18.4 ms                                                                | 18.3 ms: 1.01x faster                                               |
| generators               | 29.5 ms                                                                | 29.3 ms: 1.01x faster                                               |
| async_tree_io_tg         | 1.20 sec                                                               | 1.20 sec: 1.01x faster                                              |
| async_tree_io            | 1.18 sec                                                               | 1.18 sec: 1.00x faster                                              |
| comprehensions           | 17.2 us                                                                | 17.1 us: 1.00x faster                                               |
| go                       | 155 ms                                                                 | 155 ms: 1.00x faster                                                |
| asyncio_tcp_ssl          | 1.80 sec                                                               | 1.80 sec: 1.00x faster                                              |
| python_startup_no_site   | 11.0 ms                                                                | 11.0 ms: 1.00x slower                                               |
| python_startup           | 12.3 ms                                                                | 12.3 ms: 1.00x slower                                               |
| pidigits                 | 187 ms                                                                 | 187 ms: 1.00x slower                                                |
| 2to3                     | 276 ms                                                                 | 277 ms: 1.00x slower                                                |
| dulwich_log              | 68.4 ms                                                                | 68.6 ms: 1.00x slower                                               |
| async_tree_none_tg       | 446 ms                                                                 | 447 ms: 1.00x slower                                                |
| hexiom                   | 7.05 ms                                                                | 7.08 ms: 1.00x slower                                               |
| sqlglot_parse            | 1.28 ms                                                                | 1.29 ms: 1.00x slower                                               |
| nqueens                  | 89.6 ms                                                                | 90.2 ms: 1.01x slower                                               |
| dask                     | 530 ms                                                                 | 534 ms: 1.01x slower                                                |
| meteor_contest           | 108 ms                                                                 | 109 ms: 1.01x slower                                                |
| deepcopy                 | 346 us                                                                 | 349 us: 1.01x slower                                                |
| crypto_pyaes             | 72.6 ms                                                                | 73.2 ms: 1.01x slower                                               |
| logging_format           | 6.23 us                                                                | 6.28 us: 1.01x slower                                               |
| unpickle_pure_python     | 236 us                                                                 | 238 us: 1.01x slower                                                |
| pickle_dict              | 33.8 us                                                                | 34.2 us: 1.01x slower                                               |
| fannkuch                 | 394 ms                                                                 | 398 ms: 1.01x slower                                                |
| json_loads               | 27.4 us                                                                | 27.7 us: 1.01x slower                                               |
| regex_effbot             | 3.69 ms                                                                | 3.73 ms: 1.01x slower                                               |
| create_gc_cycles         | 1.50 ms                                                                | 1.52 ms: 1.01x slower                                               |
| mako                     | 11.0 ms                                                                | 11.2 ms: 1.01x slower                                               |
| logging_silent           | 99.5 ns                                                                | 101 ns: 1.01x slower                                                |
| scimark_sparse_mat_mult  | 4.68 ms                                                                | 4.75 ms: 1.02x slower                                               |
| pickle_list              | 4.89 us                                                                | 4.98 us: 1.02x slower                                               |
| raytrace                 | 287 ms                                                                 | 292 ms: 1.02x slower                                                |
| float                    | 78.3 ms                                                                | 80.0 ms: 1.02x slower                                               |
| logging_simple           | 5.62 us                                                                | 5.75 us: 1.02x slower                                               |
| scimark_fft              | 335 ms                                                                 | 342 ms: 1.02x slower                                                |
| tomli_loads              | 2.01 sec                                                               | 2.07 sec: 1.03x slower                                              |
| coroutines               | 22.3 ms                                                                | 23.0 ms: 1.03x slower                                               |
| regex_dna                | 222 ms                                                                 | 229 ms: 1.03x slower                                                |
| scimark_lu               | 128 ms                                                                 | 132 ms: 1.03x slower                                                |
| pycparser                | 1.17 sec                                                               | 1.21 sec: 1.03x slower                                              |
| pickle_pure_python       | 297 us                                                                 | 307 us: 1.03x slower                                                |
| pprint_safe_repr         | 746 ms                                                                 | 772 ms: 1.03x slower                                                |
| json                     | 5.12 ms                                                                | 5.30 ms: 1.04x slower                                               |
| scimark_monte_carlo      | 69.5 ms                                                                | 72.6 ms: 1.04x slower                                               |
| unpack_sequence          | 86.3 ns                                                                | 94.6 ns: 1.10x slower                                               |
| Geometric mean           | (ref)                                                                  | 1.00x slower                                                        |

Benchmark hidden because not significant (36): xml_etree_parse, richards, xml_etree_iterparse, nbody, xml_etree_process, deltablue, sympy_expand, regex_compile, docutils, bench_mp_pool, sympy_integrate, asyncio_websockets, chaos, bench_thread_pool, deepcopy_reduce, tornado_http, async_tree_cpu_io_mixed_tg, asyncio_tcp, sqlglot_normalize, pyflate, sqlglot_optimize, sympy_sum, mypy2, sympy_str, coverage, sqlite_synth, deepcopy_memo, sqlglot_transpile, spectral_norm, async_tree_cpu_io_mixed, pprint_pformat, telco, async_tree_memoization_tg, async_tree_memoization, scimark_sor, async_tree_none
Ignored benchmarks (9) of results/bm-20240229-3.13.0a4+-640fc6e-JIT/bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e.json: aiohttp, django_template, djangocms, genshi_text, genshi_xml, gunicorn, html5lib, pylint, thrift


# HPT report

- Reliability score: 99.82% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x