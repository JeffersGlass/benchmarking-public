# Results vs. 3.12.0

- fork: faster-cpython
- ref: inline_values
- machine: linux-x86_64
- commit hash: 0dc68a4
- commit date: 2024-02-24
- overall geometric mean: 1.04x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: 0.94x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 262 ms: 1.05x faster                                                      |
| chameleon      | 7.41 ms                                                | 6.72 ms: 1.10x faster                                                     |
| docutils       | 2.77 sec                                               | 2.60 sec: 1.06x faster                                                    |
| tornado_http   | 103 ms                                                 | 94.1 ms: 1.09x faster                                                     |
| Geometric mean | (ref)                                                  | 1.08x faster                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|--------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_none_tg | 450 ms                                                 | 441 ms: 1.02x faster                                                      |
| async_tree_io      | 1.16 sec                                               | 1.16 sec: 1.00x slower                                                    |
| async_tree_io_tg   | 1.18 sec                                               | 1.19 sec: 1.01x slower                                                    |
| async_tree_none    | 472 ms                                                 | 477 ms: 1.01x slower                                                      |
| Geometric mean     | (ref)                                                  | 1.00x faster                                                              |

Benchmark hidden because not significant (4): async_tree_cpu_io_mixed_tg, async_tree_memoization, async_tree_cpu_io_mixed, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 90.6 ms: 1.07x faster                                                     |
| float          | 84.7 ms                                                | 79.5 ms: 1.07x faster                                                     |
| pidigits       | 187 ms                                                 | 203 ms: 1.09x slower                                                      |
| Geometric mean | (ref)                                                  | 1.02x faster                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 130 ms: 1.14x faster                                                      |
| regex_effbot   | 3.61 ms                                                | 3.55 ms: 1.02x faster                                                     |
| regex_dna      | 212 ms                                                 | 215 ms: 1.01x slower                                                      |
| regex_v8       | 23.1 ms                                                | 25.0 ms: 1.08x slower                                                     |
| Geometric mean | (ref)                                                  | 1.01x faster                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| unpickle_list        | 5.29 us                                                | 4.74 us: 1.12x faster                                                     |
| pickle_pure_python   | 324 us                                                 | 294 us: 1.10x faster                                                      |
| unpickle_pure_python | 230 us                                                 | 212 us: 1.08x faster                                                      |
| tomli_loads          | 2.33 sec                                               | 2.15 sec: 1.08x faster                                                    |
| xml_etree_process    | 61.7 ms                                                | 58.2 ms: 1.06x faster                                                     |
| xml_etree_generate   | 89.2 ms                                                | 85.3 ms: 1.04x faster                                                     |
| json_loads           | 28.5 us                                                | 27.6 us: 1.03x faster                                                     |
| unpickle             | 15.9 us                                                | 15.5 us: 1.03x faster                                                     |
| xml_etree_iterparse  | 107 ms                                                 | 105 ms: 1.02x faster                                                      |
| json_dumps           | 10.4 ms                                                | 10.3 ms: 1.01x faster                                                     |
| pickle_dict          | 35.5 us                                                | 35.3 us: 1.01x faster                                                     |
| pickle               | 11.6 us                                                | 11.9 us: 1.02x slower                                                     |
| pickle_list          | 5.08 us                                                | 5.30 us: 1.04x slower                                                     |
| Geometric mean       | (ref)                                                  | 1.04x faster                                                              |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                     |
| python_startup_no_site | 6.94 ms                                                | 8.82 ms: 1.27x slower                                                     |
| Geometric mean         | (ref)                                                  | 1.17x slower                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|-----------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 11.2 ms: 1.06x faster                                                     |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|--------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| typing_runtime_protocols | 158 us                                                 | 110 us: 1.44x faster                                                      |
| comprehensions           | 21.8 us                                                | 16.0 us: 1.36x faster                                                     |
| raytrace                 | 312 ms                                                 | 256 ms: 1.22x faster                                                      |
| logging_format           | 7.23 us                                                | 6.12 us: 1.18x faster                                                     |
| deltablue                | 3.72 ms                                                | 3.17 ms: 1.17x faster                                                     |
| crypto_pyaes             | 81.9 ms                                                | 71.2 ms: 1.15x faster                                                     |
| logging_simple           | 6.46 us                                                | 5.63 us: 1.15x faster                                                     |
| sympy_sum                | 169 ms                                                 | 148 ms: 1.14x faster                                                      |
| regex_compile            | 148 ms                                                 | 130 ms: 1.14x faster                                                      |
| chaos                    | 67.0 ms                                                | 59.2 ms: 1.13x faster                                                     |
| scimark_monte_carlo      | 75.1 ms                                                | 66.7 ms: 1.13x faster                                                     |
| sympy_str                | 300 ms                                                 | 267 ms: 1.12x faster                                                      |
| unpickle_list            | 5.29 us                                                | 4.74 us: 1.12x faster                                                     |
| sqlglot_parse            | 1.36 ms                                                | 1.23 ms: 1.11x faster                                                     |
| chameleon                | 7.41 ms                                                | 6.72 ms: 1.10x faster                                                     |
| pickle_pure_python       | 324 us                                                 | 294 us: 1.10x faster                                                      |
| deepcopy_reduce          | 3.35 us                                                | 3.05 us: 1.10x faster                                                     |
| tornado_http             | 103 ms                                                 | 94.1 ms: 1.09x faster                                                     |
| generators               | 31.2 ms                                                | 28.6 ms: 1.09x faster                                                     |
| sqlglot_transpile        | 1.68 ms                                                | 1.55 ms: 1.09x faster                                                     |
| sympy_integrate          | 21.4 ms                                                | 19.7 ms: 1.09x faster                                                     |
| fannkuch                 | 417 ms                                                 | 384 ms: 1.09x faster                                                      |
| unpickle_pure_python     | 230 us                                                 | 212 us: 1.08x faster                                                      |
| scimark_sor              | 129 ms                                                 | 119 ms: 1.08x faster                                                      |
| tomli_loads              | 2.33 sec                                               | 2.15 sec: 1.08x faster                                                    |
| deepcopy                 | 371 us                                                 | 343 us: 1.08x faster                                                      |
| coroutines               | 23.2 ms                                                | 21.5 ms: 1.08x faster                                                     |
| spectral_norm            | 115 ms                                                 | 107 ms: 1.08x faster                                                      |
| meteor_contest           | 112 ms                                                 | 104 ms: 1.08x faster                                                      |
| pyflate                  | 482 ms                                                 | 449 ms: 1.07x faster                                                      |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 4.71 ms: 1.07x faster                                                     |
| pprint_safe_repr         | 776 ms                                                 | 723 ms: 1.07x faster                                                      |
| nbody                    | 97.0 ms                                                | 90.6 ms: 1.07x faster                                                     |
| unpack_sequence          | 54.0 ns                                                | 50.5 ns: 1.07x faster                                                     |
| deepcopy_memo            | 40.7 us                                                | 38.1 us: 1.07x faster                                                     |
| float                    | 84.7 ms                                                | 79.5 ms: 1.07x faster                                                     |
| mako                     | 11.9 ms                                                | 11.2 ms: 1.06x faster                                                     |
| docutils                 | 2.77 sec                                               | 2.60 sec: 1.06x faster                                                    |
| pprint_pformat           | 1.57 sec                                               | 1.48 sec: 1.06x faster                                                    |
| xml_etree_process        | 61.7 ms                                                | 58.2 ms: 1.06x faster                                                     |
| scimark_fft              | 382 ms                                                 | 361 ms: 1.06x faster                                                      |
| pathlib                  | 19.3 ms                                                | 18.3 ms: 1.06x faster                                                     |
| sympy_expand             | 478 ms                                                 | 452 ms: 1.06x faster                                                      |
| mdp                      | 2.63 sec                                               | 2.50 sec: 1.05x faster                                                    |
| scimark_lu               | 118 ms                                                 | 112 ms: 1.05x faster                                                      |
| logging_silent           | 104 ns                                                 | 99.7 ns: 1.05x faster                                                     |
| 2to3                     | 274 ms                                                 | 262 ms: 1.05x faster                                                      |
| xml_etree_generate       | 89.2 ms                                                | 85.3 ms: 1.04x faster                                                     |
| sqlglot_normalize        | 110 ms                                                 | 106 ms: 1.04x faster                                                      |
| hexiom                   | 6.41 ms                                                | 6.16 ms: 1.04x faster                                                     |
| sqlglot_optimize         | 54.8 ms                                                | 52.9 ms: 1.04x faster                                                     |
| json                     | 5.26 ms                                                | 5.08 ms: 1.04x faster                                                     |
| nqueens                  | 83.3 ms                                                | 80.5 ms: 1.03x faster                                                     |
| json_loads               | 28.5 us                                                | 27.6 us: 1.03x faster                                                     |
| async_generators         | 463 ms                                                 | 448 ms: 1.03x faster                                                      |
| dulwich_log              | 68.5 ms                                                | 66.5 ms: 1.03x faster                                                     |
| bench_thread_pool        | 842 us                                                 | 820 us: 1.03x faster                                                      |
| unpickle                 | 15.9 us                                                | 15.5 us: 1.03x faster                                                     |
| async_tree_none_tg       | 450 ms                                                 | 441 ms: 1.02x faster                                                      |
| xml_etree_iterparse      | 107 ms                                                 | 105 ms: 1.02x faster                                                      |
| gc_traversal             | 3.79 ms                                                | 3.73 ms: 1.02x faster                                                     |
| regex_effbot             | 3.61 ms                                                | 3.55 ms: 1.02x faster                                                     |
| go                       | 139 ms                                                 | 137 ms: 1.02x faster                                                      |
| json_dumps               | 10.4 ms                                                | 10.3 ms: 1.01x faster                                                     |
| pickle_dict              | 35.5 us                                                | 35.3 us: 1.01x faster                                                     |
| asyncio_tcp              | 491 ms                                                 | 489 ms: 1.00x faster                                                      |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.78 sec: 1.00x faster                                                    |
| async_tree_io            | 1.16 sec                                               | 1.16 sec: 1.00x slower                                                    |
| async_tree_io_tg         | 1.18 sec                                               | 1.19 sec: 1.01x slower                                                    |
| async_tree_none          | 472 ms                                                 | 477 ms: 1.01x slower                                                      |
| regex_dna                | 212 ms                                                 | 215 ms: 1.01x slower                                                      |
| sqlite_synth             | 2.83 us                                                | 2.88 us: 1.01x slower                                                     |
| richards_super           | 51.5 ms                                                | 52.6 ms: 1.02x slower                                                     |
| pickle                   | 11.6 us                                                | 11.9 us: 1.02x slower                                                     |
| richards                 | 45.8 ms                                                | 47.3 ms: 1.03x slower                                                     |
| pickle_list              | 5.08 us                                                | 5.30 us: 1.04x slower                                                     |
| create_gc_cycles         | 1.48 ms                                                | 1.56 ms: 1.05x slower                                                     |
| python_startup           | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                     |
| regex_v8                 | 23.1 ms                                                | 25.0 ms: 1.08x slower                                                     |
| pidigits                 | 187 ms                                                 | 203 ms: 1.09x slower                                                      |
| telco                    | 7.10 ms                                                | 8.42 ms: 1.19x slower                                                     |
| python_startup_no_site   | 6.94 ms                                                | 8.82 ms: 1.27x slower                                                     |
| coverage                 | 72.7 ms                                                | 97.1 ms: 1.34x slower                                                     |
| Geometric mean           | (ref)                                                  | 1.04x faster                                                              |

Benchmark hidden because not significant (9): async_tree_cpu_io_mixed_tg, async_tree_memoization, xml_etree_parse, pycparser, async_tree_cpu_io_mixed, async_tree_memoization_tg, asyncio_websockets, bench_mp_pool, mypy2
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 0.94x