
# Results vs. 3.11.0

- fork: python
- ref: v3.12.0rc2
- machine: linux-x86_64
- commit hash: 40913a5
- commit date: 2023-09-05
- overall geometric mean: 1.06x faster \*
- HPT reliability: 99.06%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230905-linux-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 268 ms: 1.01x slower                                         |
| docutils       | 2.66 sec                                               | 2.71 sec: 1.02x slower                                       |
| tornado_http   | 98.1 ms                                                | 102 ms: 1.04x slower                                         |
| Geometric mean | (ref)                                                  | 1.02x slower                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230905-linux-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_none         | 528 ms                                                 | 465 ms: 1.14x faster                                         |
| async_tree_io           | 1.29 sec                                               | 1.14 sec: 1.13x faster                                       |
| async_tree_memoization  | 639 ms                                                 | 571 ms: 1.12x faster                                         |
| async_tree_cpu_io_mixed | 749 ms                                                 | 708 ms: 1.06x faster                                         |
| Geometric mean          | (ref)                                                  | 1.11x faster                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230905-linux-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 93.4 ms: 1.03x faster                                        |
| float          | 78.9 ms                                                | 80.1 ms: 1.01x slower                                        |
| pidigits       | 194 ms                                                 | 212 ms: 1.09x slower                                         |
| Geometric mean | (ref)                                                  | 1.02x slower                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230905-linux-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| regex_v8       | 22.9 ms                                                | 22.3 ms: 1.03x faster                                        |
| regex_compile  | 141 ms                                                 | 144 ms: 1.02x slower                                         |
| regex_effbot   | 3.51 ms                                                | 3.59 ms: 1.02x slower                                        |
| regex_dna      | 205 ms                                                 | 213 ms: 1.04x slower                                         |
| Geometric mean | (ref)                                                  | 1.02x slower                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230905-linux-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 9.89 ms: 1.35x faster                                        |
| json_loads           | 29.2 us                                                | 25.1 us: 1.16x faster                                        |
| unpickle_pure_python | 242 us                                                 | 219 us: 1.10x faster                                         |
| pickle_dict          | 34.6 us                                                | 31.8 us: 1.09x faster                                        |
| xml_etree_parse      | 164 ms                                                 | 154 ms: 1.07x faster                                         |
| tomli_loads          | 2.30 sec                                               | 2.20 sec: 1.05x faster                                       |
| xml_etree_iterparse  | 108 ms                                                 | 103 ms: 1.05x faster                                         |
| pickle               | 11.0 us                                                | 10.6 us: 1.04x faster                                        |
| pickle_pure_python   | 320 us                                                 | 314 us: 1.02x faster                                         |
| pickle_list          | 4.59 us                                                | 4.67 us: 1.02x slower                                        |
| unpickle_list        | 5.21 us                                                | 5.38 us: 1.03x slower                                        |
| xml_etree_process    | 56.9 ms                                                | 58.7 ms: 1.03x slower                                        |
| xml_etree_generate   | 81.1 ms                                                | 84.3 ms: 1.04x slower                                        |
| unpickle             | 13.8 us                                                | 15.1 us: 1.09x slower                                        |
| Geometric mean       | (ref)                                                  | 1.05x faster                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230905-linux-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 9.46 ms: 1.11x slower                                        |
| python_startup_no_site | 6.01 ms                                                | 6.88 ms: 1.15x slower                                        |
| Geometric mean         | (ref)                                                  | 1.12x slower                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230905-linux-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|-----------|:------------------------------------------------------:|:------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 10.9 ms: 1.02x slower                                        |

All benchmarks:
===============

