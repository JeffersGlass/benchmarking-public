
# Results vs. 3.12.0

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: 2e91dba
- commit date: 2021-12-08
- overall geometric mean: 1.02x faster \*
- HPT reliability: 61.72%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.90x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211208-linux-x86_64-python-main-3.11.0a3-2e91dba |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| 2to3           | 274 ms                                                 | 264 ms: 1.04x faster                                  |
| tornado_http   | 103 ms                                                 | 108 ms: 1.05x slower                                  |
| Geometric mean | (ref)                                                  | 1.00x slower                                          |

Benchmark hidden because not significant (1): chameleon

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211208-linux-x86_64-python-main-3.11.0a3-2e91dba |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| float          | 84.7 ms                                                | 79.2 ms: 1.07x faster                                 |
| nbody          | 97.0 ms                                                | 96.1 ms: 1.01x faster                                 |
| pidigits       | 187 ms                                                 | 198 ms: 1.06x slower                                  |
| Geometric mean | (ref)                                                  | 1.01x faster                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211208-linux-x86_64-python-main-3.11.0a3-2e91dba |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.21 ms: 1.12x faster                                 |
| regex_compile  | 148 ms                                                 | 139 ms: 1.07x faster                                  |
| regex_dna      | 212 ms                                                 | 212 ms: 1.00x faster                                  |
| regex_v8       | 23.1 ms                                                | 24.5 ms: 1.06x slower                                 |
| Geometric mean | (ref)                                                  | 1.03x faster                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211208-linux-x86_64-python-main-3.11.0a3-2e91dba |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pickle_dict          | 35.5 us                                                | 27.7 us: 1.28x faster                                 |
| pickle               | 11.6 us                                                | 9.95 us: 1.17x faster                                 |
| json_loads           | 28.5 us                                                | 25.6 us: 1.11x faster                                 |
| xml_etree_generate   | 89.2 ms                                                | 80.8 ms: 1.10x faster                                 |
| pickle_list          | 5.08 us                                                | 4.68 us: 1.09x faster                                 |
| unpickle             | 15.9 us                                                | 14.6 us: 1.09x faster                                 |
| xml_etree_process    | 61.7 ms                                                | 57.8 ms: 1.07x faster                                 |
| xml_etree_parse      | 159 ms                                                 | 156 ms: 1.02x faster                                  |
| unpickle_list        | 5.29 us                                                | 5.21 us: 1.01x faster                                 |
| xml_etree_iterparse  | 107 ms                                                 | 105 ms: 1.01x faster                                  |
| pickle_pure_python   | 324 us                                                 | 347 us: 1.07x slower                                  |
| unpickle_pure_python | 230 us                                                 | 251 us: 1.09x slower                                  |
| json_dumps           | 10.4 ms                                                | 12.6 ms: 1.21x slower                                 |
| Geometric mean       | (ref)                                                  | 1.04x faster                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211208-linux-x86_64-python-main-3.11.0a3-2e91dba |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| python_startup_no_site | 6.94 ms                                                | 5.78 ms: 1.20x faster                                 |
| python_startup         | 9.55 ms                                                | 8.00 ms: 1.19x faster                                 |
| Geometric mean         | (ref)                                                  | 1.20x faster                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211208-linux-x86_64-python-main-3.11.0a3-2e91dba |
|-----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| django_template | 34.6 ms                                                | 36.5 ms: 1.06x slower                                 |
| Geometric mean  | (ref)                                                  | 1.03x slower                                          |

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211208-linux-x86_64-python-main-3.11.0a3-2e91dba |
|-------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pickle_dict             | 35.5 us                                                | 27.7 us: 1.28x faster                                 |
| python_startup_no_site  | 6.94 ms                                                | 5.78 ms: 1.20x faster                                 |
| python_startup          | 9.55 ms                                                | 8.00 ms: 1.19x faster                                 |
| pickle                  | 11.6 us                                                | 9.95 us: 1.17x faster                                 |
| scimark_fft             | 382 ms                                                 | 332 ms: 1.15x faster                                  |
| regex_effbot            | 3.61 ms                                                | 3.21 ms: 1.12x faster                                 |
| logging_format          | 7.23 us                                                | 6.49 us: 1.11x faster                                 |
| json_loads              | 28.5 us                                                | 25.6 us: 1.11x faster                                 |
| spectral_norm           | 115 ms                                                 | 104 ms: 1.11x faster                                  |
| xml_etree_generate      | 89.2 ms                                                | 80.8 ms: 1.10x faster                                 |
| unpack_sequence         | 54.0 ns                                                | 49.2 ns: 1.10x faster                                 |
| json                    | 5.26 ms                                                | 4.83 ms: 1.09x faster                                 |
| pickle_list             | 5.08 us                                                | 4.68 us: 1.09x faster                                 |
| unpickle                | 15.9 us                                                | 14.6 us: 1.09x faster                                 |
| telco                   | 7.10 ms                                                | 6.56 ms: 1.08x faster                                 |
| logging_simple          | 6.46 us                                                | 5.97 us: 1.08x faster                                 |
| fannkuch                | 417 ms                                                 | 386 ms: 1.08x faster                                  |
| meteor_contest          | 112 ms                                                 | 104 ms: 1.08x faster                                  |
| float                   | 84.7 ms                                                | 79.2 ms: 1.07x faster                                 |
| regex_compile           | 148 ms                                                 | 139 ms: 1.07x faster                                  |
| xml_etree_process       | 61.7 ms                                                | 57.8 ms: 1.07x faster                                 |
| scimark_sparse_mat_mult | 5.06 ms                                                | 4.77 ms: 1.06x faster                                 |
| scimark_lu              | 118 ms                                                 | 112 ms: 1.06x faster                                  |
| 2to3                    | 274 ms                                                 | 264 ms: 1.04x faster                                  |
| sqlite_synth            | 2.83 us                                                | 2.74 us: 1.04x faster                                 |
| xml_etree_parse         | 159 ms                                                 | 156 ms: 1.02x faster                                  |
| dulwich_log             | 68.5 ms                                                | 67.2 ms: 1.02x faster                                 |
| scimark_monte_carlo     | 75.1 ms                                                | 74.0 ms: 1.02x faster                                 |
| unpickle_list           | 5.29 us                                                | 5.21 us: 1.01x faster                                 |
| xml_etree_iterparse     | 107 ms                                                 | 105 ms: 1.01x faster                                  |
| pyflate                 | 482 ms                                                 | 477 ms: 1.01x faster                                  |
| nbody                   | 97.0 ms                                                | 96.1 ms: 1.01x faster                                 |
| regex_dna               | 212 ms                                                 | 212 ms: 1.00x faster                                  |
| scimark_sor             | 129 ms                                                 | 130 ms: 1.01x slower                                  |
| sympy_integrate         | 21.4 ms                                                | 21.7 ms: 1.02x slower                                 |
| nqueens                 | 83.3 ms                                                | 84.6 ms: 1.02x slower                                 |
| sympy_sum               | 169 ms                                                 | 172 ms: 1.02x slower                                  |
| sympy_str               | 300 ms                                                 | 308 ms: 1.03x slower                                  |
| pycparser               | 1.18 sec                                               | 1.24 sec: 1.05x slower                                |
| tornado_http            | 103 ms                                                 | 108 ms: 1.05x slower                                  |
| django_template         | 34.6 ms                                                | 36.5 ms: 1.06x slower                                 |
| hexiom                  | 6.41 ms                                                | 6.77 ms: 1.06x slower                                 |
| logging_silent          | 104 ns                                                 | 110 ns: 1.06x slower                                  |
| pidigits                | 187 ms                                                 | 198 ms: 1.06x slower                                  |
| regex_v8                | 23.1 ms                                                | 24.5 ms: 1.06x slower                                 |
| sympy_expand            | 478 ms                                                 | 509 ms: 1.06x slower                                  |
| raytrace                | 312 ms                                                 | 333 ms: 1.07x slower                                  |
| pickle_pure_python      | 324 us                                                 | 347 us: 1.07x slower                                  |
| crypto_pyaes            | 81.9 ms                                                | 88.1 ms: 1.08x slower                                 |
| unpickle_pure_python    | 230 us                                                 | 251 us: 1.09x slower                                  |
| chaos                   | 67.0 ms                                                | 73.9 ms: 1.10x slower                                 |
| go                      | 139 ms                                                 | 158 ms: 1.13x slower                                  |
| richards                | 45.8 ms                                                | 54.5 ms: 1.19x slower                                 |
| json_dumps              | 10.4 ms                                                | 12.6 ms: 1.21x slower                                 |
| deltablue               | 3.72 ms                                                | 4.54 ms: 1.22x slower                                 |
| Geometric mean          | (ref)                                                  | 1.02x faster                                          |

Benchmark hidden because not significant (3): mako, chameleon, pathlib
Ignored benchmarks (40) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_generators, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_io, async_tree_io_tg, async_tree_memoization, async_tree_memoization_tg, async_tree_none, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, bench_mp_pool, bench_thread_pool, comprehensions, coroutines, coverage, create_gc_cycles, dask, deepcopy, deepcopy_memo, deepcopy_reduce, docutils, gc_traversal, generators, gunicorn, mdp, mypy2, pprint_pformat, pprint_safe_repr, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, sqlglot_normalize, sqlglot_optimize, sqlglot_parse, sqlglot_transpile, tomli_loads, typing_runtime_protocols
Ignored benchmarks (2) of results/bm-20211208-3.11.0a3-2e91dba/bm-20211208-linux-x86_64-python-main-3.11.0a3-2e91dba.json: html5lib, thrift


# HPT report

- Reliability score: 61.72% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.90x