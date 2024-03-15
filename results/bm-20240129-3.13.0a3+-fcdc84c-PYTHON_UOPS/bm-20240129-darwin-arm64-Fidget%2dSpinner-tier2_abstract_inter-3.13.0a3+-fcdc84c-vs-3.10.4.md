
# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: darwin-arm64
- commit hash: fcdc84c
- commit date: 2024-01-29
- overall geometric mean: 1.13x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x faster
- Memory change: 1.12x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 174 ms: 1.10x faster                                                             |
| chameleon      | 6.26 ms                                                | 5.07 ms: 1.24x faster                                                            |
| docutils       | 1.73 sec                                               | 1.49 sec: 1.16x faster                                                           |
| tornado_http   | 86.7 ms                                                | 69.6 ms: 1.25x faster                                                            |
| Geometric mean | (ref)                                                  | 1.18x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 258 ms: 1.51x faster                                                             |
| async_tree_memoization  | 474 ms                                                 | 334 ms: 1.42x faster                                                             |
| async_tree_io           | 980 ms                                                 | 709 ms: 1.38x faster                                                             |
| async_tree_cpu_io_mixed | 649 ms                                                 | 527 ms: 1.23x faster                                                             |
| Geometric mean          | (ref)                                                  | 1.38x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 81.9 ms: 1.14x faster                                                            |
| float          | 69.0 ms                                                | 67.0 ms: 1.03x faster                                                            |
| pidigits       | 282 ms                                                 | 284 ms: 1.00x slower                                                             |
| Geometric mean | (ref)                                                  | 1.05x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 81.8 ms: 1.16x faster                                                            |
| regex_dna      | 174 ms                                                 | 157 ms: 1.11x faster                                                             |
| regex_v8       | 17.1 ms                                                | 18.0 ms: 1.05x slower                                                            |
| regex_effbot   | 2.46 ms                                                | 2.78 ms: 1.13x slower                                                            |
| Geometric mean | (ref)                                                  | 1.02x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 196 us: 1.43x faster                                                             |
| json_dumps           | 8.11 ms                                                | 6.56 ms: 1.24x faster                                                            |
| unpickle_pure_python | 194 us                                                 | 164 us: 1.19x faster                                                             |
| xml_etree_process    | 46.5 ms                                                | 40.6 ms: 1.15x faster                                                            |
| tomli_loads          | 1.71 sec                                               | 1.62 sec: 1.05x faster                                                           |
| unpickle             | 8.80 us                                                | 9.17 us: 1.04x slower                                                            |
| json_loads           | 16.4 us                                                | 17.2 us: 1.04x slower                                                            |
| pickle               | 6.97 us                                                | 7.30 us: 1.05x slower                                                            |
| pickle_dict          | 17.0 us                                                | 18.1 us: 1.07x slower                                                            |
| pickle_list          | 2.74 us                                                | 2.97 us: 1.08x slower                                                            |
| xml_etree_generate   | 53.5 ms                                                | 58.5 ms: 1.09x slower                                                            |
| xml_etree_iterparse  | 72.1 ms                                                | 80.8 ms: 1.12x slower                                                            |
| unpickle_list        | 2.69 us                                                | 3.03 us: 1.13x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                                     |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 12.9 ms: 1.18x slower                                                            |
| python_startup_no_site | 7.91 ms                                                | 11.5 ms: 1.46x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.31x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 9.87 ms                                                | 9.65 ms: 1.02x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 73.1 us: 4.42x faster                                                            |
| raytrace                 | 301 ms                                                 | 184 ms: 1.63x faster                                                             |
| logging_silent           | 117 ns                                                 | 72.3 ns: 1.62x faster                                                            |
| richards_super           | 57.8 ms                                                | 36.5 ms: 1.59x faster                                                            |
| sqlglot_parse            | 1.24 ms                                                | 810 us: 1.53x faster                                                             |
| async_tree_none          | 388 ms                                                 | 258 ms: 1.51x faster                                                             |
| asyncio_tcp              | 659 ms                                                 | 440 ms: 1.50x faster                                                             |
| richards                 | 48.7 ms                                                | 32.8 ms: 1.49x faster                                                            |
| sqlglot_transpile        | 1.44 ms                                                | 992 us: 1.45x faster                                                             |
| chaos                    | 65.8 ms                                                | 45.5 ms: 1.45x faster                                                            |
| pickle_pure_python       | 281 us                                                 | 196 us: 1.43x faster                                                             |
| async_tree_memoization   | 474 ms                                                 | 334 ms: 1.42x faster                                                             |
| deltablue                | 4.91 ms                                                | 3.52 ms: 1.40x faster                                                            |
| async_tree_io            | 980 ms                                                 | 709 ms: 1.38x faster                                                             |
| scimark_lu               | 103 ms                                                 | 75.4 ms: 1.36x faster                                                            |
| go                       | 151 ms                                                 | 111 ms: 1.36x faster                                                             |
| unpack_sequence          | 39.0 ns                                                | 29.2 ns: 1.34x faster                                                            |
| deepcopy_memo            | 34.7 us                                                | 26.7 us: 1.30x faster                                                            |
| crypto_pyaes             | 71.8 ms                                                | 55.2 ms: 1.30x faster                                                            |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.27 sec: 1.27x faster                                                           |
| logging_format           | 4.83 us                                                | 3.85 us: 1.26x faster                                                            |
| pycparser                | 877 ms                                                 | 701 ms: 1.25x faster                                                             |
| logging_simple           | 4.45 us                                                | 3.57 us: 1.25x faster                                                            |
| tornado_http             | 86.7 ms                                                | 69.6 ms: 1.25x faster                                                            |
| json_dumps               | 8.11 ms                                                | 6.56 ms: 1.24x faster                                                            |
| chameleon                | 6.26 ms                                                | 5.07 ms: 1.24x faster                                                            |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 527 ms: 1.23x faster                                                             |
| create_gc_cycles         | 860 us                                                 | 704 us: 1.22x faster                                                             |
| scimark_sor              | 128 ms                                                 | 106 ms: 1.21x faster                                                             |
| deepcopy                 | 272 us                                                 | 227 us: 1.20x faster                                                             |
| unpickle_pure_python     | 194 us                                                 | 164 us: 1.19x faster                                                             |
| dulwich_log              | 35.3 ms                                                | 30.0 ms: 1.18x faster                                                            |
| scimark_monte_carlo      | 65.6 ms                                                | 56.1 ms: 1.17x faster                                                            |
| deepcopy_reduce          | 2.33 us                                                | 2.00 us: 1.17x faster                                                            |
| regex_compile            | 95.3 ms                                                | 81.8 ms: 1.16x faster                                                            |
| sympy_sum                | 92.2 ms                                                | 79.3 ms: 1.16x faster                                                            |
| pyflate                  | 427 ms                                                 | 367 ms: 1.16x faster                                                             |
| docutils                 | 1.73 sec                                               | 1.49 sec: 1.16x faster                                                           |
| mypy2                    | 607 ms                                                 | 525 ms: 1.16x faster                                                             |
| xml_etree_process        | 46.5 ms                                                | 40.6 ms: 1.15x faster                                                            |
| sympy_integrate          | 13.1 ms                                                | 11.5 ms: 1.14x faster                                                            |
| nbody                    | 93.0 ms                                                | 81.9 ms: 1.14x faster                                                            |
| pprint_safe_repr         | 641 ms                                                 | 567 ms: 1.13x faster                                                             |
| generators               | 32.3 ms                                                | 28.7 ms: 1.13x faster                                                            |
| comprehensions           | 16.9 us                                                | 15.1 us: 1.12x faster                                                            |
| pprint_pformat           | 1.30 sec                                               | 1.16 sec: 1.12x faster                                                           |
| dask                     | 253 ms                                                 | 227 ms: 1.11x faster                                                             |
| sympy_str                | 165 ms                                                 | 149 ms: 1.11x faster                                                             |
| regex_dna                | 174 ms                                                 | 157 ms: 1.11x faster                                                             |
| 2to3                     | 192 ms                                                 | 174 ms: 1.10x faster                                                             |
| sympy_expand             | 269 ms                                                 | 245 ms: 1.10x faster                                                             |
| hexiom                   | 6.19 ms                                                | 5.87 ms: 1.06x faster                                                            |
| tomli_loads              | 1.71 sec                                               | 1.62 sec: 1.05x faster                                                           |
| coroutines               | 20.7 ms                                                | 19.7 ms: 1.05x faster                                                            |
| json                     | 3.08 ms                                                | 2.95 ms: 1.05x faster                                                            |
| bench_thread_pool        | 527 us                                                 | 510 us: 1.03x faster                                                             |
| float                    | 69.0 ms                                                | 67.0 ms: 1.03x faster                                                            |
| mako                     | 9.87 ms                                                | 9.65 ms: 1.02x faster                                                            |
| sqlglot_optimize         | 36.8 ms                                                | 36.0 ms: 1.02x faster                                                            |
| mdp                      | 1.63 sec                                               | 1.61 sec: 1.01x faster                                                           |
| meteor_contest           | 77.7 ms                                                | 77.1 ms: 1.01x faster                                                            |
| sqlglot_normalize        | 190 ms                                                 | 191 ms: 1.00x slower                                                             |
| pidigits                 | 282 ms                                                 | 284 ms: 1.00x slower                                                             |
| gc_traversal             | 2.36 ms                                                | 2.40 ms: 1.02x slower                                                            |
| spectral_norm            | 94.8 ms                                                | 96.6 ms: 1.02x slower                                                            |
| pathlib                  | 24.5 ms                                                | 24.9 ms: 1.02x slower                                                            |
| scimark_fft              | 224 ms                                                 | 233 ms: 1.04x slower                                                             |
| unpickle                 | 8.80 us                                                | 9.17 us: 1.04x slower                                                            |
| json_loads               | 16.4 us                                                | 17.2 us: 1.04x slower                                                            |
| pickle                   | 6.97 us                                                | 7.30 us: 1.05x slower                                                            |
| fannkuch                 | 303 ms                                                 | 318 ms: 1.05x slower                                                             |
| regex_v8                 | 17.1 ms                                                | 18.0 ms: 1.05x slower                                                            |
| nqueens                  | 63.8 ms                                                | 67.1 ms: 1.05x slower                                                            |
| pickle_dict              | 17.0 us                                                | 18.1 us: 1.07x slower                                                            |
| pickle_list              | 2.74 us                                                | 2.97 us: 1.08x slower                                                            |
| xml_etree_generate       | 53.5 ms                                                | 58.5 ms: 1.09x slower                                                            |
| xml_etree_iterparse      | 72.1 ms                                                | 80.8 ms: 1.12x slower                                                            |
| unpickle_list            | 2.69 us                                                | 3.03 us: 1.13x slower                                                            |
| sqlite_synth             | 1.46 us                                                | 1.65 us: 1.13x slower                                                            |
| regex_effbot             | 2.46 ms                                                | 2.78 ms: 1.13x slower                                                            |
| coverage                 | 41.5 ms                                                | 47.1 ms: 1.14x slower                                                            |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 3.96 ms: 1.16x slower                                                            |
| python_startup           | 10.9 ms                                                | 12.9 ms: 1.18x slower                                                            |
| bench_mp_pool            | 37.4 ms                                                | 45.4 ms: 1.22x slower                                                            |
| async_generators         | 231 ms                                                 | 297 ms: 1.28x slower                                                             |
| telco                    | 3.49 ms                                                | 4.63 ms: 1.33x slower                                                            |
| python_startup_no_site   | 7.91 ms                                                | 11.5 ms: 1.46x slower                                                            |
| Geometric mean           | (ref)                                                  | 1.13x faster                                                                     |

Benchmark hidden because not significant (2): xml_etree_parse, asyncio_websockets
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240129-3.13.0a3+-fcdc84c-PYTHON_UOPS/bm-20240129-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.09x
- 95% likely to have a speedup of 1.08x
- 99% likely to have a speedup of 1.05x


# Memory

- memory change: 1.12x