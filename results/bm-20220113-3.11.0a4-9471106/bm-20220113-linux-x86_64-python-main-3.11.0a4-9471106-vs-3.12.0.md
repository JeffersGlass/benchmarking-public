
# Results vs. 3.12.0

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: 9471106
- commit date: 2022-01-13
- overall geometric mean: 1.04x faster \*
- HPT reliability: 95.32%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.91x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220113-linux-x86_64-python-main-3.11.0a4-9471106 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| 2to3           | 274 ms                                                 | 264 ms: 1.04x faster                                  |
| chameleon      | 7.41 ms                                                | 7.55 ms: 1.02x slower                                 |
| tornado_http   | 103 ms                                                 | 107 ms: 1.04x slower                                  |
| Geometric mean | (ref)                                                  | 1.01x slower                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220113-linux-x86_64-python-main-3.11.0a4-9471106 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| float          | 84.7 ms                                                | 78.0 ms: 1.09x faster                                 |
| nbody          | 97.0 ms                                                | 95.1 ms: 1.02x faster                                 |
| pidigits       | 187 ms                                                 | 194 ms: 1.03x slower                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220113-linux-x86_64-python-main-3.11.0a4-9471106 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.25 ms: 1.11x faster                                 |
| regex_compile  | 148 ms                                                 | 138 ms: 1.07x faster                                  |
| regex_v8       | 23.1 ms                                                | 24.8 ms: 1.07x slower                                 |
| Geometric mean | (ref)                                                  | 1.03x faster                                          |

Benchmark hidden because not significant (1): regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220113-linux-x86_64-python-main-3.11.0a4-9471106 |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pickle_dict          | 35.5 us                                                | 26.8 us: 1.32x faster                                 |
| pickle               | 11.6 us                                                | 9.95 us: 1.17x faster                                 |
| pickle_list          | 5.08 us                                                | 4.37 us: 1.16x faster                                 |
| json_loads           | 28.5 us                                                | 25.1 us: 1.14x faster                                 |
| xml_etree_generate   | 89.2 ms                                                | 80.2 ms: 1.11x faster                                 |
| unpickle             | 15.9 us                                                | 14.3 us: 1.11x faster                                 |
| xml_etree_process    | 61.7 ms                                                | 56.9 ms: 1.09x faster                                 |
| xml_etree_parse      | 159 ms                                                 | 155 ms: 1.03x faster                                  |
| unpickle_list        | 5.29 us                                                | 5.20 us: 1.02x faster                                 |
| xml_etree_iterparse  | 107 ms                                                 | 107 ms: 1.01x slower                                  |
| pickle_pure_python   | 324 us                                                 | 329 us: 1.02x slower                                  |
| unpickle_pure_python | 230 us                                                 | 254 us: 1.10x slower                                  |
| json_dumps           | 10.4 ms                                                | 12.4 ms: 1.19x slower                                 |
| Geometric mean       | (ref)                                                  | 1.06x faster                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220113-linux-x86_64-python-main-3.11.0a4-9471106 |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| python_startup_no_site | 6.94 ms                                                | 5.85 ms: 1.19x faster                                 |
| python_startup         | 9.55 ms                                                | 8.07 ms: 1.18x faster                                 |
| Geometric mean         | (ref)                                                  | 1.18x faster                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220113-linux-x86_64-python-main-3.11.0a4-9471106 |
|-----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| mako            | 11.9 ms                                                | 11.5 ms: 1.03x faster                                 |
| django_template | 34.6 ms                                                | 35.2 ms: 1.02x slower                                 |
| Geometric mean  | (ref)                                                  | 1.01x faster                                          |

