
# Results vs. 3.12.0

- fork: python
- ref: v3.11.5
- machine: linux-x86_64
- commit hash: cce6ba9
- commit date: 2023-08-24
- overall geometric mean: 1.07x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 0.91x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230824-pythonperf2-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| chameleon      | 7.23 ms                                                      | 7.28 ms: 1.01x slower                                        |
| docutils       | 2.87 sec                                                     | 2.84 sec: 1.01x faster                                       |
| tornado_http   | 121 ms                                                       | 124 ms: 1.02x slower                                         |
| Geometric mean | (ref)                                                        | 1.00x slower                                                 |

Benchmark hidden because not significant (1): 2to3

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230824-pythonperf2-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|-------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 696 ms                                                       | 765 ms: 1.10x slower                                         |
| async_tree_io           | 1.04 sec                                                     | 1.17 sec: 1.13x slower                                       |
| async_tree_none         | 452 ms                                                       | 518 ms: 1.15x slower                                         |
| async_tree_memoization  | 544 ms                                                       | 624 ms: 1.15x slower                                         |
| Geometric mean          | (ref)                                                        | 1.13x slower                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230824-pythonperf2-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 251 ms: 1.06x faster                                         |
| float          | 76.6 ms                                                      | 74.3 ms: 1.03x faster                                        |
| nbody          | 88.0 ms                                                      | 90.5 ms: 1.03x slower                                        |
| Geometric mean | (ref)                                                        | 1.02x faster                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230824-pythonperf2-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.31 ms: 1.08x faster                                        |
| regex_dna      | 239 ms                                                       | 227 ms: 1.05x faster                                         |
| regex_v8       | 23.6 ms                                                      | 24.2 ms: 1.02x slower                                        |
| regex_compile  | 144 ms                                                       | 155 ms: 1.08x slower                                         |
| Geometric mean | (ref)                                                        | 1.01x faster                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230824-pythonperf2-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| pickle_list          | 4.43 us                                                      | 3.94 us: 1.12x faster                                        |
| unpickle             | 14.8 us                                                      | 13.3 us: 1.11x faster                                        |
| xml_etree_generate   | 86.1 ms                                                      | 80.8 ms: 1.07x faster                                        |
| pickle               | 10.5 us                                                      | 9.98 us: 1.06x faster                                        |
| xml_etree_process    | 58.4 ms                                                      | 56.1 ms: 1.04x faster                                        |
| pickle_pure_python   | 318 us                                                       | 320 us: 1.00x slower                                         |
| pickle_dict          | 32.5 us                                                      | 33.1 us: 1.02x slower                                        |
| tomli_loads          | 2.16 sec                                                     | 2.30 sec: 1.06x slower                                       |
| xml_etree_parse      | 144 ms                                                       | 157 ms: 1.09x slower                                         |
| json_loads           | 24.4 us                                                      | 27.9 us: 1.15x slower                                        |
| unpickle_pure_python | 210 us                                                       | 241 us: 1.15x slower                                         |
| json_dumps           | 10.2 ms                                                      | 13.5 ms: 1.32x slower                                        |
| Geometric mean       | (ref)                                                        | 1.02x slower                                                 |

Benchmark hidden because not significant (2): unpickle_list, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230824-pythonperf2-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup_no_site | 8.64 ms                                                      | 7.79 ms: 1.11x faster                                        |
| python_startup         | 11.6 ms                                                      | 10.8 ms: 1.08x faster                                        |
| Geometric mean         | (ref)                                                        | 1.09x faster                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230824-pythonperf2-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|-----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| mako            | 10.0 ms                                                      | 10.6 ms: 1.06x slower                                        |
| django_template | 38.2 ms                                                      | 40.7 ms: 1.07x slower                                        |
| Geometric mean  | (ref)                                                        | 1.06x slower                                                 |

All benchmarks:
===============

