
# Results vs. 3.12.0

- fork: python
- ref: v3.12.1
- machine: linux-x86_64
- commit hash: 2305ca5
- commit date: 2023-12-07
- overall geometric mean: 1.01x faster
- HPT reliability: 99.10%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.96x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 274 ms: 1.00x faster                                   |
| chameleon      | 7.41 ms                                                | 7.24 ms: 1.02x faster                                  |
| docutils       | 2.77 sec                                               | 2.71 sec: 1.02x faster                                 |
| tornado_http   | 103 ms                                                 | 99.4 ms: 1.03x faster                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|---------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_none_tg        | 450 ms                                                 | 452 ms: 1.01x slower                                   |
| async_tree_none           | 472 ms                                                 | 475 ms: 1.01x slower                                   |
| async_tree_io             | 1.16 sec                                               | 1.17 sec: 1.01x slower                                 |
| async_tree_io_tg          | 1.18 sec                                               | 1.20 sec: 1.01x slower                                 |
| async_tree_memoization_tg | 575 ms                                                 | 583 ms: 1.01x slower                                   |
| Geometric mean            | (ref)                                                  | 1.01x slower                                           |

Benchmark hidden because not significant (3): async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 93.2 ms: 1.04x faster                                  |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x slower                                   |
| Geometric mean | (ref)                                                  | 1.01x faster                                           |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_dna      | 212 ms                                                 | 205 ms: 1.03x faster                                   |
| regex_compile  | 148 ms                                                 | 145 ms: 1.02x faster                                   |
| regex_v8       | 23.1 ms                                                | 22.8 ms: 1.01x faster                                  |
| regex_effbot   | 3.61 ms                                                | 3.58 ms: 1.01x faster                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|---------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_dict         | 35.5 us                                                | 33.1 us: 1.07x faster                                  |
| unpickle_list       | 5.29 us                                                | 4.99 us: 1.06x faster                                  |
| pickle_list         | 5.08 us                                                | 4.93 us: 1.03x faster                                  |
| tomli_loads         | 2.33 sec                                               | 2.29 sec: 1.02x faster                                 |
| json_loads          | 28.5 us                                                | 28.0 us: 1.02x faster                                  |
| pickle              | 11.6 us                                                | 11.4 us: 1.02x faster                                  |
| unpickle            | 15.9 us                                                | 15.7 us: 1.01x faster                                  |
| xml_etree_generate  | 89.2 ms                                                | 88.2 ms: 1.01x faster                                  |
| xml_etree_process   | 61.7 ms                                                | 61.2 ms: 1.01x faster                                  |
| xml_etree_iterparse | 107 ms                                                 | 106 ms: 1.01x faster                                   |
| json_dumps          | 10.4 ms                                                | 10.4 ms: 1.01x slower                                  |
| Geometric mean      | (ref)                                                  | 1.02x faster                                           |

Benchmark hidden because not significant (3): pickle_pure_python, xml_etree_parse, unpickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup_no_site | 6.94 ms                                                | 6.81 ms: 1.02x faster                                  |
| python_startup         | 9.55 ms                                                | 9.44 ms: 1.01x faster                                  |
| Geometric mean         | (ref)                                                  | 1.02x faster                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako            | 11.9 ms                                                | 11.3 ms: 1.05x faster                                  |
| django_template | 34.6 ms                                                | 34.7 ms: 1.00x slower                                  |
| Geometric mean  | (ref)                                                  | 1.02x faster                                           |

