# Results vs. base

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: f58f8ce
- commit date: 2024-02-29
- overall geometric mean: 1.00x faster
- HPT reliability: 73.34%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240228-linux-x86_64-python-0a61e237009bf6b833e1-3.13.0a4+-0a61e23 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|----------------|:----------------------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 263 ms                                                                 | 264 ms: 1.00x slower                                   |
| chameleon      | 6.99 ms                                                                | 6.91 ms: 1.01x faster                                  |
| docutils       | 2.60 sec                                                               | 2.59 sec: 1.00x faster                                 |
| Geometric mean | (ref)                                                                  | 1.00x faster                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20240228-linux-x86_64-python-0a61e237009bf6b833e1-3.13.0a4+-0a61e23 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|--------------------|:----------------------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_none_tg | 447 ms                                                                 | 445 ms: 1.00x faster                                   |
| async_tree_io      | 1.17 sec                                                               | 1.17 sec: 1.00x slower                                 |
| async_tree_io_tg   | 1.19 sec                                                               | 1.19 sec: 1.01x slower                                 |
| Geometric mean     | (ref)                                                                  | 1.00x slower                                           |

Benchmark hidden because not significant (5): async_tree_none, async_tree_memoization, async_tree_memoization_tg, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240228-linux-x86_64-python-0a61e237009bf6b833e1-3.13.0a4+-0a61e23 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|----------------|:----------------------------------------------------------------------:|:------------------------------------------------------:|
| float          | 81.0 ms                                                                | 80.4 ms: 1.01x faster                                  |
| pidigits       | 187 ms                                                                 | 187 ms: 1.00x faster                                   |
| Geometric mean | (ref)                                                                  | 1.00x faster                                           |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240228-linux-x86_64-python-0a61e237009bf6b833e1-3.13.0a4+-0a61e23 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|----------------|:----------------------------------------------------------------------:|:------------------------------------------------------:|
| regex_effbot   | 3.66 ms                                                                | 3.56 ms: 1.03x faster                                  |
| regex_dna      | 219 ms                                                                 | 216 ms: 1.01x faster                                   |
| regex_compile  | 133 ms                                                                 | 132 ms: 1.01x faster                                   |
| Geometric mean | (ref)                                                                  | 1.01x faster                                           |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240228-linux-x86_64-python-0a61e237009bf6b833e1-3.13.0a4+-0a61e23 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|----------------------|:----------------------------------------------------------------------:|:------------------------------------------------------:|
| pickle_list          | 5.24 us                                                                | 4.91 us: 1.07x faster                                  |
| pickle               | 11.9 us                                                                | 11.4 us: 1.04x faster                                  |
| unpickle             | 15.1 us                                                                | 14.5 us: 1.04x faster                                  |
| pickle_dict          | 34.1 us                                                                | 33.1 us: 1.03x faster                                  |
| unpickle_list        | 5.03 us                                                                | 4.95 us: 1.02x faster                                  |
| json_dumps           | 10.4 ms                                                                | 10.3 ms: 1.01x faster                                  |
| xml_etree_generate   | 85.5 ms                                                                | 85.0 ms: 1.01x faster                                  |
| unpickle_pure_python | 215 us                                                                 | 214 us: 1.00x faster                                   |
| xml_etree_iterparse  | 104 ms                                                                 | 106 ms: 1.01x slower                                   |
| Geometric mean       | (ref)                                                                  | 1.02x faster                                           |

Benchmark hidden because not significant (5): xml_etree_parse, xml_etree_process, pickle_pure_python, json_loads, tomli_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240228-linux-x86_64-python-0a61e237009bf6b833e1-3.13.0a4+-0a61e23 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|------------------------|:----------------------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 10.2 ms                                                                | 10.1 ms: 1.01x faster                                  |
| python_startup_no_site | 8.78 ms                                                                | 8.75 ms: 1.00x faster                                  |
| Geometric mean         | (ref)                                                                  | 1.00x faster                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240228-linux-x86_64-python-0a61e237009bf6b833e1-3.13.0a4+-0a61e23 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|-----------|:----------------------------------------------------------------------:|:------------------------------------------------------:|
| mako      | 11.2 ms                                                                | 11.4 ms: 1.02x slower                                  |

All benchmarks:
===============