| Benchmark                | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230824-pythonperf2-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|--------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| async_generators         | 390 ms                                                       | 318 ms: 1.23x faster                                         |
| unpack_sequence          | 53.2 ns                                                      | 46.9 ns: 1.13x faster                                        |
| pickle_list              | 4.43 us                                                      | 3.94 us: 1.12x faster                                        |
| unpickle                 | 14.8 us                                                      | 13.3 us: 1.11x faster                                        |
| python_startup_no_site   | 8.64 ms                                                      | 7.79 ms: 1.11x faster                                        |
| sqlite_synth             | 2.77 us                                                      | 2.55 us: 1.09x faster                                        |
| regex_effbot             | 3.57 ms                                                      | 3.31 ms: 1.08x faster                                        |
| python_startup           | 11.6 ms                                                      | 10.8 ms: 1.08x faster                                        |
| scimark_fft              | 301 ms                                                       | 280 ms: 1.07x faster                                         |
| xml_etree_generate       | 86.1 ms                                                      | 80.8 ms: 1.07x faster                                        |
| pidigits                 | 265 ms                                                       | 251 ms: 1.06x faster                                         |
| pickle                   | 10.5 us                                                      | 9.98 us: 1.06x faster                                        |
| scimark_sparse_mat_mult  | 4.21 ms                                                      | 4.00 ms: 1.05x faster                                        |
| regex_dna                | 239 ms                                                       | 227 ms: 1.05x faster                                         |
| pprint_safe_repr         | 807 ms                                                       | 775 ms: 1.04x faster                                         |
| xml_etree_process        | 58.4 ms                                                      | 56.1 ms: 1.04x faster                                        |
| sqlalchemy_declarative   | 159 ms                                                       | 154 ms: 1.03x faster                                         |
| telco                    | 6.96 ms                                                      | 6.75 ms: 1.03x faster                                        |
| float                    | 76.6 ms                                                      | 74.3 ms: 1.03x faster                                        |
| pprint_pformat           | 1.65 sec                                                     | 1.61 sec: 1.03x faster                                       |
| aiohttp                  | 1.02 ms                                                      | 991 us: 1.03x faster                                         |
| docutils                 | 2.87 sec                                                     | 2.84 sec: 1.01x faster                                       |
| pickle_pure_python       | 318 us                                                       | 320 us: 1.00x slower                                         |
| pyflate                  | 439 ms                                                       | 441 ms: 1.00x slower                                         |
| pathlib                  | 18.9 ms                                                      | 19.0 ms: 1.01x slower                                        |
| chameleon                | 7.23 ms                                                      | 7.28 ms: 1.01x slower                                        |
| deepcopy_reduce          | 3.37 us                                                      | 3.40 us: 1.01x slower                                        |
| pickle_dict              | 32.5 us                                                      | 33.1 us: 1.02x slower                                        |
| deepcopy_memo            | 36.8 us                                                      | 37.4 us: 1.02x slower                                        |
| crypto_pyaes             | 80.3 ms                                                      | 81.7 ms: 1.02x slower                                        |
| create_gc_cycles         | 1.59 ms                                                      | 1.62 ms: 1.02x slower                                        |
| spectral_norm            | 91.6 ms                                                      | 93.3 ms: 1.02x slower                                        |
| tornado_http             | 121 ms                                                       | 124 ms: 1.02x slower                                         |
| scimark_sor              | 109 ms                                                       | 111 ms: 1.02x slower                                         |
| regex_v8                 | 23.6 ms                                                      | 24.2 ms: 1.02x slower                                        |
| meteor_contest           | 128 ms                                                       | 131 ms: 1.02x slower                                         |
| sqlglot_optimize         | 57.5 ms                                                      | 58.9 ms: 1.02x slower                                        |
| nbody                    | 88.0 ms                                                      | 90.5 ms: 1.03x slower                                        |
| sqlalchemy_imperative    | 18.7 ms                                                      | 19.5 ms: 1.04x slower                                        |
| bench_thread_pool        | 950 us                                                       | 989 us: 1.04x slower                                         |
| dask                     | 392 ms                                                       | 409 ms: 1.04x slower                                         |
| logging_format           | 7.48 us                                                      | 7.83 us: 1.05x slower                                        |
| logging_silent           | 94.4 ns                                                      | 100 ns: 1.06x slower                                         |
| mako                     | 10.0 ms                                                      | 10.6 ms: 1.06x slower                                        |
| tomli_loads              | 2.16 sec                                                     | 2.30 sec: 1.06x slower                                       |
| django_template          | 38.2 ms                                                      | 40.7 ms: 1.07x slower                                        |
| raytrace                 | 298 ms                                                       | 318 ms: 1.07x slower                                         |
| sympy_integrate          | 23.9 ms                                                      | 25.6 ms: 1.07x slower                                        |
| pycparser                | 1.23 sec                                                     | 1.32 sec: 1.07x slower                                       |
| deepcopy                 | 368 us                                                       | 396 us: 1.07x slower                                         |
| sqlglot_normalize        | 116 ms                                                       | 124 ms: 1.08x slower                                         |
| sqlglot_transpile        | 1.78 ms                                                      | 1.91 ms: 1.08x slower                                        |
| regex_compile            | 144 ms                                                       | 155 ms: 1.08x slower                                         |
| mdp                      | 2.57 sec                                                     | 2.78 sec: 1.08x slower                                       |
| json                     | 5.12 ms                                                      | 5.55 ms: 1.09x slower                                        |
| gc_traversal             | 3.48 ms                                                      | 3.77 ms: 1.09x slower                                        |
| go                       | 150 ms                                                       | 163 ms: 1.09x slower                                         |
| logging_simple           | 6.71 us                                                      | 7.33 us: 1.09x slower                                        |
| xml_etree_parse          | 144 ms                                                       | 157 ms: 1.09x slower                                         |
| async_tree_cpu_io_mixed  | 696 ms                                                       | 765 ms: 1.10x slower                                         |
| sympy_str                | 302 ms                                                       | 336 ms: 1.11x slower                                         |
| sqlglot_parse            | 1.38 ms                                                      | 1.54 ms: 1.12x slower                                        |
| async_tree_io            | 1.04 sec                                                     | 1.17 sec: 1.13x slower                                       |
| richards                 | 45.7 ms                                                      | 51.6 ms: 1.13x slower                                        |
| nqueens                  | 89.9 ms                                                      | 102 ms: 1.13x slower                                         |
| sympy_sum                | 162 ms                                                       | 184 ms: 1.14x slower                                         |
| comprehensions           | 21.9 us                                                      | 25.0 us: 1.14x slower                                        |
| json_loads               | 24.4 us                                                      | 27.9 us: 1.15x slower                                        |
| async_tree_none          | 452 ms                                                       | 518 ms: 1.15x slower                                         |
| sympy_expand             | 484 ms                                                       | 555 ms: 1.15x slower                                         |
| async_tree_memoization   | 544 ms                                                       | 624 ms: 1.15x slower                                         |
| scimark_lu               | 98.8 ms                                                      | 113 ms: 1.15x slower                                         |
| unpickle_pure_python     | 210 us                                                       | 241 us: 1.15x slower                                         |
| coroutines               | 23.0 ms                                                      | 27.7 ms: 1.20x slower                                        |
| hexiom                   | 5.96 ms                                                      | 7.21 ms: 1.21x slower                                        |
| chaos                    | 64.0 ms                                                      | 79.1 ms: 1.24x slower                                        |
| deltablue                | 3.24 ms                                                      | 4.03 ms: 1.24x slower                                        |
| richards_super           | 51.3 ms                                                      | 64.3 ms: 1.25x slower                                        |
| json_dumps               | 10.2 ms                                                      | 13.5 ms: 1.32x slower                                        |
| fannkuch                 | 350 ms                                                       | 470 ms: 1.34x slower                                         |
| generators               | 37.4 ms                                                      | 55.4 ms: 1.48x slower                                        |
| asyncio_tcp_ssl          | 1.59 sec                                                     | 3.08 sec: 1.94x slower                                       |
| asyncio_tcp              | 378 ms                                                       | 753 ms: 1.99x slower                                         |
| typing_runtime_protocols | 152 us                                                       | 518 us: 3.42x slower                                         |
| Geometric mean           | (ref)                                                        | 1.07x slower                                                 |

Benchmark hidden because not significant (7): unpickle_list, bench_mp_pool, gunicorn, dulwich_log, 2to3, scimark_monte_carlo, xml_etree_iterparse
Ignored benchmarks (7) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, coverage, mypy2
Ignored benchmarks (6) of results/bm-20230824-3.11.5-cce6ba9/bm-20230824-pythonperf2-x86_64-python-v3.11.5-3.11.5-cce6ba9.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 0.91x