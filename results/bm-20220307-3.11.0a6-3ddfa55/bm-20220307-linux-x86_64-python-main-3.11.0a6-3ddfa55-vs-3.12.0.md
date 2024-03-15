
# Results vs. 3.12.0

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: 3ddfa55
- commit date: 2022-03-07
- overall geometric mean: 1.02x faster \*
- HPT reliability: 97.77%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.91x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220307-linux-x86_64-python-main-3.11.0a6-3ddfa55 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| 2to3           | 274 ms                                                 | 268 ms: 1.02x faster                                  |
| chameleon      | 7.41 ms                                                | 6.93 ms: 1.07x faster                                 |
| tornado_http   | 103 ms                                                 | 99.2 ms: 1.03x faster                                 |
| Geometric mean | (ref)                                                  | 1.04x faster                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220307-linux-x86_64-python-main-3.11.0a6-3ddfa55 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| float          | 84.7 ms                                                | 78.7 ms: 1.08x faster                                 |
| nbody          | 97.0 ms                                                | 97.7 ms: 1.01x slower                                 |
| pidigits       | 187 ms                                                 | 208 ms: 1.11x slower                                  |
| Geometric mean | (ref)                                                  | 1.01x slower                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220307-linux-x86_64-python-main-3.11.0a6-3ddfa55 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 140 ms: 1.06x faster                                  |
| regex_effbot   | 3.61 ms                                                | 3.49 ms: 1.04x faster                                 |
| regex_v8       | 23.1 ms                                                | 23.0 ms: 1.01x faster                                 |
| regex_dna      | 212 ms                                                 | 221 ms: 1.04x slower                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220307-linux-x86_64-python-main-3.11.0a6-3ddfa55 |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pickle_dict          | 35.5 us                                                | 28.1 us: 1.26x faster                                 |
| pickle               | 11.6 us                                                | 9.69 us: 1.20x faster                                 |
| pickle_list          | 5.08 us                                                | 4.51 us: 1.13x faster                                 |
| xml_etree_generate   | 89.2 ms                                                | 79.6 ms: 1.12x faster                                 |
| unpickle             | 15.9 us                                                | 14.2 us: 1.12x faster                                 |
| xml_etree_process    | 61.7 ms                                                | 56.0 ms: 1.10x faster                                 |
| unpickle_list        | 5.29 us                                                | 4.92 us: 1.07x faster                                 |
| xml_etree_parse      | 159 ms                                                 | 156 ms: 1.02x faster                                  |
| xml_etree_iterparse  | 107 ms                                                 | 105 ms: 1.02x faster                                  |
| json_loads           | 28.5 us                                                | 28.1 us: 1.01x faster                                 |
| pickle_pure_python   | 324 us                                                 | 335 us: 1.03x slower                                  |
| unpickle_pure_python | 230 us                                                 | 246 us: 1.07x slower                                  |
| json_dumps           | 10.4 ms                                                | 12.6 ms: 1.21x slower                                 |
| Geometric mean       | (ref)                                                  | 1.05x faster                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220307-linux-x86_64-python-main-3.11.0a6-3ddfa55 |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 8.20 ms: 1.17x faster                                 |
| python_startup_no_site | 6.94 ms                                                | 6.07 ms: 1.14x faster                                 |
| Geometric mean         | (ref)                                                  | 1.15x faster                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220307-linux-x86_64-python-main-3.11.0a6-3ddfa55 |
|-----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| mako            | 11.9 ms                                                | 10.6 ms: 1.12x faster                                 |
| django_template | 34.6 ms                                                | 36.0 ms: 1.04x slower                                 |
| Geometric mean  | (ref)                                                  | 1.04x faster                                          |

