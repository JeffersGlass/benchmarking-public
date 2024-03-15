
# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: darwin-arm64
- commit hash: 0929bb8
- commit date: 2024-01-16
- overall geometric mean: 1.12x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x faster
- Memory change: 1.41x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a2+-0929bb8 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 176 ms: 1.09x faster                                                             |
| chameleon      | 6.26 ms                                                | 5.16 ms: 1.21x faster                                                            |
| docutils       | 1.73 sec                                               | 1.51 sec: 1.15x faster                                                           |
| tornado_http   | 86.7 ms                                                | 69.6 ms: 1.25x faster                                                            |
| Geometric mean | (ref)                                                  | 1.17x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a2+-0929bb8 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 259 ms: 1.50x faster                                                             |
| async_tree_memoization  | 474 ms                                                 | 337 ms: 1.40x faster                                                             |
| async_tree_io           | 980 ms                                                 | 716 ms: 1.37x faster                                                             |
| async_tree_cpu_io_mixed | 649 ms                                                 | 528 ms: 1.23x faster                                                             |
| Geometric mean          | (ref)                                                  | 1.37x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a2+-0929bb8 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| float          | 69.0 ms                                                | 68.1 ms: 1.01x faster                                                            |
| pidigits       | 282 ms                                                 | 284 ms: 1.00x slower                                                             |
| nbody          | 93.0 ms                                                | 118 ms: 1.26x slower                                                             |
| Geometric mean | (ref)                                                  | 1.08x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a2+-0929bb8 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 82.0 ms: 1.16x faster                                                            |
| regex_dna      | 174 ms                                                 | 156 ms: 1.12x faster                                                             |
| regex_v8       | 17.1 ms                                                | 17.9 ms: 1.04x slower                                                            |
| regex_effbot   | 2.46 ms                                                | 2.75 ms: 1.12x slower                                                            |
| Geometric mean | (ref)                                                  | 1.03x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a2+-0929bb8 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 197 us: 1.42x faster                                                             |
| json_dumps           | 8.11 ms                                                | 6.58 ms: 1.23x faster                                                            |
| unpickle_pure_python | 194 us                                                 | 164 us: 1.18x faster                                                             |
| xml_etree_process    | 46.5 ms                                                | 40.6 ms: 1.15x faster                                                            |
| tomli_loads          | 1.71 sec                                               | 1.64 sec: 1.04x faster                                                           |
| xml_etree_parse      | 108 ms                                                 | 107 ms: 1.01x faster                                                             |
| json_loads           | 16.4 us                                                | 17.1 us: 1.04x slower                                                            |
| unpickle             | 8.80 us                                                | 9.17 us: 1.04x slower                                                            |
| pickle_dict          | 17.0 us                                                | 18.2 us: 1.07x slower                                                            |
| pickle               | 6.97 us                                                | 7.48 us: 1.07x slower                                                            |
| pickle_list          | 2.74 us                                                | 2.95 us: 1.08x slower                                                            |
| xml_etree_generate   | 53.5 ms                                                | 59.4 ms: 1.11x slower                                                            |
| xml_etree_iterparse  | 72.1 ms                                                | 80.4 ms: 1.11x slower                                                            |
| unpickle_list        | 2.69 us                                                | 3.00 us: 1.12x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a2+-0929bb8 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 12.3 ms: 1.13x slower                                                            |
| python_startup_no_site | 7.91 ms                                                | 11.0 ms: 1.39x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.26x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a2+-0929bb8 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 9.87 ms                                                | 9.66 ms: 1.02x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a2+-0929bb8 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 74.3 us: 4.35x faster                                                            |
| asyncio_tcp              | 659 ms                                                 | 374 ms: 1.76x faster                                                             |
| logging_silent           | 117 ns                                                 | 72.1 ns: 1.63x faster                                                            |
| raytrace                 | 301 ms                                                 | 186 ms: 1.62x faster                                                             |
| richards_super           | 57.8 ms                                                | 36.9 ms: 1.57x faster                                                            |
| sqlglot_parse            | 1.24 ms                                                | 813 us: 1.53x faster                                                             |
| async_tree_none          | 388 ms                                                 | 259 ms: 1.50x faster                                                             |
| richards                 | 48.7 ms                                                | 32.6 ms: 1.49x faster                                                            |
| sqlglot_transpile        | 1.44 ms                                                | 994 us: 1.45x faster                                                             |
| pickle_pure_python       | 281 us                                                 | 197 us: 1.42x faster                                                             |
| async_tree_memoization   | 474 ms                                                 | 337 ms: 1.40x faster                                                             |
| deltablue                | 4.91 ms                                                | 3.58 ms: 1.37x faster                                                            |
| async_tree_io            | 980 ms                                                 | 716 ms: 1.37x faster                                                             |
| chaos                    | 65.8 ms                                                | 48.4 ms: 1.36x faster                                                            |
| go                       | 151 ms                                                 | 111 ms: 1.36x faster                                                             |
| scimark_lu               | 103 ms                                                 | 76.5 ms: 1.34x faster                                                            |
| crypto_pyaes             | 71.8 ms                                                | 54.7 ms: 1.31x faster                                                            |
| unpack_sequence          | 39.0 ns                                                | 29.9 ns: 1.31x faster                                                            |
| deepcopy_memo            | 34.7 us                                                | 26.7 us: 1.30x faster                                                            |
| logging_format           | 4.83 us                                                | 3.85 us: 1.26x faster                                                            |
| tornado_http             | 86.7 ms                                                | 69.6 ms: 1.25x faster                                                            |
| logging_simple           | 4.45 us                                                | 3.57 us: 1.25x faster                                                            |
| pycparser                | 877 ms                                                 | 706 ms: 1.24x faster                                                             |
| json_dumps               | 8.11 ms                                                | 6.58 ms: 1.23x faster                                                            |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 528 ms: 1.23x faster                                                             |
| create_gc_cycles         | 860 us                                                 | 704 us: 1.22x faster                                                             |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.31 sec: 1.22x faster                                                           |
| chameleon                | 6.26 ms                                                | 5.16 ms: 1.21x faster                                                            |
| deepcopy                 | 272 us                                                 | 226 us: 1.20x faster                                                             |
| scimark_sor              | 128 ms                                                 | 107 ms: 1.20x faster                                                             |
| unpickle_pure_python     | 194 us                                                 | 164 us: 1.18x faster                                                             |
| dulwich_log              | 35.3 ms                                                | 30.1 ms: 1.17x faster                                                            |
| deepcopy_reduce          | 2.33 us                                                | 1.99 us: 1.17x faster                                                            |
| pyflate                  | 427 ms                                                 | 366 ms: 1.17x faster                                                             |
| regex_compile            | 95.3 ms                                                | 82.0 ms: 1.16x faster                                                            |
| docutils                 | 1.73 sec                                               | 1.51 sec: 1.15x faster                                                           |
| scimark_monte_carlo      | 65.6 ms                                                | 57.1 ms: 1.15x faster                                                            |
| mypy2                    | 607 ms                                                 | 529 ms: 1.15x faster                                                             |
| xml_etree_process        | 46.5 ms                                                | 40.6 ms: 1.15x faster                                                            |
| sympy_sum                | 92.2 ms                                                | 80.6 ms: 1.14x faster                                                            |
| regex_dna                | 174 ms                                                 | 156 ms: 1.12x faster                                                             |
| generators               | 32.3 ms                                                | 28.9 ms: 1.12x faster                                                            |
| sympy_integrate          | 13.1 ms                                                | 11.8 ms: 1.11x faster                                                            |
| dask                     | 253 ms                                                 | 228 ms: 1.11x faster                                                             |
| sympy_str                | 165 ms                                                 | 149 ms: 1.11x faster                                                             |
| sympy_expand             | 269 ms                                                 | 246 ms: 1.09x faster                                                             |
| 2to3                     | 192 ms                                                 | 176 ms: 1.09x faster                                                             |
| pprint_safe_repr         | 641 ms                                                 | 590 ms: 1.09x faster                                                             |
| pprint_pformat           | 1.30 sec                                               | 1.21 sec: 1.08x faster                                                           |
| comprehensions           | 16.9 us                                                | 15.7 us: 1.08x faster                                                            |
| json                     | 3.08 ms                                                | 2.94 ms: 1.05x faster                                                            |
| coroutines               | 20.7 ms                                                | 19.8 ms: 1.05x faster                                                            |
| tomli_loads              | 1.71 sec                                               | 1.64 sec: 1.04x faster                                                           |
| hexiom                   | 6.19 ms                                                | 5.97 ms: 1.04x faster                                                            |
| mako                     | 9.87 ms                                                | 9.66 ms: 1.02x faster                                                            |
| sqlglot_optimize         | 36.8 ms                                                | 36.0 ms: 1.02x faster                                                            |
| bench_thread_pool        | 527 us                                                 | 517 us: 1.02x faster                                                             |
| meteor_contest           | 77.7 ms                                                | 76.7 ms: 1.01x faster                                                            |
| float                    | 69.0 ms                                                | 68.1 ms: 1.01x faster                                                            |
| xml_etree_parse          | 108 ms                                                 | 107 ms: 1.01x faster                                                             |
| mdp                      | 1.63 sec                                               | 1.62 sec: 1.00x faster                                                           |
| pidigits                 | 282 ms                                                 | 284 ms: 1.00x slower                                                             |
| gc_traversal             | 2.36 ms                                                | 2.40 ms: 1.02x slower                                                            |
| json_loads               | 16.4 us                                                | 17.1 us: 1.04x slower                                                            |
| unpickle                 | 8.80 us                                                | 9.17 us: 1.04x slower                                                            |
| pathlib                  | 24.5 ms                                                | 25.6 ms: 1.04x slower                                                            |
| regex_v8                 | 17.1 ms                                                | 17.9 ms: 1.04x slower                                                            |
| fannkuch                 | 303 ms                                                 | 316 ms: 1.05x slower                                                             |
| nqueens                  | 63.8 ms                                                | 67.7 ms: 1.06x slower                                                            |
| spectral_norm            | 94.8 ms                                                | 101 ms: 1.07x slower                                                             |
| pickle_dict              | 17.0 us                                                | 18.2 us: 1.07x slower                                                            |
| pickle                   | 6.97 us                                                | 7.48 us: 1.07x slower                                                            |
| pickle_list              | 2.74 us                                                | 2.95 us: 1.08x slower                                                            |
| xml_etree_generate       | 53.5 ms                                                | 59.4 ms: 1.11x slower                                                            |
| xml_etree_iterparse      | 72.1 ms                                                | 80.4 ms: 1.11x slower                                                            |
| unpickle_list            | 2.69 us                                                | 3.00 us: 1.12x slower                                                            |
| regex_effbot             | 2.46 ms                                                | 2.75 ms: 1.12x slower                                                            |
| sqlite_synth             | 1.46 us                                                | 1.64 us: 1.12x slower                                                            |
| python_startup           | 10.9 ms                                                | 12.3 ms: 1.13x slower                                                            |
| scimark_fft              | 224 ms                                                 | 255 ms: 1.14x slower                                                             |
| coverage                 | 41.5 ms                                                | 47.4 ms: 1.14x slower                                                            |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 4.06 ms: 1.19x slower                                                            |
| bench_mp_pool            | 37.4 ms                                                | 45.4 ms: 1.22x slower                                                            |
| nbody                    | 93.0 ms                                                | 118 ms: 1.26x slower                                                             |
| async_generators         | 231 ms                                                 | 299 ms: 1.29x slower                                                             |
| telco                    | 3.49 ms                                                | 4.68 ms: 1.34x slower                                                            |
| python_startup_no_site   | 7.91 ms                                                | 11.0 ms: 1.39x slower                                                            |
| Geometric mean           | (ref)                                                  | 1.12x faster                                                                     |

Benchmark hidden because not significant (2): asyncio_websockets, sqlglot_normalize
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240116-3.13.0a2+-0929bb8-PYTHON_UOPS/bm-20240116-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a2+-0929bb8.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.07x
- 95% likely to have a speedup of 1.06x
- 99% likely to have a speedup of 1.04x


# Memory

- memory change: 1.41x