# Results vs. base

- fork: faster-cpython
- ref: abstract_interpreter
- machine: linux-x86_64
- commit hash: a932d36
- commit date: 2024-02-02
- overall geometric mean: 1.00x faster \*
- HPT reliability: 55.86%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240202-linux-x86_64-python-0e71a295e9530c939a5e-3.13.0a3+-0e71a29 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 281 ms                                                                 | 284 ms: 1.01x slower                                                             |
| docutils       | 2.70 sec                                                               | 2.72 sec: 1.01x slower                                                           |
| tornado_http   | 98.4 ms                                                                | 99.2 ms: 1.01x slower                                                            |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (1): chameleon

Benchmarks with tag 'asyncio':
==============================

| Benchmark              | bm-20240202-linux-x86_64-python-0e71a295e9530c939a5e-3.13.0a3+-0e71a29 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_memoization | 576 ms                                                                 | 570 ms: 1.01x faster                                                             |
| async_tree_io_tg       | 1.21 sec                                                               | 1.20 sec: 1.01x faster                                                           |
| async_tree_io          | 1.20 sec                                                               | 1.19 sec: 1.01x faster                                                           |
| Geometric mean         | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (5): async_tree_none, async_tree_none_tg, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240202-linux-x86_64-python-0e71a295e9530c939a5e-3.13.0a3+-0e71a29 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 122 ms                                                                 | 117 ms: 1.04x faster                                                             |
| pidigits       | 188 ms                                                                 | 189 ms: 1.00x slower                                                             |
| float          | 92.6 ms                                                                | 93.1 ms: 1.01x slower                                                            |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240202-linux-x86_64-python-0e71a295e9530c939a5e-3.13.0a3+-0e71a29 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_v8       | 25.2 ms                                                                | 24.8 ms: 1.02x faster                                                            |
| regex_dna      | 224 ms                                                                 | 226 ms: 1.01x slower                                                             |
| regex_effbot   | 3.65 ms                                                                | 3.74 ms: 1.02x slower                                                            |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark          | bm-20240202-linux-x86_64-python-0e71a295e9530c939a5e-3.13.0a3+-0e71a29 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|--------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| unpickle_list      | 5.03 us                                                                | 4.96 us: 1.01x faster                                                            |
| tomli_loads        | 2.62 sec                                                               | 2.59 sec: 1.01x faster                                                           |
| pickle             | 11.9 us                                                                | 11.8 us: 1.01x faster                                                            |
| pickle_pure_python | 301 us                                                                 | 300 us: 1.00x faster                                                             |
| xml_etree_generate | 89.4 ms                                                                | 89.1 ms: 1.00x faster                                                            |
| pickle_list        | 5.34 us                                                                | 5.37 us: 1.00x slower                                                            |
| json_loads         | 28.4 us                                                                | 28.6 us: 1.01x slower                                                            |
| json_dumps         | 10.5 ms                                                                | 10.6 ms: 1.01x slower                                                            |
| pickle_dict        | 35.5 us                                                                | 36.6 us: 1.03x slower                                                            |
| unpickle           | 16.0 us                                                                | 17.0 us: 1.06x slower                                                            |
| Geometric mean     | (ref)                                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (4): xml_etree_iterparse, xml_etree_parse, unpickle_pure_python, xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240202-linux-x86_64-python-0e71a295e9530c939a5e-3.13.0a3+-0e71a29 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                | 10.2 ms: 1.01x slower                                                            |
| python_startup_no_site | 8.76 ms                                                                | 8.84 ms: 1.01x slower                                                            |
| Geometric mean         | (ref)                                                                  | 1.01x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240202-linux-x86_64-python-0e71a295e9530c939a5e-3.13.0a3+-0e71a29 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 14.8 ms                                                                | 14.0 ms: 1.06x faster                                                            |

All benchmarks:
===============

