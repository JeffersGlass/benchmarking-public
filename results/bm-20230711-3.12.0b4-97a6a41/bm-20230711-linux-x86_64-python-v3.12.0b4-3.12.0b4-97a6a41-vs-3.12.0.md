
# Results vs. 3.12.0

- fork: python
- ref: v3.12.0b4
- machine: linux-x86_64
- commit hash: 97a6a41
- commit date: 2023-07-11
- overall geometric mean: 1.03x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230711-linux-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 267 ms: 1.03x faster                                       |
| docutils       | 2.77 sec                                               | 2.70 sec: 1.02x faster                                     |
| tornado_http   | 103 ms                                                 | 99.1 ms: 1.04x faster                                      |
| Geometric mean | (ref)                                                  | 1.03x faster                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230711-linux-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| async_tree_cpu_io_mixed | 726 ms                                                 | 715 ms: 1.02x faster                                       |
| async_tree_memoization  | 578 ms                                                 | 573 ms: 1.01x faster                                       |
| async_tree_io           | 1.16 sec                                               | 1.16 sec: 1.00x slower                                     |
| Geometric mean          | (ref)                                                  | 1.01x faster                                               |

Benchmark hidden because not significant (1): async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230711-linux-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 89.2 ms: 1.09x faster                                      |
| float          | 84.7 ms                                                | 80.7 ms: 1.05x faster                                      |
| pidigits       | 187 ms                                                 | 192 ms: 1.02x slower                                       |
| Geometric mean | (ref)                                                  | 1.04x faster                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230711-linux-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 142 ms: 1.04x faster                                       |
| regex_dna      | 212 ms                                                 | 207 ms: 1.03x faster                                       |
| regex_effbot   | 3.61 ms                                                | 3.57 ms: 1.01x faster                                      |
| regex_v8       | 23.1 ms                                                | 23.0 ms: 1.01x faster                                      |
| Geometric mean | (ref)                                                  | 1.02x faster                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230711-linux-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| pickle_dict          | 35.5 us                                                | 31.6 us: 1.13x faster                                      |
| json_loads           | 28.5 us                                                | 25.7 us: 1.11x faster                                      |
| pickle_list          | 5.08 us                                                | 4.59 us: 1.11x faster                                      |
| pickle               | 11.6 us                                                | 10.6 us: 1.09x faster                                      |
| json_dumps           | 10.4 ms                                                | 9.66 ms: 1.07x faster                                      |
| unpickle_list        | 5.29 us                                                | 4.95 us: 1.07x faster                                      |
| unpickle_pure_python | 230 us                                                 | 217 us: 1.06x faster                                       |
| pickle_pure_python   | 324 us                                                 | 306 us: 1.06x faster                                       |
| unpickle             | 15.9 us                                                | 15.1 us: 1.05x faster                                      |
| xml_etree_generate   | 89.2 ms                                                | 85.0 ms: 1.05x faster                                      |
| xml_etree_parse      | 159 ms                                                 | 152 ms: 1.05x faster                                       |
| tomli_loads          | 2.33 sec                                               | 2.23 sec: 1.05x faster                                     |
| xml_etree_iterparse  | 107 ms                                                 | 102 ms: 1.05x faster                                       |
| xml_etree_process    | 61.7 ms                                                | 59.4 ms: 1.04x faster                                      |
| Geometric mean       | (ref)                                                  | 1.07x faster                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230711-linux-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| python_startup_no_site | 6.94 ms                                                | 6.79 ms: 1.02x faster                                      |
| python_startup         | 9.55 ms                                                | 9.35 ms: 1.02x faster                                      |
| Geometric mean         | (ref)                                                  | 1.02x faster                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230711-linux-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------:|
| mako      | 11.9 ms                                                | 10.9 ms: 1.09x faster                                      |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230711-linux-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| spectral_norm            | 115 ms                                                 | 102 ms: 1.13x faster                                       |
| pickle_dict              | 35.5 us                                                | 31.6 us: 1.13x faster                                      |
| pyflate                  | 482 ms                                                 | 434 ms: 1.11x faster                                       |
| json_loads               | 28.5 us                                                | 25.7 us: 1.11x faster                                      |
| pickle_list              | 5.08 us                                                | 4.59 us: 1.11x faster                                      |
| unpack_sequence          | 54.0 ns                                                | 48.9 ns: 1.10x faster                                      |
| mako                     | 11.9 ms                                                | 10.9 ms: 1.09x faster                                      |
| pickle                   | 11.6 us                                                | 10.6 us: 1.09x faster                                      |
| typing_runtime_protocols | 158 us                                                 | 145 us: 1.09x faster                                       |
| nbody                    | 97.0 ms                                                | 89.2 ms: 1.09x faster                                      |
| scimark_sor              | 129 ms                                                 | 119 ms: 1.08x faster                                       |
| fannkuch                 | 417 ms                                                 | 385 ms: 1.08x faster                                       |
| deepcopy_reduce          | 3.35 us                                                | 3.11 us: 1.08x faster                                      |
| meteor_contest           | 112 ms                                                 | 104 ms: 1.08x faster                                       |
| json_dumps               | 10.4 ms                                                | 9.66 ms: 1.07x faster                                      |
| deepcopy_memo            | 40.7 us                                                | 37.9 us: 1.07x faster                                      |
| unpickle_list            | 5.29 us                                                | 4.95 us: 1.07x faster                                      |
| chaos                    | 67.0 ms                                                | 62.7 ms: 1.07x faster                                      |
| logging_silent           | 104 ns                                                 | 97.8 ns: 1.07x faster                                      |
| scimark_fft              | 382 ms                                                 | 358 ms: 1.07x faster                                       |
| raytrace                 | 312 ms                                                 | 293 ms: 1.06x faster                                       |
| deltablue                | 3.72 ms                                                | 3.49 ms: 1.06x faster                                      |
| json                     | 5.26 ms                                                | 4.95 ms: 1.06x faster                                      |
| unpickle_pure_python     | 230 us                                                 | 217 us: 1.06x faster                                       |
| pprint_safe_repr         | 776 ms                                                 | 731 ms: 1.06x faster                                       |
| crypto_pyaes             | 81.9 ms                                                | 77.2 ms: 1.06x faster                                      |
| hexiom                   | 6.41 ms                                                | 6.05 ms: 1.06x faster                                      |
| pickle_pure_python       | 324 us                                                 | 306 us: 1.06x faster                                       |
| richards                 | 45.8 ms                                                | 43.3 ms: 1.06x faster                                      |
| comprehensions           | 21.8 us                                                | 20.7 us: 1.05x faster                                      |
| pprint_pformat           | 1.57 sec                                               | 1.49 sec: 1.05x faster                                     |
| unpickle                 | 15.9 us                                                | 15.1 us: 1.05x faster                                      |
| scimark_lu               | 118 ms                                                 | 112 ms: 1.05x faster                                       |
| float                    | 84.7 ms                                                | 80.7 ms: 1.05x faster                                      |
| xml_etree_generate       | 89.2 ms                                                | 85.0 ms: 1.05x faster                                      |
| richards_super           | 51.5 ms                                                | 49.2 ms: 1.05x faster                                      |
| xml_etree_parse          | 159 ms                                                 | 152 ms: 1.05x faster                                       |
| tomli_loads              | 2.33 sec                                               | 2.23 sec: 1.05x faster                                     |
| xml_etree_iterparse      | 107 ms                                                 | 102 ms: 1.05x faster                                       |
| deepcopy                 | 371 us                                                 | 355 us: 1.05x faster                                       |
| regex_compile            | 148 ms                                                 | 142 ms: 1.04x faster                                       |
| logging_format           | 7.23 us                                                | 6.93 us: 1.04x faster                                      |
| logging_simple           | 6.46 us                                                | 6.21 us: 1.04x faster                                      |
| telco                    | 7.10 ms                                                | 6.83 ms: 1.04x faster                                      |
| xml_etree_process        | 61.7 ms                                                | 59.4 ms: 1.04x faster                                      |
| scimark_monte_carlo      | 75.1 ms                                                | 72.4 ms: 1.04x faster                                      |
| sqlite_synth             | 2.83 us                                                | 2.74 us: 1.04x faster                                      |
| tornado_http             | 103 ms                                                 | 99.1 ms: 1.04x faster                                      |
| async_generators         | 463 ms                                                 | 448 ms: 1.03x faster                                       |
| go                       | 139 ms                                                 | 135 ms: 1.03x faster                                       |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 4.91 ms: 1.03x faster                                      |
| coroutines               | 23.2 ms                                                | 22.5 ms: 1.03x faster                                      |
| pathlib                  | 19.3 ms                                                | 18.8 ms: 1.03x faster                                      |
| nqueens                  | 83.3 ms                                                | 80.9 ms: 1.03x faster                                      |
| sqlglot_parse            | 1.36 ms                                                | 1.33 ms: 1.03x faster                                      |
| 2to3                     | 274 ms                                                 | 267 ms: 1.03x faster                                       |
| regex_dna                | 212 ms                                                 | 207 ms: 1.03x faster                                       |
| sqlglot_transpile        | 1.68 ms                                                | 1.64 ms: 1.02x faster                                      |
| docutils                 | 2.77 sec                                               | 2.70 sec: 1.02x faster                                     |
| python_startup_no_site   | 6.94 ms                                                | 6.79 ms: 1.02x faster                                      |
| generators               | 31.2 ms                                                | 30.5 ms: 1.02x faster                                      |
| python_startup           | 9.55 ms                                                | 9.35 ms: 1.02x faster                                      |
| sqlalchemy_declarative   | 147 ms                                                 | 144 ms: 1.02x faster                                       |
| bench_thread_pool        | 842 us                                                 | 827 us: 1.02x faster                                       |
| sqlglot_optimize         | 54.8 ms                                                | 53.9 ms: 1.02x faster                                      |
| sqlglot_normalize        | 110 ms                                                 | 109 ms: 1.02x faster                                       |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 715 ms: 1.02x faster                                       |
| regex_effbot             | 3.61 ms                                                | 3.57 ms: 1.01x faster                                      |
| pycparser                | 1.18 sec                                               | 1.17 sec: 1.01x faster                                     |
| async_tree_memoization   | 578 ms                                                 | 573 ms: 1.01x faster                                       |
| dulwich_log              | 68.5 ms                                                | 67.9 ms: 1.01x faster                                      |
| regex_v8                 | 23.1 ms                                                | 23.0 ms: 1.01x faster                                      |
| async_tree_io            | 1.16 sec                                               | 1.16 sec: 1.00x slower                                     |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.80 sec: 1.01x slower                                     |
| pidigits                 | 187 ms                                                 | 192 ms: 1.02x slower                                       |
| create_gc_cycles         | 1.48 ms                                                | 1.51 ms: 1.03x slower                                      |
| gc_traversal             | 3.79 ms                                                | 3.91 ms: 1.03x slower                                      |
| mdp                      | 2.63 sec                                               | 2.73 sec: 1.04x slower                                     |
| asyncio_tcp              | 491 ms                                                 | 517 ms: 1.05x slower                                       |
| coverage                 | 72.7 ms                                                | 93.5 ms: 1.29x slower                                      |
| dask                     | 372 ms                                                 | 535 ms: 1.44x slower                                       |
| Geometric mean           | (ref)                                                  | 1.03x faster                                               |

Benchmark hidden because not significant (3): sqlalchemy_imperative, bench_mp_pool, async_tree_none
Ignored benchmarks (14) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, chameleon, django_template, gunicorn, mypy2, sympy_expand, sympy_integrate, sympy_str, sympy_sum


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 1.02x