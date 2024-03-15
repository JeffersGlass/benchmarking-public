
# Results vs. 3.10.4

- fork: python
- ref: v3.12.0b4
- machine: linux-x86_64
- commit hash: 97a6a41
- commit date: 2023-07-11
- overall geometric mean: 1.36x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.28x faster
- Memory change: 1.17x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230711-linux-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 267 ms: 1.30x faster                                       |
| docutils       | 3.30 sec                                               | 2.70 sec: 1.22x faster                                     |
| tornado_http   | 136 ms                                                 | 99.1 ms: 1.38x faster                                      |
| Geometric mean | (ref)                                                  | 1.30x faster                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230711-linux-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 472 ms: 1.54x faster                                       |
| async_tree_io           | 1.77 sec                                               | 1.16 sec: 1.52x faster                                     |
| async_tree_memoization  | 870 ms                                                 | 573 ms: 1.52x faster                                       |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 715 ms: 1.42x faster                                       |
| Geometric mean          | (ref)                                                  | 1.50x faster                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230711-linux-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| nbody          | 154 ms                                                 | 89.2 ms: 1.72x faster                                      |
| float          | 117 ms                                                 | 80.7 ms: 1.45x faster                                      |
| pidigits       | 191 ms                                                 | 192 ms: 1.00x slower                                       |
| Geometric mean | (ref)                                                  | 1.36x faster                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230711-linux-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 142 ms: 1.33x faster                                       |
| regex_v8       | 27.8 ms                                                | 23.0 ms: 1.21x faster                                      |
| regex_dna      | 227 ms                                                 | 207 ms: 1.10x faster                                       |
| regex_effbot   | 3.63 ms                                                | 3.57 ms: 1.02x faster                                      |
| Geometric mean | (ref)                                                  | 1.16x faster                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230711-linux-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 306 us: 1.59x faster                                       |
| unpickle_pure_python | 331 us                                                 | 217 us: 1.53x faster                                       |
| json_dumps           | 14.2 ms                                                | 9.66 ms: 1.47x faster                                      |
| tomli_loads          | 3.14 sec                                               | 2.23 sec: 1.41x faster                                     |
| xml_etree_process    | 79.1 ms                                                | 59.4 ms: 1.33x faster                                      |
| json_loads           | 31.2 us                                                | 25.7 us: 1.21x faster                                      |
| xml_etree_generate   | 99.4 ms                                                | 85.0 ms: 1.17x faster                                      |
| xml_etree_iterparse  | 115 ms                                                 | 102 ms: 1.13x faster                                       |
| pickle_list          | 5.08 us                                                | 4.59 us: 1.11x faster                                      |
| xml_etree_parse      | 168 ms                                                 | 152 ms: 1.10x faster                                       |
| unpickle_list        | 5.20 us                                                | 4.95 us: 1.05x faster                                      |
| unpickle             | 14.4 us                                                | 15.1 us: 1.05x slower                                      |
| pickle_dict          | 29.6 us                                                | 31.6 us: 1.07x slower                                      |
| Geometric mean       | (ref)                                                  | 1.20x faster                                               |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230711-linux-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 9.35 ms: 1.56x faster                                      |
| python_startup_no_site | 5.93 ms                                                | 6.79 ms: 1.14x slower                                      |
| Geometric mean         | (ref)                                                  | 1.17x faster                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230711-linux-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------:|
| mako      | 16.3 ms                                                | 10.9 ms: 1.50x faster                                      |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230711-linux-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 145 us: 3.76x faster                                       |
| generators               | 80.1 ms                                                | 30.5 ms: 2.62x faster                                      |
| deltablue                | 7.91 ms                                                | 3.49 ms: 2.27x faster                                      |
| logging_silent           | 190 ns                                                 | 97.8 ns: 1.94x faster                                      |
| richards_super           | 94.7 ms                                                | 49.2 ms: 1.93x faster                                      |
| scimark_sor              | 220 ms                                                 | 119 ms: 1.84x faster                                       |
| chaos                    | 115 ms                                                 | 62.7 ms: 1.84x faster                                      |
| richards                 | 79.3 ms                                                | 43.3 ms: 1.83x faster                                      |
| asyncio_tcp              | 922 ms                                                 | 517 ms: 1.78x faster                                       |
| go                       | 240 ms                                                 | 135 ms: 1.78x faster                                       |
| raytrace                 | 507 ms                                                 | 293 ms: 1.73x faster                                       |
| nbody                    | 154 ms                                                 | 89.2 ms: 1.72x faster                                      |
| hexiom                   | 10.4 ms                                                | 6.05 ms: 1.72x faster                                      |
| spectral_norm            | 170 ms                                                 | 102 ms: 1.67x faster                                       |
| crypto_pyaes             | 128 ms                                                 | 77.2 ms: 1.66x faster                                      |
| pyflate                  | 716 ms                                                 | 434 ms: 1.65x faster                                       |
| sqlglot_parse            | 2.17 ms                                                | 1.33 ms: 1.63x faster                                      |
| scimark_monte_carlo      | 118 ms                                                 | 72.4 ms: 1.63x faster                                      |
| pickle_pure_python       | 484 us                                                 | 306 us: 1.59x faster                                       |
| scimark_lu               | 176 ms                                                 | 112 ms: 1.57x faster                                       |
| sqlglot_transpile        | 2.57 ms                                                | 1.64 ms: 1.57x faster                                      |
| python_startup           | 14.6 ms                                                | 9.35 ms: 1.56x faster                                      |
| coroutines               | 35.1 ms                                                | 22.5 ms: 1.56x faster                                      |
| async_tree_none          | 728 ms                                                 | 472 ms: 1.54x faster                                       |
| deepcopy_memo            | 58.5 us                                                | 37.9 us: 1.54x faster                                      |
| unpickle_pure_python     | 331 us                                                 | 217 us: 1.53x faster                                       |
| async_tree_io            | 1.77 sec                                               | 1.16 sec: 1.52x faster                                     |
| async_tree_memoization   | 870 ms                                                 | 573 ms: 1.52x faster                                       |
| mako                     | 16.3 ms                                                | 10.9 ms: 1.50x faster                                      |
| json_dumps               | 14.2 ms                                                | 9.66 ms: 1.47x faster                                      |
| float                    | 117 ms                                                 | 80.7 ms: 1.45x faster                                      |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                     |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 715 ms: 1.42x faster                                       |
| pprint_pformat           | 2.10 sec                                               | 1.49 sec: 1.41x faster                                     |
| tomli_loads              | 3.14 sec                                               | 2.23 sec: 1.41x faster                                     |
| pprint_safe_repr         | 1.02 sec                                               | 731 ms: 1.39x faster                                       |
| comprehensions           | 28.8 us                                                | 20.7 us: 1.39x faster                                      |
| fannkuch                 | 532 ms                                                 | 385 ms: 1.38x faster                                       |
| tornado_http             | 136 ms                                                 | 99.1 ms: 1.38x faster                                      |
| pycparser                | 1.58 sec                                               | 1.17 sec: 1.35x faster                                     |
| deepcopy                 | 479 us                                                 | 355 us: 1.35x faster                                       |
| deepcopy_reduce          | 4.17 us                                                | 3.11 us: 1.34x faster                                      |
| logging_simple           | 8.30 us                                                | 6.21 us: 1.34x faster                                      |
| xml_etree_process        | 79.1 ms                                                | 59.4 ms: 1.33x faster                                      |
| regex_compile            | 188 ms                                                 | 142 ms: 1.33x faster                                       |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.91 ms: 1.32x faster                                      |
| sqlglot_normalize        | 143 ms                                                 | 109 ms: 1.32x faster                                       |
| logging_format           | 9.09 us                                                | 6.93 us: 1.31x faster                                      |
| nqueens                  | 106 ms                                                 | 80.9 ms: 1.31x faster                                      |
| 2to3                     | 348 ms                                                 | 267 ms: 1.30x faster                                       |
| scimark_fft              | 466 ms                                                 | 358 ms: 1.30x faster                                       |
| sqlglot_optimize         | 69.2 ms                                                | 53.9 ms: 1.28x faster                                      |
| sqlalchemy_imperative    | 23.3 ms                                                | 18.5 ms: 1.26x faster                                      |
| dulwich_log              | 84.3 ms                                                | 67.9 ms: 1.24x faster                                      |
| unpack_sequence          | 60.0 ns                                                | 48.9 ns: 1.23x faster                                      |
| docutils                 | 3.30 sec                                               | 2.70 sec: 1.22x faster                                     |
| json_loads               | 31.2 us                                                | 25.7 us: 1.21x faster                                      |
| regex_v8                 | 27.8 ms                                                | 23.0 ms: 1.21x faster                                      |
| sqlalchemy_declarative   | 172 ms                                                 | 144 ms: 1.20x faster                                       |
| bench_thread_pool        | 986 us                                                 | 827 us: 1.19x faster                                       |
| xml_etree_generate       | 99.4 ms                                                | 85.0 ms: 1.17x faster                                      |
| json                     | 5.69 ms                                                | 4.95 ms: 1.15x faster                                      |
| meteor_contest           | 120 ms                                                 | 104 ms: 1.15x faster                                       |
| xml_etree_iterparse      | 115 ms                                                 | 102 ms: 1.13x faster                                       |
| pickle_list              | 5.08 us                                                | 4.59 us: 1.11x faster                                      |
| sqlite_synth             | 3.02 us                                                | 2.74 us: 1.11x faster                                      |
| xml_etree_parse          | 168 ms                                                 | 152 ms: 1.10x faster                                       |
| regex_dna                | 227 ms                                                 | 207 ms: 1.10x faster                                       |
| pathlib                  | 20.5 ms                                                | 18.8 ms: 1.09x faster                                      |
| create_gc_cycles         | 1.62 ms                                                | 1.51 ms: 1.07x faster                                      |
| telco                    | 7.27 ms                                                | 6.83 ms: 1.06x faster                                      |
| unpickle_list            | 5.20 us                                                | 4.95 us: 1.05x faster                                      |
| mdp                      | 2.85 sec                                               | 2.73 sec: 1.04x faster                                     |
| regex_effbot             | 3.63 ms                                                | 3.57 ms: 1.02x faster                                      |
| pidigits                 | 191 ms                                                 | 192 ms: 1.00x slower                                       |
| async_generators         | 444 ms                                                 | 448 ms: 1.01x slower                                       |
| unpickle                 | 14.4 us                                                | 15.1 us: 1.05x slower                                      |
| pickle_dict              | 29.6 us                                                | 31.6 us: 1.07x slower                                      |
| gc_traversal             | 3.62 ms                                                | 3.91 ms: 1.08x slower                                      |
| python_startup_no_site   | 5.93 ms                                                | 6.79 ms: 1.14x slower                                      |
| coverage                 | 79.4 ms                                                | 93.5 ms: 1.18x slower                                      |
| dask                     | 441 ms                                                 | 535 ms: 1.21x slower                                       |
| Geometric mean           | (ref)                                                  | 1.36x faster                                               |

Benchmark hidden because not significant (2): pickle, bench_mp_pool
Ignored benchmarks (17) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_websockets, chameleon, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.31x
- 95% likely to have a speedup of 1.30x
- 99% likely to have a speedup of 1.28x


# Memory

- memory change: 1.17x