| Benchmark               | bm-20240202-linux-x86_64-python-0e71a295e9530c939a5e-3.13.0a3+-0e71a29 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|-------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| unpack_sequence         | 53.7 ns                                                                | 39.4 ns: 1.36x faster                                                            |
| gc_traversal            | 3.98 ms                                                                | 3.49 ms: 1.14x faster                                                            |
| mako                    | 14.8 ms                                                                | 14.0 ms: 1.06x faster                                                            |
| nbody                   | 122 ms                                                                 | 117 ms: 1.04x faster                                                             |
| scimark_fft             | 449 ms                                                                 | 436 ms: 1.03x faster                                                             |
| chaos                   | 73.8 ms                                                                | 72.4 ms: 1.02x faster                                                            |
| regex_v8                | 25.2 ms                                                                | 24.8 ms: 1.02x faster                                                            |
| sympy_str               | 295 ms                                                                 | 291 ms: 1.02x faster                                                             |
| fannkuch                | 452 ms                                                                 | 445 ms: 1.02x faster                                                             |
| async_generators        | 457 ms                                                                 | 450 ms: 1.01x faster                                                             |
| unpickle_list           | 5.03 us                                                                | 4.96 us: 1.01x faster                                                            |
| deepcopy_reduce         | 3.18 us                                                                | 3.14 us: 1.01x faster                                                            |
| json                    | 5.33 ms                                                                | 5.27 ms: 1.01x faster                                                            |
| hexiom                  | 8.48 ms                                                                | 8.38 ms: 1.01x faster                                                            |
| tomli_loads             | 2.62 sec                                                               | 2.59 sec: 1.01x faster                                                           |
| sympy_expand            | 493 ms                                                                 | 488 ms: 1.01x faster                                                             |
| scimark_lu              | 117 ms                                                                 | 116 ms: 1.01x faster                                                             |
| logging_simple          | 5.94 us                                                                | 5.88 us: 1.01x faster                                                            |
| async_tree_memoization  | 576 ms                                                                 | 570 ms: 1.01x faster                                                             |
| async_tree_io_tg        | 1.21 sec                                                               | 1.20 sec: 1.01x faster                                                           |
| logging_format          | 6.75 us                                                                | 6.68 us: 1.01x faster                                                            |
| sqlite_synth            | 2.86 us                                                                | 2.84 us: 1.01x faster                                                            |
| sympy_integrate         | 21.2 ms                                                                | 21.1 ms: 1.01x faster                                                            |
| sqlglot_optimize        | 57.8 ms                                                                | 57.4 ms: 1.01x faster                                                            |
| async_tree_io           | 1.20 sec                                                               | 1.19 sec: 1.01x faster                                                           |
| pickle                  | 11.9 us                                                                | 11.8 us: 1.01x faster                                                            |
| pickle_pure_python      | 301 us                                                                 | 300 us: 1.00x faster                                                             |
| asyncio_tcp_ssl         | 1.80 sec                                                               | 1.79 sec: 1.00x faster                                                           |
| crypto_pyaes            | 84.2 ms                                                                | 83.9 ms: 1.00x faster                                                            |
| create_gc_cycles        | 1.48 ms                                                                | 1.48 ms: 1.00x faster                                                            |
| sqlglot_normalize       | 113 ms                                                                 | 113 ms: 1.00x faster                                                             |
| xml_etree_generate      | 89.4 ms                                                                | 89.1 ms: 1.00x faster                                                            |
| dulwich_log             | 69.2 ms                                                                | 69.0 ms: 1.00x faster                                                            |
| nqueens                 | 94.7 ms                                                                | 94.5 ms: 1.00x faster                                                            |
| pyflate                 | 518 ms                                                                 | 519 ms: 1.00x slower                                                             |
| asyncio_tcp             | 490 ms                                                                 | 492 ms: 1.00x slower                                                             |
| sqlglot_parse           | 1.33 ms                                                                | 1.34 ms: 1.00x slower                                                            |
| pidigits                | 188 ms                                                                 | 189 ms: 1.00x slower                                                             |
| pickle_list             | 5.34 us                                                                | 5.37 us: 1.00x slower                                                            |
| sqlglot_transpile       | 1.66 ms                                                                | 1.67 ms: 1.01x slower                                                            |
| pprint_safe_repr        | 800 ms                                                                 | 804 ms: 1.01x slower                                                             |
| float                   | 92.6 ms                                                                | 93.1 ms: 1.01x slower                                                            |
| docutils                | 2.70 sec                                                               | 2.72 sec: 1.01x slower                                                           |
| bench_thread_pool       | 842 us                                                                 | 848 us: 1.01x slower                                                             |
| json_loads              | 28.4 us                                                                | 28.6 us: 1.01x slower                                                            |
| json_dumps              | 10.5 ms                                                                | 10.6 ms: 1.01x slower                                                            |
| tornado_http            | 98.4 ms                                                                | 99.2 ms: 1.01x slower                                                            |
| regex_dna               | 224 ms                                                                 | 226 ms: 1.01x slower                                                             |
| 2to3                    | 281 ms                                                                 | 284 ms: 1.01x slower                                                             |
| python_startup          | 10.1 ms                                                                | 10.2 ms: 1.01x slower                                                            |
| python_startup_no_site  | 8.76 ms                                                                | 8.84 ms: 1.01x slower                                                            |
| raytrace                | 298 ms                                                                 | 301 ms: 1.01x slower                                                             |
| pprint_pformat          | 1.65 sec                                                               | 1.67 sec: 1.01x slower                                                           |
| deepcopy                | 358 us                                                                 | 362 us: 1.01x slower                                                             |
| scimark_sor             | 124 ms                                                                 | 126 ms: 1.01x slower                                                             |
| meteor_contest          | 114 ms                                                                 | 116 ms: 1.01x slower                                                             |
| generators              | 29.4 ms                                                                | 29.8 ms: 1.01x slower                                                            |
| mdp                     | 2.64 sec                                                               | 2.69 sec: 1.02x slower                                                           |
| pycparser               | 1.22 sec                                                               | 1.24 sec: 1.02x slower                                                           |
| regex_effbot            | 3.65 ms                                                                | 3.74 ms: 1.02x slower                                                            |
| coroutines              | 21.7 ms                                                                | 22.2 ms: 1.02x slower                                                            |
| deltablue               | 3.48 ms                                                                | 3.57 ms: 1.02x slower                                                            |
| scimark_sparse_mat_mult | 5.90 ms                                                                | 6.06 ms: 1.03x slower                                                            |
| pickle_dict             | 35.5 us                                                                | 36.6 us: 1.03x slower                                                            |
| logging_silent          | 100 ns                                                                 | 103 ns: 1.03x slower                                                             |
| telco                   | 8.64 ms                                                                | 8.97 ms: 1.04x slower                                                            |
| unpickle                | 16.0 us                                                                | 17.0 us: 1.06x slower                                                            |
| Geometric mean          | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (26): xml_etree_iterparse, typing_runtime_protocols, coverage, xml_etree_parse, sympy_sum, chameleon, go, bench_mp_pool, async_tree_none, async_tree_none_tg, unpickle_pure_python, mypy2, comprehensions, pathlib, asyncio_websockets, spectral_norm, xml_etree_process, async_tree_cpu_io_mixed, dask, richards_super, deepcopy_memo, scimark_monte_carlo, regex_compile, richards, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg


# HPT report

- Reliability score: 55.86% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x