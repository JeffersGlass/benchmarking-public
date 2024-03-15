# Results vs. base

- fork: faster-cpython
- ref: inline_values
- machine: linux-x86_64
- commit hash: 0dc68a4
- commit date: 2024-02-24
- overall geometric mean: 1.01x slower
- HPT reliability: 99.85%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 261 ms                                                                 | 262 ms: 1.00x slower                                                      |
| chameleon      | 6.82 ms                                                                | 6.72 ms: 1.01x faster                                                     |
| docutils       | 2.56 sec                                                               | 2.60 sec: 1.02x slower                                                    |
| tornado_http   | 94.7 ms                                                                | 94.1 ms: 1.01x faster                                                     |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|---------------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_io             | 1.16 sec                                                               | 1.16 sec: 1.00x faster                                                    |
| async_tree_io_tg          | 1.19 sec                                                               | 1.19 sec: 1.00x slower                                                    |
| async_tree_memoization_tg | 566 ms                                                                 | 574 ms: 1.01x slower                                                      |
| async_tree_memoization    | 555 ms                                                                 | 575 ms: 1.04x slower                                                      |
| async_tree_cpu_io_mixed   | 699 ms                                                                 | 725 ms: 1.04x slower                                                      |
| async_tree_none           | 431 ms                                                                 | 477 ms: 1.11x slower                                                      |
| Geometric mean            | (ref)                                                                  | 1.02x slower                                                              |

Benchmark hidden because not significant (2): async_tree_none_tg, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| float          | 79.0 ms                                                                | 79.5 ms: 1.01x slower                                                     |
| nbody          | 86.5 ms                                                                | 90.6 ms: 1.05x slower                                                     |
| pidigits       | 187 ms                                                                 | 203 ms: 1.09x slower                                                      |
| Geometric mean | (ref)                                                                  | 1.05x slower                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_effbot   | 3.73 ms                                                                | 3.55 ms: 1.05x faster                                                     |
| regex_dna      | 219 ms                                                                 | 215 ms: 1.02x faster                                                      |
| regex_v8       | 24.8 ms                                                                | 25.0 ms: 1.01x slower                                                     |
| Geometric mean | (ref)                                                                  | 1.02x faster                                                              |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|---------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| unpickle_list       | 4.92 us                                                                | 4.74 us: 1.04x faster                                                     |
| pickle_pure_python  | 292 us                                                                 | 294 us: 1.01x slower                                                      |
| pickle_dict         | 35.1 us                                                                | 35.3 us: 1.01x slower                                                     |
| xml_etree_generate  | 84.7 ms                                                                | 85.3 ms: 1.01x slower                                                     |
| xml_etree_process   | 57.8 ms                                                                | 58.2 ms: 1.01x slower                                                     |
| xml_etree_iterparse | 104 ms                                                                 | 105 ms: 1.01x slower                                                      |
| pickle              | 11.7 us                                                                | 11.9 us: 1.01x slower                                                     |
| json_loads          | 27.1 us                                                                | 27.6 us: 1.02x slower                                                     |
| xml_etree_parse     | 156 ms                                                                 | 159 ms: 1.02x slower                                                      |
| Geometric mean      | (ref)                                                                  | 1.00x slower                                                              |

Benchmark hidden because not significant (5): unpickle, json_dumps, pickle_list, unpickle_pure_python, tomli_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|------------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup_no_site | 8.81 ms                                                                | 8.82 ms: 1.00x slower                                                     |
| python_startup         | 10.2 ms                                                                | 10.2 ms: 1.00x slower                                                     |
| Geometric mean         | (ref)                                                                  | 1.00x slower                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|-----------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| mako      | 11.0 ms                                                                | 11.2 ms: 1.02x slower                                                     |

All benchmarks:
===============

