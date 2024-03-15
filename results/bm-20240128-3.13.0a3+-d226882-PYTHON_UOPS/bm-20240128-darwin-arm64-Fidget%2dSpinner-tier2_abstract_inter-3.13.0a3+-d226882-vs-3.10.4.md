
# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: darwin-arm64
- commit hash: d226882
- commit date: 2024-01-28
- overall geometric mean: 1.13x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x faster
- Memory change: 1.12x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 174 ms: 1.10x faster                                                             |
| chameleon      | 6.26 ms                                                | 5.06 ms: 1.24x faster                                                            |
| docutils       | 1.73 sec                                               | 1.50 sec: 1.15x faster                                                           |
| tornado_http   | 86.7 ms                                                | 68.7 ms: 1.26x faster                                                            |
| Geometric mean | (ref)                                                  | 1.19x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 258 ms: 1.50x faster                                                             |
| async_tree_memoization  | 474 ms                                                 | 334 ms: 1.42x faster                                                             |
| async_tree_io           | 980 ms                                                 | 710 ms: 1.38x faster                                                             |
| async_tree_cpu_io_mixed | 649 ms                                                 | 526 ms: 1.23x faster                                                             |
| Geometric mean          | (ref)                                                  | 1.38x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 82.1 ms: 1.13x faster                                                            |
| float          | 69.0 ms                                                | 67.0 ms: 1.03x faster                                                            |
| pidigits       | 282 ms                                                 | 284 ms: 1.01x slower                                                             |
| Geometric mean | (ref)                                                  | 1.05x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 81.5 ms: 1.17x faster                                                            |
| regex_dna      | 174 ms                                                 | 159 ms: 1.10x faster                                                             |
| regex_v8       | 17.1 ms                                                | 18.2 ms: 1.06x slower                                                            |
| regex_effbot   | 2.46 ms                                                | 2.81 ms: 1.14x slower                                                            |
| Geometric mean | (ref)                                                  | 1.02x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 197 us: 1.42x faster                                                             |
| json_dumps           | 8.11 ms                                                | 6.57 ms: 1.23x faster                                                            |
| unpickle_pure_python | 194 us                                                 | 163 us: 1.19x faster                                                             |
| xml_etree_process    | 46.5 ms                                                | 40.9 ms: 1.14x faster                                                            |
| tomli_loads          | 1.71 sec                                               | 1.64 sec: 1.04x faster                                                           |
| pickle               | 6.97 us                                                | 7.23 us: 1.04x slower                                                            |
| unpickle             | 8.80 us                                                | 9.14 us: 1.04x slower                                                            |
| json_loads           | 16.4 us                                                | 17.1 us: 1.04x slower                                                            |
| pickle_dict          | 17.0 us                                                | 18.1 us: 1.07x slower                                                            |
| pickle_list          | 2.74 us                                                | 2.97 us: 1.09x slower                                                            |
| xml_etree_generate   | 53.5 ms                                                | 58.3 ms: 1.09x slower                                                            |
| unpickle_list        | 2.69 us                                                | 3.03 us: 1.13x slower                                                            |
| xml_etree_iterparse  | 72.1 ms                                                | 81.4 ms: 1.13x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                                     |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 12.8 ms: 1.18x slower                                                            |
| python_startup_no_site | 7.91 ms                                                | 11.5 ms: 1.45x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.31x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 9.87 ms                                                | 9.60 ms: 1.03x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 73.3 us: 4.41x faster                                                            |
| raytrace                 | 301 ms                                                 | 185 ms: 1.63x faster                                                             |
| logging_silent           | 117 ns                                                 | 71.9 ns: 1.63x faster                                                            |
| asyncio_tcp              | 659 ms                                                 | 411 ms: 1.61x faster                                                             |
| richards_super           | 57.8 ms                                                | 36.5 ms: 1.59x faster                                                            |
| sqlglot_parse            | 1.24 ms                                                | 812 us: 1.53x faster                                                             |
| async_tree_none          | 388 ms                                                 | 258 ms: 1.50x faster                                                             |
| richards                 | 48.7 ms                                                | 32.6 ms: 1.49x faster                                                            |
| sqlglot_transpile        | 1.44 ms                                                | 991 us: 1.46x faster                                                             |
| chaos                    | 65.8 ms                                                | 45.6 ms: 1.44x faster                                                            |
| pickle_pure_python       | 281 us                                                 | 197 us: 1.42x faster                                                             |
| async_tree_memoization   | 474 ms                                                 | 334 ms: 1.42x faster                                                             |
| deltablue                | 4.91 ms                                                | 3.52 ms: 1.40x faster                                                            |
| unpack_sequence          | 39.0 ns                                                | 28.1 ns: 1.39x faster                                                            |
| async_tree_io            | 980 ms                                                 | 710 ms: 1.38x faster                                                             |
| go                       | 151 ms                                                 | 112 ms: 1.35x faster                                                             |
| scimark_lu               | 103 ms                                                 | 76.9 ms: 1.34x faster                                                            |
| crypto_pyaes             | 71.8 ms                                                | 55.1 ms: 1.30x faster                                                            |
| deepcopy_memo            | 34.7 us                                                | 26.6 us: 1.30x faster                                                            |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.24 sec: 1.29x faster                                                           |
| tornado_http             | 86.7 ms                                                | 68.7 ms: 1.26x faster                                                            |
| logging_format           | 4.83 us                                                | 3.84 us: 1.26x faster                                                            |
| logging_simple           | 4.45 us                                                | 3.54 us: 1.26x faster                                                            |
| pycparser                | 877 ms                                                 | 703 ms: 1.25x faster                                                             |
| chameleon                | 6.26 ms                                                | 5.06 ms: 1.24x faster                                                            |
| json_dumps               | 8.11 ms                                                | 6.57 ms: 1.23x faster                                                            |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 526 ms: 1.23x faster                                                             |
| create_gc_cycles         | 860 us                                                 | 711 us: 1.21x faster                                                             |
| scimark_sor              | 128 ms                                                 | 106 ms: 1.21x faster                                                             |
| deepcopy                 | 272 us                                                 | 226 us: 1.20x faster                                                             |
| unpickle_pure_python     | 194 us                                                 | 163 us: 1.19x faster                                                             |
| dulwich_log              | 35.3 ms                                                | 30.0 ms: 1.18x faster                                                            |
| sympy_sum                | 92.2 ms                                                | 78.7 ms: 1.17x faster                                                            |
| regex_compile            | 95.3 ms                                                | 81.5 ms: 1.17x faster                                                            |
| scimark_monte_carlo      | 65.6 ms                                                | 56.3 ms: 1.17x faster                                                            |
| pyflate                  | 427 ms                                                 | 367 ms: 1.16x faster                                                             |
| deepcopy_reduce          | 2.33 us                                                | 2.00 us: 1.16x faster                                                            |
| mypy2                    | 607 ms                                                 | 524 ms: 1.16x faster                                                             |
| docutils                 | 1.73 sec                                               | 1.50 sec: 1.15x faster                                                           |
| sympy_integrate          | 13.1 ms                                                | 11.5 ms: 1.14x faster                                                            |
| xml_etree_process        | 46.5 ms                                                | 40.9 ms: 1.14x faster                                                            |
| nbody                    | 93.0 ms                                                | 82.1 ms: 1.13x faster                                                            |
| generators               | 32.3 ms                                                | 28.6 ms: 1.13x faster                                                            |
| pprint_safe_repr         | 641 ms                                                 | 567 ms: 1.13x faster                                                             |
| pprint_pformat           | 1.30 sec                                               | 1.16 sec: 1.12x faster                                                           |
| sympy_str                | 165 ms                                                 | 148 ms: 1.12x faster                                                             |
| comprehensions           | 16.9 us                                                | 15.2 us: 1.12x faster                                                            |
| dask                     | 253 ms                                                 | 228 ms: 1.11x faster                                                             |
| 2to3                     | 192 ms                                                 | 174 ms: 1.10x faster                                                             |
| regex_dna                | 174 ms                                                 | 159 ms: 1.10x faster                                                             |
| sympy_expand             | 269 ms                                                 | 245 ms: 1.10x faster                                                             |
| coroutines               | 20.7 ms                                                | 19.5 ms: 1.06x faster                                                            |
| hexiom                   | 6.19 ms                                                | 5.88 ms: 1.05x faster                                                            |
| tomli_loads              | 1.71 sec                                               | 1.64 sec: 1.04x faster                                                           |
| json                     | 3.08 ms                                                | 2.96 ms: 1.04x faster                                                            |
| bench_thread_pool        | 527 us                                                 | 512 us: 1.03x faster                                                             |
| float                    | 69.0 ms                                                | 67.0 ms: 1.03x faster                                                            |
| mako                     | 9.87 ms                                                | 9.60 ms: 1.03x faster                                                            |
| sqlglot_optimize         | 36.8 ms                                                | 35.8 ms: 1.03x faster                                                            |
| meteor_contest           | 77.7 ms                                                | 77.1 ms: 1.01x faster                                                            |
| mdp                      | 1.63 sec                                               | 1.62 sec: 1.01x faster                                                           |
| sqlglot_normalize        | 190 ms                                                 | 190 ms: 1.00x faster                                                             |
| pidigits                 | 282 ms                                                 | 284 ms: 1.01x slower                                                             |
| gc_traversal             | 2.36 ms                                                | 2.41 ms: 1.02x slower                                                            |
| spectral_norm            | 94.8 ms                                                | 98.2 ms: 1.04x slower                                                            |
| pickle                   | 6.97 us                                                | 7.23 us: 1.04x slower                                                            |
| unpickle                 | 8.80 us                                                | 9.14 us: 1.04x slower                                                            |
| scimark_fft              | 224 ms                                                 | 233 ms: 1.04x slower                                                             |
| json_loads               | 16.4 us                                                | 17.1 us: 1.04x slower                                                            |
| nqueens                  | 63.8 ms                                                | 67.4 ms: 1.06x slower                                                            |
| regex_v8                 | 17.1 ms                                                | 18.2 ms: 1.06x slower                                                            |
| pickle_dict              | 17.0 us                                                | 18.1 us: 1.07x slower                                                            |
| fannkuch                 | 303 ms                                                 | 323 ms: 1.07x slower                                                             |
| pickle_list              | 2.74 us                                                | 2.97 us: 1.09x slower                                                            |
| xml_etree_generate       | 53.5 ms                                                | 58.3 ms: 1.09x slower                                                            |
| sqlite_synth             | 1.46 us                                                | 1.63 us: 1.12x slower                                                            |
| unpickle_list            | 2.69 us                                                | 3.03 us: 1.13x slower                                                            |
| xml_etree_iterparse      | 72.1 ms                                                | 81.4 ms: 1.13x slower                                                            |
| regex_effbot             | 2.46 ms                                                | 2.81 ms: 1.14x slower                                                            |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 3.96 ms: 1.16x slower                                                            |
| python_startup           | 10.9 ms                                                | 12.8 ms: 1.18x slower                                                            |
| bench_mp_pool            | 37.4 ms                                                | 45.5 ms: 1.22x slower                                                            |
| coverage                 | 41.5 ms                                                | 51.0 ms: 1.23x slower                                                            |
| async_generators         | 231 ms                                                 | 298 ms: 1.29x slower                                                             |
| telco                    | 3.49 ms                                                | 4.61 ms: 1.32x slower                                                            |
| python_startup_no_site   | 7.91 ms                                                | 11.5 ms: 1.45x slower                                                            |
| Geometric mean           | (ref)                                                  | 1.13x faster                                                                     |

Benchmark hidden because not significant (3): xml_etree_parse, asyncio_websockets, pathlib
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240128-3.13.0a3+-d226882-PYTHON_UOPS/bm-20240128-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.09x
- 95% likely to have a speedup of 1.08x
- 99% likely to have a speedup of 1.05x


# Memory

- memory change: 1.12x