All benchmarks:
===============

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220307-linux-x86_64-python-main-3.11.0a6-3ddfa55 |
|-------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pickle_dict             | 35.5 us                                                | 28.1 us: 1.26x faster                                 |
| pickle                  | 11.6 us                                                | 9.69 us: 1.20x faster                                 |
| logging_format          | 7.23 us                                                | 6.08 us: 1.19x faster                                 |
| logging_simple          | 6.46 us                                                | 5.52 us: 1.17x faster                                 |
| python_startup          | 9.55 ms                                                | 8.20 ms: 1.17x faster                                 |
| python_startup_no_site  | 6.94 ms                                                | 6.07 ms: 1.14x faster                                 |
| scimark_fft             | 382 ms                                                 | 336 ms: 1.14x faster                                  |
| sqlite_synth            | 2.83 us                                                | 2.51 us: 1.13x faster                                 |
| pickle_list             | 5.08 us                                                | 4.51 us: 1.13x faster                                 |
| mako                    | 11.9 ms                                                | 10.6 ms: 1.12x faster                                 |
| xml_etree_generate      | 89.2 ms                                                | 79.6 ms: 1.12x faster                                 |
| unpickle                | 15.9 us                                                | 14.2 us: 1.12x faster                                 |
| xml_etree_process       | 61.7 ms                                                | 56.0 ms: 1.10x faster                                 |
| float                   | 84.7 ms                                                | 78.7 ms: 1.08x faster                                 |
| unpickle_list           | 5.29 us                                                | 4.92 us: 1.07x faster                                 |
| chameleon               | 7.41 ms                                                | 6.93 ms: 1.07x faster                                 |
| spectral_norm           | 115 ms                                                 | 107 ms: 1.07x faster                                  |
| pyflate                 | 482 ms                                                 | 453 ms: 1.06x faster                                  |
| pathlib                 | 19.3 ms                                                | 18.2 ms: 1.06x faster                                 |
| meteor_contest          | 112 ms                                                 | 106 ms: 1.06x faster                                  |
| regex_compile           | 148 ms                                                 | 140 ms: 1.06x faster                                  |
| json                    | 5.26 ms                                                | 5.00 ms: 1.05x faster                                 |
| scimark_sparse_mat_mult | 5.06 ms                                                | 4.82 ms: 1.05x faster                                 |
| fannkuch                | 417 ms                                                 | 398 ms: 1.05x faster                                  |
| scimark_sor             | 129 ms                                                 | 123 ms: 1.05x faster                                  |
| sympy_sum               | 169 ms                                                 | 163 ms: 1.04x faster                                  |
| sympy_str               | 300 ms                                                 | 289 ms: 1.04x faster                                  |
| regex_effbot            | 3.61 ms                                                | 3.49 ms: 1.04x faster                                 |
| tornado_http            | 103 ms                                                 | 99.2 ms: 1.03x faster                                 |
| scimark_monte_carlo     | 75.1 ms                                                | 72.9 ms: 1.03x faster                                 |
| dulwich_log             | 68.5 ms                                                | 66.5 ms: 1.03x faster                                 |
| sympy_integrate         | 21.4 ms                                                | 20.9 ms: 1.03x faster                                 |
| telco                   | 7.10 ms                                                | 6.92 ms: 1.03x faster                                 |
| 2to3                    | 274 ms                                                 | 268 ms: 1.02x faster                                  |
| scimark_lu              | 118 ms                                                 | 115 ms: 1.02x faster                                  |
| xml_etree_parse         | 159 ms                                                 | 156 ms: 1.02x faster                                  |
| xml_etree_iterparse     | 107 ms                                                 | 105 ms: 1.02x faster                                  |
| json_loads              | 28.5 us                                                | 28.1 us: 1.01x faster                                 |
| regex_v8                | 23.1 ms                                                | 23.0 ms: 1.01x faster                                 |
| sympy_expand            | 478 ms                                                 | 481 ms: 1.01x slower                                  |
| nbody                   | 97.0 ms                                                | 97.7 ms: 1.01x slower                                 |
| raytrace                | 312 ms                                                 | 318 ms: 1.02x slower                                  |
| pycparser               | 1.18 sec                                               | 1.21 sec: 1.03x slower                                |
| crypto_pyaes            | 81.9 ms                                                | 84.6 ms: 1.03x slower                                 |
| pickle_pure_python      | 324 us                                                 | 335 us: 1.03x slower                                  |
| regex_dna               | 212 ms                                                 | 221 ms: 1.04x slower                                  |
| django_template         | 34.6 ms                                                | 36.0 ms: 1.04x slower                                 |
| nqueens                 | 83.3 ms                                                | 87.0 ms: 1.04x slower                                 |
| go                      | 139 ms                                                 | 148 ms: 1.06x slower                                  |
| richards                | 45.8 ms                                                | 48.5 ms: 1.06x slower                                 |
| unpickle_pure_python    | 230 us                                                 | 246 us: 1.07x slower                                  |
| logging_silent          | 104 ns                                                 | 113 ns: 1.08x slower                                  |
| hexiom                  | 6.41 ms                                                | 7.04 ms: 1.10x slower                                 |
| chaos                   | 67.0 ms                                                | 73.5 ms: 1.10x slower                                 |
| pidigits                | 187 ms                                                 | 208 ms: 1.11x slower                                  |
| deltablue               | 3.72 ms                                                | 4.16 ms: 1.12x slower                                 |
| json_dumps              | 10.4 ms                                                | 12.6 ms: 1.21x slower                                 |
| unpack_sequence         | 54.0 ns                                                | 131 ns: 2.43x slower                                  |
| Geometric mean          | (ref)                                                  | 1.02x faster                                          |
Ignored benchmarks (40) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_generators, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_io, async_tree_io_tg, async_tree_memoization, async_tree_memoization_tg, async_tree_none, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, bench_mp_pool, bench_thread_pool, comprehensions, coroutines, coverage, create_gc_cycles, dask, deepcopy, deepcopy_memo, deepcopy_reduce, docutils, gc_traversal, generators, gunicorn, mdp, mypy2, pprint_pformat, pprint_safe_repr, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, sqlglot_normalize, sqlglot_optimize, sqlglot_parse, sqlglot_transpile, tomli_loads, typing_runtime_protocols
Ignored benchmarks (2) of results/bm-20220307-3.11.0a6-3ddfa55/bm-20220307-linux-x86_64-python-main-3.11.0a6-3ddfa55.json: html5lib, thrift


# HPT report

- Reliability score: 97.77% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.91x