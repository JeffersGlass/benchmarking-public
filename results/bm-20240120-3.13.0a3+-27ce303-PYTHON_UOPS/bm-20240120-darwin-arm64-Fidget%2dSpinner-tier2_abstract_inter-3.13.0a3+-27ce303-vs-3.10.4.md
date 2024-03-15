
# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: darwin-arm64
- commit hash: 27ce303
- commit date: 2024-01-20
- overall geometric mean: 1.13x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x faster
- Memory change: 1.41x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 175 ms: 1.09x faster                                                             |
| chameleon      | 6.26 ms                                                | 5.00 ms: 1.25x faster                                                            |
| docutils       | 1.73 sec                                               | 1.50 sec: 1.16x faster                                                           |
| tornado_http   | 86.7 ms                                                | 70.4 ms: 1.23x faster                                                            |
| Geometric mean | (ref)                                                  | 1.18x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 260 ms: 1.49x faster                                                             |
| async_tree_memoization  | 474 ms                                                 | 338 ms: 1.40x faster                                                             |
| async_tree_io           | 980 ms                                                 | 715 ms: 1.37x faster                                                             |
| async_tree_cpu_io_mixed | 649 ms                                                 | 529 ms: 1.23x faster                                                             |
| Geometric mean          | (ref)                                                  | 1.37x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 85.6 ms: 1.09x faster                                                            |
| float          | 69.0 ms                                                | 68.0 ms: 1.01x faster                                                            |
| pidigits       | 282 ms                                                 | 284 ms: 1.00x slower                                                             |
| Geometric mean | (ref)                                                  | 1.03x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 81.8 ms: 1.16x faster                                                            |
| regex_dna      | 174 ms                                                 | 155 ms: 1.12x faster                                                             |
| regex_v8       | 17.1 ms                                                | 17.9 ms: 1.04x slower                                                            |
| regex_effbot   | 2.46 ms                                                | 2.75 ms: 1.12x slower                                                            |
| Geometric mean | (ref)                                                  | 1.03x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 197 us: 1.43x faster                                                             |
| json_dumps           | 8.11 ms                                                | 6.57 ms: 1.23x faster                                                            |
| unpickle_pure_python | 194 us                                                 | 164 us: 1.19x faster                                                             |
| xml_etree_process    | 46.5 ms                                                | 40.7 ms: 1.14x faster                                                            |
| tomli_loads          | 1.71 sec                                               | 1.66 sec: 1.03x faster                                                           |
| unpickle             | 8.80 us                                                | 9.17 us: 1.04x slower                                                            |
| json_loads           | 16.4 us                                                | 17.2 us: 1.05x slower                                                            |
| pickle               | 6.97 us                                                | 7.45 us: 1.07x slower                                                            |
| pickle_list          | 2.74 us                                                | 2.93 us: 1.07x slower                                                            |
| pickle_dict          | 17.0 us                                                | 18.2 us: 1.07x slower                                                            |
| xml_etree_generate   | 53.5 ms                                                | 58.7 ms: 1.10x slower                                                            |
| xml_etree_iterparse  | 72.1 ms                                                | 81.1 ms: 1.12x slower                                                            |
| unpickle_list        | 2.69 us                                                | 3.04 us: 1.13x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                                     |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 11.8 ms: 1.09x slower                                                            |
| python_startup_no_site | 7.91 ms                                                | 10.5 ms: 1.33x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.20x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 9.87 ms                                                | 9.56 ms: 1.03x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 74.7 us: 4.33x faster                                                            |
| asyncio_tcp              | 659 ms                                                 | 393 ms: 1.68x faster                                                             |
| logging_silent           | 117 ns                                                 | 72.2 ns: 1.62x faster                                                            |
| raytrace                 | 301 ms                                                 | 186 ms: 1.62x faster                                                             |
| richards_super           | 57.8 ms                                                | 36.7 ms: 1.58x faster                                                            |
| sqlglot_parse            | 1.24 ms                                                | 810 us: 1.53x faster                                                             |
| richards                 | 48.7 ms                                                | 32.6 ms: 1.49x faster                                                            |
| async_tree_none          | 388 ms                                                 | 260 ms: 1.49x faster                                                             |
| sqlglot_transpile        | 1.44 ms                                                | 992 us: 1.45x faster                                                             |
| chaos                    | 65.8 ms                                                | 46.1 ms: 1.43x faster                                                            |
| pickle_pure_python       | 281 us                                                 | 197 us: 1.43x faster                                                             |
| async_tree_memoization   | 474 ms                                                 | 338 ms: 1.40x faster                                                             |
| deltablue                | 4.91 ms                                                | 3.58 ms: 1.37x faster                                                            |
| unpack_sequence          | 39.0 ns                                                | 28.4 ns: 1.37x faster                                                            |
| async_tree_io            | 980 ms                                                 | 715 ms: 1.37x faster                                                             |
| go                       | 151 ms                                                 | 111 ms: 1.36x faster                                                             |
| scimark_lu               | 103 ms                                                 | 76.7 ms: 1.34x faster                                                            |
| crypto_pyaes             | 71.8 ms                                                | 54.5 ms: 1.32x faster                                                            |
| deepcopy_memo            | 34.7 us                                                | 26.8 us: 1.29x faster                                                            |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.27 sec: 1.26x faster                                                           |
| logging_format           | 4.83 us                                                | 3.86 us: 1.25x faster                                                            |
| chameleon                | 6.26 ms                                                | 5.00 ms: 1.25x faster                                                            |
| logging_simple           | 4.45 us                                                | 3.56 us: 1.25x faster                                                            |
| pycparser                | 877 ms                                                 | 704 ms: 1.25x faster                                                             |
| json_dumps               | 8.11 ms                                                | 6.57 ms: 1.23x faster                                                            |
| tornado_http             | 86.7 ms                                                | 70.4 ms: 1.23x faster                                                            |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 529 ms: 1.23x faster                                                             |
| create_gc_cycles         | 860 us                                                 | 702 us: 1.22x faster                                                             |
| scimark_sor              | 128 ms                                                 | 106 ms: 1.21x faster                                                             |
| deepcopy                 | 272 us                                                 | 227 us: 1.20x faster                                                             |
| unpickle_pure_python     | 194 us                                                 | 164 us: 1.19x faster                                                             |
| dulwich_log              | 35.3 ms                                                | 30.0 ms: 1.18x faster                                                            |
| deepcopy_reduce          | 2.33 us                                                | 1.99 us: 1.17x faster                                                            |
| regex_compile            | 95.3 ms                                                | 81.8 ms: 1.16x faster                                                            |
| sympy_sum                | 92.2 ms                                                | 79.5 ms: 1.16x faster                                                            |
| scimark_monte_carlo      | 65.6 ms                                                | 56.7 ms: 1.16x faster                                                            |
| docutils                 | 1.73 sec                                               | 1.50 sec: 1.16x faster                                                           |
| pyflate                  | 427 ms                                                 | 370 ms: 1.15x faster                                                             |
| mypy2                    | 607 ms                                                 | 529 ms: 1.15x faster                                                             |
| xml_etree_process        | 46.5 ms                                                | 40.7 ms: 1.14x faster                                                            |
| sympy_integrate          | 13.1 ms                                                | 11.5 ms: 1.14x faster                                                            |
| generators               | 32.3 ms                                                | 28.7 ms: 1.13x faster                                                            |
| regex_dna                | 174 ms                                                 | 155 ms: 1.12x faster                                                             |
| pprint_safe_repr         | 641 ms                                                 | 572 ms: 1.12x faster                                                             |
| sympy_str                | 165 ms                                                 | 148 ms: 1.12x faster                                                             |
| dask                     | 253 ms                                                 | 227 ms: 1.11x faster                                                             |
| pprint_pformat           | 1.30 sec                                               | 1.18 sec: 1.11x faster                                                           |
| coroutines               | 20.7 ms                                                | 18.9 ms: 1.10x faster                                                            |
| sympy_expand             | 269 ms                                                 | 245 ms: 1.10x faster                                                             |
| 2to3                     | 192 ms                                                 | 175 ms: 1.09x faster                                                             |
| nbody                    | 93.0 ms                                                | 85.6 ms: 1.09x faster                                                            |
| comprehensions           | 16.9 us                                                | 15.6 us: 1.09x faster                                                            |
| hexiom                   | 6.19 ms                                                | 5.95 ms: 1.04x faster                                                            |
| json                     | 3.08 ms                                                | 2.96 ms: 1.04x faster                                                            |
| mako                     | 9.87 ms                                                | 9.56 ms: 1.03x faster                                                            |
| tomli_loads              | 1.71 sec                                               | 1.66 sec: 1.03x faster                                                           |
| sqlglot_optimize         | 36.8 ms                                                | 35.9 ms: 1.03x faster                                                            |
| bench_thread_pool        | 527 us                                                 | 519 us: 1.02x faster                                                             |
| float                    | 69.0 ms                                                | 68.0 ms: 1.01x faster                                                            |
| mdp                      | 1.63 sec                                               | 1.61 sec: 1.01x faster                                                           |
| meteor_contest           | 77.7 ms                                                | 77.4 ms: 1.00x faster                                                            |
| asyncio_websockets       | 410 ms                                                 | 408 ms: 1.00x faster                                                             |
| pidigits                 | 282 ms                                                 | 284 ms: 1.00x slower                                                             |
| gc_traversal             | 2.36 ms                                                | 2.40 ms: 1.02x slower                                                            |
| unpickle                 | 8.80 us                                                | 9.17 us: 1.04x slower                                                            |
| regex_v8                 | 17.1 ms                                                | 17.9 ms: 1.04x slower                                                            |
| fannkuch                 | 303 ms                                                 | 317 ms: 1.05x slower                                                             |
| json_loads               | 16.4 us                                                | 17.2 us: 1.05x slower                                                            |
| scimark_fft              | 224 ms                                                 | 237 ms: 1.06x slower                                                             |
| spectral_norm            | 94.8 ms                                                | 100 ms: 1.06x slower                                                             |
| nqueens                  | 63.8 ms                                                | 67.6 ms: 1.06x slower                                                            |
| pickle                   | 6.97 us                                                | 7.45 us: 1.07x slower                                                            |
| pickle_list              | 2.74 us                                                | 2.93 us: 1.07x slower                                                            |
| pickle_dict              | 17.0 us                                                | 18.2 us: 1.07x slower                                                            |
| python_startup           | 10.9 ms                                                | 11.8 ms: 1.09x slower                                                            |
| xml_etree_generate       | 53.5 ms                                                | 58.7 ms: 1.10x slower                                                            |
| regex_effbot             | 2.46 ms                                                | 2.75 ms: 1.12x slower                                                            |
| xml_etree_iterparse      | 72.1 ms                                                | 81.1 ms: 1.12x slower                                                            |
| unpickle_list            | 2.69 us                                                | 3.04 us: 1.13x slower                                                            |
| sqlite_synth             | 1.46 us                                                | 1.65 us: 1.13x slower                                                            |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 4.11 ms: 1.20x slower                                                            |
| coverage                 | 41.5 ms                                                | 50.0 ms: 1.20x slower                                                            |
| bench_mp_pool            | 37.4 ms                                                | 45.4 ms: 1.21x slower                                                            |
| async_generators         | 231 ms                                                 | 300 ms: 1.30x slower                                                             |
| python_startup_no_site   | 7.91 ms                                                | 10.5 ms: 1.33x slower                                                            |
| telco                    | 3.49 ms                                                | 4.64 ms: 1.33x slower                                                            |
| Geometric mean           | (ref)                                                  | 1.13x faster                                                                     |

Benchmark hidden because not significant (3): xml_etree_parse, sqlglot_normalize, pathlib
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240120-3.13.0a3+-27ce303-PYTHON_UOPS/bm-20240120-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.09x
- 95% likely to have a speedup of 1.08x
- 99% likely to have a speedup of 1.04x


# Memory

- memory change: 1.41x