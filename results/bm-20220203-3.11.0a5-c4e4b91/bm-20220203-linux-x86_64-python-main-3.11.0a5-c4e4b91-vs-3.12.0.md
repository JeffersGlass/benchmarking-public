
# Results vs. 3.12.0

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: c4e4b91
- commit date: 2022-02-03
- overall geometric mean: 1.03x faster \*
- HPT reliability: 83.25%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.91x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220203-linux-x86_64-python-main-3.11.0a5-c4e4b91 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| 2to3           | 274 ms                                                 | 267 ms: 1.03x faster                                  |
| chameleon      | 7.41 ms                                                | 6.95 ms: 1.07x faster                                 |
| tornado_http   | 103 ms                                                 | 106 ms: 1.03x slower                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220203-linux-x86_64-python-main-3.11.0a5-c4e4b91 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| float          | 84.7 ms                                                | 77.5 ms: 1.09x faster                                 |
| nbody          | 97.0 ms                                                | 94.7 ms: 1.02x faster                                 |
| pidigits       | 187 ms                                                 | 190 ms: 1.01x slower                                  |
| Geometric mean | (ref)                                                  | 1.03x faster                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220203-linux-x86_64-python-main-3.11.0a5-c4e4b91 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.14 ms: 1.15x faster                                 |
| regex_compile  | 148 ms                                                 | 140 ms: 1.06x faster                                  |
| regex_dna      | 212 ms                                                 | 213 ms: 1.00x slower                                  |
| regex_v8       | 23.1 ms                                                | 24.0 ms: 1.04x slower                                 |
| Geometric mean | (ref)                                                  | 1.04x faster                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220203-linux-x86_64-python-main-3.11.0a5-c4e4b91 |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pickle_dict          | 35.5 us                                                | 28.1 us: 1.26x faster                                 |
| unpickle             | 15.9 us                                                | 13.4 us: 1.18x faster                                 |
| pickle               | 11.6 us                                                | 9.93 us: 1.17x faster                                 |
| pickle_list          | 5.08 us                                                | 4.47 us: 1.14x faster                                 |
| xml_etree_generate   | 89.2 ms                                                | 79.6 ms: 1.12x faster                                 |
| xml_etree_process    | 61.7 ms                                                | 57.0 ms: 1.08x faster                                 |
| json_loads           | 28.5 us                                                | 26.7 us: 1.07x faster                                 |
| xml_etree_parse      | 159 ms                                                 | 153 ms: 1.04x faster                                  |
| pickle_pure_python   | 324 us                                                 | 334 us: 1.03x slower                                  |
| unpickle_pure_python | 230 us                                                 | 249 us: 1.08x slower                                  |
| json_dumps           | 10.4 ms                                                | 12.2 ms: 1.18x slower                                 |
| Geometric mean       | (ref)                                                  | 1.06x faster                                          |

Benchmark hidden because not significant (2): xml_etree_iterparse, unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220203-linux-x86_64-python-main-3.11.0a5-c4e4b91 |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 8.13 ms: 1.17x faster                                 |
| python_startup_no_site | 6.94 ms                                                | 5.92 ms: 1.17x faster                                 |
| Geometric mean         | (ref)                                                  | 1.17x faster                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220203-linux-x86_64-python-main-3.11.0a5-c4e4b91 |
|-----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| mako            | 11.9 ms                                                | 10.5 ms: 1.14x faster                                 |
| django_template | 34.6 ms                                                | 35.4 ms: 1.02x slower                                 |
| Geometric mean  | (ref)                                                  | 1.05x faster                                          |

