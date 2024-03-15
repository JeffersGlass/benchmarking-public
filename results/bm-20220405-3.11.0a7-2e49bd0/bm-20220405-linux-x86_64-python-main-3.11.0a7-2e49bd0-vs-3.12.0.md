
# Results vs. 3.12.0

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: 2e49bd0
- commit date: 2022-04-05
- overall geometric mean: 1.05x faster \*
- HPT reliability: 99.98%
- HPT 99th percentile: 1.02x faster
- Memory change: 0.89x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220405-linux-x86_64-python-main-3.11.0a7-2e49bd0 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| 2to3           | 274 ms                                                 | 264 ms: 1.04x faster                                  |
| chameleon      | 7.41 ms                                                | 6.87 ms: 1.08x faster                                 |
| tornado_http   | 103 ms                                                 | 95.4 ms: 1.08x faster                                 |
| Geometric mean | (ref)                                                  | 1.06x faster                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220405-linux-x86_64-python-main-3.11.0a7-2e49bd0 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| float          | 84.7 ms                                                | 74.4 ms: 1.14x faster                                 |
| nbody          | 97.0 ms                                                | 95.2 ms: 1.02x faster                                 |
| pidigits       | 187 ms                                                 | 197 ms: 1.05x slower                                  |
| Geometric mean | (ref)                                                  | 1.03x faster                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220405-linux-x86_64-python-main-3.11.0a7-2e49bd0 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.34 ms: 1.08x faster                                 |
| regex_compile  | 148 ms                                                 | 137 ms: 1.08x faster                                  |
| regex_dna      | 212 ms                                                 | 231 ms: 1.09x slower                                  |
| regex_v8       | 23.1 ms                                                | 25.9 ms: 1.12x slower                                 |
| Geometric mean | (ref)                                                  | 1.01x slower                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220405-linux-x86_64-python-main-3.11.0a7-2e49bd0 |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pickle_dict          | 35.5 us                                                | 27.6 us: 1.29x faster                                 |
| pickle               | 11.6 us                                                | 9.55 us: 1.21x faster                                 |
| xml_etree_generate   | 89.2 ms                                                | 78.5 ms: 1.14x faster                                 |
| unpickle             | 15.9 us                                                | 14.1 us: 1.13x faster                                 |
| xml_etree_process    | 61.7 ms                                                | 55.2 ms: 1.12x faster                                 |
| pickle_list          | 5.08 us                                                | 4.57 us: 1.11x faster                                 |
| unpickle_list        | 5.29 us                                                | 4.97 us: 1.06x faster                                 |
| pickle_pure_python   | 324 us                                                 | 311 us: 1.04x faster                                  |
| xml_etree_iterparse  | 107 ms                                                 | 104 ms: 1.03x faster                                  |
| xml_etree_parse      | 159 ms                                                 | 157 ms: 1.02x faster                                  |
| json_loads           | 28.5 us                                                | 28.1 us: 1.01x faster                                 |
| unpickle_pure_python | 230 us                                                 | 231 us: 1.00x slower                                  |
| json_dumps           | 10.4 ms                                                | 12.5 ms: 1.20x slower                                 |
| Geometric mean       | (ref)                                                  | 1.07x faster                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220405-linux-x86_64-python-main-3.11.0a7-2e49bd0 |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 8.07 ms: 1.18x faster                                 |
| python_startup_no_site | 6.94 ms                                                | 5.98 ms: 1.16x faster                                 |
| Geometric mean         | (ref)                                                  | 1.17x faster                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220405-linux-x86_64-python-main-3.11.0a7-2e49bd0 |
|-----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| mako            | 11.9 ms                                                | 10.2 ms: 1.17x faster                                 |
| django_template | 34.6 ms                                                | 34.3 ms: 1.01x faster                                 |
| Geometric mean  | (ref)                                                  | 1.09x faster                                          |

