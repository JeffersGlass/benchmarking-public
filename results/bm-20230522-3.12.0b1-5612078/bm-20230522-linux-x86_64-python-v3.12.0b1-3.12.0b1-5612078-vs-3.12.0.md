
# Results vs. 3.12.0

- fork: python
- ref: v3.12.0b1
- machine: linux-x86_64
- commit hash: 5612078
- commit date: 2023-05-22
- overall geometric mean: 1.03x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230522-linux-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 268 ms: 1.02x faster                                       |
| docutils       | 2.77 sec                                               | 2.71 sec: 1.02x faster                                     |
| tornado_http   | 103 ms                                                 | 99.2 ms: 1.03x faster                                      |
| Geometric mean | (ref)                                                  | 1.03x faster                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230522-linux-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| async_tree_cpu_io_mixed | 726 ms                                                 | 708 ms: 1.02x faster                                       |
| async_tree_memoization  | 578 ms                                                 | 572 ms: 1.01x faster                                       |
| async_tree_io           | 1.16 sec                                               | 1.16 sec: 1.01x slower                                     |
| Geometric mean          | (ref)                                                  | 1.01x faster                                               |

Benchmark hidden because not significant (1): async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230522-linux-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 88.9 ms: 1.09x faster                                      |
| float          | 84.7 ms                                                | 80.7 ms: 1.05x faster                                      |
| pidigits       | 187 ms                                                 | 196 ms: 1.05x slower                                       |
| Geometric mean | (ref)                                                  | 1.03x faster                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230522-linux-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| regex_v8       | 23.1 ms                                                | 21.8 ms: 1.06x faster                                      |
| regex_compile  | 148 ms                                                 | 144 ms: 1.03x faster                                       |
| regex_effbot   | 3.61 ms                                                | 3.54 ms: 1.02x faster                                      |
| regex_dna      | 212 ms                                                 | 208 ms: 1.02x faster                                       |
| Geometric mean | (ref)                                                  | 1.03x faster                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230522-linux-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| json_loads           | 28.5 us                                                | 25.1 us: 1.14x faster                                      |
| pickle               | 11.6 us                                                | 10.6 us: 1.10x faster                                      |
| pickle_list          | 5.08 us                                                | 4.73 us: 1.07x faster                                      |
| pickle_dict          | 35.5 us                                                | 33.3 us: 1.07x faster                                      |
| tomli_loads          | 2.33 sec                                               | 2.18 sec: 1.07x faster                                     |
| unpickle_pure_python | 230 us                                                 | 216 us: 1.07x faster                                       |
| unpickle             | 15.9 us                                                | 14.9 us: 1.06x faster                                      |
| json_dumps           | 10.4 ms                                                | 9.76 ms: 1.06x faster                                      |
| xml_etree_process    | 61.7 ms                                                | 59.0 ms: 1.05x faster                                      |
| xml_etree_parse      | 159 ms                                                 | 153 ms: 1.04x faster                                       |
| xml_etree_generate   | 89.2 ms                                                | 85.6 ms: 1.04x faster                                      |
| pickle_pure_python   | 324 us                                                 | 312 us: 1.04x faster                                       |
| xml_etree_iterparse  | 107 ms                                                 | 103 ms: 1.03x faster                                       |
| unpickle_list        | 5.29 us                                                | 5.17 us: 1.02x faster                                      |
| Geometric mean       | (ref)                                                  | 1.06x faster                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230522-linux-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 9.34 ms: 1.02x faster                                      |
| python_startup_no_site | 6.94 ms                                                | 6.78 ms: 1.02x faster                                      |
| Geometric mean         | (ref)                                                  | 1.02x faster                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230522-linux-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------:|
| mako      | 11.9 ms                                                | 10.8 ms: 1.10x faster                                      |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230522-linux-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| unpack_sequence          | 54.0 ns                                                | 47.3 ns: 1.14x faster                                      |
| json_loads               | 28.5 us                                                | 25.1 us: 1.14x faster                                      |
| typing_runtime_protocols | 158 us                                                 | 140 us: 1.13x faster                                       |
| json                     | 5.26 ms                                                | 4.77 ms: 1.10x faster                                      |
| pickle                   | 11.6 us                                                | 10.6 us: 1.10x faster                                      |
| mako                     | 11.9 ms                                                | 10.8 ms: 1.10x faster                                      |
| fannkuch                 | 417 ms                                                 | 382 ms: 1.09x faster                                       |
| nbody                    | 97.0 ms                                                | 88.9 ms: 1.09x faster                                      |
| pyflate                  | 482 ms                                                 | 443 ms: 1.09x faster                                       |
| deepcopy_memo            | 40.7 us                                                | 37.6 us: 1.08x faster                                      |
| deltablue                | 3.72 ms                                                | 3.44 ms: 1.08x faster                                      |
| pickle_list              | 5.08 us                                                | 4.73 us: 1.07x faster                                      |
| scimark_fft              | 382 ms                                                 | 356 ms: 1.07x faster                                       |
| pickle_dict              | 35.5 us                                                | 33.3 us: 1.07x faster                                      |
| tomli_loads              | 2.33 sec                                               | 2.18 sec: 1.07x faster                                     |
| meteor_contest           | 112 ms                                                 | 105 ms: 1.07x faster                                       |
| unpickle_pure_python     | 230 us                                                 | 216 us: 1.07x faster                                       |
| unpickle                 | 15.9 us                                                | 14.9 us: 1.06x faster                                      |
| json_dumps               | 10.4 ms                                                | 9.76 ms: 1.06x faster                                      |
| spectral_norm            | 115 ms                                                 | 108 ms: 1.06x faster                                       |
| comprehensions           | 21.8 us                                                | 20.6 us: 1.06x faster                                      |
| regex_v8                 | 23.1 ms                                                | 21.8 ms: 1.06x faster                                      |
| coroutines               | 23.2 ms                                                | 21.9 ms: 1.06x faster                                      |
| pprint_safe_repr         | 776 ms                                                 | 733 ms: 1.06x faster                                       |
| pathlib                  | 19.3 ms                                                | 18.3 ms: 1.06x faster                                      |
| richards                 | 45.8 ms                                                | 43.6 ms: 1.05x faster                                      |
| deepcopy_reduce          | 3.35 us                                                | 3.18 us: 1.05x faster                                      |
| crypto_pyaes             | 81.9 ms                                                | 77.9 ms: 1.05x faster                                      |
| scimark_sor              | 129 ms                                                 | 123 ms: 1.05x faster                                       |
| float                    | 84.7 ms                                                | 80.7 ms: 1.05x faster                                      |
| pprint_pformat           | 1.57 sec                                               | 1.50 sec: 1.05x faster                                     |
| hexiom                   | 6.41 ms                                                | 6.12 ms: 1.05x faster                                      |
| raytrace                 | 312 ms                                                 | 298 ms: 1.05x faster                                       |
| xml_etree_process        | 61.7 ms                                                | 59.0 ms: 1.05x faster                                      |
| xml_etree_parse          | 159 ms                                                 | 153 ms: 1.04x faster                                       |
| scimark_lu               | 118 ms                                                 | 113 ms: 1.04x faster                                       |
| logging_silent           | 104 ns                                                 | 100 ns: 1.04x faster                                       |
| xml_etree_generate       | 89.2 ms                                                | 85.6 ms: 1.04x faster                                      |
| sqlite_synth             | 2.83 us                                                | 2.72 us: 1.04x faster                                      |
| pickle_pure_python       | 324 us                                                 | 312 us: 1.04x faster                                       |
| telco                    | 7.10 ms                                                | 6.84 ms: 1.04x faster                                      |
| chaos                    | 67.0 ms                                                | 64.6 ms: 1.04x faster                                      |
| richards_super           | 51.5 ms                                                | 49.8 ms: 1.04x faster                                      |
| tornado_http             | 103 ms                                                 | 99.2 ms: 1.03x faster                                      |
| xml_etree_iterparse      | 107 ms                                                 | 103 ms: 1.03x faster                                       |
| gc_traversal             | 3.79 ms                                                | 3.67 ms: 1.03x faster                                      |
| regex_compile            | 148 ms                                                 | 144 ms: 1.03x faster                                       |
| scimark_monte_carlo      | 75.1 ms                                                | 72.7 ms: 1.03x faster                                      |
| async_generators         | 463 ms                                                 | 449 ms: 1.03x faster                                       |
| deepcopy                 | 371 us                                                 | 361 us: 1.03x faster                                       |
| go                       | 139 ms                                                 | 136 ms: 1.03x faster                                       |
| sqlglot_transpile        | 1.68 ms                                                | 1.64 ms: 1.03x faster                                      |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 708 ms: 1.02x faster                                       |
| sqlglot_parse            | 1.36 ms                                                | 1.33 ms: 1.02x faster                                      |
| 2to3                     | 274 ms                                                 | 268 ms: 1.02x faster                                       |
| unpickle_list            | 5.29 us                                                | 5.17 us: 1.02x faster                                      |
| nqueens                  | 83.3 ms                                                | 81.4 ms: 1.02x faster                                      |
| python_startup           | 9.55 ms                                                | 9.34 ms: 1.02x faster                                      |
| python_startup_no_site   | 6.94 ms                                                | 6.78 ms: 1.02x faster                                      |
| docutils                 | 2.77 sec                                               | 2.71 sec: 1.02x faster                                     |
| regex_effbot             | 3.61 ms                                                | 3.54 ms: 1.02x faster                                      |
| logging_simple           | 6.46 us                                                | 6.33 us: 1.02x faster                                      |
| logging_format           | 7.23 us                                                | 7.09 us: 1.02x faster                                      |
| regex_dna                | 212 ms                                                 | 208 ms: 1.02x faster                                       |
| bench_thread_pool        | 842 us                                                 | 827 us: 1.02x faster                                       |
| sqlglot_normalize        | 110 ms                                                 | 109 ms: 1.02x faster                                       |
| sqlglot_optimize         | 54.8 ms                                                | 54.1 ms: 1.01x faster                                      |
| sqlalchemy_declarative   | 147 ms                                                 | 145 ms: 1.01x faster                                       |
| dulwich_log              | 68.5 ms                                                | 67.7 ms: 1.01x faster                                      |
| async_tree_memoization   | 578 ms                                                 | 572 ms: 1.01x faster                                       |
| async_tree_io            | 1.16 sec                                               | 1.16 sec: 1.01x slower                                     |
| generators               | 31.2 ms                                                | 31.4 ms: 1.01x slower                                      |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.80 sec: 1.01x slower                                     |
| pycparser                | 1.18 sec                                               | 1.19 sec: 1.01x slower                                     |
| create_gc_cycles         | 1.48 ms                                                | 1.50 ms: 1.01x slower                                      |
| mdp                      | 2.63 sec                                               | 2.68 sec: 1.02x slower                                     |
| asyncio_tcp              | 491 ms                                                 | 513 ms: 1.04x slower                                       |
| pidigits                 | 187 ms                                                 | 196 ms: 1.05x slower                                       |
| coverage                 | 72.7 ms                                                | 96.8 ms: 1.33x slower                                      |
| dask                     | 372 ms                                                 | 535 ms: 1.44x slower                                       |
| Geometric mean           | (ref)                                                  | 1.03x faster                                               |

Benchmark hidden because not significant (4): sqlalchemy_imperative, async_tree_none, scimark_sparse_mat_mult, bench_mp_pool
Ignored benchmarks (14) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, chameleon, django_template, gunicorn, mypy2, sympy_expand, sympy_integrate, sympy_str, sympy_sum


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 1.01x