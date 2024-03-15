# Results vs. 3.12.0

- fork: python
- ref: f0df35eeca2ccdfd58cf
- machine: linux-x86_64
- commit hash: f0df35e
- commit date: 2024-02-29
- overall geometric mean: 1.01x slower \*
- HPT reliability: 66.15%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.17x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 280 ms: 1.02x slower                                                   |
| chameleon      | 7.41 ms                                                | 6.77 ms: 1.09x faster                                                  |
| docutils       | 2.77 sec                                               | 2.72 sec: 1.02x faster                                                 |
| tornado_http   | 103 ms                                                 | 97.0 ms: 1.06x faster                                                  |
| Geometric mean | (ref)                                                  | 1.04x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 472 ms                                                 | 439 ms: 1.07x faster                                                   |
| async_tree_memoization  | 578 ms                                                 | 566 ms: 1.02x faster                                                   |
| async_tree_cpu_io_mixed | 726 ms                                                 | 712 ms: 1.02x faster                                                   |
| async_tree_none_tg      | 450 ms                                                 | 449 ms: 1.00x faster                                                   |
| async_tree_io_tg        | 1.18 sec                                               | 1.21 sec: 1.02x slower                                                 |
| async_tree_io           | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                 |
| Geometric mean          | (ref)                                                  | 1.01x faster                                                           |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| float          | 84.7 ms                                                | 81.5 ms: 1.04x faster                                                  |
| nbody          | 97.0 ms                                                | 95.0 ms: 1.02x faster                                                  |
| pidigits       | 187 ms                                                 | 188 ms: 1.00x slower                                                   |
| Geometric mean | (ref)                                                  | 1.02x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.63 ms: 1.01x slower                                                  |
| regex_compile  | 148 ms                                                 | 151 ms: 1.02x slower                                                   |
| regex_dna      | 212 ms                                                 | 224 ms: 1.06x slower                                                   |
| regex_v8       | 23.1 ms                                                | 24.7 ms: 1.07x slower                                                  |
| Geometric mean | (ref)                                                  | 1.04x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| unpickle_list        | 5.29 us                                                | 4.94 us: 1.07x faster                                                  |
| tomli_loads          | 2.33 sec                                               | 2.18 sec: 1.07x faster                                                 |
| pickle_pure_python   | 324 us                                                 | 305 us: 1.06x faster                                                   |
| unpickle             | 15.9 us                                                | 15.0 us: 1.06x faster                                                  |
| xml_etree_process    | 61.7 ms                                                | 58.7 ms: 1.05x faster                                                  |
| json_loads           | 28.5 us                                                | 27.3 us: 1.04x faster                                                  |
| xml_etree_generate   | 89.2 ms                                                | 86.2 ms: 1.03x faster                                                  |
| xml_etree_parse      | 159 ms                                                 | 158 ms: 1.01x faster                                                   |
| pickle_dict          | 35.5 us                                                | 35.2 us: 1.01x faster                                                  |
| json_dumps           | 10.4 ms                                                | 10.3 ms: 1.01x faster                                                  |
| xml_etree_iterparse  | 107 ms                                                 | 108 ms: 1.01x slower                                                   |
| pickle_list          | 5.08 us                                                | 5.26 us: 1.03x slower                                                  |
| unpickle_pure_python | 230 us                                                 | 245 us: 1.07x slower                                                   |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                           |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 12.3 ms: 1.29x slower                                                  |
| python_startup_no_site | 6.94 ms                                                | 10.9 ms: 1.57x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.42x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 11.6 ms: 1.03x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 158 us                                                 | 110 us: 1.44x faster                                                   |
| comprehensions           | 21.8 us                                                | 18.0 us: 1.21x faster                                                  |
| logging_format           | 7.23 us                                                | 6.25 us: 1.16x faster                                                  |
| logging_simple           | 6.46 us                                                | 5.71 us: 1.13x faster                                                  |
| deepcopy_reduce          | 3.35 us                                                | 3.05 us: 1.10x faster                                                  |
| chameleon                | 7.41 ms                                                | 6.77 ms: 1.09x faster                                                  |
| crypto_pyaes             | 81.9 ms                                                | 74.9 ms: 1.09x faster                                                  |
| deltablue                | 3.72 ms                                                | 3.43 ms: 1.08x faster                                                  |
| scimark_fft              | 382 ms                                                 | 354 ms: 1.08x faster                                                   |
| async_tree_none          | 472 ms                                                 | 439 ms: 1.07x faster                                                   |
| generators               | 31.2 ms                                                | 29.1 ms: 1.07x faster                                                  |
| unpickle_list            | 5.29 us                                                | 4.94 us: 1.07x faster                                                  |
| tomli_loads              | 2.33 sec                                               | 2.18 sec: 1.07x faster                                                 |
| raytrace                 | 312 ms                                                 | 293 ms: 1.07x faster                                                   |
| pickle_pure_python       | 324 us                                                 | 305 us: 1.06x faster                                                   |
| sympy_sum                | 169 ms                                                 | 160 ms: 1.06x faster                                                   |
| tornado_http             | 103 ms                                                 | 97.0 ms: 1.06x faster                                                  |
| sympy_str                | 300 ms                                                 | 284 ms: 1.06x faster                                                   |
| unpickle                 | 15.9 us                                                | 15.0 us: 1.06x faster                                                  |
| deepcopy                 | 371 us                                                 | 352 us: 1.05x faster                                                   |
| xml_etree_process        | 61.7 ms                                                | 58.7 ms: 1.05x faster                                                  |
| chaos                    | 67.0 ms                                                | 64.0 ms: 1.05x faster                                                  |
| logging_silent           | 104 ns                                                 | 100 ns: 1.04x faster                                                   |
| json_loads               | 28.5 us                                                | 27.3 us: 1.04x faster                                                  |
| pathlib                  | 19.3 ms                                                | 18.6 ms: 1.04x faster                                                  |
| float                    | 84.7 ms                                                | 81.5 ms: 1.04x faster                                                  |
| coroutines               | 23.2 ms                                                | 22.3 ms: 1.04x faster                                                  |
| json                     | 5.26 ms                                                | 5.08 ms: 1.04x faster                                                  |
| deepcopy_memo            | 40.7 us                                                | 39.4 us: 1.03x faster                                                  |
| xml_etree_generate       | 89.2 ms                                                | 86.2 ms: 1.03x faster                                                  |
| sqlglot_parse            | 1.36 ms                                                | 1.32 ms: 1.03x faster                                                  |
| mako                     | 11.9 ms                                                | 11.6 ms: 1.03x faster                                                  |
| sqlglot_normalize        | 110 ms                                                 | 108 ms: 1.02x faster                                                   |
| meteor_contest           | 112 ms                                                 | 110 ms: 1.02x faster                                                   |
| nbody                    | 97.0 ms                                                | 95.0 ms: 1.02x faster                                                  |
| async_tree_memoization   | 578 ms                                                 | 566 ms: 1.02x faster                                                   |
| sympy_integrate          | 21.4 ms                                                | 21.0 ms: 1.02x faster                                                  |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 712 ms: 1.02x faster                                                   |
| docutils                 | 2.77 sec                                               | 2.72 sec: 1.02x faster                                                 |
| sqlglot_transpile        | 1.68 ms                                                | 1.66 ms: 1.02x faster                                                  |
| xml_etree_parse          | 159 ms                                                 | 158 ms: 1.01x faster                                                   |
| pickle_dict              | 35.5 us                                                | 35.2 us: 1.01x faster                                                  |
| asyncio_tcp              | 491 ms                                                 | 487 ms: 1.01x faster                                                   |
| sqlite_synth             | 2.83 us                                                | 2.81 us: 1.01x faster                                                  |
| json_dumps               | 10.4 ms                                                | 10.3 ms: 1.01x faster                                                  |
| gc_traversal             | 3.79 ms                                                | 3.77 ms: 1.01x faster                                                  |
| async_tree_none_tg       | 450 ms                                                 | 449 ms: 1.00x faster                                                   |
| pidigits                 | 187 ms                                                 | 188 ms: 1.00x slower                                                   |
| regex_effbot             | 3.61 ms                                                | 3.63 ms: 1.01x slower                                                  |
| xml_etree_iterparse      | 107 ms                                                 | 108 ms: 1.01x slower                                                   |
| bench_thread_pool        | 842 us                                                 | 850 us: 1.01x slower                                                   |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.80 sec: 1.01x slower                                                 |
| dulwich_log              | 68.5 ms                                                | 69.3 ms: 1.01x slower                                                  |
| sympy_expand             | 478 ms                                                 | 484 ms: 1.01x slower                                                   |
| fannkuch                 | 417 ms                                                 | 423 ms: 1.01x slower                                                   |
| scimark_monte_carlo      | 75.1 ms                                                | 76.2 ms: 1.02x slower                                                  |
| create_gc_cycles         | 1.48 ms                                                | 1.50 ms: 1.02x slower                                                  |
| regex_compile            | 148 ms                                                 | 151 ms: 1.02x slower                                                   |
| 2to3                     | 274 ms                                                 | 280 ms: 1.02x slower                                                   |
| async_tree_io_tg         | 1.18 sec                                               | 1.21 sec: 1.02x slower                                                 |
| pprint_safe_repr         | 776 ms                                                 | 794 ms: 1.02x slower                                                   |
| richards_super           | 51.5 ms                                                | 52.9 ms: 1.03x slower                                                  |
| async_tree_io            | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                 |
| pycparser                | 1.18 sec                                               | 1.22 sec: 1.03x slower                                                 |
| richards                 | 45.8 ms                                                | 47.3 ms: 1.03x slower                                                  |
| pickle_list              | 5.08 us                                                | 5.26 us: 1.03x slower                                                  |
| spectral_norm            | 115 ms                                                 | 119 ms: 1.04x slower                                                   |
| sqlglot_optimize         | 54.8 ms                                                | 56.9 ms: 1.04x slower                                                  |
| mdp                      | 2.63 sec                                               | 2.76 sec: 1.05x slower                                                 |
| regex_dna                | 212 ms                                                 | 224 ms: 1.06x slower                                                   |
| pyflate                  | 482 ms                                                 | 513 ms: 1.06x slower                                                   |
| unpickle_pure_python     | 230 us                                                 | 245 us: 1.07x slower                                                   |
| pprint_pformat           | 1.57 sec                                               | 1.67 sec: 1.07x slower                                                 |
| regex_v8                 | 23.1 ms                                                | 24.7 ms: 1.07x slower                                                  |
| nqueens                  | 83.3 ms                                                | 92.0 ms: 1.11x slower                                                  |
| scimark_lu               | 118 ms                                                 | 133 ms: 1.13x slower                                                   |
| go                       | 139 ms                                                 | 158 ms: 1.13x slower                                                   |
| bench_mp_pool            | 24.0 ms                                                | 28.0 ms: 1.16x slower                                                  |
| hexiom                   | 6.41 ms                                                | 7.53 ms: 1.17x slower                                                  |
| telco                    | 7.10 ms                                                | 8.66 ms: 1.22x slower                                                  |
| python_startup           | 9.55 ms                                                | 12.3 ms: 1.29x slower                                                  |
| coverage                 | 72.7 ms                                                | 96.3 ms: 1.32x slower                                                  |
| python_startup_no_site   | 6.94 ms                                                | 10.9 ms: 1.57x slower                                                  |
| unpack_sequence          | 54.0 ns                                                | 121 ns: 2.25x slower                                                   |
| Geometric mean           | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (8): scimark_sor, scimark_sparse_mat_mult, async_tree_cpu_io_mixed_tg, async_generators, asyncio_websockets, pickle, async_tree_memoization_tg, mypy2
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 66.15% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.17x