| Benchmark                 | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|---------------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| gc_traversal              | 4.00 ms                                                                | 3.73 ms: 1.07x faster                                                     |
| mdp                       | 2.68 sec                                                               | 2.50 sec: 1.07x faster                                                    |
| regex_effbot              | 3.73 ms                                                                | 3.55 ms: 1.05x faster                                                     |
| unpickle_list             | 4.92 us                                                                | 4.74 us: 1.04x faster                                                     |
| coroutines                | 22.3 ms                                                                | 21.5 ms: 1.04x faster                                                     |
| generators                | 29.4 ms                                                                | 28.6 ms: 1.03x faster                                                     |
| richards_super            | 53.8 ms                                                                | 52.6 ms: 1.02x faster                                                     |
| logging_format            | 6.24 us                                                                | 6.12 us: 1.02x faster                                                     |
| regex_dna                 | 219 ms                                                                 | 215 ms: 1.02x faster                                                      |
| spectral_norm             | 109 ms                                                                 | 107 ms: 1.02x faster                                                      |
| raytrace                  | 260 ms                                                                 | 256 ms: 1.02x faster                                                      |
| asyncio_websockets        | 560 ms                                                                 | 551 ms: 1.02x faster                                                      |
| sqlglot_parse             | 1.24 ms                                                                | 1.23 ms: 1.02x faster                                                     |
| chameleon                 | 6.82 ms                                                                | 6.72 ms: 1.01x faster                                                     |
| scimark_monte_carlo       | 67.5 ms                                                                | 66.7 ms: 1.01x faster                                                     |
| deepcopy                  | 347 us                                                                 | 343 us: 1.01x faster                                                      |
| chaos                     | 59.8 ms                                                                | 59.2 ms: 1.01x faster                                                     |
| scimark_lu                | 113 ms                                                                 | 112 ms: 1.01x faster                                                      |
| sqlglot_transpile         | 1.56 ms                                                                | 1.55 ms: 1.01x faster                                                     |
| tornado_http              | 94.7 ms                                                                | 94.1 ms: 1.01x faster                                                     |
| comprehensions            | 16.1 us                                                                | 16.0 us: 1.01x faster                                                     |
| richards                  | 47.5 ms                                                                | 47.3 ms: 1.01x faster                                                     |
| meteor_contest            | 105 ms                                                                 | 104 ms: 1.01x faster                                                      |
| asyncio_tcp_ssl           | 1.79 sec                                                               | 1.78 sec: 1.00x faster                                                    |
| async_tree_io             | 1.16 sec                                                               | 1.16 sec: 1.00x faster                                                    |
| python_startup_no_site    | 8.81 ms                                                                | 8.82 ms: 1.00x slower                                                     |
| pprint_pformat            | 1.47 sec                                                               | 1.48 sec: 1.00x slower                                                    |
| async_tree_io_tg          | 1.19 sec                                                               | 1.19 sec: 1.00x slower                                                    |
| python_startup            | 10.2 ms                                                                | 10.2 ms: 1.00x slower                                                     |
| 2to3                      | 261 ms                                                                 | 262 ms: 1.00x slower                                                      |
| deltablue                 | 3.15 ms                                                                | 3.17 ms: 1.01x slower                                                     |
| async_generators          | 445 ms                                                                 | 448 ms: 1.01x slower                                                      |
| pickle_pure_python        | 292 us                                                                 | 294 us: 1.01x slower                                                      |
| float                     | 79.0 ms                                                                | 79.5 ms: 1.01x slower                                                     |
| pickle_dict               | 35.1 us                                                                | 35.3 us: 1.01x slower                                                     |
| xml_etree_generate        | 84.7 ms                                                                | 85.3 ms: 1.01x slower                                                     |
| bench_thread_pool         | 814 us                                                                 | 820 us: 1.01x slower                                                      |
| xml_etree_process         | 57.8 ms                                                                | 58.2 ms: 1.01x slower                                                     |
| xml_etree_iterparse       | 104 ms                                                                 | 105 ms: 1.01x slower                                                      |
| regex_v8                  | 24.8 ms                                                                | 25.0 ms: 1.01x slower                                                     |
| telco                     | 8.34 ms                                                                | 8.42 ms: 1.01x slower                                                     |
| pprint_safe_repr          | 715 ms                                                                 | 723 ms: 1.01x slower                                                      |
| pickle                    | 11.7 us                                                                | 11.9 us: 1.01x slower                                                     |
| asyncio_tcp               | 483 ms                                                                 | 489 ms: 1.01x slower                                                      |
| sympy_sum                 | 147 ms                                                                 | 148 ms: 1.01x slower                                                      |
| sqlglot_normalize         | 104 ms                                                                 | 106 ms: 1.01x slower                                                      |
| sympy_integrate           | 19.4 ms                                                                | 19.7 ms: 1.01x slower                                                     |
| go                        | 135 ms                                                                 | 137 ms: 1.01x slower                                                      |
| async_tree_memoization_tg | 566 ms                                                                 | 574 ms: 1.01x slower                                                      |
| docutils                  | 2.56 sec                                                               | 2.60 sec: 1.02x slower                                                    |
| deepcopy_memo             | 37.5 us                                                                | 38.1 us: 1.02x slower                                                     |
| json_loads                | 27.1 us                                                                | 27.6 us: 1.02x slower                                                     |
| mako                      | 11.0 ms                                                                | 11.2 ms: 1.02x slower                                                     |
| pyflate                   | 442 ms                                                                 | 449 ms: 1.02x slower                                                      |
| sqlite_synth              | 2.83 us                                                                | 2.88 us: 1.02x slower                                                     |
| crypto_pyaes              | 69.9 ms                                                                | 71.2 ms: 1.02x slower                                                     |
| coverage                  | 95.2 ms                                                                | 97.1 ms: 1.02x slower                                                     |
| fannkuch                  | 376 ms                                                                 | 384 ms: 1.02x slower                                                      |
| scimark_fft               | 353 ms                                                                 | 361 ms: 1.02x slower                                                      |
| xml_etree_parse           | 156 ms                                                                 | 159 ms: 1.02x slower                                                      |
| dulwich_log               | 65.0 ms                                                                | 66.5 ms: 1.02x slower                                                     |
| json                      | 4.96 ms                                                                | 5.08 ms: 1.02x slower                                                     |
| scimark_sparse_mat_mult   | 4.60 ms                                                                | 4.71 ms: 1.02x slower                                                     |
| pathlib                   | 17.9 ms                                                                | 18.3 ms: 1.02x slower                                                     |
| pycparser                 | 1.15 sec                                                               | 1.18 sec: 1.03x slower                                                    |
| async_tree_memoization    | 555 ms                                                                 | 575 ms: 1.04x slower                                                      |
| async_tree_cpu_io_mixed   | 699 ms                                                                 | 725 ms: 1.04x slower                                                      |
| nqueens                   | 77.5 ms                                                                | 80.5 ms: 1.04x slower                                                     |
| nbody                     | 86.5 ms                                                                | 90.6 ms: 1.05x slower                                                     |
| logging_silent            | 95.1 ns                                                                | 99.7 ns: 1.05x slower                                                     |
| hexiom                    | 5.86 ms                                                                | 6.16 ms: 1.05x slower                                                     |
| create_gc_cycles          | 1.48 ms                                                                | 1.56 ms: 1.05x slower                                                     |
| pidigits                  | 187 ms                                                                 | 203 ms: 1.09x slower                                                      |
| async_tree_none           | 431 ms                                                                 | 477 ms: 1.11x slower                                                      |
| unpack_sequence           | 42.5 ns                                                                | 50.5 ns: 1.19x slower                                                     |
| Geometric mean            | (ref)                                                                  | 1.01x slower                                                              |

Benchmark hidden because not significant (17): unpickle, typing_runtime_protocols, scimark_sor, json_dumps, async_tree_none_tg, logging_simple, regex_compile, sqlglot_optimize, bench_mp_pool, pickle_list, sympy_expand, unpickle_pure_python, tomli_loads, sympy_str, deepcopy_reduce, mypy2, async_tree_cpu_io_mixed_tg


# HPT report

- Reliability score: 99.85% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.01x