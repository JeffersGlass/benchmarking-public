# Results vs. base

- fork: brandtbucher
- ref: justin_arena
- machine: linux-x86_64
- commit hash: 1a78317
- commit date: 2024-02-29
- overall geometric mean: 1.00x faster \*
- HPT reliability: 85.18%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-linux-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| chameleon      | 6.81 ms                                                                | 6.86 ms: 1.01x slower                                                |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                         |

Benchmark hidden because not significant (3): 2to3, docutils, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark        | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-linux-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_io_tg | 1.20 sec                                                               | 1.20 sec: 1.00x faster                                               |
| Geometric mean   | (ref)                                                                  | 1.00x slower                                                         |

Benchmark hidden because not significant (7): async_tree_io, async_tree_memoization, async_tree_none_tg, async_tree_cpu_io_mixed_tg, async_tree_none, async_tree_cpu_io_mixed, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-linux-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| nbody          | 94.5 ms                                                                | 92.0 ms: 1.03x faster                                                |
| float          | 78.3 ms                                                                | 77.9 ms: 1.01x faster                                                |
| pidigits       | 187 ms                                                                 | 187 ms: 1.00x faster                                                 |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-linux-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_v8       | 25.3 ms                                                                | 24.2 ms: 1.04x faster                                                |
| regex_compile  | 142 ms                                                                 | 142 ms: 1.00x faster                                                 |
| regex_dna      | 222 ms                                                                 | 224 ms: 1.01x slower                                                 |
| regex_effbot   | 3.69 ms                                                                | 3.74 ms: 1.02x slower                                                |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark          | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-linux-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|--------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| pickle             | 11.6 us                                                                | 11.3 us: 1.02x faster                                                |
| xml_etree_generate | 86.5 ms                                                                | 84.9 ms: 1.02x faster                                                |
| xml_etree_process  | 58.7 ms                                                                | 58.2 ms: 1.01x faster                                                |
| json_dumps         | 10.4 ms                                                                | 10.4 ms: 1.01x slower                                                |
| pickle_dict        | 33.8 us                                                                | 34.7 us: 1.03x slower                                                |
| unpickle           | 15.0 us                                                                | 15.4 us: 1.03x slower                                                |
| Geometric mean     | (ref)                                                                  | 1.00x slower                                                         |

Benchmark hidden because not significant (8): xml_etree_parse, xml_etree_iterparse, tomli_loads, unpickle_list, pickle_pure_python, json_loads, pickle_list, unpickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-linux-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup_no_site | 11.0 ms                                                                | 10.7 ms: 1.02x faster                                                |
| python_startup         | 12.3 ms                                                                | 12.1 ms: 1.02x faster                                                |
| Geometric mean         | (ref)                                                                  | 1.02x faster                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-linux-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 11.0 ms                                                                | 10.9 ms: 1.01x faster                                                |

All benchmarks:
===============

