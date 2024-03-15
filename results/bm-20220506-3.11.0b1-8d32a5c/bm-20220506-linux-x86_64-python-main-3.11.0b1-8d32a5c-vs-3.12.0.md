
# Results vs. 3.12.0

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: 8d32a5c
- commit date: 2022-05-06
- overall geometric mean: 1.09x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x faster
- Memory change: 0.87x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220506-linux-x86_64-python-main-3.11.0b1-8d32a5c |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| 2to3           | 274 ms                                                 | 256 ms: 1.07x faster                                  |
| chameleon      | 7.41 ms                                                | 6.57 ms: 1.13x faster                                 |
| tornado_http   | 103 ms                                                 | 94.6 ms: 1.08x faster                                 |
| Geometric mean | (ref)                                                  | 1.09x faster                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220506-linux-x86_64-python-main-3.11.0b1-8d32a5c |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| float          | 84.7 ms                                                | 72.5 ms: 1.17x faster                                 |
| nbody          | 97.0 ms                                                | 93.1 ms: 1.04x faster                                 |
| pidigits       | 187 ms                                                 | 190 ms: 1.01x slower                                  |
| Geometric mean | (ref)                                                  | 1.06x faster                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220506-linux-x86_64-python-main-3.11.0b1-8d32a5c |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 2.93 ms: 1.23x faster                                 |
| regex_compile  | 148 ms                                                 | 135 ms: 1.10x faster                                  |
| regex_v8       | 23.1 ms                                                | 21.6 ms: 1.07x faster                                 |
| regex_dna      | 212 ms                                                 | 204 ms: 1.04x faster                                  |
| Geometric mean | (ref)                                                  | 1.11x faster                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220506-linux-x86_64-python-main-3.11.0b1-8d32a5c |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pickle_dict          | 35.5 us                                                | 25.6 us: 1.39x faster                                 |
| pickle               | 11.6 us                                                | 9.56 us: 1.21x faster                                 |
| pickle_list          | 5.08 us                                                | 4.26 us: 1.19x faster                                 |
| unpickle             | 15.9 us                                                | 13.4 us: 1.19x faster                                 |
| xml_etree_generate   | 89.2 ms                                                | 76.5 ms: 1.17x faster                                 |
| xml_etree_process    | 61.7 ms                                                | 53.6 ms: 1.15x faster                                 |
| json_loads           | 28.5 us                                                | 25.4 us: 1.12x faster                                 |
| pickle_pure_python   | 324 us                                                 | 305 us: 1.06x faster                                  |
| unpickle_list        | 5.29 us                                                | 5.05 us: 1.05x faster                                 |
| xml_etree_iterparse  | 107 ms                                                 | 104 ms: 1.02x faster                                  |
| xml_etree_parse      | 159 ms                                                 | 157 ms: 1.02x faster                                  |
| unpickle_pure_python | 230 us                                                 | 229 us: 1.01x faster                                  |
| json_dumps           | 10.4 ms                                                | 12.4 ms: 1.19x slower                                 |
| Geometric mean       | (ref)                                                  | 1.10x faster                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220506-linux-x86_64-python-main-3.11.0b1-8d32a5c |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 8.25 ms: 1.16x faster                                 |
| python_startup_no_site | 6.94 ms                                                | 6.16 ms: 1.13x faster                                 |
| Geometric mean         | (ref)                                                  | 1.14x faster                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220506-linux-x86_64-python-main-3.11.0b1-8d32a5c |
|-----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| mako            | 11.9 ms                                                | 9.88 ms: 1.20x faster                                 |
| django_template | 34.6 ms                                                | 32.8 ms: 1.06x faster                                 |
| Geometric mean  | (ref)                                                  | 1.13x faster                                          |

