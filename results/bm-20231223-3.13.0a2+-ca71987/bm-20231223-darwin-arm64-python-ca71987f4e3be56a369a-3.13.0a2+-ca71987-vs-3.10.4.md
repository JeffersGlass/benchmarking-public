
# Results vs. 3.10.4

- fork: python
- ref: ca71987f4e3be56a369a
- machine: darwin-arm64
- commit hash: ca71987
- commit date: 2023-12-23
- overall geometric mean: 1.18x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.11x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231223-darwin-arm64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 173 ms: 1.11x faster                                                   |
| chameleon      | 6.26 ms                                                | 4.80 ms: 1.30x faster                                                  |
| docutils       | 1.73 sec                                               | 1.49 sec: 1.16x faster                                                 |
| tornado_http   | 86.7 ms                                                | 70.2 ms: 1.24x faster                                                  |
| Geometric mean | (ref)                                                  | 1.20x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231223-darwin-arm64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 252 ms: 1.54x faster                                                   |
| async_tree_memoization  | 474 ms                                                 | 327 ms: 1.45x faster                                                   |
| async_tree_io           | 980 ms                                                 | 701 ms: 1.40x faster                                                   |
| async_tree_cpu_io_mixed | 649 ms                                                 | 523 ms: 1.24x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.40x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231223-darwin-arm64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| float          | 69.0 ms                                                | 58.2 ms: 1.19x faster                                                  |
| nbody          | 93.0 ms                                                | 78.8 ms: 1.18x faster                                                  |
| pidigits       | 282 ms                                                 | 283 ms: 1.00x slower                                                   |
| Geometric mean | (ref)                                                  | 1.12x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231223-darwin-arm64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 74.4 ms: 1.28x faster                                                  |
| regex_dna      | 174 ms                                                 | 149 ms: 1.17x faster                                                   |
| regex_v8       | 17.1 ms                                                | 16.9 ms: 1.02x faster                                                  |
| regex_effbot   | 2.46 ms                                                | 2.48 ms: 1.01x slower                                                  |
| Geometric mean | (ref)                                                  | 1.11x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231223-darwin-arm64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 199 us: 1.41x faster                                                   |
| json_dumps           | 8.11 ms                                                | 6.62 ms: 1.22x faster                                                  |
| unpickle_pure_python | 194 us                                                 | 160 us: 1.22x faster                                                   |
| xml_etree_process    | 46.5 ms                                                | 40.5 ms: 1.15x faster                                                  |
| tomli_loads          | 1.71 sec                                               | 1.58 sec: 1.08x faster                                                 |
| json_loads           | 16.4 us                                                | 17.2 us: 1.04x slower                                                  |
| unpickle             | 8.80 us                                                | 9.20 us: 1.05x slower                                                  |
| pickle_dict          | 17.0 us                                                | 18.0 us: 1.06x slower                                                  |
| xml_etree_iterparse  | 72.1 ms                                                | 76.4 ms: 1.06x slower                                                  |
| pickle_list          | 2.74 us                                                | 2.93 us: 1.07x slower                                                  |
| xml_etree_generate   | 53.5 ms                                                | 57.4 ms: 1.07x slower                                                  |
| pickle               | 6.97 us                                                | 7.49 us: 1.07x slower                                                  |
| unpickle_list        | 2.69 us                                                | 3.15 us: 1.17x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                           |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231223-darwin-arm64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 13.2 ms: 1.22x slower                                                  |
| python_startup_no_site | 7.91 ms                                                | 11.8 ms: 1.50x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.35x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231223-darwin-arm64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 9.87 ms                                                | 7.67 ms: 1.29x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231223-darwin-arm64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 73.9 us: 4.37x faster                                                  |
| deltablue                | 4.91 ms                                                | 2.47 ms: 1.99x faster                                                  |
| raytrace                 | 301 ms                                                 | 175 ms: 1.72x faster                                                   |
| logging_silent           | 117 ns                                                 | 71.2 ns: 1.65x faster                                                  |
| chaos                    | 65.8 ms                                                | 40.0 ms: 1.64x faster                                                  |
| async_tree_none          | 388 ms                                                 | 252 ms: 1.54x faster                                                   |
| richards_super           | 57.8 ms                                                | 37.6 ms: 1.54x faster                                                  |
| asyncio_tcp              | 659 ms                                                 | 433 ms: 1.52x faster                                                   |
| sqlglot_parse            | 1.24 ms                                                | 819 us: 1.52x faster                                                   |
| crypto_pyaes             | 71.8 ms                                                | 48.3 ms: 1.49x faster                                                  |
| unpack_sequence          | 39.0 ns                                                | 26.6 ns: 1.47x faster                                                  |
| richards                 | 48.7 ms                                                | 33.6 ms: 1.45x faster                                                  |
| async_tree_memoization   | 474 ms                                                 | 327 ms: 1.45x faster                                                   |
| sqlglot_transpile        | 1.44 ms                                                | 998 us: 1.44x faster                                                   |
| go                       | 151 ms                                                 | 105 ms: 1.44x faster                                                   |
| pickle_pure_python       | 281 us                                                 | 199 us: 1.41x faster                                                   |
| deepcopy_memo            | 34.7 us                                                | 24.8 us: 1.40x faster                                                  |
| async_tree_io            | 980 ms                                                 | 701 ms: 1.40x faster                                                   |
| comprehensions           | 16.9 us                                                | 12.2 us: 1.39x faster                                                  |
| scimark_monte_carlo      | 65.6 ms                                                | 47.6 ms: 1.38x faster                                                  |
| hexiom                   | 6.19 ms                                                | 4.52 ms: 1.37x faster                                                  |
| scimark_lu               | 103 ms                                                 | 75.9 ms: 1.35x faster                                                  |
| chameleon                | 6.26 ms                                                | 4.80 ms: 1.30x faster                                                  |
| spectral_norm            | 94.8 ms                                                | 73.5 ms: 1.29x faster                                                  |
| mako                     | 9.87 ms                                                | 7.67 ms: 1.29x faster                                                  |
| generators               | 32.3 ms                                                | 25.2 ms: 1.29x faster                                                  |
| regex_compile            | 95.3 ms                                                | 74.4 ms: 1.28x faster                                                  |
| pyflate                  | 427 ms                                                 | 341 ms: 1.25x faster                                                   |
| logging_simple           | 4.45 us                                                | 3.56 us: 1.25x faster                                                  |
| pycparser                | 877 ms                                                 | 703 ms: 1.25x faster                                                   |
| logging_format           | 4.83 us                                                | 3.88 us: 1.24x faster                                                  |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 523 ms: 1.24x faster                                                   |
| tornado_http             | 86.7 ms                                                | 70.2 ms: 1.24x faster                                                  |
| sympy_sum                | 92.2 ms                                                | 75.0 ms: 1.23x faster                                                  |
| pprint_pformat           | 1.30 sec                                               | 1.06 sec: 1.23x faster                                                 |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.31 sec: 1.23x faster                                                 |
| json_dumps               | 8.11 ms                                                | 6.62 ms: 1.22x faster                                                  |
| create_gc_cycles         | 860 us                                                 | 703 us: 1.22x faster                                                   |
| pprint_safe_repr         | 641 ms                                                 | 525 ms: 1.22x faster                                                   |
| unpickle_pure_python     | 194 us                                                 | 160 us: 1.22x faster                                                   |
| scimark_sor              | 128 ms                                                 | 106 ms: 1.22x faster                                                   |
| sympy_integrate          | 13.1 ms                                                | 11.0 ms: 1.20x faster                                                  |
| dulwich_log              | 35.3 ms                                                | 29.7 ms: 1.19x faster                                                  |
| deepcopy                 | 272 us                                                 | 228 us: 1.19x faster                                                   |
| float                    | 69.0 ms                                                | 58.2 ms: 1.19x faster                                                  |
| nbody                    | 93.0 ms                                                | 78.8 ms: 1.18x faster                                                  |
| regex_dna                | 174 ms                                                 | 149 ms: 1.17x faster                                                   |
| mypy2                    | 607 ms                                                 | 522 ms: 1.16x faster                                                   |
| docutils                 | 1.73 sec                                               | 1.49 sec: 1.16x faster                                                 |
| coroutines               | 20.7 ms                                                | 17.9 ms: 1.16x faster                                                  |
| xml_etree_process        | 46.5 ms                                                | 40.5 ms: 1.15x faster                                                  |
| sympy_str                | 165 ms                                                 | 144 ms: 1.14x faster                                                   |
| deepcopy_reduce          | 2.33 us                                                | 2.04 us: 1.14x faster                                                  |
| dask                     | 253 ms                                                 | 227 ms: 1.12x faster                                                   |
| 2to3                     | 192 ms                                                 | 173 ms: 1.11x faster                                                   |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 3.10 ms: 1.10x faster                                                  |
| scimark_fft              | 224 ms                                                 | 203 ms: 1.10x faster                                                   |
| tomli_loads              | 1.71 sec                                               | 1.58 sec: 1.08x faster                                                 |
| sympy_expand             | 269 ms                                                 | 251 ms: 1.07x faster                                                   |
| sqlglot_optimize         | 36.8 ms                                                | 35.0 ms: 1.05x faster                                                  |
| nqueens                  | 63.8 ms                                                | 60.8 ms: 1.05x faster                                                  |
| meteor_contest           | 77.7 ms                                                | 74.4 ms: 1.05x faster                                                  |
| fannkuch                 | 303 ms                                                 | 291 ms: 1.04x faster                                                   |
| bench_thread_pool        | 527 us                                                 | 513 us: 1.03x faster                                                   |
| sqlglot_normalize        | 190 ms                                                 | 186 ms: 1.02x faster                                                   |
| regex_v8                 | 17.1 ms                                                | 16.9 ms: 1.02x faster                                                  |
| pidigits                 | 282 ms                                                 | 283 ms: 1.00x slower                                                   |
| regex_effbot             | 2.46 ms                                                | 2.48 ms: 1.01x slower                                                  |
| mdp                      | 1.63 sec                                               | 1.65 sec: 1.01x slower                                                 |
| gc_traversal             | 2.36 ms                                                | 2.40 ms: 1.02x slower                                                  |
| json                     | 3.08 ms                                                | 3.15 ms: 1.02x slower                                                  |
| json_loads               | 16.4 us                                                | 17.2 us: 1.04x slower                                                  |
| unpickle                 | 8.80 us                                                | 9.20 us: 1.05x slower                                                  |
| pickle_dict              | 17.0 us                                                | 18.0 us: 1.06x slower                                                  |
| xml_etree_iterparse      | 72.1 ms                                                | 76.4 ms: 1.06x slower                                                  |
| pickle_list              | 2.74 us                                                | 2.93 us: 1.07x slower                                                  |
| xml_etree_generate       | 53.5 ms                                                | 57.4 ms: 1.07x slower                                                  |
| pickle                   | 6.97 us                                                | 7.49 us: 1.07x slower                                                  |
| sqlite_synth             | 1.46 us                                                | 1.65 us: 1.13x slower                                                  |
| coverage                 | 41.5 ms                                                | 47.4 ms: 1.14x slower                                                  |
| unpickle_list            | 2.69 us                                                | 3.15 us: 1.17x slower                                                  |
| python_startup           | 10.9 ms                                                | 13.2 ms: 1.22x slower                                                  |
| bench_mp_pool            | 37.4 ms                                                | 45.6 ms: 1.22x slower                                                  |
| async_generators         | 231 ms                                                 | 303 ms: 1.31x slower                                                   |
| telco                    | 3.49 ms                                                | 4.72 ms: 1.35x slower                                                  |
| python_startup_no_site   | 7.91 ms                                                | 11.8 ms: 1.50x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.18x faster                                                           |

Benchmark hidden because not significant (3): xml_etree_parse, asyncio_websockets, pathlib
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231223-3.13.0a2+-ca71987/bm-20231223-darwin-arm64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.15x
- 95% likely to have a speedup of 1.14x
- 99% likely to have a speedup of 1.11x


# Memory

- memory change: 1.10x