| Benchmark                | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-linux-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|--------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| gc_traversal             | 4.04 ms                                                                | 3.51 ms: 1.15x faster                                                |
| mdp                      | 2.77 sec                                                               | 2.65 sec: 1.05x faster                                               |
| regex_v8                 | 25.3 ms                                                                | 24.2 ms: 1.04x faster                                                |
| pyflate                  | 489 ms                                                                 | 471 ms: 1.04x faster                                                 |
| nbody                    | 94.5 ms                                                                | 92.0 ms: 1.03x faster                                                |
| pickle                   | 11.6 us                                                                | 11.3 us: 1.02x faster                                                |
| typing_runtime_protocols | 112 us                                                                 | 110 us: 1.02x faster                                                 |
| python_startup_no_site   | 11.0 ms                                                                | 10.7 ms: 1.02x faster                                                |
| xml_etree_generate       | 86.5 ms                                                                | 84.9 ms: 1.02x faster                                                |
| richards_super           | 53.1 ms                                                                | 52.2 ms: 1.02x faster                                                |
| python_startup           | 12.3 ms                                                                | 12.1 ms: 1.02x faster                                                |
| logging_silent           | 99.5 ns                                                                | 97.9 ns: 1.02x faster                                                |
| meteor_contest           | 108 ms                                                                 | 107 ms: 1.02x faster                                                 |
| async_generators         | 468 ms                                                                 | 462 ms: 1.01x faster                                                 |
| mako                     | 11.0 ms                                                                | 10.9 ms: 1.01x faster                                                |
| spectral_norm            | 113 ms                                                                 | 112 ms: 1.01x faster                                                 |
| hexiom                   | 7.05 ms                                                                | 6.98 ms: 1.01x faster                                                |
| pycparser                | 1.17 sec                                                               | 1.16 sec: 1.01x faster                                               |
| xml_etree_process        | 58.7 ms                                                                | 58.2 ms: 1.01x faster                                                |
| deepcopy_reduce          | 3.04 us                                                                | 3.02 us: 1.01x faster                                                |
| deltablue                | 3.41 ms                                                                | 3.39 ms: 1.01x faster                                                |
| comprehensions           | 17.2 us                                                                | 17.1 us: 1.01x faster                                                |
| nqueens                  | 89.6 ms                                                                | 89.0 ms: 1.01x faster                                                |
| float                    | 78.3 ms                                                                | 77.9 ms: 1.01x faster                                                |
| generators               | 29.5 ms                                                                | 29.3 ms: 1.01x faster                                                |
| sympy_sum                | 157 ms                                                                 | 156 ms: 1.00x faster                                                 |
| scimark_fft              | 335 ms                                                                 | 333 ms: 1.00x faster                                                 |
| regex_compile            | 142 ms                                                                 | 142 ms: 1.00x faster                                                 |
| sqlglot_normalize        | 107 ms                                                                 | 106 ms: 1.00x faster                                                 |
| pidigits                 | 187 ms                                                                 | 187 ms: 1.00x faster                                                 |
| async_tree_io_tg         | 1.20 sec                                                               | 1.20 sec: 1.00x faster                                               |
| create_gc_cycles         | 1.50 ms                                                                | 1.50 ms: 1.00x faster                                                |
| asyncio_tcp_ssl          | 1.80 sec                                                               | 1.80 sec: 1.00x slower                                               |
| dulwich_log              | 68.4 ms                                                                | 68.6 ms: 1.00x slower                                                |
| raytrace                 | 287 ms                                                                 | 288 ms: 1.00x slower                                                 |
| json_dumps               | 10.4 ms                                                                | 10.4 ms: 1.01x slower                                                |
| logging_simple           | 5.62 us                                                                | 5.65 us: 1.01x slower                                                |
| regex_dna                | 222 ms                                                                 | 224 ms: 1.01x slower                                                 |
| chameleon                | 6.81 ms                                                                | 6.86 ms: 1.01x slower                                                |
| asyncio_tcp              | 486 ms                                                                 | 489 ms: 1.01x slower                                                 |
| scimark_sor              | 127 ms                                                                 | 129 ms: 1.01x slower                                                 |
| crypto_pyaes             | 72.6 ms                                                                | 73.7 ms: 1.01x slower                                                |
| regex_effbot             | 3.69 ms                                                                | 3.74 ms: 1.02x slower                                                |
| coroutines               | 22.3 ms                                                                | 22.8 ms: 1.02x slower                                                |
| scimark_monte_carlo      | 69.5 ms                                                                | 71.0 ms: 1.02x slower                                                |
| pickle_dict              | 33.8 us                                                                | 34.7 us: 1.03x slower                                                |
| unpickle                 | 15.0 us                                                                | 15.4 us: 1.03x slower                                                |
| unpack_sequence          | 86.3 ns                                                                | 92.1 ns: 1.07x slower                                                |
| Geometric mean           | (ref)                                                                  | 1.00x faster                                                         |

Benchmark hidden because not significant (45): chaos, json, xml_etree_parse, richards, xml_etree_iterparse, async_tree_io, tomli_loads, unpickle_list, docutils, fannkuch, pathlib, go, dask, async_tree_memoization, bench_thread_pool, asyncio_websockets, pickle_pure_python, tornado_http, sqlglot_optimize, sympy_integrate, 2to3, pprint_safe_repr, deepcopy_memo, scimark_sparse_mat_mult, async_tree_none_tg, json_loads, mypy2, async_tree_cpu_io_mixed_tg, pickle_list, sqlglot_parse, sympy_expand, unpickle_pure_python, sympy_str, telco, logging_format, bench_mp_pool, sqlite_synth, deepcopy, async_tree_none, async_tree_cpu_io_mixed, coverage, sqlglot_transpile, scimark_lu, async_tree_memoization_tg, pprint_pformat
Ignored benchmarks (9) of results/bm-20240229-3.13.0a4+-1a78317-JIT/bm-20240229-linux-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317.json: aiohttp, django_template, djangocms, genshi_text, genshi_xml, gunicorn, html5lib, pylint, thrift


# HPT report

- Reliability score: 85.18% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x