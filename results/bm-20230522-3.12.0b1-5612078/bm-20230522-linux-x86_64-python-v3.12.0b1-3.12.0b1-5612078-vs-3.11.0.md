
# Results vs. 3.11.0

- fork: python
- ref: v3.12.0b1
- machine: linux-x86_64
- commit hash: 5612078
- commit date: 2023-05-22
- overall geometric mean: 1.06x faster \*
- HPT reliability: 97.19%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.09x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230522-linux-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 268 ms: 1.01x slower                                       |
| docutils       | 2.66 sec                                               | 2.71 sec: 1.02x slower                                     |
| tornado_http   | 98.1 ms                                                | 99.2 ms: 1.01x slower                                      |
| Geometric mean | (ref)                                                  | 1.01x slower                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230522-linux-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| async_tree_none         | 528 ms                                                 | 469 ms: 1.13x faster                                       |
| async_tree_memoization  | 639 ms                                                 | 572 ms: 1.12x faster                                       |
| async_tree_io           | 1.29 sec                                               | 1.16 sec: 1.11x faster                                     |
| async_tree_cpu_io_mixed | 749 ms                                                 | 708 ms: 1.06x faster                                       |
| Geometric mean          | (ref)                                                  | 1.10x faster                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230522-linux-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 88.9 ms: 1.08x faster                                      |
| pidigits       | 194 ms                                                 | 196 ms: 1.01x slower                                       |
| float          | 78.9 ms                                                | 80.7 ms: 1.02x slower                                      |
| Geometric mean | (ref)                                                  | 1.01x faster                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230522-linux-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| regex_v8       | 22.9 ms                                                | 21.8 ms: 1.05x faster                                      |
| regex_effbot   | 3.51 ms                                                | 3.54 ms: 1.01x slower                                      |
| regex_compile  | 141 ms                                                 | 144 ms: 1.02x slower                                       |
| regex_dna      | 205 ms                                                 | 208 ms: 1.02x slower                                       |
| Geometric mean | (ref)                                                  | 1.00x faster                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230522-linux-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 9.76 ms: 1.37x faster                                      |
| json_loads           | 29.2 us                                                | 25.1 us: 1.16x faster                                      |
| unpickle_pure_python | 242 us                                                 | 216 us: 1.12x faster                                       |
| xml_etree_parse      | 164 ms                                                 | 153 ms: 1.07x faster                                       |
| tomli_loads          | 2.30 sec                                               | 2.18 sec: 1.06x faster                                     |
| xml_etree_iterparse  | 108 ms                                                 | 103 ms: 1.05x faster                                       |
| pickle               | 11.0 us                                                | 10.6 us: 1.04x faster                                      |
| pickle_dict          | 34.6 us                                                | 33.3 us: 1.04x faster                                      |
| pickle_pure_python   | 320 us                                                 | 312 us: 1.03x faster                                       |
| unpickle_list        | 5.21 us                                                | 5.17 us: 1.01x faster                                      |
| pickle_list          | 4.59 us                                                | 4.73 us: 1.03x slower                                      |
| xml_etree_process    | 56.9 ms                                                | 59.0 ms: 1.04x slower                                      |
| xml_etree_generate   | 81.1 ms                                                | 85.6 ms: 1.06x slower                                      |
| unpickle             | 13.8 us                                                | 14.9 us: 1.08x slower                                      |
| Geometric mean       | (ref)                                                  | 1.05x faster                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230522-linux-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 9.34 ms: 1.09x slower                                      |
| python_startup_no_site | 6.01 ms                                                | 6.78 ms: 1.13x slower                                      |
| Geometric mean         | (ref)                                                  | 1.11x slower                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230522-linux-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------:|
| mako      | 10.7 ms                                                | 10.8 ms: 1.02x slower                                      |

All benchmarks:
===============

