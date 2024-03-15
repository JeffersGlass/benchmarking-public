
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin
- machine: linux-x86_64
- commit hash: 4d3e207
- commit date: 2024-01-25
- overall geometric mean: 1.30x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.22x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 276 ms: 1.26x faster                                           |
| chameleon      | 9.68 ms                                                | 6.96 ms: 1.39x faster                                          |
| docutils       | 3.30 sec                                               | 2.66 sec: 1.24x faster                                         |
| tornado_http   | 136 ms                                                 | 97.4 ms: 1.40x faster                                          |
| Geometric mean | (ref)                                                  | 1.32x faster                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 446 ms: 1.63x faster                                           |
| async_tree_memoization  | 870 ms                                                 | 572 ms: 1.52x faster                                           |
| async_tree_io           | 1.77 sec                                               | 1.19 sec: 1.48x faster                                         |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 715 ms: 1.42x faster                                           |
| Geometric mean          | (ref)                                                  | 1.51x faster                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 104 ms: 1.48x faster                                           |
| float          | 117 ms                                                 | 87.1 ms: 1.34x faster                                          |
| pidigits       | 191 ms                                                 | 188 ms: 1.02x faster                                           |
| Geometric mean | (ref)                                                  | 1.27x faster                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 141 ms: 1.34x faster                                           |
| regex_v8       | 27.8 ms                                                | 25.5 ms: 1.09x faster                                          |
| regex_dna      | 227 ms                                                 | 220 ms: 1.03x faster                                           |
| Geometric mean | (ref)                                                  | 1.11x faster                                                   |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 293 us: 1.65x faster                                           |
| unpickle_pure_python | 331 us                                                 | 229 us: 1.44x faster                                           |
| tomli_loads          | 3.14 sec                                               | 2.20 sec: 1.43x faster                                         |
| json_dumps           | 14.2 ms                                                | 10.3 ms: 1.37x faster                                          |
| xml_etree_process    | 79.1 ms                                                | 59.4 ms: 1.33x faster                                          |
| xml_etree_generate   | 99.4 ms                                                | 87.9 ms: 1.13x faster                                          |
| json_loads           | 31.2 us                                                | 28.2 us: 1.11x faster                                          |
| xml_etree_parse      | 168 ms                                                 | 158 ms: 1.07x faster                                           |
| xml_etree_iterparse  | 115 ms                                                 | 109 ms: 1.06x faster                                           |
| unpickle_list        | 5.20 us                                                | 5.35 us: 1.03x slower                                          |
| pickle_list          | 5.08 us                                                | 5.23 us: 1.03x slower                                          |
| unpickle             | 14.4 us                                                | 15.5 us: 1.08x slower                                          |
| pickle               | 10.7 us                                                | 11.7 us: 1.10x slower                                          |
| pickle_dict          | 29.6 us                                                | 34.0 us: 1.15x slower                                          |
| Geometric mean       | (ref)                                                  | 1.14x faster                                                   |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.43x faster                                          |
| python_startup_no_site | 5.93 ms                                                | 8.82 ms: 1.49x slower                                          |
| Geometric mean         | (ref)                                                  | 1.02x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 12.7 ms: 1.29x faster                                          |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 111 us: 4.88x faster                                           |
| generators               | 80.1 ms                                                | 29.2 ms: 2.74x faster                                          |
| deltablue                | 7.91 ms                                                | 4.05 ms: 1.95x faster                                          |
| asyncio_tcp              | 922 ms                                                 | 490 ms: 1.88x faster                                           |
| richards_super           | 94.7 ms                                                | 51.9 ms: 1.83x faster                                          |
| raytrace                 | 507 ms                                                 | 282 ms: 1.80x faster                                           |
| logging_silent           | 190 ns                                                 | 106 ns: 1.78x faster                                           |
| scimark_sor              | 220 ms                                                 | 123 ms: 1.78x faster                                           |
| richards                 | 79.3 ms                                                | 46.0 ms: 1.72x faster                                          |
| sqlglot_parse            | 2.17 ms                                                | 1.28 ms: 1.69x faster                                          |
| pickle_pure_python       | 484 us                                                 | 293 us: 1.65x faster                                           |
| async_tree_none          | 728 ms                                                 | 446 ms: 1.63x faster                                           |
| chaos                    | 115 ms                                                 | 70.8 ms: 1.63x faster                                          |
| crypto_pyaes             | 128 ms                                                 | 79.3 ms: 1.61x faster                                          |
| go                       | 240 ms                                                 | 149 ms: 1.61x faster                                           |
| sqlglot_transpile        | 2.57 ms                                                | 1.62 ms: 1.59x faster                                          |
| scimark_monte_carlo      | 118 ms                                                 | 74.6 ms: 1.58x faster                                          |
| coroutines               | 35.1 ms                                                | 22.5 ms: 1.56x faster                                          |
| scimark_lu               | 176 ms                                                 | 114 ms: 1.54x faster                                           |
| async_tree_memoization   | 870 ms                                                 | 572 ms: 1.52x faster                                           |
| deepcopy_memo            | 58.5 us                                                | 39.2 us: 1.49x faster                                          |
| async_tree_io            | 1.77 sec                                               | 1.19 sec: 1.48x faster                                         |
| nbody                    | 154 ms                                                 | 104 ms: 1.48x faster                                           |
| comprehensions           | 28.8 us                                                | 19.6 us: 1.47x faster                                          |
| unpickle_pure_python     | 331 us                                                 | 229 us: 1.44x faster                                           |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.79 sec: 1.43x faster                                         |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.43x faster                                          |
| logging_simple           | 8.30 us                                                | 5.81 us: 1.43x faster                                          |
| logging_format           | 9.09 us                                                | 6.37 us: 1.43x faster                                          |
| tomli_loads              | 3.14 sec                                               | 2.20 sec: 1.43x faster                                         |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 715 ms: 1.42x faster                                           |
| tornado_http             | 136 ms                                                 | 97.4 ms: 1.40x faster                                          |
| pyflate                  | 716 ms                                                 | 513 ms: 1.40x faster                                           |
| chameleon                | 9.68 ms                                                | 6.96 ms: 1.39x faster                                          |
| json_dumps               | 14.2 ms                                                | 10.3 ms: 1.37x faster                                          |
| deepcopy                 | 479 us                                                 | 350 us: 1.37x faster                                           |
| deepcopy_reduce          | 4.17 us                                                | 3.09 us: 1.35x faster                                          |
| float                    | 117 ms                                                 | 87.1 ms: 1.34x faster                                          |
| regex_compile            | 188 ms                                                 | 141 ms: 1.34x faster                                           |
| xml_etree_process        | 79.1 ms                                                | 59.4 ms: 1.33x faster                                          |
| pycparser                | 1.58 sec                                               | 1.20 sec: 1.31x faster                                         |
| hexiom                   | 10.4 ms                                                | 7.98 ms: 1.30x faster                                          |
| sqlglot_normalize        | 143 ms                                                 | 110 ms: 1.30x faster                                           |
| mako                     | 16.3 ms                                                | 12.7 ms: 1.29x faster                                          |
| 2to3                     | 348 ms                                                 | 276 ms: 1.26x faster                                           |
| dulwich_log              | 84.3 ms                                                | 67.9 ms: 1.24x faster                                          |
| docutils                 | 3.30 sec                                               | 2.66 sec: 1.24x faster                                         |
| pprint_pformat           | 2.10 sec                                               | 1.70 sec: 1.24x faster                                         |
| sympy_integrate          | 25.8 ms                                                | 20.9 ms: 1.24x faster                                          |
| pprint_safe_repr         | 1.02 sec                                               | 827 ms: 1.23x faster                                           |
| fannkuch                 | 532 ms                                                 | 433 ms: 1.23x faster                                           |
| sympy_sum                | 196 ms                                                 | 160 ms: 1.22x faster                                           |
| sqlglot_optimize         | 69.2 ms                                                | 56.5 ms: 1.22x faster                                          |
| scimark_fft              | 466 ms                                                 | 382 ms: 1.22x faster                                           |
| sympy_str                | 346 ms                                                 | 285 ms: 1.21x faster                                           |
| unpack_sequence          | 60.0 ns                                                | 49.7 ns: 1.21x faster                                          |
| dask                     | 441 ms                                                 | 366 ms: 1.20x faster                                           |
| spectral_norm            | 170 ms                                                 | 141 ms: 1.20x faster                                           |
| sympy_expand             | 566 ms                                                 | 479 ms: 1.18x faster                                           |
| bench_thread_pool        | 986 us                                                 | 837 us: 1.18x faster                                           |
| nqueens                  | 106 ms                                                 | 89.9 ms: 1.18x faster                                          |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.55 ms: 1.17x faster                                          |
| xml_etree_generate       | 99.4 ms                                                | 87.9 ms: 1.13x faster                                          |
| pathlib                  | 20.5 ms                                                | 18.2 ms: 1.12x faster                                          |
| json                     | 5.69 ms                                                | 5.11 ms: 1.11x faster                                          |
| json_loads               | 31.2 us                                                | 28.2 us: 1.11x faster                                          |
| regex_v8                 | 27.8 ms                                                | 25.5 ms: 1.09x faster                                          |
| create_gc_cycles         | 1.62 ms                                                | 1.50 ms: 1.08x faster                                          |
| meteor_contest           | 120 ms                                                 | 111 ms: 1.08x faster                                           |
| mdp                      | 2.85 sec                                               | 2.64 sec: 1.08x faster                                         |
| sqlite_synth             | 3.02 us                                                | 2.84 us: 1.07x faster                                          |
| xml_etree_parse          | 168 ms                                                 | 158 ms: 1.07x faster                                           |
| xml_etree_iterparse      | 115 ms                                                 | 109 ms: 1.06x faster                                           |
| regex_dna                | 227 ms                                                 | 220 ms: 1.03x faster                                           |
| pidigits                 | 191 ms                                                 | 188 ms: 1.02x faster                                           |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                           |
| async_generators         | 444 ms                                                 | 452 ms: 1.02x slower                                           |
| unpickle_list            | 5.20 us                                                | 5.35 us: 1.03x slower                                          |
| pickle_list              | 5.08 us                                                | 5.23 us: 1.03x slower                                          |
| gc_traversal             | 3.62 ms                                                | 3.77 ms: 1.04x slower                                          |
| unpickle                 | 14.4 us                                                | 15.5 us: 1.08x slower                                          |
| pickle                   | 10.7 us                                                | 11.7 us: 1.10x slower                                          |
| pickle_dict              | 29.6 us                                                | 34.0 us: 1.15x slower                                          |
| telco                    | 7.27 ms                                                | 8.54 ms: 1.18x slower                                          |
| coverage                 | 79.4 ms                                                | 94.1 ms: 1.18x slower                                          |
| python_startup_no_site   | 5.93 ms                                                | 8.82 ms: 1.49x slower                                          |
| Geometric mean           | (ref)                                                  | 1.30x faster                                                   |

Benchmark hidden because not significant (3): mypy2, regex_effbot, bench_mp_pool
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240125-3.13.0a3+-4d3e207-JIT/bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.24x
- 95% likely to have a speedup of 1.24x
- 99% likely to have a speedup of 1.22x


# Memory

- memory change: 1.10x