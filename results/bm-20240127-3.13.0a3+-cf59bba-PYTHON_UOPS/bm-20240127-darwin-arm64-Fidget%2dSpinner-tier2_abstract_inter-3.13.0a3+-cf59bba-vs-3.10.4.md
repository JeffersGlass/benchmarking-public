
# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: darwin-arm64
- commit hash: cf59bba
- commit date: 2024-01-27
- overall geometric mean: 1.13x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x faster
- Memory change: 1.13x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 175 ms: 1.10x faster                                                             |
| chameleon      | 6.26 ms                                                | 4.98 ms: 1.26x faster                                                            |
| docutils       | 1.73 sec                                               | 1.51 sec: 1.15x faster                                                           |
| tornado_http   | 86.7 ms                                                | 69.2 ms: 1.25x faster                                                            |
| Geometric mean | (ref)                                                  | 1.19x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 258 ms: 1.50x faster                                                             |
| async_tree_memoization  | 474 ms                                                 | 334 ms: 1.42x faster                                                             |
| async_tree_io           | 980 ms                                                 | 708 ms: 1.38x faster                                                             |
| async_tree_cpu_io_mixed | 649 ms                                                 | 527 ms: 1.23x faster                                                             |
| Geometric mean          | (ref)                                                  | 1.38x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 81.7 ms: 1.14x faster                                                            |
| float          | 69.0 ms                                                | 67.3 ms: 1.02x faster                                                            |
| pidigits       | 282 ms                                                 | 284 ms: 1.01x slower                                                             |
| Geometric mean | (ref)                                                  | 1.05x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 82.1 ms: 1.16x faster                                                            |
| regex_dna      | 174 ms                                                 | 157 ms: 1.11x faster                                                             |
| regex_v8       | 17.1 ms                                                | 18.1 ms: 1.06x slower                                                            |
| regex_effbot   | 2.46 ms                                                | 2.78 ms: 1.13x slower                                                            |
| Geometric mean | (ref)                                                  | 1.02x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 197 us: 1.42x faster                                                             |
| json_dumps           | 8.11 ms                                                | 6.54 ms: 1.24x faster                                                            |
| unpickle_pure_python | 194 us                                                 | 163 us: 1.20x faster                                                             |
| xml_etree_process    | 46.5 ms                                                | 40.7 ms: 1.14x faster                                                            |
| tomli_loads          | 1.71 sec                                               | 1.64 sec: 1.04x faster                                                           |
| xml_etree_parse      | 108 ms                                                 | 107 ms: 1.01x faster                                                             |
| pickle               | 6.97 us                                                | 7.23 us: 1.04x slower                                                            |
| unpickle             | 8.80 us                                                | 9.20 us: 1.05x slower                                                            |
| json_loads           | 16.4 us                                                | 17.2 us: 1.05x slower                                                            |
| pickle_dict          | 17.0 us                                                | 18.1 us: 1.07x slower                                                            |
| pickle_list          | 2.74 us                                                | 2.98 us: 1.09x slower                                                            |
| xml_etree_generate   | 53.5 ms                                                | 58.5 ms: 1.09x slower                                                            |
| xml_etree_iterparse  | 72.1 ms                                                | 80.7 ms: 1.12x slower                                                            |
| unpickle_list        | 2.69 us                                                | 3.04 us: 1.13x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 12.7 ms: 1.17x slower                                                            |
| python_startup_no_site | 7.91 ms                                                | 11.4 ms: 1.44x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.30x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 9.87 ms                                                | 9.64 ms: 1.02x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 73.6 us: 4.39x faster                                                            |
| raytrace                 | 301 ms                                                 | 184 ms: 1.64x faster                                                             |
| logging_silent           | 117 ns                                                 | 71.9 ns: 1.63x faster                                                            |
| asyncio_tcp              | 659 ms                                                 | 409 ms: 1.61x faster                                                             |
| richards_super           | 57.8 ms                                                | 36.5 ms: 1.58x faster                                                            |
| sqlglot_parse            | 1.24 ms                                                | 812 us: 1.53x faster                                                             |
| async_tree_none          | 388 ms                                                 | 258 ms: 1.50x faster                                                             |
| richards                 | 48.7 ms                                                | 32.6 ms: 1.49x faster                                                            |
| chaos                    | 65.8 ms                                                | 45.3 ms: 1.45x faster                                                            |
| sqlglot_transpile        | 1.44 ms                                                | 995 us: 1.45x faster                                                             |
| pickle_pure_python       | 281 us                                                 | 197 us: 1.42x faster                                                             |
| async_tree_memoization   | 474 ms                                                 | 334 ms: 1.42x faster                                                             |
| unpack_sequence          | 39.0 ns                                                | 28.1 ns: 1.39x faster                                                            |
| deltablue                | 4.91 ms                                                | 3.54 ms: 1.39x faster                                                            |
| async_tree_io            | 980 ms                                                 | 708 ms: 1.38x faster                                                             |
| go                       | 151 ms                                                 | 112 ms: 1.35x faster                                                             |
| scimark_lu               | 103 ms                                                 | 76.8 ms: 1.34x faster                                                            |
| crypto_pyaes             | 71.8 ms                                                | 54.8 ms: 1.31x faster                                                            |
| deepcopy_memo            | 34.7 us                                                | 26.5 us: 1.31x faster                                                            |
| chameleon                | 6.26 ms                                                | 4.98 ms: 1.26x faster                                                            |
| tornado_http             | 86.7 ms                                                | 69.2 ms: 1.25x faster                                                            |
| logging_simple           | 4.45 us                                                | 3.56 us: 1.25x faster                                                            |
| logging_format           | 4.83 us                                                | 3.87 us: 1.25x faster                                                            |
| pycparser                | 877 ms                                                 | 704 ms: 1.24x faster                                                             |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.29 sec: 1.24x faster                                                           |
| json_dumps               | 8.11 ms                                                | 6.54 ms: 1.24x faster                                                            |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 527 ms: 1.23x faster                                                             |
| create_gc_cycles         | 860 us                                                 | 707 us: 1.22x faster                                                             |
| scimark_sor              | 128 ms                                                 | 106 ms: 1.21x faster                                                             |
| deepcopy                 | 272 us                                                 | 227 us: 1.20x faster                                                             |
| unpickle_pure_python     | 194 us                                                 | 163 us: 1.20x faster                                                             |
| dulwich_log              | 35.3 ms                                                | 30.0 ms: 1.18x faster                                                            |
| scimark_monte_carlo      | 65.6 ms                                                | 56.3 ms: 1.17x faster                                                            |
| pyflate                  | 427 ms                                                 | 367 ms: 1.16x faster                                                             |
| deepcopy_reduce          | 2.33 us                                                | 2.01 us: 1.16x faster                                                            |
| regex_compile            | 95.3 ms                                                | 82.1 ms: 1.16x faster                                                            |
| sympy_sum                | 92.2 ms                                                | 79.5 ms: 1.16x faster                                                            |
| mypy2                    | 607 ms                                                 | 525 ms: 1.16x faster                                                             |
| docutils                 | 1.73 sec                                               | 1.51 sec: 1.15x faster                                                           |
| xml_etree_process        | 46.5 ms                                                | 40.7 ms: 1.14x faster                                                            |
| nbody                    | 93.0 ms                                                | 81.7 ms: 1.14x faster                                                            |
| sympy_integrate          | 13.1 ms                                                | 11.6 ms: 1.13x faster                                                            |
| pprint_safe_repr         | 641 ms                                                 | 566 ms: 1.13x faster                                                             |
| generators               | 32.3 ms                                                | 28.7 ms: 1.13x faster                                                            |
| dask                     | 253 ms                                                 | 226 ms: 1.12x faster                                                             |
| pprint_pformat           | 1.30 sec                                               | 1.16 sec: 1.12x faster                                                           |
| comprehensions           | 16.9 us                                                | 15.2 us: 1.11x faster                                                            |
| regex_dna                | 174 ms                                                 | 157 ms: 1.11x faster                                                             |
| sympy_str                | 165 ms                                                 | 150 ms: 1.11x faster                                                             |
| 2to3                     | 192 ms                                                 | 175 ms: 1.10x faster                                                             |
| sympy_expand             | 269 ms                                                 | 246 ms: 1.09x faster                                                             |
| coroutines               | 20.7 ms                                                | 19.4 ms: 1.07x faster                                                            |
| hexiom                   | 6.19 ms                                                | 5.89 ms: 1.05x faster                                                            |
| json                     | 3.08 ms                                                | 2.97 ms: 1.04x faster                                                            |
| tomli_loads              | 1.71 sec                                               | 1.64 sec: 1.04x faster                                                           |
| bench_thread_pool        | 527 us                                                 | 512 us: 1.03x faster                                                             |
| sqlglot_optimize         | 36.8 ms                                                | 35.9 ms: 1.03x faster                                                            |
| float                    | 69.0 ms                                                | 67.3 ms: 1.02x faster                                                            |
| mako                     | 9.87 ms                                                | 9.64 ms: 1.02x faster                                                            |
| xml_etree_parse          | 108 ms                                                 | 107 ms: 1.01x faster                                                             |
| meteor_contest           | 77.7 ms                                                | 77.1 ms: 1.01x faster                                                            |
| mdp                      | 1.63 sec                                               | 1.62 sec: 1.01x faster                                                           |
| sqlglot_normalize        | 190 ms                                                 | 191 ms: 1.00x slower                                                             |
| pidigits                 | 282 ms                                                 | 284 ms: 1.01x slower                                                             |
| spectral_norm            | 94.8 ms                                                | 98.2 ms: 1.04x slower                                                            |
| pickle                   | 6.97 us                                                | 7.23 us: 1.04x slower                                                            |
| unpickle                 | 8.80 us                                                | 9.20 us: 1.05x slower                                                            |
| json_loads               | 16.4 us                                                | 17.2 us: 1.05x slower                                                            |
| scimark_fft              | 224 ms                                                 | 235 ms: 1.05x slower                                                             |
| nqueens                  | 63.8 ms                                                | 67.3 ms: 1.05x slower                                                            |
| regex_v8                 | 17.1 ms                                                | 18.1 ms: 1.06x slower                                                            |
| fannkuch                 | 303 ms                                                 | 321 ms: 1.06x slower                                                             |
| pickle_dict              | 17.0 us                                                | 18.1 us: 1.07x slower                                                            |
| gc_traversal             | 2.36 ms                                                | 2.55 ms: 1.08x slower                                                            |
| pickle_list              | 2.74 us                                                | 2.98 us: 1.09x slower                                                            |
| xml_etree_generate       | 53.5 ms                                                | 58.5 ms: 1.09x slower                                                            |
| xml_etree_iterparse      | 72.1 ms                                                | 80.7 ms: 1.12x slower                                                            |
| sqlite_synth             | 1.46 us                                                | 1.64 us: 1.12x slower                                                            |
| unpickle_list            | 2.69 us                                                | 3.04 us: 1.13x slower                                                            |
| regex_effbot             | 2.46 ms                                                | 2.78 ms: 1.13x slower                                                            |
| coverage                 | 41.5 ms                                                | 47.9 ms: 1.16x slower                                                            |
| python_startup           | 10.9 ms                                                | 12.7 ms: 1.17x slower                                                            |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 4.04 ms: 1.18x slower                                                            |
| bench_mp_pool            | 37.4 ms                                                | 45.7 ms: 1.22x slower                                                            |
| async_generators         | 231 ms                                                 | 299 ms: 1.29x slower                                                             |
| telco                    | 3.49 ms                                                | 4.64 ms: 1.33x slower                                                            |
| python_startup_no_site   | 7.91 ms                                                | 11.4 ms: 1.44x slower                                                            |
| Geometric mean           | (ref)                                                  | 1.13x faster                                                                     |

Benchmark hidden because not significant (2): asyncio_websockets, pathlib
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240127-3.13.0a3+-cf59bba-PYTHON_UOPS/bm-20240127-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.09x
- 95% likely to have a speedup of 1.08x
- 99% likely to have a speedup of 1.04x


# Memory

- memory change: 1.13x