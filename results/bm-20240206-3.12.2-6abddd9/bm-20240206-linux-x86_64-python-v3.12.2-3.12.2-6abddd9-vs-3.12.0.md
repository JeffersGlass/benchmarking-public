
# Results vs. 3.12.0

- fork: python
- ref: v3.12.2
- machine: linux-x86_64
- commit hash: 6abddd9
- commit date: 2024-02-06
- overall geometric mean: 1.01x faster \*
- HPT reliability: 99.82%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.96x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-linux-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 272 ms: 1.01x faster                                   |
| chameleon      | 7.41 ms                                                | 7.26 ms: 1.02x faster                                  |
| docutils       | 2.77 sec                                               | 2.71 sec: 1.02x faster                                 |
| tornado_http   | 103 ms                                                 | 99.4 ms: 1.03x faster                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-linux-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|--------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_none_tg | 450 ms                                                 | 446 ms: 1.01x faster                                   |
| async_tree_io      | 1.16 sec                                               | 1.15 sec: 1.00x faster                                 |
| Geometric mean     | (ref)                                                  | 1.00x faster                                           |

Benchmark hidden because not significant (6): async_tree_memoization_tg, async_tree_memoization, async_tree_io_tg, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-linux-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 94.5 ms: 1.03x faster                                  |
| float          | 84.7 ms                                                | 84.1 ms: 1.01x faster                                  |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x faster                                   |
| Geometric mean | (ref)                                                  | 1.01x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-linux-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 144 ms: 1.03x faster                                   |
| regex_v8       | 23.1 ms                                                | 23.0 ms: 1.01x faster                                  |
| regex_dna      | 212 ms                                                 | 214 ms: 1.01x slower                                   |
| regex_effbot   | 3.61 ms                                                | 3.89 ms: 1.08x slower                                  |
| Geometric mean | (ref)                                                  | 1.01x slower                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-linux-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_dict          | 35.5 us                                                | 33.4 us: 1.06x faster                                  |
| pickle_list          | 5.08 us                                                | 4.89 us: 1.04x faster                                  |
| unpickle             | 15.9 us                                                | 15.3 us: 1.03x faster                                  |
| pickle               | 11.6 us                                                | 11.3 us: 1.03x faster                                  |
| pickle_pure_python   | 324 us                                                 | 319 us: 1.01x faster                                   |
| tomli_loads          | 2.33 sec                                               | 2.30 sec: 1.01x faster                                 |
| json_loads           | 28.5 us                                                | 28.1 us: 1.01x faster                                  |
| xml_etree_generate   | 89.2 ms                                                | 88.0 ms: 1.01x faster                                  |
| xml_etree_parse      | 159 ms                                                 | 158 ms: 1.01x faster                                   |
| xml_etree_process    | 61.7 ms                                                | 61.2 ms: 1.01x faster                                  |
| unpickle_pure_python | 230 us                                                 | 228 us: 1.01x faster                                   |
| xml_etree_iterparse  | 107 ms                                                 | 106 ms: 1.01x faster                                   |
| json_dumps           | 10.4 ms                                                | 10.4 ms: 1.01x slower                                  |
| unpickle_list        | 5.29 us                                                | 5.36 us: 1.01x slower                                  |
| Geometric mean       | (ref)                                                  | 1.02x faster                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-linux-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup_no_site | 6.94 ms                                                | 6.80 ms: 1.02x faster                                  |
| python_startup         | 9.55 ms                                                | 9.45 ms: 1.01x faster                                  |
| Geometric mean         | (ref)                                                  | 1.02x faster                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-linux-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako            | 11.9 ms                                                | 11.7 ms: 1.02x faster                                  |
| django_template | 34.6 ms                                                | 34.8 ms: 1.01x slower                                  |
| Geometric mean  | (ref)                                                  | 1.00x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-linux-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| typing_runtime_protocols | 158 us                                                 | 123 us: 1.29x faster                                   |
| mypy2                    | 830 ms                                                 | 692 ms: 1.20x faster                                   |
| unpack_sequence          | 54.0 ns                                                | 47.6 ns: 1.13x faster                                  |
| gc_traversal             | 3.79 ms                                                | 3.54 ms: 1.07x faster                                  |
| pickle_dict              | 35.5 us                                                | 33.4 us: 1.06x faster                                  |
| pickle_list              | 5.08 us                                                | 4.89 us: 1.04x faster                                  |
| sympy_sum                | 169 ms                                                 | 163 ms: 1.04x faster                                   |
| comprehensions           | 21.8 us                                                | 21.0 us: 1.04x faster                                  |
| unpickle                 | 15.9 us                                                | 15.3 us: 1.03x faster                                  |
| deepcopy_reduce          | 3.35 us                                                | 3.24 us: 1.03x faster                                  |
| tornado_http             | 103 ms                                                 | 99.4 ms: 1.03x faster                                  |
| pickle                   | 11.6 us                                                | 11.3 us: 1.03x faster                                  |
| regex_compile            | 148 ms                                                 | 144 ms: 1.03x faster                                   |
| pathlib                  | 19.3 ms                                                | 18.8 ms: 1.03x faster                                  |
| sympy_integrate          | 21.4 ms                                                | 20.8 ms: 1.03x faster                                  |
| nbody                    | 97.0 ms                                                | 94.5 ms: 1.03x faster                                  |
| deepcopy_memo            | 40.7 us                                                | 39.7 us: 1.03x faster                                  |
| async_generators         | 463 ms                                                 | 453 ms: 1.02x faster                                   |
| richards_super           | 51.5 ms                                                | 50.4 ms: 1.02x faster                                  |
| docutils                 | 2.77 sec                                               | 2.71 sec: 1.02x faster                                 |
| chameleon                | 7.41 ms                                                | 7.26 ms: 1.02x faster                                  |
| deepcopy                 | 371 us                                                 | 364 us: 1.02x faster                                   |
| deltablue                | 3.72 ms                                                | 3.64 ms: 1.02x faster                                  |
| python_startup_no_site   | 6.94 ms                                                | 6.80 ms: 1.02x faster                                  |
| sympy_str                | 300 ms                                                 | 294 ms: 1.02x faster                                   |
| scimark_monte_carlo      | 75.1 ms                                                | 73.9 ms: 1.02x faster                                  |
| mako                     | 11.9 ms                                                | 11.7 ms: 1.02x faster                                  |
| logging_format           | 7.23 us                                                | 7.12 us: 1.02x faster                                  |
| raytrace                 | 312 ms                                                 | 308 ms: 1.01x faster                                   |
| pickle_pure_python       | 324 us                                                 | 319 us: 1.01x faster                                   |
| tomli_loads              | 2.33 sec                                               | 2.30 sec: 1.01x faster                                 |
| richards                 | 45.8 ms                                                | 45.2 ms: 1.01x faster                                  |
| pprint_safe_repr         | 776 ms                                                 | 765 ms: 1.01x faster                                   |
| sqlalchemy_imperative    | 18.7 ms                                                | 18.4 ms: 1.01x faster                                  |
| json_loads               | 28.5 us                                                | 28.1 us: 1.01x faster                                  |
| aiohttp                  | 1.15 ms                                                | 1.14 ms: 1.01x faster                                  |
| xml_etree_generate       | 89.2 ms                                                | 88.0 ms: 1.01x faster                                  |
| pyflate                  | 482 ms                                                 | 477 ms: 1.01x faster                                   |
| crypto_pyaes             | 81.9 ms                                                | 80.9 ms: 1.01x faster                                  |
| logging_simple           | 6.46 us                                                | 6.38 us: 1.01x faster                                  |
| xml_etree_parse          | 159 ms                                                 | 158 ms: 1.01x faster                                   |
| create_gc_cycles         | 1.48 ms                                                | 1.46 ms: 1.01x faster                                  |
| python_startup           | 9.55 ms                                                | 9.45 ms: 1.01x faster                                  |
| chaos                    | 67.0 ms                                                | 66.3 ms: 1.01x faster                                  |
| xml_etree_process        | 61.7 ms                                                | 61.2 ms: 1.01x faster                                  |
| dulwich_log              | 68.5 ms                                                | 67.9 ms: 1.01x faster                                  |
| pprint_pformat           | 1.57 sec                                               | 1.56 sec: 1.01x faster                                 |
| float                    | 84.7 ms                                                | 84.1 ms: 1.01x faster                                  |
| async_tree_none_tg       | 450 ms                                                 | 446 ms: 1.01x faster                                   |
| 2to3                     | 274 ms                                                 | 272 ms: 1.01x faster                                   |
| unpickle_pure_python     | 230 us                                                 | 228 us: 1.01x faster                                   |
| regex_v8                 | 23.1 ms                                                | 23.0 ms: 1.01x faster                                  |
| spectral_norm            | 115 ms                                                 | 114 ms: 1.01x faster                                   |
| xml_etree_iterparse      | 107 ms                                                 | 106 ms: 1.01x faster                                   |
| meteor_contest           | 112 ms                                                 | 112 ms: 1.00x faster                                   |
| bench_thread_pool        | 842 us                                                 | 839 us: 1.00x faster                                   |
| async_tree_io            | 1.16 sec                                               | 1.15 sec: 1.00x faster                                 |
| pidigits                 | 187 ms                                                 | 187 ms: 1.00x faster                                   |
| sqlglot_optimize         | 54.8 ms                                                | 55.0 ms: 1.00x slower                                  |
| scimark_fft              | 382 ms                                                 | 383 ms: 1.00x slower                                   |
| hexiom                   | 6.41 ms                                                | 6.44 ms: 1.00x slower                                  |
| nqueens                  | 83.3 ms                                                | 83.7 ms: 1.00x slower                                  |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.80 sec: 1.01x slower                                 |
| logging_silent           | 104 ns                                                 | 105 ns: 1.01x slower                                   |
| json_dumps               | 10.4 ms                                                | 10.4 ms: 1.01x slower                                  |
| django_template          | 34.6 ms                                                | 34.8 ms: 1.01x slower                                  |
| fannkuch                 | 417 ms                                                 | 420 ms: 1.01x slower                                   |
| regex_dna                | 212 ms                                                 | 214 ms: 1.01x slower                                   |
| coverage                 | 72.7 ms                                                | 73.3 ms: 1.01x slower                                  |
| sqlite_synth             | 2.83 us                                                | 2.86 us: 1.01x slower                                  |
| sqlglot_normalize        | 110 ms                                                 | 112 ms: 1.01x slower                                   |
| unpickle_list            | 5.29 us                                                | 5.36 us: 1.01x slower                                  |
| coroutines               | 23.2 ms                                                | 23.5 ms: 1.02x slower                                  |
| go                       | 139 ms                                                 | 142 ms: 1.02x slower                                   |
| scimark_lu               | 118 ms                                                 | 120 ms: 1.02x slower                                   |
| generators               | 31.2 ms                                                | 32.3 ms: 1.03x slower                                  |
| pycparser                | 1.18 sec                                               | 1.22 sec: 1.04x slower                                 |
| asyncio_tcp              | 491 ms                                                 | 509 ms: 1.04x slower                                   |
| mdp                      | 2.63 sec                                               | 2.76 sec: 1.05x slower                                 |
| regex_effbot             | 3.61 ms                                                | 3.89 ms: 1.08x slower                                  |
| Geometric mean           | (ref)                                                  | 1.01x faster                                           |

Benchmark hidden because not significant (18): dask, sqlalchemy_declarative, json, async_tree_memoization_tg, async_tree_memoization, sympy_expand, gunicorn, scimark_sor, asyncio_websockets, async_tree_io_tg, bench_mp_pool, async_tree_cpu_io_mixed_tg, sqlglot_transpile, async_tree_cpu_io_mixed, sqlglot_parse, telco, async_tree_none, scimark_sparse_mat_mult


# HPT report

- Reliability score: 99.82% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.96x