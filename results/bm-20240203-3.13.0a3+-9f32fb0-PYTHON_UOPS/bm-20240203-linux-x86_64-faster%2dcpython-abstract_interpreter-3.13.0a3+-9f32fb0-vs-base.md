# Results vs. base

- fork: faster-cpython
- ref: abstract_interpreter
- machine: linux-x86_64
- commit hash: 9f32fb0
- commit date: 2024-02-03
- overall geometric mean: 1.01x faster
- HPT reliability: 99.54%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240202-linux-x86_64-python-0e71a295e9530c939a5e-3.13.0a3+-0e71a29 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 281 ms                                                                 | 284 ms: 1.01x slower                                                             |
| chameleon      | 7.33 ms                                                                | 7.28 ms: 1.01x faster                                                            |
| tornado_http   | 98.4 ms                                                                | 99.0 ms: 1.01x slower                                                            |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (1): docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark      | bm-20240202-linux-x86_64-python-0e71a295e9530c939a5e-3.13.0a3+-0e71a29 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_io  | 1.20 sec                                                               | 1.19 sec: 1.00x faster                                                           |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (7): async_tree_memoization_tg, async_tree_cpu_io_mixed, async_tree_none, async_tree_cpu_io_mixed_tg, async_tree_memoization, async_tree_io_tg, async_tree_none_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240202-linux-x86_64-python-0e71a295e9530c939a5e-3.13.0a3+-0e71a29 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 122 ms                                                                 | 109 ms: 1.12x faster                                                             |
| float          | 92.6 ms                                                                | 90.0 ms: 1.03x faster                                                            |
| Geometric mean | (ref)                                                                  | 1.05x faster                                                                     |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240202-linux-x86_64-python-0e71a295e9530c939a5e-3.13.0a3+-0e71a29 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_dna      | 224 ms                                                                 | 220 ms: 1.02x faster                                                             |
| regex_v8       | 25.2 ms                                                                | 25.0 ms: 1.01x faster                                                            |
| regex_compile  | 151 ms                                                                 | 149 ms: 1.01x faster                                                             |
| regex_effbot   | 3.65 ms                                                                | 3.67 ms: 1.01x slower                                                            |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240202-linux-x86_64-python-0e71a295e9530c939a5e-3.13.0a3+-0e71a29 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| tomli_loads          | 2.62 sec                                                               | 2.55 sec: 1.03x faster                                                           |
| pickle_dict          | 35.5 us                                                                | 34.6 us: 1.03x faster                                                            |
| xml_etree_iterparse  | 110 ms                                                                 | 108 ms: 1.02x faster                                                             |
| pickle_list          | 5.34 us                                                                | 5.26 us: 1.02x faster                                                            |
| pickle               | 11.9 us                                                                | 11.7 us: 1.01x faster                                                            |
| xml_etree_generate   | 89.4 ms                                                                | 88.3 ms: 1.01x faster                                                            |
| xml_etree_process    | 60.7 ms                                                                | 60.1 ms: 1.01x faster                                                            |
| xml_etree_parse      | 159 ms                                                                 | 157 ms: 1.01x faster                                                             |
| unpickle_pure_python | 236 us                                                                 | 234 us: 1.01x faster                                                             |
| json_loads           | 28.4 us                                                                | 28.6 us: 1.01x slower                                                            |
| json_dumps           | 10.5 ms                                                                | 10.7 ms: 1.01x slower                                                            |
| Geometric mean       | (ref)                                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (3): unpickle_list, pickle_pure_python, unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240202-linux-x86_64-python-0e71a295e9530c939a5e-3.13.0a3+-0e71a29 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                | 10.2 ms: 1.00x slower                                                            |
| python_startup_no_site | 8.76 ms                                                                | 8.80 ms: 1.00x slower                                                            |
| Geometric mean         | (ref)                                                                  | 1.00x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240202-linux-x86_64-python-0e71a295e9530c939a5e-3.13.0a3+-0e71a29 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 14.8 ms                                                                | 13.1 ms: 1.13x faster                                                            |