| Benchmark                | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230905-linux-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| typing_runtime_protocols | 520 us                                                 | 144 us: 3.60x faster                                         |
| generators               | 74.9 ms                                                | 30.8 ms: 2.43x faster                                        |
| asyncio_tcp              | 875 ms                                                 | 505 ms: 1.73x faster                                         |
| asyncio_tcp_ssl          | 3.11 sec                                               | 1.80 sec: 1.73x faster                                       |
| json_dumps               | 13.3 ms                                                | 9.89 ms: 1.35x faster                                        |
| richards_super           | 61.9 ms                                                | 48.9 ms: 1.27x faster                                        |
| coroutines               | 27.0 ms                                                | 22.1 ms: 1.22x faster                                        |
| json_loads               | 29.2 us                                                | 25.1 us: 1.16x faster                                        |
| richards                 | 49.8 ms                                                | 43.3 ms: 1.15x faster                                        |
| comprehensions           | 23.6 us                                                | 20.7 us: 1.14x faster                                        |
| async_tree_none          | 528 ms                                                 | 465 ms: 1.14x faster                                         |
| async_tree_io            | 1.29 sec                                               | 1.14 sec: 1.13x faster                                       |
| logging_silent           | 111 ns                                                 | 98.5 ns: 1.13x faster                                        |
| chaos                    | 71.9 ms                                                | 63.8 ms: 1.13x faster                                        |
| deltablue                | 3.92 ms                                                | 3.49 ms: 1.13x faster                                        |
| async_tree_memoization   | 639 ms                                                 | 571 ms: 1.12x faster                                         |
| hexiom                   | 6.89 ms                                                | 6.17 ms: 1.12x faster                                        |
| unpickle_pure_python     | 242 us                                                 | 219 us: 1.10x faster                                         |
| go                       | 149 ms                                                 | 135 ms: 1.10x faster                                         |
| json                     | 5.24 ms                                                | 4.80 ms: 1.09x faster                                        |
| pickle_dict              | 34.6 us                                                | 31.8 us: 1.09x faster                                        |
| nqueens                  | 87.9 ms                                                | 81.4 ms: 1.08x faster                                        |
| mdp                      | 2.77 sec                                               | 2.58 sec: 1.08x faster                                       |
| sqlglot_parse            | 1.43 ms                                                | 1.33 ms: 1.07x faster                                        |
| deepcopy_memo            | 40.2 us                                                | 37.5 us: 1.07x faster                                        |
| xml_etree_parse          | 164 ms                                                 | 154 ms: 1.07x faster                                         |
| sqlglot_transpile        | 1.75 ms                                                | 1.65 ms: 1.06x faster                                        |
| async_tree_cpu_io_mixed  | 749 ms                                                 | 708 ms: 1.06x faster                                         |
| raytrace                 | 309 ms                                                 | 293 ms: 1.05x faster                                         |
| tomli_loads              | 2.30 sec                                               | 2.20 sec: 1.05x faster                                       |
| gc_traversal             | 4.01 ms                                                | 3.83 ms: 1.05x faster                                        |
| xml_etree_iterparse      | 108 ms                                                 | 103 ms: 1.05x faster                                         |
| scimark_sparse_mat_mult  | 5.03 ms                                                | 4.81 ms: 1.05x faster                                        |
| sqlglot_normalize        | 113 ms                                                 | 108 ms: 1.04x faster                                         |
| deepcopy                 | 365 us                                                 | 351 us: 1.04x faster                                         |
| pickle                   | 11.0 us                                                | 10.6 us: 1.04x faster                                        |
| sqlglot_optimize         | 55.3 ms                                                | 53.5 ms: 1.03x faster                                        |
| deepcopy_reduce          | 3.22 us                                                | 3.12 us: 1.03x faster                                        |
| pprint_pformat           | 1.55 sec                                               | 1.51 sec: 1.03x faster                                       |
| nbody                    | 96.0 ms                                                | 93.4 ms: 1.03x faster                                        |
| scimark_lu               | 116 ms                                                 | 113 ms: 1.03x faster                                         |
| meteor_contest           | 109 ms                                                 | 106 ms: 1.03x faster                                         |
| regex_v8                 | 22.9 ms                                                | 22.3 ms: 1.03x faster                                        |
| pycparser                | 1.19 sec                                               | 1.16 sec: 1.02x faster                                       |
| spectral_norm            | 108 ms                                                 | 106 ms: 1.02x faster                                         |
| pickle_pure_python       | 320 us                                                 | 314 us: 1.02x faster                                         |
| pprint_safe_repr         | 747 ms                                                 | 736 ms: 1.02x faster                                         |
| fannkuch                 | 405 ms                                                 | 400 ms: 1.01x faster                                         |
| pathlib                  | 18.5 ms                                                | 18.4 ms: 1.01x faster                                        |
| bench_thread_pool        | 834 us                                                 | 829 us: 1.01x faster                                         |
| scimark_monte_carlo      | 70.7 ms                                                | 71.4 ms: 1.01x slower                                        |
| logging_simple           | 6.22 us                                                | 6.28 us: 1.01x slower                                        |
| float                    | 78.9 ms                                                | 80.1 ms: 1.01x slower                                        |
| 2to3                     | 264 ms                                                 | 268 ms: 1.01x slower                                         |
| pickle_list              | 4.59 us                                                | 4.67 us: 1.02x slower                                        |
| docutils                 | 2.66 sec                                               | 2.71 sec: 1.02x slower                                       |
| regex_compile            | 141 ms                                                 | 144 ms: 1.02x slower                                         |
| mako                     | 10.7 ms                                                | 10.9 ms: 1.02x slower                                        |
| scimark_sor              | 121 ms                                                 | 124 ms: 1.02x slower                                         |
| regex_effbot             | 3.51 ms                                                | 3.59 ms: 1.02x slower                                        |
| unpickle_list            | 5.21 us                                                | 5.38 us: 1.03x slower                                        |
| xml_etree_process        | 56.9 ms                                                | 58.7 ms: 1.03x slower                                        |
| sqlalchemy_declarative   | 140 ms                                                 | 145 ms: 1.03x slower                                         |
| tornado_http             | 98.1 ms                                                | 102 ms: 1.04x slower                                         |
| crypto_pyaes             | 76.7 ms                                                | 79.6 ms: 1.04x slower                                        |
| xml_etree_generate       | 81.1 ms                                                | 84.3 ms: 1.04x slower                                        |
| logging_format           | 6.81 us                                                | 7.08 us: 1.04x slower                                        |
| regex_dna                | 205 ms                                                 | 213 ms: 1.04x slower                                         |
| unpack_sequence          | 43.5 ns                                                | 45.6 ns: 1.05x slower                                        |
| scimark_fft              | 345 ms                                                 | 364 ms: 1.05x slower                                         |
| create_gc_cycles         | 1.43 ms                                                | 1.51 ms: 1.05x slower                                        |
| dulwich_log              | 64.6 ms                                                | 68.2 ms: 1.06x slower                                        |
| sqlite_synth             | 2.57 us                                                | 2.74 us: 1.07x slower                                        |
| pyflate                  | 434 ms                                                 | 467 ms: 1.08x slower                                         |
| pidigits                 | 194 ms                                                 | 212 ms: 1.09x slower                                         |
| unpickle                 | 13.8 us                                                | 15.1 us: 1.09x slower                                        |
| python_startup           | 8.56 ms                                                | 9.46 ms: 1.11x slower                                        |
| python_startup_no_site   | 6.01 ms                                                | 6.88 ms: 1.15x slower                                        |
| async_generators         | 374 ms                                                 | 445 ms: 1.19x slower                                         |
| coverage                 | 78.8 ms                                                | 94.7 ms: 1.20x slower                                        |
| dask                     | 365 ms                                                 | 537 ms: 1.47x slower                                         |
| Geometric mean           | (ref)                                                  | 1.06x faster                                                 |

Benchmark hidden because not significant (3): telco, bench_mp_pool, sqlalchemy_imperative
Ignored benchmarks (21) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, chameleon, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 99.06% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.10x