All benchmarks:
===============

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220113-linux-x86_64-python-main-3.11.0a4-9471106 |
|-------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pickle_dict             | 35.5 us                                                | 26.8 us: 1.32x faster                                 |
| unpack_sequence         | 54.0 ns                                                | 44.8 ns: 1.21x faster                                 |
| python_startup_no_site  | 6.94 ms                                                | 5.85 ms: 1.19x faster                                 |
| python_startup          | 9.55 ms                                                | 8.07 ms: 1.18x faster                                 |
| pickle                  | 11.6 us                                                | 9.95 us: 1.17x faster                                 |
| pickle_list             | 5.08 us                                                | 4.37 us: 1.16x faster                                 |
| spectral_norm           | 115 ms                                                 | 99.0 ms: 1.16x faster                                 |
| scimark_fft             | 382 ms                                                 | 330 ms: 1.16x faster                                  |
| json_loads              | 28.5 us                                                | 25.1 us: 1.14x faster                                 |
| regex_effbot            | 3.61 ms                                                | 3.25 ms: 1.11x faster                                 |
| xml_etree_generate      | 89.2 ms                                                | 80.2 ms: 1.11x faster                                 |
| logging_format          | 7.23 us                                                | 6.51 us: 1.11x faster                                 |
| unpickle                | 15.9 us                                                | 14.3 us: 1.11x faster                                 |
| json                    | 5.26 ms                                                | 4.74 ms: 1.11x faster                                 |
| meteor_contest          | 112 ms                                                 | 103 ms: 1.09x faster                                  |
| pyflate                 | 482 ms                                                 | 444 ms: 1.09x faster                                  |
| logging_simple          | 6.46 us                                                | 5.95 us: 1.09x faster                                 |
| xml_etree_process       | 61.7 ms                                                | 56.9 ms: 1.09x faster                                 |
| float                   | 84.7 ms                                                | 78.0 ms: 1.09x faster                                 |
| scimark_sparse_mat_mult | 5.06 ms                                                | 4.69 ms: 1.08x faster                                 |
| regex_compile           | 148 ms                                                 | 138 ms: 1.07x faster                                  |
| fannkuch                | 417 ms                                                 | 392 ms: 1.06x faster                                  |
| telco                   | 7.10 ms                                                | 6.69 ms: 1.06x faster                                 |
| dulwich_log             | 68.5 ms                                                | 65.8 ms: 1.04x faster                                 |
| 2to3                    | 274 ms                                                 | 264 ms: 1.04x faster                                  |
| scimark_sor             | 129 ms                                                 | 124 ms: 1.04x faster                                  |
| sqlite_synth            | 2.83 us                                                | 2.73 us: 1.04x faster                                 |
| scimark_lu              | 118 ms                                                 | 114 ms: 1.04x faster                                  |
| scimark_monte_carlo     | 75.1 ms                                                | 72.7 ms: 1.03x faster                                 |
| mako                    | 11.9 ms                                                | 11.5 ms: 1.03x faster                                 |
| xml_etree_parse         | 159 ms                                                 | 155 ms: 1.03x faster                                  |
| nbody                   | 97.0 ms                                                | 95.1 ms: 1.02x faster                                 |
| unpickle_list           | 5.29 us                                                | 5.20 us: 1.02x faster                                 |
| pathlib                 | 19.3 ms                                                | 19.1 ms: 1.01x faster                                 |
| pycparser               | 1.18 sec                                               | 1.17 sec: 1.01x faster                                |
| xml_etree_iterparse     | 107 ms                                                 | 107 ms: 1.01x slower                                  |
| sympy_str               | 300 ms                                                 | 302 ms: 1.01x slower                                  |
| nqueens                 | 83.3 ms                                                | 84.0 ms: 1.01x slower                                 |
| pickle_pure_python      | 324 us                                                 | 329 us: 1.02x slower                                  |
| django_template         | 34.6 ms                                                | 35.2 ms: 1.02x slower                                 |
| chameleon               | 7.41 ms                                                | 7.55 ms: 1.02x slower                                 |
| crypto_pyaes            | 81.9 ms                                                | 83.8 ms: 1.02x slower                                 |
| raytrace                | 312 ms                                                 | 320 ms: 1.03x slower                                  |
| hexiom                  | 6.41 ms                                                | 6.63 ms: 1.03x slower                                 |
| pidigits                | 187 ms                                                 | 194 ms: 1.03x slower                                  |
| tornado_http            | 103 ms                                                 | 107 ms: 1.04x slower                                  |
| sympy_expand            | 478 ms                                                 | 506 ms: 1.06x slower                                  |
| go                      | 139 ms                                                 | 148 ms: 1.06x slower                                  |
| regex_v8                | 23.1 ms                                                | 24.8 ms: 1.07x slower                                 |
| chaos                   | 67.0 ms                                                | 72.7 ms: 1.09x slower                                 |
| logging_silent          | 104 ns                                                 | 113 ns: 1.09x slower                                  |
| unpickle_pure_python    | 230 us                                                 | 254 us: 1.10x slower                                  |
| deltablue               | 3.72 ms                                                | 4.16 ms: 1.12x slower                                 |
| richards                | 45.8 ms                                                | 51.5 ms: 1.12x slower                                 |
| json_dumps              | 10.4 ms                                                | 12.4 ms: 1.19x slower                                 |
| Geometric mean          | (ref)                                                  | 1.04x faster                                          |

Benchmark hidden because not significant (3): sympy_integrate, regex_dna, sympy_sum
Ignored benchmarks (40) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_generators, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_io, async_tree_io_tg, async_tree_memoization, async_tree_memoization_tg, async_tree_none, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, bench_mp_pool, bench_thread_pool, comprehensions, coroutines, coverage, create_gc_cycles, dask, deepcopy, deepcopy_memo, deepcopy_reduce, docutils, gc_traversal, generators, gunicorn, mdp, mypy2, pprint_pformat, pprint_safe_repr, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, sqlglot_normalize, sqlglot_optimize, sqlglot_parse, sqlglot_transpile, tomli_loads, typing_runtime_protocols
Ignored benchmarks (2) of results/bm-20220113-3.11.0a4-9471106/bm-20220113-linux-x86_64-python-main-3.11.0a4-9471106.json: html5lib, thrift


# HPT report

- Reliability score: 95.32% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.91x