All benchmarks:
===============

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220506-linux-x86_64-python-main-3.11.0b1-8d32a5c |
|-------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pickle_dict             | 35.5 us                                                | 25.6 us: 1.39x faster                                 |
| regex_effbot            | 3.61 ms                                                | 2.93 ms: 1.23x faster                                 |
| unpack_sequence         | 54.0 ns                                                | 44.3 ns: 1.22x faster                                 |
| pickle                  | 11.6 us                                                | 9.56 us: 1.21x faster                                 |
| mako                    | 11.9 ms                                                | 9.88 ms: 1.20x faster                                 |
| pickle_list             | 5.08 us                                                | 4.26 us: 1.19x faster                                 |
| unpickle                | 15.9 us                                                | 13.4 us: 1.19x faster                                 |
| spectral_norm           | 115 ms                                                 | 97.6 ms: 1.18x faster                                 |
| pyflate                 | 482 ms                                                 | 411 ms: 1.17x faster                                  |
| scimark_fft             | 382 ms                                                 | 325 ms: 1.17x faster                                  |
| float                   | 84.7 ms                                                | 72.5 ms: 1.17x faster                                 |
| xml_etree_generate      | 89.2 ms                                                | 76.5 ms: 1.17x faster                                 |
| python_startup          | 9.55 ms                                                | 8.25 ms: 1.16x faster                                 |
| xml_etree_process       | 61.7 ms                                                | 53.6 ms: 1.15x faster                                 |
| scimark_monte_carlo     | 75.1 ms                                                | 66.5 ms: 1.13x faster                                 |
| chameleon               | 7.41 ms                                                | 6.57 ms: 1.13x faster                                 |
| scimark_sor             | 129 ms                                                 | 115 ms: 1.13x faster                                  |
| python_startup_no_site  | 6.94 ms                                                | 6.16 ms: 1.13x faster                                 |
| json_loads              | 28.5 us                                                | 25.4 us: 1.12x faster                                 |
| logging_format          | 7.23 us                                                | 6.44 us: 1.12x faster                                 |
| sqlite_synth            | 2.83 us                                                | 2.53 us: 1.12x faster                                 |
| scimark_sparse_mat_mult | 5.06 ms                                                | 4.57 ms: 1.11x faster                                 |
| regex_compile           | 148 ms                                                 | 135 ms: 1.10x faster                                  |
| crypto_pyaes            | 81.9 ms                                                | 74.3 ms: 1.10x faster                                 |
| logging_simple          | 6.46 us                                                | 5.89 us: 1.10x faster                                 |
| dulwich_log             | 68.5 ms                                                | 62.8 ms: 1.09x faster                                 |
| tornado_http            | 103 ms                                                 | 94.6 ms: 1.08x faster                                 |
| fannkuch                | 417 ms                                                 | 385 ms: 1.08x faster                                  |
| pathlib                 | 19.3 ms                                                | 17.9 ms: 1.08x faster                                 |
| scimark_lu              | 118 ms                                                 | 109 ms: 1.08x faster                                  |
| meteor_contest          | 112 ms                                                 | 105 ms: 1.07x faster                                  |
| json                    | 5.26 ms                                                | 4.91 ms: 1.07x faster                                 |
| regex_v8                | 23.1 ms                                                | 21.6 ms: 1.07x faster                                 |
| 2to3                    | 274 ms                                                 | 256 ms: 1.07x faster                                  |
| logging_silent          | 104 ns                                                 | 98.2 ns: 1.06x faster                                 |
| raytrace                | 312 ms                                                 | 294 ms: 1.06x faster                                  |
| pickle_pure_python      | 324 us                                                 | 305 us: 1.06x faster                                  |
| sympy_str               | 300 ms                                                 | 284 ms: 1.06x faster                                  |
| django_template         | 34.6 ms                                                | 32.8 ms: 1.06x faster                                 |
| sympy_sum               | 169 ms                                                 | 161 ms: 1.05x faster                                  |
| sympy_integrate         | 21.4 ms                                                | 20.5 ms: 1.05x faster                                 |
| unpickle_list           | 5.29 us                                                | 5.05 us: 1.05x faster                                 |
| nbody                   | 97.0 ms                                                | 93.1 ms: 1.04x faster                                 |
| regex_dna               | 212 ms                                                 | 204 ms: 1.04x faster                                  |
| telco                   | 7.10 ms                                                | 6.84 ms: 1.04x faster                                 |
| deltablue               | 3.72 ms                                                | 3.61 ms: 1.03x faster                                 |
| go                      | 139 ms                                                 | 136 ms: 1.02x faster                                  |
| xml_etree_iterparse     | 107 ms                                                 | 104 ms: 1.02x faster                                  |
| sympy_expand            | 478 ms                                                 | 468 ms: 1.02x faster                                  |
| hexiom                  | 6.41 ms                                                | 6.29 ms: 1.02x faster                                 |
| xml_etree_parse         | 159 ms                                                 | 157 ms: 1.02x faster                                  |
| unpickle_pure_python    | 230 us                                                 | 229 us: 1.01x faster                                  |
| richards                | 45.8 ms                                                | 46.4 ms: 1.01x slower                                 |
| pidigits                | 187 ms                                                 | 190 ms: 1.01x slower                                  |
| nqueens                 | 83.3 ms                                                | 84.7 ms: 1.02x slower                                 |
| chaos                   | 67.0 ms                                                | 68.6 ms: 1.02x slower                                 |
| json_dumps              | 10.4 ms                                                | 12.4 ms: 1.19x slower                                 |
| Geometric mean          | (ref)                                                  | 1.09x faster                                          |

Benchmark hidden because not significant (1): pycparser
Ignored benchmarks (40) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_generators, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_io, async_tree_io_tg, async_tree_memoization, async_tree_memoization_tg, async_tree_none, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, bench_mp_pool, bench_thread_pool, comprehensions, coroutines, coverage, create_gc_cycles, dask, deepcopy, deepcopy_memo, deepcopy_reduce, docutils, gc_traversal, generators, gunicorn, mdp, mypy2, pprint_pformat, pprint_safe_repr, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, sqlglot_normalize, sqlglot_optimize, sqlglot_parse, sqlglot_transpile, tomli_loads, typing_runtime_protocols
Ignored benchmarks (2) of results/bm-20220506-3.11.0b1-8d32a5c/bm-20220506-linux-x86_64-python-main-3.11.0b1-8d32a5c.json: html5lib, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.05x
- 95% likely to have a speedup of 1.05x
- 99% likely to have a speedup of 1.04x


# Memory

- memory change: 0.87x