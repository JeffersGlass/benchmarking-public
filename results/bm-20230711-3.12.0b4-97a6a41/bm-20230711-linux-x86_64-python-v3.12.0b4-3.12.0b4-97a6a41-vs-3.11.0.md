
# Results vs. 3.11.0

- fork: python
- ref: v3.12.0b4
- machine: linux-x86_64
- commit hash: 97a6a41
- commit date: 2023-07-11
- overall geometric mean: 1.06x faster \*
- HPT reliability: 99.82%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230711-linux-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 267 ms: 1.01x slower                                       |
| docutils       | 2.66 sec                                               | 2.70 sec: 1.01x slower                                     |
| tornado_http   | 98.1 ms                                                | 99.1 ms: 1.01x slower                                      |
| Geometric mean | (ref)                                                  | 1.01x slower                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230711-linux-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| async_tree_none         | 528 ms                                                 | 472 ms: 1.12x faster                                       |
| async_tree_memoization  | 639 ms                                                 | 573 ms: 1.12x faster                                       |
| async_tree_io           | 1.29 sec                                               | 1.16 sec: 1.11x faster                                     |
| async_tree_cpu_io_mixed | 749 ms                                                 | 715 ms: 1.05x faster                                       |
| Geometric mean          | (ref)                                                  | 1.10x faster                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230711-linux-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 89.2 ms: 1.08x faster                                      |
| pidigits       | 194 ms                                                 | 192 ms: 1.01x faster                                       |
| float          | 78.9 ms                                                | 80.7 ms: 1.02x slower                                      |
| Geometric mean | (ref)                                                  | 1.02x faster                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230711-linux-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| regex_v8       | 22.9 ms                                                | 23.0 ms: 1.01x slower                                      |
| regex_compile  | 141 ms                                                 | 142 ms: 1.01x slower                                       |
| regex_dna      | 205 ms                                                 | 207 ms: 1.01x slower                                       |
| regex_effbot   | 3.51 ms                                                | 3.57 ms: 1.02x slower                                      |
| Geometric mean | (ref)                                                  | 1.01x slower                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230711-linux-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 9.66 ms: 1.38x faster                                      |
| json_loads           | 29.2 us                                                | 25.7 us: 1.14x faster                                      |
| unpickle_pure_python | 242 us                                                 | 217 us: 1.12x faster                                       |
| pickle_dict          | 34.6 us                                                | 31.6 us: 1.10x faster                                      |
| xml_etree_parse      | 164 ms                                                 | 152 ms: 1.08x faster                                       |
| xml_etree_iterparse  | 108 ms                                                 | 102 ms: 1.06x faster                                       |
| unpickle_list        | 5.21 us                                                | 4.95 us: 1.05x faster                                      |
| pickle_pure_python   | 320 us                                                 | 306 us: 1.05x faster                                       |
| tomli_loads          | 2.30 sec                                               | 2.23 sec: 1.03x faster                                     |
| pickle               | 11.0 us                                                | 10.6 us: 1.03x faster                                      |
| xml_etree_process    | 56.9 ms                                                | 59.4 ms: 1.04x slower                                      |
| xml_etree_generate   | 81.1 ms                                                | 85.0 ms: 1.05x slower                                      |
| unpickle             | 13.8 us                                                | 15.1 us: 1.09x slower                                      |
| Geometric mean       | (ref)                                                  | 1.06x faster                                               |

Benchmark hidden because not significant (1): pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230711-linux-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 9.35 ms: 1.09x slower                                      |
| python_startup_no_site | 6.01 ms                                                | 6.79 ms: 1.13x slower                                      |
| Geometric mean         | (ref)                                                  | 1.11x slower                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230711-linux-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------:|
| mako      | 10.7 ms                                                | 10.9 ms: 1.02x slower                                      |

All benchmarks:
===============

