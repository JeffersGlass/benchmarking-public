
# Results vs. 3.12.0

- fork: python
- ref: v3.12.0b2
- machine: linux-x86_64
- commit hash: e6c0efa
- commit date: 2023-06-06
- overall geometric mean: 1.03x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-linux-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 269 ms: 1.02x faster                                       |
| docutils       | 2.77 sec                                               | 2.72 sec: 1.02x faster                                     |
| tornado_http   | 103 ms                                                 | 99.3 ms: 1.03x faster                                      |
| Geometric mean | (ref)                                                  | 1.02x faster                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-linux-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| async_tree_cpu_io_mixed | 726 ms                                                 | 708 ms: 1.03x faster                                       |
| async_tree_memoization  | 578 ms                                                 | 570 ms: 1.01x faster                                       |
| async_tree_none         | 472 ms                                                 | 468 ms: 1.01x faster                                       |
| Geometric mean          | (ref)                                                  | 1.01x faster                                               |

Benchmark hidden because not significant (1): async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-linux-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 89.7 ms: 1.08x faster                                      |
| float          | 84.7 ms                                                | 80.3 ms: 1.05x faster                                      |
| pidigits       | 187 ms                                                 | 197 ms: 1.05x slower                                       |
| Geometric mean | (ref)                                                  | 1.03x faster                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-linux-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| regex_dna      | 212 ms                                                 | 202 ms: 1.05x faster                                       |
| regex_compile  | 148 ms                                                 | 145 ms: 1.03x faster                                       |
| regex_v8       | 23.1 ms                                                | 22.9 ms: 1.01x faster                                      |
| regex_effbot   | 3.61 ms                                                | 3.83 ms: 1.06x slower                                      |
| Geometric mean | (ref)                                                  | 1.01x faster                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-linux-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| json_loads           | 28.5 us                                                | 25.1 us: 1.13x faster                                      |
| pickle_dict          | 35.5 us                                                | 31.3 us: 1.13x faster                                      |
| unpickle_list        | 5.29 us                                                | 4.90 us: 1.08x faster                                      |
| json_dumps           | 10.4 ms                                                | 9.69 ms: 1.07x faster                                      |
| pickle_list          | 5.08 us                                                | 4.75 us: 1.07x faster                                      |
| pickle               | 11.6 us                                                | 10.9 us: 1.06x faster                                      |
| unpickle_pure_python | 230 us                                                 | 217 us: 1.06x faster                                       |
| unpickle             | 15.9 us                                                | 15.0 us: 1.06x faster                                      |
| xml_etree_process    | 61.7 ms                                                | 59.1 ms: 1.05x faster                                      |
| xml_etree_generate   | 89.2 ms                                                | 85.6 ms: 1.04x faster                                      |
| tomli_loads          | 2.33 sec                                               | 2.24 sec: 1.04x faster                                     |
| pickle_pure_python   | 324 us                                                 | 314 us: 1.03x faster                                       |
| xml_etree_iterparse  | 107 ms                                                 | 104 ms: 1.02x faster                                       |
| xml_etree_parse      | 159 ms                                                 | 156 ms: 1.02x faster                                       |
| Geometric mean       | (ref)                                                  | 1.06x faster                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-linux-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 9.30 ms: 1.03x faster                                      |
| python_startup_no_site | 6.94 ms                                                | 6.76 ms: 1.03x faster                                      |
| Geometric mean         | (ref)                                                  | 1.03x faster                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-linux-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------:|
| mako      | 11.9 ms                                                | 10.6 ms: 1.12x faster                                      |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-linux-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| unpack_sequence          | 54.0 ns                                                | 46.7 ns: 1.16x faster                                      |
| json_loads               | 28.5 us                                                | 25.1 us: 1.13x faster                                      |
| pickle_dict              | 35.5 us                                                | 31.3 us: 1.13x faster                                      |
| mako                     | 11.9 ms                                                | 10.6 ms: 1.12x faster                                      |
| json                     | 5.26 ms                                                | 4.76 ms: 1.10x faster                                      |
| spectral_norm            | 115 ms                                                 | 104 ms: 1.10x faster                                       |
| nbody                    | 97.0 ms                                                | 89.7 ms: 1.08x faster                                      |
| unpickle_list            | 5.29 us                                                | 4.90 us: 1.08x faster                                      |
| pyflate                  | 482 ms                                                 | 448 ms: 1.08x faster                                       |
| deltablue                | 3.72 ms                                                | 3.46 ms: 1.07x faster                                      |
| scimark_sor              | 129 ms                                                 | 120 ms: 1.07x faster                                       |
| json_dumps               | 10.4 ms                                                | 9.69 ms: 1.07x faster                                      |
| pickle_list              | 5.08 us                                                | 4.75 us: 1.07x faster                                      |
| deepcopy_memo            | 40.7 us                                                | 38.1 us: 1.07x faster                                      |
| typing_runtime_protocols | 158 us                                                 | 148 us: 1.07x faster                                       |
| scimark_fft              | 382 ms                                                 | 358 ms: 1.07x faster                                       |
| richards                 | 45.8 ms                                                | 43.1 ms: 1.06x faster                                      |
| pickle                   | 11.6 us                                                | 10.9 us: 1.06x faster                                      |
| unpickle_pure_python     | 230 us                                                 | 217 us: 1.06x faster                                       |
| meteor_contest           | 112 ms                                                 | 106 ms: 1.06x faster                                       |
| unpickle                 | 15.9 us                                                | 15.0 us: 1.06x faster                                      |
| raytrace                 | 312 ms                                                 | 296 ms: 1.06x faster                                       |
| pprint_safe_repr         | 776 ms                                                 | 735 ms: 1.06x faster                                       |
| float                    | 84.7 ms                                                | 80.3 ms: 1.05x faster                                      |
| richards_super           | 51.5 ms                                                | 48.9 ms: 1.05x faster                                      |
| chaos                    | 67.0 ms                                                | 63.6 ms: 1.05x faster                                      |
| scimark_monte_carlo      | 75.1 ms                                                | 71.3 ms: 1.05x faster                                      |
| coroutines               | 23.2 ms                                                | 22.1 ms: 1.05x faster                                      |
| crypto_pyaes             | 81.9 ms                                                | 78.0 ms: 1.05x faster                                      |
| deepcopy_reduce          | 3.35 us                                                | 3.19 us: 1.05x faster                                      |
| regex_dna                | 212 ms                                                 | 202 ms: 1.05x faster                                       |
| fannkuch                 | 417 ms                                                 | 398 ms: 1.05x faster                                       |
| xml_etree_process        | 61.7 ms                                                | 59.1 ms: 1.05x faster                                      |
| scimark_lu               | 118 ms                                                 | 113 ms: 1.04x faster                                       |
| comprehensions           | 21.8 us                                                | 20.9 us: 1.04x faster                                      |
| xml_etree_generate       | 89.2 ms                                                | 85.6 ms: 1.04x faster                                      |
| tomli_loads              | 2.33 sec                                               | 2.24 sec: 1.04x faster                                     |
| pprint_pformat           | 1.57 sec                                               | 1.51 sec: 1.04x faster                                     |
| logging_format           | 7.23 us                                                | 6.96 us: 1.04x faster                                      |
| sqlite_synth             | 2.83 us                                                | 2.73 us: 1.04x faster                                      |
| telco                    | 7.10 ms                                                | 6.83 ms: 1.04x faster                                      |
| hexiom                   | 6.41 ms                                                | 6.19 ms: 1.04x faster                                      |
| logging_simple           | 6.46 us                                                | 6.24 us: 1.04x faster                                      |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 4.89 ms: 1.03x faster                                      |
| tornado_http             | 103 ms                                                 | 99.3 ms: 1.03x faster                                      |
| deepcopy                 | 371 us                                                 | 359 us: 1.03x faster                                       |
| mdp                      | 2.63 sec                                               | 2.55 sec: 1.03x faster                                     |
| pickle_pure_python       | 324 us                                                 | 314 us: 1.03x faster                                       |
| async_generators         | 463 ms                                                 | 450 ms: 1.03x faster                                       |
| pathlib                  | 19.3 ms                                                | 18.8 ms: 1.03x faster                                      |
| go                       | 139 ms                                                 | 136 ms: 1.03x faster                                       |
| python_startup           | 9.55 ms                                                | 9.30 ms: 1.03x faster                                      |
| regex_compile            | 148 ms                                                 | 145 ms: 1.03x faster                                       |
| python_startup_no_site   | 6.94 ms                                                | 6.76 ms: 1.03x faster                                      |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 708 ms: 1.03x faster                                       |
| xml_etree_iterparse      | 107 ms                                                 | 104 ms: 1.02x faster                                       |
| 2to3                     | 274 ms                                                 | 269 ms: 1.02x faster                                       |
| xml_etree_parse          | 159 ms                                                 | 156 ms: 1.02x faster                                       |
| logging_silent           | 104 ns                                                 | 103 ns: 1.02x faster                                       |
| docutils                 | 2.77 sec                                               | 2.72 sec: 1.02x faster                                     |
| bench_thread_pool        | 842 us                                                 | 829 us: 1.02x faster                                       |
| sqlglot_normalize        | 110 ms                                                 | 109 ms: 1.01x faster                                       |
| async_tree_memoization   | 578 ms                                                 | 570 ms: 1.01x faster                                       |
| sqlalchemy_declarative   | 147 ms                                                 | 145 ms: 1.01x faster                                       |
| sqlglot_optimize         | 54.8 ms                                                | 54.2 ms: 1.01x faster                                      |
| sqlglot_parse            | 1.36 ms                                                | 1.35 ms: 1.01x faster                                      |
| regex_v8                 | 23.1 ms                                                | 22.9 ms: 1.01x faster                                      |
| async_tree_none          | 472 ms                                                 | 468 ms: 1.01x faster                                       |
| nqueens                  | 83.3 ms                                                | 82.6 ms: 1.01x faster                                      |
| sqlglot_transpile        | 1.68 ms                                                | 1.67 ms: 1.01x faster                                      |
| pycparser                | 1.18 sec                                               | 1.17 sec: 1.01x faster                                     |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.80 sec: 1.01x slower                                     |
| generators               | 31.2 ms                                                | 31.6 ms: 1.01x slower                                      |
| create_gc_cycles         | 1.48 ms                                                | 1.52 ms: 1.03x slower                                      |
| asyncio_tcp              | 491 ms                                                 | 511 ms: 1.04x slower                                       |
| pidigits                 | 187 ms                                                 | 197 ms: 1.05x slower                                       |
| regex_effbot             | 3.61 ms                                                | 3.83 ms: 1.06x slower                                      |
| gc_traversal             | 3.79 ms                                                | 4.25 ms: 1.12x slower                                      |
| coverage                 | 72.7 ms                                                | 93.8 ms: 1.29x slower                                      |
| dask                     | 372 ms                                                 | 536 ms: 1.44x slower                                       |
| Geometric mean           | (ref)                                                  | 1.03x faster                                               |

Benchmark hidden because not significant (4): dulwich_log, bench_mp_pool, async_tree_io, sqlalchemy_imperative
Ignored benchmarks (14) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, chameleon, django_template, gunicorn, mypy2, sympy_expand, sympy_integrate, sympy_str, sympy_sum


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 1.01x