All benchmarks:
===============

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220203-linux-x86_64-python-main-3.11.0a5-c4e4b91 |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pickle_dict            | 35.5 us                                                | 28.1 us: 1.26x faster                                 |
| unpickle               | 15.9 us                                                | 13.4 us: 1.18x faster                                 |
| python_startup         | 9.55 ms                                                | 8.13 ms: 1.17x faster                                 |
| python_startup_no_site | 6.94 ms                                                | 5.92 ms: 1.17x faster                                 |
| unpack_sequence        | 54.0 ns                                                | 46.0 ns: 1.17x faster                                 |
| pickle                 | 11.6 us                                                | 9.93 us: 1.17x faster                                 |
| regex_effbot           | 3.61 ms                                                | 3.14 ms: 1.15x faster                                 |
| pickle_list            | 5.08 us                                                | 4.47 us: 1.14x faster                                 |
| mako                   | 11.9 ms                                                | 10.5 ms: 1.14x faster                                 |
| logging_format         | 7.23 us                                                | 6.37 us: 1.14x faster                                 |
| xml_etree_generate     | 89.2 ms                                                | 79.6 ms: 1.12x faster                                 |
| logging_simple         | 6.46 us                                                | 5.84 us: 1.11x faster                                 |
| spectral_norm          | 115 ms                                                 | 104 ms: 1.10x faster                                  |
| scimark_fft            | 382 ms                                                 | 347 ms: 1.10x faster                                  |
| float                  | 84.7 ms                                                | 77.5 ms: 1.09x faster                                 |
| json                   | 5.26 ms                                                | 4.84 ms: 1.09x faster                                 |
| xml_etree_process      | 61.7 ms                                                | 57.0 ms: 1.08x faster                                 |
| meteor_contest         | 112 ms                                                 | 105 ms: 1.07x faster                                  |
| json_loads             | 28.5 us                                                | 26.7 us: 1.07x faster                                 |
| chameleon              | 7.41 ms                                                | 6.95 ms: 1.07x faster                                 |
| telco                  | 7.10 ms                                                | 6.70 ms: 1.06x faster                                 |
| regex_compile          | 148 ms                                                 | 140 ms: 1.06x faster                                  |
| pyflate                | 482 ms                                                 | 459 ms: 1.05x faster                                  |
| pathlib                | 19.3 ms                                                | 18.5 ms: 1.05x faster                                 |
| sqlite_synth           | 2.83 us                                                | 2.71 us: 1.05x faster                                 |
| xml_etree_parse        | 159 ms                                                 | 153 ms: 1.04x faster                                  |
| dulwich_log            | 68.5 ms                                                | 65.7 ms: 1.04x faster                                 |
| fannkuch               | 417 ms                                                 | 400 ms: 1.04x faster                                  |
| scimark_monte_carlo    | 75.1 ms                                                | 72.6 ms: 1.04x faster                                 |
| 2to3                   | 274 ms                                                 | 267 ms: 1.03x faster                                  |
| nbody                  | 97.0 ms                                                | 94.7 ms: 1.02x faster                                 |
| sympy_integrate        | 21.4 ms                                                | 21.3 ms: 1.01x faster                                 |
| regex_dna              | 212 ms                                                 | 213 ms: 1.00x slower                                  |
| sympy_sum              | 169 ms                                                 | 170 ms: 1.00x slower                                  |
| pycparser              | 1.18 sec                                               | 1.19 sec: 1.01x slower                                |
| pidigits               | 187 ms                                                 | 190 ms: 1.01x slower                                  |
| sympy_str              | 300 ms                                                 | 304 ms: 1.01x slower                                  |
| scimark_lu             | 118 ms                                                 | 120 ms: 1.02x slower                                  |
| django_template        | 34.6 ms                                                | 35.4 ms: 1.02x slower                                 |
| crypto_pyaes           | 81.9 ms                                                | 83.8 ms: 1.02x slower                                 |
| raytrace               | 312 ms                                                 | 321 ms: 1.03x slower                                  |
| tornado_http           | 103 ms                                                 | 106 ms: 1.03x slower                                  |
| pickle_pure_python     | 324 us                                                 | 334 us: 1.03x slower                                  |
| regex_v8               | 23.1 ms                                                | 24.0 ms: 1.04x slower                                 |
| nqueens                | 83.3 ms                                                | 87.2 ms: 1.05x slower                                 |
| sympy_expand           | 478 ms                                                 | 503 ms: 1.05x slower                                  |
| hexiom                 | 6.41 ms                                                | 6.76 ms: 1.05x slower                                 |
| go                     | 139 ms                                                 | 147 ms: 1.06x slower                                  |
| logging_silent         | 104 ns                                                 | 113 ns: 1.08x slower                                  |
| unpickle_pure_python   | 230 us                                                 | 249 us: 1.08x slower                                  |
| richards               | 45.8 ms                                                | 50.8 ms: 1.11x slower                                 |
| deltablue              | 3.72 ms                                                | 4.13 ms: 1.11x slower                                 |
| chaos                  | 67.0 ms                                                | 74.9 ms: 1.12x slower                                 |
| json_dumps             | 10.4 ms                                                | 12.2 ms: 1.18x slower                                 |
| Geometric mean         | (ref)                                                  | 1.03x faster                                          |

Benchmark hidden because not significant (4): xml_etree_iterparse, unpickle_list, scimark_sor, scimark_sparse_mat_mult
Ignored benchmarks (40) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_generators, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_io, async_tree_io_tg, async_tree_memoization, async_tree_memoization_tg, async_tree_none, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, bench_mp_pool, bench_thread_pool, comprehensions, coroutines, coverage, create_gc_cycles, dask, deepcopy, deepcopy_memo, deepcopy_reduce, docutils, gc_traversal, generators, gunicorn, mdp, mypy2, pprint_pformat, pprint_safe_repr, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, sqlglot_normalize, sqlglot_optimize, sqlglot_parse, sqlglot_transpile, tomli_loads, typing_runtime_protocols
Ignored benchmarks (2) of results/bm-20220203-3.11.0a5-c4e4b91/bm-20220203-linux-x86_64-python-main-3.11.0a5-c4e4b91.json: html5lib, thrift


# HPT report

- Reliability score: 83.25% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.91x