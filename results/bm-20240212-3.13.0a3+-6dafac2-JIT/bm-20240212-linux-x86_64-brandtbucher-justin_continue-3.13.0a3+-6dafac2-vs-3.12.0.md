
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_continue
- machine: linux-x86_64
- commit hash: 6dafac2
- commit date: 2024-02-12
- overall geometric mean: 1.02x faster \*
- HPT reliability: 99.69%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.96x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| chameleon      | 7.41 ms                                                | 6.93 ms: 1.07x faster                                                   |
| docutils       | 2.77 sec                                               | 2.64 sec: 1.05x faster                                                  |
| tornado_http   | 103 ms                                                 | 96.7 ms: 1.06x faster                                                   |
| Geometric mean | (ref)                                                  | 1.04x faster                                                            |

Benchmark hidden because not significant (1): 2to3

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|-------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| async_tree_none         | 472 ms                                                 | 440 ms: 1.07x faster                                                    |
| async_tree_memoization  | 578 ms                                                 | 565 ms: 1.02x faster                                                    |
| async_tree_cpu_io_mixed | 726 ms                                                 | 715 ms: 1.02x faster                                                    |
| async_tree_io_tg        | 1.18 sec                                               | 1.20 sec: 1.01x slower                                                  |
| async_tree_io           | 1.16 sec                                               | 1.18 sec: 1.02x slower                                                  |
| Geometric mean          | (ref)                                                  | 1.01x faster                                                            |

Benchmark hidden because not significant (3): async_tree_cpu_io_mixed_tg, async_tree_none_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 93.6 ms: 1.04x faster                                                   |
| float          | 84.7 ms                                                | 82.8 ms: 1.02x faster                                                   |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x faster                                                    |
| Geometric mean | (ref)                                                  | 1.02x faster                                                            |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 137 ms: 1.09x faster                                                    |
| regex_effbot   | 3.61 ms                                                | 3.68 ms: 1.02x slower                                                   |
| regex_dna      | 212 ms                                                 | 226 ms: 1.06x slower                                                    |
| regex_v8       | 23.1 ms                                                | 25.7 ms: 1.11x slower                                                   |
| Geometric mean | (ref)                                                  | 1.03x slower                                                            |

Benchmarks with tag 'serialize':
================================

| Benchmark          | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|--------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| tomli_loads        | 2.33 sec                                               | 2.06 sec: 1.13x faster                                                  |
| pickle_pure_python | 324 us                                                 | 297 us: 1.09x faster                                                    |
| pickle_dict        | 35.5 us                                                | 32.9 us: 1.08x faster                                                   |
| xml_etree_process  | 61.7 ms                                                | 57.5 ms: 1.07x faster                                                   |
| unpickle_list      | 5.29 us                                                | 5.04 us: 1.05x faster                                                   |
| xml_etree_generate | 89.2 ms                                                | 85.5 ms: 1.04x faster                                                   |
| pickle_list        | 5.08 us                                                | 4.89 us: 1.04x faster                                                   |
| unpickle           | 15.9 us                                                | 15.3 us: 1.04x faster                                                   |
| json_loads         | 28.5 us                                                | 27.8 us: 1.02x faster                                                   |
| pickle             | 11.6 us                                                | 11.4 us: 1.02x faster                                                   |
| xml_etree_parse    | 159 ms                                                 | 157 ms: 1.01x faster                                                    |
| Geometric mean     | (ref)                                                  | 1.04x faster                                                            |