| Benchmark                | bm-20240228-linux-x86_64-python-0a61e237009bf6b833e1-3.13.0a4+-0a61e23 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|--------------------------|:----------------------------------------------------------------------:|:------------------------------------------------------:|
| unpack_sequence          | 52.7 ns                                                                | 47.4 ns: 1.11x faster                                  |
| pickle_list              | 5.24 us                                                                | 4.91 us: 1.07x faster                                  |
| pickle                   | 11.9 us                                                                | 11.4 us: 1.04x faster                                  |
| unpickle                 | 15.1 us                                                                | 14.5 us: 1.04x faster                                  |
| pickle_dict              | 34.1 us                                                                | 33.1 us: 1.03x faster                                  |
| regex_effbot             | 3.66 ms                                                                | 3.56 ms: 1.03x faster                                  |
| gc_traversal             | 3.85 ms                                                                | 3.75 ms: 1.03x faster                                  |
| scimark_lu               | 112 ms                                                                 | 110 ms: 1.02x faster                                   |
| coverage                 | 94.8 ms                                                                | 93.0 ms: 1.02x faster                                  |
| crypto_pyaes             | 70.9 ms                                                                | 69.6 ms: 1.02x faster                                  |
| deepcopy_memo            | 37.9 us                                                                | 37.2 us: 1.02x faster                                  |
| unpickle_list            | 5.03 us                                                                | 4.95 us: 1.02x faster                                  |
| logging_format           | 6.23 us                                                                | 6.14 us: 1.02x faster                                  |
| raytrace                 | 266 ms                                                                 | 263 ms: 1.01x faster                                   |
| chameleon                | 6.99 ms                                                                | 6.91 ms: 1.01x faster                                  |
| richards_super           | 53.5 ms                                                                | 52.9 ms: 1.01x faster                                  |
| regex_dna                | 219 ms                                                                 | 216 ms: 1.01x faster                                   |
| regex_compile            | 133 ms                                                                 | 132 ms: 1.01x faster                                   |
| typing_runtime_protocols | 111 us                                                                 | 110 us: 1.01x faster                                   |
| chaos                    | 60.3 ms                                                                | 59.8 ms: 1.01x faster                                  |
| json_dumps               | 10.4 ms                                                                | 10.3 ms: 1.01x faster                                  |
| float                    | 81.0 ms                                                                | 80.4 ms: 1.01x faster                                  |
| async_generators         | 452 ms                                                                 | 448 ms: 1.01x faster                                   |
| generators               | 29.5 ms                                                                | 29.3 ms: 1.01x faster                                  |
| python_startup           | 10.2 ms                                                                | 10.1 ms: 1.01x faster                                  |
| deepcopy                 | 346 us                                                                 | 344 us: 1.01x faster                                   |
| xml_etree_generate       | 85.5 ms                                                                | 85.0 ms: 1.01x faster                                  |
| async_tree_none_tg       | 447 ms                                                                 | 445 ms: 1.00x faster                                   |
| unpickle_pure_python     | 215 us                                                                 | 214 us: 1.00x faster                                   |
| docutils                 | 2.60 sec                                                               | 2.59 sec: 1.00x faster                                 |
| python_startup_no_site   | 8.78 ms                                                                | 8.75 ms: 1.00x faster                                  |
| hexiom                   | 5.99 ms                                                                | 5.97 ms: 1.00x faster                                  |
| pidigits                 | 187 ms                                                                 | 187 ms: 1.00x faster                                   |
| 2to3                     | 263 ms                                                                 | 264 ms: 1.00x slower                                   |
| sympy_integrate          | 19.5 ms                                                                | 19.6 ms: 1.00x slower                                  |
| pprint_safe_repr         | 721 ms                                                                 | 724 ms: 1.00x slower                                   |
| create_gc_cycles         | 1.49 ms                                                                | 1.50 ms: 1.00x slower                                  |
| async_tree_io            | 1.17 sec                                                               | 1.17 sec: 1.00x slower                                 |
| async_tree_io_tg         | 1.19 sec                                                               | 1.19 sec: 1.01x slower                                 |
| sqlglot_optimize         | 53.0 ms                                                                | 53.4 ms: 1.01x slower                                  |
| sqlglot_transpile        | 1.56 ms                                                                | 1.57 ms: 1.01x slower                                  |
| sympy_str                | 265 ms                                                                 | 268 ms: 1.01x slower                                   |
| pycparser                | 1.19 sec                                                               | 1.21 sec: 1.01x slower                                 |
| sqlite_synth             | 2.85 us                                                                | 2.88 us: 1.01x slower                                  |
| sympy_expand             | 449 ms                                                                 | 454 ms: 1.01x slower                                   |
| sqlglot_normalize        | 104 ms                                                                 | 105 ms: 1.01x slower                                   |
| pyflate                  | 459 ms                                                                 | 466 ms: 1.01x slower                                   |
| xml_etree_iterparse      | 104 ms                                                                 | 106 ms: 1.01x slower                                   |
| comprehensions           | 15.8 us                                                                | 16.0 us: 1.01x slower                                  |
| scimark_fft              | 354 ms                                                                 | 360 ms: 1.02x slower                                   |
| mako                     | 11.2 ms                                                                | 11.4 ms: 1.02x slower                                  |
| meteor_contest           | 105 ms                                                                 | 107 ms: 1.02x slower                                   |
| spectral_norm            | 106 ms                                                                 | 110 ms: 1.03x slower                                   |
| mdp                      | 2.56 sec                                                               | 2.68 sec: 1.05x slower                                 |
| logging_silent           | 95.0 ns                                                                | 102 ns: 1.08x slower                                   |
| Geometric mean           | (ref)                                                                  | 1.00x faster                                           |

Benchmark hidden because not significant (37): logging_simple, xml_etree_parse, xml_etree_process, json, deltablue, pickle_pure_python, nqueens, fannkuch, bench_mp_pool, nbody, async_tree_none, telco, scimark_monte_carlo, pathlib, go, dulwich_log, asyncio_websockets, coroutines, asyncio_tcp, json_loads, regex_v8, asyncio_tcp_ssl, bench_thread_pool, async_tree_memoization, mypy2, sympy_sum, tomli_loads, deepcopy_reduce, async_tree_memoization_tg, tornado_http, pprint_pformat, richards, sqlglot_parse, scimark_sparse_mat_mult, async_tree_cpu_io_mixed_tg, scimark_sor, async_tree_cpu_io_mixed


# HPT report

- Reliability score: 73.34% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x