| Benchmark                | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230711-linux-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| typing_runtime_protocols | 520 us                                                 | 145 us: 3.59x faster                                       |
| generators               | 74.9 ms                                                | 30.5 ms: 2.45x faster                                      |
| asyncio_tcp_ssl          | 3.11 sec                                               | 1.80 sec: 1.73x faster                                     |
| asyncio_tcp              | 875 ms                                                 | 517 ms: 1.69x faster                                       |
| json_dumps               | 13.3 ms                                                | 9.66 ms: 1.38x faster                                      |
| richards_super           | 61.9 ms                                                | 49.2 ms: 1.26x faster                                      |
| coroutines               | 27.0 ms                                                | 22.5 ms: 1.20x faster                                      |
| richards                 | 49.8 ms                                                | 43.3 ms: 1.15x faster                                      |
| chaos                    | 71.9 ms                                                | 62.7 ms: 1.15x faster                                      |
| comprehensions           | 23.6 us                                                | 20.7 us: 1.14x faster                                      |
| hexiom                   | 6.89 ms                                                | 6.05 ms: 1.14x faster                                      |
| json_loads               | 29.2 us                                                | 25.7 us: 1.14x faster                                      |
| logging_silent           | 111 ns                                                 | 97.8 ns: 1.14x faster                                      |
| deltablue                | 3.92 ms                                                | 3.49 ms: 1.12x faster                                      |
| async_tree_none          | 528 ms                                                 | 472 ms: 1.12x faster                                       |
| unpickle_pure_python     | 242 us                                                 | 217 us: 1.12x faster                                       |
| async_tree_memoization   | 639 ms                                                 | 573 ms: 1.12x faster                                       |
| async_tree_io            | 1.29 sec                                               | 1.16 sec: 1.11x faster                                     |
| go                       | 149 ms                                                 | 135 ms: 1.10x faster                                       |
| pickle_dict              | 34.6 us                                                | 31.6 us: 1.10x faster                                      |
| nqueens                  | 87.9 ms                                                | 80.9 ms: 1.09x faster                                      |
| sqlglot_parse            | 1.43 ms                                                | 1.33 ms: 1.08x faster                                      |
| xml_etree_parse          | 164 ms                                                 | 152 ms: 1.08x faster                                       |
| nbody                    | 96.0 ms                                                | 89.2 ms: 1.08x faster                                      |
| sqlglot_transpile        | 1.75 ms                                                | 1.64 ms: 1.07x faster                                      |
| spectral_norm            | 108 ms                                                 | 102 ms: 1.06x faster                                       |
| json                     | 5.24 ms                                                | 4.95 ms: 1.06x faster                                      |
| deepcopy_memo            | 40.2 us                                                | 37.9 us: 1.06x faster                                      |
| xml_etree_iterparse      | 108 ms                                                 | 102 ms: 1.06x faster                                       |
| unpickle_list            | 5.21 us                                                | 4.95 us: 1.05x faster                                      |
| fannkuch                 | 405 ms                                                 | 385 ms: 1.05x faster                                       |
| raytrace                 | 309 ms                                                 | 293 ms: 1.05x faster                                       |
| async_tree_cpu_io_mixed  | 749 ms                                                 | 715 ms: 1.05x faster                                       |
| pickle_pure_python       | 320 us                                                 | 306 us: 1.05x faster                                       |
| meteor_contest           | 109 ms                                                 | 104 ms: 1.04x faster                                       |
| pprint_pformat           | 1.55 sec                                               | 1.49 sec: 1.04x faster                                     |
| sqlglot_normalize        | 113 ms                                                 | 109 ms: 1.04x faster                                       |
| scimark_lu               | 116 ms                                                 | 112 ms: 1.04x faster                                       |
| deepcopy_reduce          | 3.22 us                                                | 3.11 us: 1.04x faster                                      |
| tomli_loads              | 2.30 sec                                               | 2.23 sec: 1.03x faster                                     |
| pickle                   | 11.0 us                                                | 10.6 us: 1.03x faster                                      |
| deepcopy                 | 365 us                                                 | 355 us: 1.03x faster                                       |
| gc_traversal             | 4.01 ms                                                | 3.91 ms: 1.03x faster                                      |
| sqlglot_optimize         | 55.3 ms                                                | 53.9 ms: 1.03x faster                                      |
| scimark_sparse_mat_mult  | 5.03 ms                                                | 4.91 ms: 1.02x faster                                      |
| pprint_safe_repr         | 747 ms                                                 | 731 ms: 1.02x faster                                       |
| scimark_sor              | 121 ms                                                 | 119 ms: 1.02x faster                                       |
| mdp                      | 2.77 sec                                               | 2.73 sec: 1.02x faster                                     |
| pycparser                | 1.19 sec                                               | 1.17 sec: 1.02x faster                                     |
| pidigits                 | 194 ms                                                 | 192 ms: 1.01x faster                                       |
| bench_thread_pool        | 834 us                                                 | 827 us: 1.01x faster                                       |
| regex_v8                 | 22.9 ms                                                | 23.0 ms: 1.01x slower                                      |
| crypto_pyaes             | 76.7 ms                                                | 77.2 ms: 1.01x slower                                      |
| regex_compile            | 141 ms                                                 | 142 ms: 1.01x slower                                       |
| regex_dna                | 205 ms                                                 | 207 ms: 1.01x slower                                       |
| tornado_http             | 98.1 ms                                                | 99.1 ms: 1.01x slower                                      |
| 2to3                     | 264 ms                                                 | 267 ms: 1.01x slower                                       |
| pathlib                  | 18.5 ms                                                | 18.8 ms: 1.01x slower                                      |
| docutils                 | 2.66 sec                                               | 2.70 sec: 1.01x slower                                     |
| regex_effbot             | 3.51 ms                                                | 3.57 ms: 1.02x slower                                      |
| logging_format           | 6.81 us                                                | 6.93 us: 1.02x slower                                      |
| mako                     | 10.7 ms                                                | 10.9 ms: 1.02x slower                                      |
| float                    | 78.9 ms                                                | 80.7 ms: 1.02x slower                                      |
| sqlalchemy_declarative   | 140 ms                                                 | 144 ms: 1.02x slower                                       |
| scimark_monte_carlo      | 70.7 ms                                                | 72.4 ms: 1.02x slower                                      |
| scimark_fft              | 345 ms                                                 | 358 ms: 1.04x slower                                       |
| xml_etree_process        | 56.9 ms                                                | 59.4 ms: 1.04x slower                                      |
| xml_etree_generate       | 81.1 ms                                                | 85.0 ms: 1.05x slower                                      |
| dulwich_log              | 64.6 ms                                                | 67.9 ms: 1.05x slower                                      |
| create_gc_cycles         | 1.43 ms                                                | 1.51 ms: 1.06x slower                                      |
| sqlite_synth             | 2.57 us                                                | 2.74 us: 1.06x slower                                      |
| unpickle                 | 13.8 us                                                | 15.1 us: 1.09x slower                                      |
| python_startup           | 8.56 ms                                                | 9.35 ms: 1.09x slower                                      |
| unpack_sequence          | 43.5 ns                                                | 48.9 ns: 1.13x slower                                      |
| python_startup_no_site   | 6.01 ms                                                | 6.79 ms: 1.13x slower                                      |
| coverage                 | 78.8 ms                                                | 93.5 ms: 1.19x slower                                      |
| async_generators         | 374 ms                                                 | 448 ms: 1.20x slower                                       |
| dask                     | 365 ms                                                 | 535 ms: 1.46x slower                                       |
| Geometric mean           | (ref)                                                  | 1.06x faster                                               |

Benchmark hidden because not significant (6): telco, logging_simple, bench_mp_pool, pickle_list, pyflate, sqlalchemy_imperative
Ignored benchmarks (21) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, chameleon, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 99.82% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.10x