Benchmark hidden because not significant (3): unpickle_pure_python, xml_etree_iterparse, json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                   |
| python_startup_no_site | 6.94 ms                                                | 8.88 ms: 1.28x slower                                                   |
| Geometric mean         | (ref)                                                  | 1.17x slower                                                            |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|-----------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 11.8 ms: 1.01x faster                                                   |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|--------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| typing_runtime_protocols | 158 us                                                 | 109 us: 1.45x faster                                                    |
| unpack_sequence          | 54.0 ns                                                | 39.0 ns: 1.38x faster                                                   |
| comprehensions           | 21.8 us                                                | 17.8 us: 1.22x faster                                                   |
| logging_format           | 7.23 us                                                | 6.20 us: 1.17x faster                                                   |
| logging_simple           | 6.46 us                                                | 5.61 us: 1.15x faster                                                   |
| raytrace                 | 312 ms                                                 | 275 ms: 1.13x faster                                                    |
| tomli_loads              | 2.33 sec                                               | 2.06 sec: 1.13x faster                                                  |
| deltablue                | 3.72 ms                                                | 3.32 ms: 1.12x faster                                                   |
| deepcopy_reduce          | 3.35 us                                                | 3.04 us: 1.10x faster                                                   |
| deepcopy_memo            | 40.7 us                                                | 37.2 us: 1.09x faster                                                   |
| deepcopy                 | 371 us                                                 | 340 us: 1.09x faster                                                    |
| pickle_pure_python       | 324 us                                                 | 297 us: 1.09x faster                                                    |
| regex_compile            | 148 ms                                                 | 137 ms: 1.09x faster                                                    |
| crypto_pyaes             | 81.9 ms                                                | 75.8 ms: 1.08x faster                                                   |
| pickle_dict              | 35.5 us                                                | 32.9 us: 1.08x faster                                                   |
| generators               | 31.2 ms                                                | 29.1 ms: 1.07x faster                                                   |
| xml_etree_process        | 61.7 ms                                                | 57.5 ms: 1.07x faster                                                   |
| async_tree_none          | 472 ms                                                 | 440 ms: 1.07x faster                                                    |
| scimark_fft              | 382 ms                                                 | 357 ms: 1.07x faster                                                    |
| chameleon                | 7.41 ms                                                | 6.93 ms: 1.07x faster                                                   |
| sympy_sum                | 169 ms                                                 | 158 ms: 1.07x faster                                                    |
| sqlglot_parse            | 1.36 ms                                                | 1.28 ms: 1.06x faster                                                   |
| sympy_str                | 300 ms                                                 | 282 ms: 1.06x faster                                                    |
| pathlib                  | 19.3 ms                                                | 18.2 ms: 1.06x faster                                                   |
| tornado_http             | 103 ms                                                 | 96.7 ms: 1.06x faster                                                   |
| meteor_contest           | 112 ms                                                 | 106 ms: 1.06x faster                                                    |
| scimark_monte_carlo      | 75.1 ms                                                | 71.2 ms: 1.05x faster                                                   |
| scimark_lu               | 118 ms                                                 | 112 ms: 1.05x faster                                                    |
| unpickle_list            | 5.29 us                                                | 5.04 us: 1.05x faster                                                   |
| docutils                 | 2.77 sec                                               | 2.64 sec: 1.05x faster                                                  |
| json                     | 5.26 ms                                                | 5.03 ms: 1.04x faster                                                   |
| scimark_sor              | 129 ms                                                 | 124 ms: 1.04x faster                                                    |
| xml_etree_generate       | 89.2 ms                                                | 85.5 ms: 1.04x faster                                                   |
| pprint_safe_repr         | 776 ms                                                 | 744 ms: 1.04x faster                                                    |
| sqlglot_transpile        | 1.68 ms                                                | 1.62 ms: 1.04x faster                                                   |
| pickle_list              | 5.08 us                                                | 4.89 us: 1.04x faster                                                   |
| unpickle                 | 15.9 us                                                | 15.3 us: 1.04x faster                                                   |
| sympy_integrate          | 21.4 ms                                                | 20.7 ms: 1.04x faster                                                   |
| nbody                    | 97.0 ms                                                | 93.6 ms: 1.04x faster                                                   |
| logging_silent           | 104 ns                                                 | 101 ns: 1.03x faster                                                    |
| pprint_pformat           | 1.57 sec                                               | 1.53 sec: 1.03x faster                                                  |
| json_loads               | 28.5 us                                                | 27.8 us: 1.02x faster                                                   |
| float                    | 84.7 ms                                                | 82.8 ms: 1.02x faster                                                   |
| chaos                    | 67.0 ms                                                | 65.5 ms: 1.02x faster                                                   |
| async_tree_memoization   | 578 ms                                                 | 565 ms: 1.02x faster                                                    |
| sqlite_synth             | 2.83 us                                                | 2.78 us: 1.02x faster                                                   |
| dask                     | 372 ms                                                 | 365 ms: 1.02x faster                                                    |
| richards_super           | 51.5 ms                                                | 50.5 ms: 1.02x faster                                                   |
| sqlglot_normalize        | 110 ms                                                 | 108 ms: 1.02x faster                                                    |
| coroutines               | 23.2 ms                                                | 22.7 ms: 1.02x faster                                                   |
| fannkuch                 | 417 ms                                                 | 410 ms: 1.02x faster                                                    |
| pickle                   | 11.6 us                                                | 11.4 us: 1.02x faster                                                   |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 715 ms: 1.02x faster                                                    |
| xml_etree_parse          | 159 ms                                                 | 157 ms: 1.01x faster                                                    |
| dulwich_log              | 68.5 ms                                                | 67.6 ms: 1.01x faster                                                   |
| richards                 | 45.8 ms                                                | 45.3 ms: 1.01x faster                                                   |
| mako                     | 11.9 ms                                                | 11.8 ms: 1.01x faster                                                   |
| sympy_expand             | 478 ms                                                 | 473 ms: 1.01x faster                                                    |
| bench_thread_pool        | 842 us                                                 | 836 us: 1.01x faster                                                    |
| pidigits                 | 187 ms                                                 | 187 ms: 1.00x faster                                                    |
| asyncio_tcp              | 491 ms                                                 | 493 ms: 1.00x slower                                                    |
| sqlglot_optimize         | 54.8 ms                                                | 55.2 ms: 1.01x slower                                                   |
| create_gc_cycles         | 1.48 ms                                                | 1.49 ms: 1.01x slower                                                   |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.80 sec: 1.01x slower                                                  |
| async_tree_io_tg         | 1.18 sec                                               | 1.20 sec: 1.01x slower                                                  |
| gc_traversal             | 3.79 ms                                                | 3.85 ms: 1.01x slower                                                   |
| regex_effbot             | 3.61 ms                                                | 3.68 ms: 1.02x slower                                                   |
| async_tree_io            | 1.16 sec                                               | 1.18 sec: 1.02x slower                                                  |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 5.21 ms: 1.03x slower                                                   |
| nqueens                  | 83.3 ms                                                | 86.0 ms: 1.03x slower                                                   |
| pycparser                | 1.18 sec                                               | 1.22 sec: 1.04x slower                                                  |
| go                       | 139 ms                                                 | 145 ms: 1.04x slower                                                    |
| mdp                      | 2.63 sec                                               | 2.78 sec: 1.06x slower                                                  |
| regex_dna                | 212 ms                                                 | 226 ms: 1.06x slower                                                    |
| python_startup           | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                   |
| regex_v8                 | 23.1 ms                                                | 25.7 ms: 1.11x slower                                                   |
| spectral_norm            | 115 ms                                                 | 130 ms: 1.13x slower                                                    |
| hexiom                   | 6.41 ms                                                | 7.31 ms: 1.14x slower                                                   |
| telco                    | 7.10 ms                                                | 8.29 ms: 1.17x slower                                                   |
| python_startup_no_site   | 6.94 ms                                                | 8.88 ms: 1.28x slower                                                   |
| coverage                 | 72.7 ms                                                | 98.9 ms: 1.36x slower                                                   |
| Geometric mean           | (ref)                                                  | 1.02x faster                                                            |

Benchmark hidden because not significant (12): unpickle_pure_python, xml_etree_iterparse, async_tree_cpu_io_mixed_tg, async_generators, async_tree_none_tg, bench_mp_pool, 2to3, asyncio_websockets, json_dumps, pyflate, async_tree_memoization_tg, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.69% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.96x