All benchmarks:
===============

| Benchmark               | bm-20240202-linux-x86_64-python-0e71a295e9530c939a5e-3.13.0a3+-0e71a29 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|-------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako                    | 14.8 ms                                                                | 13.1 ms: 1.13x faster                                                            |
| nbody                   | 122 ms                                                                 | 109 ms: 1.12x faster                                                             |
| spectral_norm           | 147 ms                                                                 | 134 ms: 1.10x faster                                                             |
| unpack_sequence         | 53.7 ns                                                                | 50.7 ns: 1.06x faster                                                            |
| gc_traversal            | 3.98 ms                                                                | 3.79 ms: 1.05x faster                                                            |
| hexiom                  | 8.48 ms                                                                | 8.11 ms: 1.05x faster                                                            |
| scimark_fft             | 449 ms                                                                 | 431 ms: 1.04x faster                                                             |
| crypto_pyaes            | 84.2 ms                                                                | 81.7 ms: 1.03x faster                                                            |
| float                   | 92.6 ms                                                                | 90.0 ms: 1.03x faster                                                            |
| comprehensions          | 21.4 us                                                                | 20.8 us: 1.03x faster                                                            |
| tomli_loads             | 2.62 sec                                                               | 2.55 sec: 1.03x faster                                                           |
| nqueens                 | 94.7 ms                                                                | 92.3 ms: 1.03x faster                                                            |
| pickle_dict             | 35.5 us                                                                | 34.6 us: 1.03x faster                                                            |
| scimark_sparse_mat_mult | 5.90 ms                                                                | 5.75 ms: 1.02x faster                                                            |
| fannkuch                | 452 ms                                                                 | 441 ms: 1.02x faster                                                             |
| chaos                   | 73.8 ms                                                                | 72.2 ms: 1.02x faster                                                            |
| regex_dna               | 224 ms                                                                 | 220 ms: 1.02x faster                                                             |
| pyflate                 | 518 ms                                                                 | 509 ms: 1.02x faster                                                             |
| logging_format          | 6.75 us                                                                | 6.63 us: 1.02x faster                                                            |
| xml_etree_iterparse     | 110 ms                                                                 | 108 ms: 1.02x faster                                                             |
| meteor_contest          | 114 ms                                                                 | 112 ms: 1.02x faster                                                             |
| logging_simple          | 5.94 us                                                                | 5.85 us: 1.02x faster                                                            |
| pickle_list             | 5.34 us                                                                | 5.26 us: 1.02x faster                                                            |
| sympy_integrate         | 21.2 ms                                                                | 20.9 ms: 1.02x faster                                                            |
| pickle                  | 11.9 us                                                                | 11.7 us: 1.01x faster                                                            |
| scimark_sor             | 124 ms                                                                 | 122 ms: 1.01x faster                                                             |
| deepcopy_reduce         | 3.18 us                                                                | 3.14 us: 1.01x faster                                                            |
| deepcopy_memo           | 40.2 us                                                                | 39.6 us: 1.01x faster                                                            |
| json                    | 5.33 ms                                                                | 5.26 ms: 1.01x faster                                                            |
| xml_etree_generate      | 89.4 ms                                                                | 88.3 ms: 1.01x faster                                                            |
| sqlglot_optimize        | 57.8 ms                                                                | 57.1 ms: 1.01x faster                                                            |
| scimark_monte_carlo     | 80.8 ms                                                                | 79.9 ms: 1.01x faster                                                            |
| regex_v8                | 25.2 ms                                                                | 25.0 ms: 1.01x faster                                                            |
| xml_etree_process       | 60.7 ms                                                                | 60.1 ms: 1.01x faster                                                            |
| regex_compile           | 151 ms                                                                 | 149 ms: 1.01x faster                                                             |
| xml_etree_parse         | 159 ms                                                                 | 157 ms: 1.01x faster                                                             |
| create_gc_cycles        | 1.48 ms                                                                | 1.47 ms: 1.01x faster                                                            |
| unpickle_pure_python    | 236 us                                                                 | 234 us: 1.01x faster                                                             |
| chameleon               | 7.33 ms                                                                | 7.28 ms: 1.01x faster                                                            |
| scimark_lu              | 117 ms                                                                 | 117 ms: 1.01x faster                                                             |
| sympy_sum               | 161 ms                                                                 | 160 ms: 1.01x faster                                                             |
| sqlglot_parse           | 1.33 ms                                                                | 1.33 ms: 1.00x faster                                                            |
| async_tree_io           | 1.20 sec                                                               | 1.19 sec: 1.00x faster                                                           |
| sqlglot_normalize       | 113 ms                                                                 | 113 ms: 1.00x faster                                                             |
| asyncio_tcp             | 490 ms                                                                 | 491 ms: 1.00x slower                                                             |
| python_startup          | 10.1 ms                                                                | 10.2 ms: 1.00x slower                                                            |
| python_startup_no_site  | 8.76 ms                                                                | 8.80 ms: 1.00x slower                                                            |
| mdp                     | 2.64 sec                                                               | 2.66 sec: 1.01x slower                                                           |
| regex_effbot            | 3.65 ms                                                                | 3.67 ms: 1.01x slower                                                            |
| tornado_http            | 98.4 ms                                                                | 99.0 ms: 1.01x slower                                                            |
| bench_thread_pool       | 842 us                                                                 | 848 us: 1.01x slower                                                             |
| richards_super          | 54.1 ms                                                                | 54.5 ms: 1.01x slower                                                            |
| richards                | 48.4 ms                                                                | 48.8 ms: 1.01x slower                                                            |
| json_loads              | 28.4 us                                                                | 28.6 us: 1.01x slower                                                            |
| 2to3                    | 281 ms                                                                 | 284 ms: 1.01x slower                                                             |
| go                      | 173 ms                                                                 | 175 ms: 1.01x slower                                                             |
| raytrace                | 298 ms                                                                 | 301 ms: 1.01x slower                                                             |
| dulwich_log             | 69.2 ms                                                                | 69.9 ms: 1.01x slower                                                            |
| json_dumps              | 10.5 ms                                                                | 10.7 ms: 1.01x slower                                                            |
| coroutines              | 21.7 ms                                                                | 22.0 ms: 1.01x slower                                                            |
| deltablue               | 3.48 ms                                                                | 3.54 ms: 1.02x slower                                                            |
| telco                   | 8.64 ms                                                                | 8.79 ms: 1.02x slower                                                            |
| generators              | 29.4 ms                                                                | 30.3 ms: 1.03x slower                                                            |
| pycparser               | 1.22 sec                                                               | 1.27 sec: 1.04x slower                                                           |
| logging_silent          | 100 ns                                                                 | 105 ns: 1.05x slower                                                             |
| Geometric mean          | (ref)                                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (27): coverage, sympy_str, async_tree_memoization_tg, pprint_safe_repr, typing_runtime_protocols, sqlite_synth, async_tree_cpu_io_mixed, unpickle_list, pprint_pformat, async_tree_none, async_tree_cpu_io_mixed_tg, async_tree_memoization, bench_mp_pool, async_tree_io_tg, pickle_pure_python, deepcopy, sqlglot_transpile, docutils, pidigits, asyncio_websockets, asyncio_tcp_ssl, async_generators, pathlib, async_tree_none_tg, dask, sympy_expand, unpickle
Ignored benchmarks (1) of results/bm-20240202-3.13.0a3+-0e71a29-PYTHON_UOPS/bm-20240202-linux-x86_64-python-0e71a295e9530c939a5e-3.13.0a3+-0e71a29.json: mypy2


# HPT report

- Reliability score: 99.54% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x