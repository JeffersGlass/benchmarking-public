
# Results vs. 3.10.4

- fork: mdboom
- ref: compact_long
- machine: darwin-arm64
- commit hash: 39bbca4
- commit date: 2023-12-21
- overall geometric mean: 1.15x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.07x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 178 ms: 1.08x faster                                           |
| chameleon      | 6.26 ms                                                | 5.16 ms: 1.21x faster                                          |
| docutils       | 1.73 sec                                               | 1.51 sec: 1.15x faster                                         |
| tornado_http   | 86.7 ms                                                | 71.2 ms: 1.22x faster                                          |
| Geometric mean | (ref)                                                  | 1.16x faster                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 258 ms: 1.50x faster                                           |
| async_tree_memoization  | 474 ms                                                 | 335 ms: 1.41x faster                                           |
| async_tree_io           | 980 ms                                                 | 713 ms: 1.37x faster                                           |
| async_tree_cpu_io_mixed | 649 ms                                                 | 534 ms: 1.22x faster                                           |
| Geometric mean          | (ref)                                                  | 1.37x faster                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| float          | 69.0 ms                                                | 58.5 ms: 1.18x faster                                          |
| nbody          | 93.0 ms                                                | 81.7 ms: 1.14x faster                                          |
| pidigits       | 282 ms                                                 | 274 ms: 1.03x faster                                           |
| Geometric mean | (ref)                                                  | 1.11x faster                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 80.5 ms: 1.18x faster                                          |
| regex_dna      | 174 ms                                                 | 149 ms: 1.17x faster                                           |
| regex_v8       | 17.1 ms                                                | 16.9 ms: 1.01x faster                                          |
| regex_effbot   | 2.46 ms                                                | 2.57 ms: 1.05x slower                                          |
| Geometric mean | (ref)                                                  | 1.08x faster                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 208 us: 1.35x faster                                           |
| json_dumps           | 8.11 ms                                                | 6.72 ms: 1.21x faster                                          |
| unpickle_pure_python | 194 us                                                 | 166 us: 1.17x faster                                           |
| xml_etree_process    | 46.5 ms                                                | 42.0 ms: 1.11x faster                                          |
| tomli_loads          | 1.71 sec                                               | 1.60 sec: 1.06x faster                                         |
| xml_etree_parse      | 108 ms                                                 | 109 ms: 1.01x slower                                           |
| unpickle             | 8.80 us                                                | 9.13 us: 1.04x slower                                          |
| pickle               | 6.97 us                                                | 7.36 us: 1.06x slower                                          |
| json_loads           | 16.4 us                                                | 17.4 us: 1.06x slower                                          |
| pickle_dict          | 17.0 us                                                | 18.1 us: 1.06x slower                                          |
| pickle_list          | 2.74 us                                                | 2.92 us: 1.07x slower                                          |
| xml_etree_iterparse  | 72.1 ms                                                | 77.1 ms: 1.07x slower                                          |
| xml_etree_generate   | 53.5 ms                                                | 60.9 ms: 1.14x slower                                          |
| unpickle_list        | 2.69 us                                                | 3.12 us: 1.16x slower                                          |
| Geometric mean       | (ref)                                                  | 1.01x faster                                                   |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 13.3 ms: 1.22x slower                                          |
| python_startup_no_site | 7.91 ms                                                | 11.9 ms: 1.51x slower                                          |
| Geometric mean         | (ref)                                                  | 1.36x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 9.87 ms                                                | 7.90 ms: 1.25x faster                                          |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 79.4 us: 4.07x faster                                          |
| deltablue                | 4.91 ms                                                | 2.48 ms: 1.98x faster                                          |
| logging_silent           | 117 ns                                                 | 72.0 ns: 1.63x faster                                          |
| raytrace                 | 301 ms                                                 | 185 ms: 1.62x faster                                           |
| asyncio_tcp              | 659 ms                                                 | 424 ms: 1.55x faster                                           |
| chaos                    | 65.8 ms                                                | 43.5 ms: 1.51x faster                                          |
| async_tree_none          | 388 ms                                                 | 258 ms: 1.50x faster                                           |
| sqlglot_parse            | 1.24 ms                                                | 837 us: 1.49x faster                                           |
| richards_super           | 57.8 ms                                                | 40.7 ms: 1.42x faster                                          |
| async_tree_memoization   | 474 ms                                                 | 335 ms: 1.41x faster                                           |
| sqlglot_transpile        | 1.44 ms                                                | 1.02 ms: 1.41x faster                                          |
| crypto_pyaes             | 71.8 ms                                                | 50.9 ms: 1.41x faster                                          |
| go                       | 151 ms                                                 | 107 ms: 1.40x faster                                           |
| async_tree_io            | 980 ms                                                 | 713 ms: 1.37x faster                                           |
| comprehensions           | 16.9 us                                                | 12.4 us: 1.36x faster                                          |
| pickle_pure_python       | 281 us                                                 | 208 us: 1.35x faster                                           |
| scimark_monte_carlo      | 65.6 ms                                                | 48.9 ms: 1.34x faster                                          |
| scimark_lu               | 103 ms                                                 | 77.1 ms: 1.33x faster                                          |
| unpack_sequence          | 39.0 ns                                                | 29.5 ns: 1.33x faster                                          |
| richards                 | 48.7 ms                                                | 36.8 ms: 1.32x faster                                          |
| deepcopy_memo            | 34.7 us                                                | 27.0 us: 1.28x faster                                          |
| spectral_norm            | 94.8 ms                                                | 75.8 ms: 1.25x faster                                          |
| mako                     | 9.87 ms                                                | 7.90 ms: 1.25x faster                                          |
| hexiom                   | 6.19 ms                                                | 5.00 ms: 1.24x faster                                          |
| pyflate                  | 427 ms                                                 | 346 ms: 1.23x faster                                           |
| pycparser                | 877 ms                                                 | 712 ms: 1.23x faster                                           |
| generators               | 32.3 ms                                                | 26.3 ms: 1.23x faster                                          |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.31 sec: 1.22x faster                                         |
| create_gc_cycles         | 860 us                                                 | 706 us: 1.22x faster                                           |
| tornado_http             | 86.7 ms                                                | 71.2 ms: 1.22x faster                                          |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 534 ms: 1.22x faster                                           |
| chameleon                | 6.26 ms                                                | 5.16 ms: 1.21x faster                                          |
| json_dumps               | 8.11 ms                                                | 6.72 ms: 1.21x faster                                          |
| scimark_sor              | 128 ms                                                 | 106 ms: 1.20x faster                                           |
| sympy_sum                | 92.2 ms                                                | 76.7 ms: 1.20x faster                                          |
| logging_format           | 4.83 us                                                | 4.06 us: 1.19x faster                                          |
| regex_compile            | 95.3 ms                                                | 80.5 ms: 1.18x faster                                          |
| logging_simple           | 4.45 us                                                | 3.76 us: 1.18x faster                                          |
| float                    | 69.0 ms                                                | 58.5 ms: 1.18x faster                                          |
| pprint_pformat           | 1.30 sec                                               | 1.11 sec: 1.18x faster                                         |
| dulwich_log              | 35.3 ms                                                | 30.1 ms: 1.17x faster                                          |
| regex_dna                | 174 ms                                                 | 149 ms: 1.17x faster                                           |
| unpickle_pure_python     | 194 us                                                 | 166 us: 1.17x faster                                           |
| pprint_safe_repr         | 641 ms                                                 | 547 ms: 1.17x faster                                           |
| sympy_integrate          | 13.1 ms                                                | 11.3 ms: 1.16x faster                                          |
| mypy2                    | 607 ms                                                 | 528 ms: 1.15x faster                                           |
| docutils                 | 1.73 sec                                               | 1.51 sec: 1.15x faster                                         |
| nbody                    | 93.0 ms                                                | 81.7 ms: 1.14x faster                                          |
| deepcopy                 | 272 us                                                 | 240 us: 1.13x faster                                           |
| xml_etree_process        | 46.5 ms                                                | 42.0 ms: 1.11x faster                                          |
| sympy_str                | 165 ms                                                 | 150 ms: 1.10x faster                                           |
| deepcopy_reduce          | 2.33 us                                                | 2.12 us: 1.10x faster                                          |
| 2to3                     | 192 ms                                                 | 178 ms: 1.08x faster                                           |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 3.20 ms: 1.07x faster                                          |
| tomli_loads              | 1.71 sec                                               | 1.60 sec: 1.06x faster                                         |
| coroutines               | 20.7 ms                                                | 19.5 ms: 1.06x faster                                          |
| scimark_fft              | 224 ms                                                 | 212 ms: 1.06x faster                                           |
| fannkuch                 | 303 ms                                                 | 287 ms: 1.05x faster                                           |
| sympy_expand             | 269 ms                                                 | 258 ms: 1.04x faster                                           |
| pidigits                 | 282 ms                                                 | 274 ms: 1.03x faster                                           |
| meteor_contest           | 77.7 ms                                                | 76.3 ms: 1.02x faster                                          |
| sqlglot_optimize         | 36.8 ms                                                | 36.2 ms: 1.02x faster                                          |
| regex_v8                 | 17.1 ms                                                | 16.9 ms: 1.01x faster                                          |
| json                     | 3.08 ms                                                | 3.07 ms: 1.00x faster                                          |
| xml_etree_parse          | 108 ms                                                 | 109 ms: 1.01x slower                                           |
| gc_traversal             | 2.36 ms                                                | 2.40 ms: 1.02x slower                                          |
| sqlglot_normalize        | 190 ms                                                 | 194 ms: 1.02x slower                                           |
| unpickle                 | 8.80 us                                                | 9.13 us: 1.04x slower                                          |
| regex_effbot             | 2.46 ms                                                | 2.57 ms: 1.05x slower                                          |
| pickle                   | 6.97 us                                                | 7.36 us: 1.06x slower                                          |
| json_loads               | 16.4 us                                                | 17.4 us: 1.06x slower                                          |
| mdp                      | 1.63 sec                                               | 1.72 sec: 1.06x slower                                         |
| pickle_dict              | 17.0 us                                                | 18.1 us: 1.06x slower                                          |
| pickle_list              | 2.74 us                                                | 2.92 us: 1.07x slower                                          |
| xml_etree_iterparse      | 72.1 ms                                                | 77.1 ms: 1.07x slower                                          |
| sqlite_synth             | 1.46 us                                                | 1.66 us: 1.14x slower                                          |
| xml_etree_generate       | 53.5 ms                                                | 60.9 ms: 1.14x slower                                          |
| unpickle_list            | 2.69 us                                                | 3.12 us: 1.16x slower                                          |
| coverage                 | 41.5 ms                                                | 48.3 ms: 1.17x slower                                          |
| python_startup           | 10.9 ms                                                | 13.3 ms: 1.22x slower                                          |
| bench_mp_pool            | 37.4 ms                                                | 45.9 ms: 1.23x slower                                          |
| async_generators         | 231 ms                                                 | 308 ms: 1.33x slower                                           |
| telco                    | 3.49 ms                                                | 4.77 ms: 1.37x slower                                          |
| python_startup_no_site   | 7.91 ms                                                | 11.9 ms: 1.51x slower                                          |
| Geometric mean           | (ref)                                                  | 1.15x faster                                                   |

Benchmark hidden because not significant (4): asyncio_websockets, bench_thread_pool, nqueens, pathlib
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231221-3.13.0a2+-39bbca4/bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.12x
- 95% likely to have a speedup of 1.10x
- 99% likely to have a speedup of 1.07x


# Memory

- memory change: 1.10x