| Benchmark                | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230522-linux-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| typing_runtime_protocols | 520 us                                                 | 140 us: 3.71x faster                                       |
| generators               | 74.9 ms                                                | 31.4 ms: 2.38x faster                                      |
| asyncio_tcp_ssl          | 3.11 sec                                               | 1.80 sec: 1.73x faster                                     |
| asyncio_tcp              | 875 ms                                                 | 513 ms: 1.71x faster                                       |
| json_dumps               | 13.3 ms                                                | 9.76 ms: 1.37x faster                                      |
| richards_super           | 61.9 ms                                                | 49.8 ms: 1.24x faster                                      |
| coroutines               | 27.0 ms                                                | 21.9 ms: 1.24x faster                                      |
| json_loads               | 29.2 us                                                | 25.1 us: 1.16x faster                                      |
| comprehensions           | 23.6 us                                                | 20.6 us: 1.15x faster                                      |
| richards                 | 49.8 ms                                                | 43.6 ms: 1.14x faster                                      |
| deltablue                | 3.92 ms                                                | 3.44 ms: 1.14x faster                                      |
| async_tree_none          | 528 ms                                                 | 469 ms: 1.13x faster                                       |
| hexiom                   | 6.89 ms                                                | 6.12 ms: 1.12x faster                                      |
| unpickle_pure_python     | 242 us                                                 | 216 us: 1.12x faster                                       |
| async_tree_memoization   | 639 ms                                                 | 572 ms: 1.12x faster                                       |
| chaos                    | 71.9 ms                                                | 64.6 ms: 1.11x faster                                      |
| logging_silent           | 111 ns                                                 | 100 ns: 1.11x faster                                       |
| async_tree_io            | 1.29 sec                                               | 1.16 sec: 1.11x faster                                     |
| json                     | 5.24 ms                                                | 4.77 ms: 1.10x faster                                      |
| go                       | 149 ms                                                 | 136 ms: 1.09x faster                                       |
| gc_traversal             | 4.01 ms                                                | 3.67 ms: 1.09x faster                                      |
| nbody                    | 96.0 ms                                                | 88.9 ms: 1.08x faster                                      |
| nqueens                  | 87.9 ms                                                | 81.4 ms: 1.08x faster                                      |
| sqlglot_parse            | 1.43 ms                                                | 1.33 ms: 1.08x faster                                      |
| xml_etree_parse          | 164 ms                                                 | 153 ms: 1.07x faster                                       |
| deepcopy_memo            | 40.2 us                                                | 37.6 us: 1.07x faster                                      |
| sqlglot_transpile        | 1.75 ms                                                | 1.64 ms: 1.07x faster                                      |
| fannkuch                 | 405 ms                                                 | 382 ms: 1.06x faster                                       |
| async_tree_cpu_io_mixed  | 749 ms                                                 | 708 ms: 1.06x faster                                       |
| tomli_loads              | 2.30 sec                                               | 2.18 sec: 1.06x faster                                     |
| regex_v8                 | 22.9 ms                                                | 21.8 ms: 1.05x faster                                      |
| xml_etree_iterparse      | 108 ms                                                 | 103 ms: 1.05x faster                                       |
| pickle                   | 11.0 us                                                | 10.6 us: 1.04x faster                                      |
| pickle_dict              | 34.6 us                                                | 33.3 us: 1.04x faster                                      |
| pprint_pformat           | 1.55 sec                                               | 1.50 sec: 1.04x faster                                     |
| sqlglot_normalize        | 113 ms                                                 | 109 ms: 1.04x faster                                       |
| mdp                      | 2.77 sec                                               | 2.68 sec: 1.04x faster                                     |
| meteor_contest           | 109 ms                                                 | 105 ms: 1.03x faster                                       |
| raytrace                 | 309 ms                                                 | 298 ms: 1.03x faster                                       |
| scimark_lu               | 116 ms                                                 | 113 ms: 1.03x faster                                       |
| pickle_pure_python       | 320 us                                                 | 312 us: 1.03x faster                                       |
| sqlglot_optimize         | 55.3 ms                                                | 54.1 ms: 1.02x faster                                      |
| pprint_safe_repr         | 747 ms                                                 | 733 ms: 1.02x faster                                       |
| deepcopy                 | 365 us                                                 | 361 us: 1.01x faster                                       |
| pathlib                  | 18.5 ms                                                | 18.3 ms: 1.01x faster                                      |
| deepcopy_reduce          | 3.22 us                                                | 3.18 us: 1.01x faster                                      |
| unpickle_list            | 5.21 us                                                | 5.17 us: 1.01x faster                                      |
| bench_thread_pool        | 834 us                                                 | 827 us: 1.01x faster                                       |
| regex_effbot             | 3.51 ms                                                | 3.54 ms: 1.01x slower                                      |
| pidigits                 | 194 ms                                                 | 196 ms: 1.01x slower                                       |
| tornado_http             | 98.1 ms                                                | 99.2 ms: 1.01x slower                                      |
| scimark_sor              | 121 ms                                                 | 123 ms: 1.01x slower                                       |
| sqlalchemy_imperative    | 18.3 ms                                                | 18.6 ms: 1.01x slower                                      |
| 2to3                     | 264 ms                                                 | 268 ms: 1.01x slower                                       |
| crypto_pyaes             | 76.7 ms                                                | 77.9 ms: 1.02x slower                                      |
| regex_compile            | 141 ms                                                 | 144 ms: 1.02x slower                                       |
| regex_dna                | 205 ms                                                 | 208 ms: 1.02x slower                                       |
| logging_simple           | 6.22 us                                                | 6.33 us: 1.02x slower                                      |
| mako                     | 10.7 ms                                                | 10.8 ms: 1.02x slower                                      |
| docutils                 | 2.66 sec                                               | 2.71 sec: 1.02x slower                                     |
| pyflate                  | 434 ms                                                 | 443 ms: 1.02x slower                                       |
| float                    | 78.9 ms                                                | 80.7 ms: 1.02x slower                                      |
| scimark_monte_carlo      | 70.7 ms                                                | 72.7 ms: 1.03x slower                                      |
| scimark_fft              | 345 ms                                                 | 356 ms: 1.03x slower                                       |
| pickle_list              | 4.59 us                                                | 4.73 us: 1.03x slower                                      |
| sqlalchemy_declarative   | 140 ms                                                 | 145 ms: 1.03x slower                                       |
| xml_etree_process        | 56.9 ms                                                | 59.0 ms: 1.04x slower                                      |
| logging_format           | 6.81 us                                                | 7.09 us: 1.04x slower                                      |
| create_gc_cycles         | 1.43 ms                                                | 1.50 ms: 1.04x slower                                      |
| dulwich_log              | 64.6 ms                                                | 67.7 ms: 1.05x slower                                      |
| xml_etree_generate       | 81.1 ms                                                | 85.6 ms: 1.06x slower                                      |
| sqlite_synth             | 2.57 us                                                | 2.72 us: 1.06x slower                                      |
| unpickle                 | 13.8 us                                                | 14.9 us: 1.08x slower                                      |
| unpack_sequence          | 43.5 ns                                                | 47.3 ns: 1.09x slower                                      |
| python_startup           | 8.56 ms                                                | 9.34 ms: 1.09x slower                                      |
| python_startup_no_site   | 6.01 ms                                                | 6.78 ms: 1.13x slower                                      |
| async_generators         | 374 ms                                                 | 449 ms: 1.20x slower                                       |
| coverage                 | 78.8 ms                                                | 96.8 ms: 1.23x slower                                      |
| dask                     | 365 ms                                                 | 535 ms: 1.47x slower                                       |
| Geometric mean           | (ref)                                                  | 1.06x faster                                               |

Benchmark hidden because not significant (5): telco, bench_mp_pool, spectral_norm, pycparser, scimark_sparse_mat_mult
Ignored benchmarks (21) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, chameleon, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 97.19% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.09x