All benchmarks:
===============

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220405-linux-x86_64-python-main-3.11.0a7-2e49bd0 |
|-------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pickle_dict             | 35.5 us                                                | 27.6 us: 1.29x faster                                 |
| pickle                  | 11.6 us                                                | 9.55 us: 1.21x faster                                 |
| unpack_sequence         | 54.0 ns                                                | 44.9 ns: 1.20x faster                                 |
| python_startup          | 9.55 ms                                                | 8.07 ms: 1.18x faster                                 |
| mako                    | 11.9 ms                                                | 10.2 ms: 1.17x faster                                 |
| python_startup_no_site  | 6.94 ms                                                | 5.98 ms: 1.16x faster                                 |
| scimark_fft             | 382 ms                                                 | 335 ms: 1.14x faster                                  |
| float                   | 84.7 ms                                                | 74.4 ms: 1.14x faster                                 |
| logging_format          | 7.23 us                                                | 6.35 us: 1.14x faster                                 |
| xml_etree_generate      | 89.2 ms                                                | 78.5 ms: 1.14x faster                                 |
| sqlite_synth            | 2.83 us                                                | 2.51 us: 1.13x faster                                 |
| unpickle                | 15.9 us                                                | 14.1 us: 1.13x faster                                 |
| xml_etree_process       | 61.7 ms                                                | 55.2 ms: 1.12x faster                                 |
| pickle_list             | 5.08 us                                                | 4.57 us: 1.11x faster                                 |
| logging_simple          | 6.46 us                                                | 5.80 us: 1.11x faster                                 |
| pyflate                 | 482 ms                                                 | 438 ms: 1.10x faster                                  |
| spectral_norm           | 115 ms                                                 | 105 ms: 1.10x faster                                  |
| scimark_lu              | 118 ms                                                 | 108 ms: 1.09x faster                                  |
| regex_effbot            | 3.61 ms                                                | 3.34 ms: 1.08x faster                                 |
| regex_compile           | 148 ms                                                 | 137 ms: 1.08x faster                                  |
| chameleon               | 7.41 ms                                                | 6.87 ms: 1.08x faster                                 |
| telco                   | 7.10 ms                                                | 6.59 ms: 1.08x faster                                 |
| tornado_http            | 103 ms                                                 | 95.4 ms: 1.08x faster                                 |
| dulwich_log             | 68.5 ms                                                | 63.8 ms: 1.07x faster                                 |
| unpickle_list           | 5.29 us                                                | 4.97 us: 1.06x faster                                 |
| scimark_monte_carlo     | 75.1 ms                                                | 70.8 ms: 1.06x faster                                 |
| sympy_sum               | 169 ms                                                 | 160 ms: 1.06x faster                                  |
| meteor_contest          | 112 ms                                                 | 107 ms: 1.05x faster                                  |
| scimark_sor             | 129 ms                                                 | 123 ms: 1.05x faster                                  |
| pathlib                 | 19.3 ms                                                | 18.5 ms: 1.05x faster                                 |
| sympy_integrate         | 21.4 ms                                                | 20.5 ms: 1.05x faster                                 |
| sympy_str               | 300 ms                                                 | 287 ms: 1.04x faster                                  |
| scimark_sparse_mat_mult | 5.06 ms                                                | 4.85 ms: 1.04x faster                                 |
| fannkuch                | 417 ms                                                 | 401 ms: 1.04x faster                                  |
| pickle_pure_python      | 324 us                                                 | 311 us: 1.04x faster                                  |
| json                    | 5.26 ms                                                | 5.07 ms: 1.04x faster                                 |
| 2to3                    | 274 ms                                                 | 264 ms: 1.04x faster                                  |
| xml_etree_iterparse     | 107 ms                                                 | 104 ms: 1.03x faster                                  |
| raytrace                | 312 ms                                                 | 306 ms: 1.02x faster                                  |
| nbody                   | 97.0 ms                                                | 95.2 ms: 1.02x faster                                 |
| xml_etree_parse         | 159 ms                                                 | 157 ms: 1.02x faster                                  |
| json_loads              | 28.5 us                                                | 28.1 us: 1.01x faster                                 |
| django_template         | 34.6 ms                                                | 34.3 ms: 1.01x faster                                 |
| logging_silent          | 104 ns                                                 | 104 ns: 1.01x faster                                  |
| deltablue               | 3.72 ms                                                | 3.70 ms: 1.00x faster                                 |
| sympy_expand            | 478 ms                                                 | 476 ms: 1.00x faster                                  |
| unpickle_pure_python    | 230 us                                                 | 231 us: 1.00x slower                                  |
| crypto_pyaes            | 81.9 ms                                                | 82.7 ms: 1.01x slower                                 |
| go                      | 139 ms                                                 | 143 ms: 1.02x slower                                  |
| nqueens                 | 83.3 ms                                                | 85.2 ms: 1.02x slower                                 |
| richards                | 45.8 ms                                                | 47.5 ms: 1.04x slower                                 |
| chaos                   | 67.0 ms                                                | 70.2 ms: 1.05x slower                                 |
| pycparser               | 1.18 sec                                               | 1.24 sec: 1.05x slower                                |
| pidigits                | 187 ms                                                 | 197 ms: 1.05x slower                                  |
| hexiom                  | 6.41 ms                                                | 6.84 ms: 1.07x slower                                 |
| regex_dna               | 212 ms                                                 | 231 ms: 1.09x slower                                  |
| regex_v8                | 23.1 ms                                                | 25.9 ms: 1.12x slower                                 |
| json_dumps              | 10.4 ms                                                | 12.5 ms: 1.20x slower                                 |
| Geometric mean          | (ref)                                                  | 1.05x faster                                          |
Ignored benchmarks (40) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_generators, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_io, async_tree_io_tg, async_tree_memoization, async_tree_memoization_tg, async_tree_none, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, bench_mp_pool, bench_thread_pool, comprehensions, coroutines, coverage, create_gc_cycles, dask, deepcopy, deepcopy_memo, deepcopy_reduce, docutils, gc_traversal, generators, gunicorn, mdp, mypy2, pprint_pformat, pprint_safe_repr, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, sqlglot_normalize, sqlglot_optimize, sqlglot_parse, sqlglot_transpile, tomli_loads, typing_runtime_protocols
Ignored benchmarks (2) of results/bm-20220405-3.11.0a7-2e49bd0/bm-20220405-linux-x86_64-python-main-3.11.0a7-2e49bd0.json: html5lib, thrift


# HPT report

- Reliability score: 99.98% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 0.89x