All benchmarks:
===============

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|---------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| typing_runtime_protocols  | 158 us                                                 | 121 us: 1.31x faster                                   |
| mypy2                     | 830 ms                                                 | 696 ms: 1.19x faster                                   |
| pickle_dict               | 35.5 us                                                | 33.1 us: 1.07x faster                                  |
| unpickle_list             | 5.29 us                                                | 4.99 us: 1.06x faster                                  |
| mako                      | 11.9 ms                                                | 11.3 ms: 1.05x faster                                  |
| pyflate                   | 482 ms                                                 | 460 ms: 1.05x faster                                   |
| comprehensions            | 21.8 us                                                | 20.9 us: 1.04x faster                                  |
| pathlib                   | 19.3 ms                                                | 18.5 ms: 1.04x faster                                  |
| nbody                     | 97.0 ms                                                | 93.2 ms: 1.04x faster                                  |
| deepcopy_memo             | 40.7 us                                                | 39.2 us: 1.04x faster                                  |
| regex_dna                 | 212 ms                                                 | 205 ms: 1.03x faster                                   |
| tornado_http              | 103 ms                                                 | 99.4 ms: 1.03x faster                                  |
| meteor_contest            | 112 ms                                                 | 109 ms: 1.03x faster                                   |
| pickle_list               | 5.08 us                                                | 4.93 us: 1.03x faster                                  |
| sympy_integrate           | 21.4 ms                                                | 20.8 ms: 1.03x faster                                  |
| sympy_sum                 | 169 ms                                                 | 164 ms: 1.03x faster                                   |
| deepcopy_reduce           | 3.35 us                                                | 3.27 us: 1.02x faster                                  |
| chameleon                 | 7.41 ms                                                | 7.24 ms: 1.02x faster                                  |
| docutils                  | 2.77 sec                                               | 2.71 sec: 1.02x faster                                 |
| regex_compile             | 148 ms                                                 | 145 ms: 1.02x faster                                   |
| fannkuch                  | 417 ms                                                 | 409 ms: 1.02x faster                                   |
| tomli_loads               | 2.33 sec                                               | 2.29 sec: 1.02x faster                                 |
| python_startup_no_site    | 6.94 ms                                                | 6.81 ms: 1.02x faster                                  |
| unpack_sequence           | 54.0 ns                                                | 53.0 ns: 1.02x faster                                  |
| sympy_str                 | 300 ms                                                 | 294 ms: 1.02x faster                                   |
| json_loads                | 28.5 us                                                | 28.0 us: 1.02x faster                                  |
| pprint_safe_repr          | 776 ms                                                 | 764 ms: 1.02x faster                                   |
| scimark_fft               | 382 ms                                                 | 376 ms: 1.02x faster                                   |
| async_generators          | 463 ms                                                 | 456 ms: 1.02x faster                                   |
| pickle                    | 11.6 us                                                | 11.4 us: 1.02x faster                                  |
| deepcopy                  | 371 us                                                 | 366 us: 1.01x faster                                   |
| create_gc_cycles          | 1.48 ms                                                | 1.46 ms: 1.01x faster                                  |
| regex_v8                  | 23.1 ms                                                | 22.8 ms: 1.01x faster                                  |
| raytrace                  | 312 ms                                                 | 308 ms: 1.01x faster                                   |
| unpickle                  | 15.9 us                                                | 15.7 us: 1.01x faster                                  |
| python_startup            | 9.55 ms                                                | 9.44 ms: 1.01x faster                                  |
| json                      | 5.26 ms                                                | 5.20 ms: 1.01x faster                                  |
| xml_etree_generate        | 89.2 ms                                                | 88.2 ms: 1.01x faster                                  |
| scimark_monte_carlo       | 75.1 ms                                                | 74.3 ms: 1.01x faster                                  |
| regex_effbot              | 3.61 ms                                                | 3.58 ms: 1.01x faster                                  |
| xml_etree_process         | 61.7 ms                                                | 61.2 ms: 1.01x faster                                  |
| xml_etree_iterparse       | 107 ms                                                 | 106 ms: 1.01x faster                                   |
| bench_thread_pool         | 842 us                                                 | 836 us: 1.01x faster                                   |
| mdp                       | 2.63 sec                                               | 2.61 sec: 1.01x faster                                 |
| pycparser                 | 1.18 sec                                               | 1.17 sec: 1.01x faster                                 |
| aiohttp                   | 1.15 ms                                                | 1.14 ms: 1.01x faster                                  |
| logging_silent            | 104 ns                                                 | 104 ns: 1.01x faster                                   |
| pprint_pformat            | 1.57 sec                                               | 1.56 sec: 1.00x faster                                 |
| 2to3                      | 274 ms                                                 | 274 ms: 1.00x faster                                   |
| pidigits                  | 187 ms                                                 | 187 ms: 1.00x slower                                   |
| django_template           | 34.6 ms                                                | 34.7 ms: 1.00x slower                                  |
| json_dumps                | 10.4 ms                                                | 10.4 ms: 1.01x slower                                  |
| async_tree_none_tg        | 450 ms                                                 | 452 ms: 1.01x slower                                   |
| coroutines                | 23.2 ms                                                | 23.3 ms: 1.01x slower                                  |
| async_tree_none           | 472 ms                                                 | 475 ms: 1.01x slower                                   |
| go                        | 139 ms                                                 | 140 ms: 1.01x slower                                   |
| asyncio_tcp_ssl           | 1.79 sec                                               | 1.80 sec: 1.01x slower                                 |
| richards_super            | 51.5 ms                                                | 52.0 ms: 1.01x slower                                  |
| nqueens                   | 83.3 ms                                                | 84.2 ms: 1.01x slower                                  |
| sqlglot_parse             | 1.36 ms                                                | 1.38 ms: 1.01x slower                                  |
| async_tree_io             | 1.16 sec                                               | 1.17 sec: 1.01x slower                                 |
| sqlglot_transpile         | 1.68 ms                                                | 1.70 ms: 1.01x slower                                  |
| spectral_norm             | 115 ms                                                 | 116 ms: 1.01x slower                                   |
| deltablue                 | 3.72 ms                                                | 3.76 ms: 1.01x slower                                  |
| async_tree_io_tg          | 1.18 sec                                               | 1.20 sec: 1.01x slower                                 |
| async_tree_memoization_tg | 575 ms                                                 | 583 ms: 1.01x slower                                   |
| generators                | 31.2 ms                                                | 31.7 ms: 1.02x slower                                  |
| telco                     | 7.10 ms                                                | 7.23 ms: 1.02x slower                                  |
| crypto_pyaes              | 81.9 ms                                                | 83.5 ms: 1.02x slower                                  |
| scimark_sor               | 129 ms                                                 | 132 ms: 1.02x slower                                   |
| hexiom                    | 6.41 ms                                                | 6.60 ms: 1.03x slower                                  |
| scimark_sparse_mat_mult   | 5.06 ms                                                | 5.23 ms: 1.03x slower                                  |
| coverage                  | 72.7 ms                                                | 75.2 ms: 1.03x slower                                  |
| gc_traversal              | 3.79 ms                                                | 3.93 ms: 1.04x slower                                  |
| asyncio_tcp               | 491 ms                                                 | 510 ms: 1.04x slower                                   |
| Geometric mean            | (ref)                                                  | 1.01x faster                                           |

Benchmark hidden because not significant (23): sqlalchemy_declarative, pickle_pure_python, dask, logging_format, sympy_expand, chaos, richards, sqlglot_optimize, scimark_lu, float, async_tree_cpu_io_mixed, dulwich_log, asyncio_websockets, bench_mp_pool, sqlglot_normalize, async_tree_cpu_io_mixed_tg, logging_simple, xml_etree_parse, gunicorn, sqlite_synth, unpickle_pure_python, sqlalchemy_imperative, async_tree_memoization


# HPT report

- Reliability score: 99.10% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.96x