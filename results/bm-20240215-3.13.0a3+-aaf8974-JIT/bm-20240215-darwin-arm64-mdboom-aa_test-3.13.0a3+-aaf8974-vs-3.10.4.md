
# Results vs. 3.10.4

- fork: mdboom
- ref: aa_test
- machine: darwin-arm64
- commit hash: aaf8974
- commit date: 2024-02-15
- overall geometric mean: 1.18x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.12x faster
- Memory change: 1.26x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-darwin-arm64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 191 ms: 1.00x faster                                      |
| chameleon      | 6.26 ms                                                | 4.82 ms: 1.30x faster                                     |
| docutils       | 1.73 sec                                               | 1.47 sec: 1.18x faster                                    |
| tornado_http   | 86.7 ms                                                | 69.7 ms: 1.24x faster                                     |
| Geometric mean | (ref)                                                  | 1.18x faster                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-darwin-arm64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 250 ms: 1.55x faster                                      |
| async_tree_memoization  | 474 ms                                                 | 328 ms: 1.45x faster                                      |
| async_tree_io           | 980 ms                                                 | 699 ms: 1.40x faster                                      |
| async_tree_cpu_io_mixed | 649 ms                                                 | 518 ms: 1.25x faster                                      |
| Geometric mean          | (ref)                                                  | 1.41x faster                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-darwin-arm64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| float          | 69.0 ms                                                | 55.4 ms: 1.24x faster                                     |
| nbody          | 93.0 ms                                                | 76.0 ms: 1.22x faster                                     |
| Geometric mean | (ref)                                                  | 1.15x faster                                              |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-darwin-arm64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 75.2 ms: 1.27x faster                                     |
| regex_dna      | 174 ms                                                 | 145 ms: 1.20x faster                                      |
| regex_v8       | 17.1 ms                                                | 16.9 ms: 1.01x faster                                     |
| Geometric mean | (ref)                                                  | 1.12x faster                                              |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-darwin-arm64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 195 us: 1.44x faster                                      |
| json_dumps           | 8.11 ms                                                | 6.53 ms: 1.24x faster                                     |
| unpickle_pure_python | 194 us                                                 | 158 us: 1.23x faster                                      |
| tomli_loads          | 1.71 sec                                               | 1.41 sec: 1.21x faster                                    |
| xml_etree_process    | 46.5 ms                                                | 39.3 ms: 1.18x faster                                     |
| xml_etree_parse      | 108 ms                                                 | 106 ms: 1.02x faster                                      |
| json_loads           | 16.4 us                                                | 17.0 us: 1.03x slower                                     |
| xml_etree_generate   | 53.5 ms                                                | 55.7 ms: 1.04x slower                                     |
| pickle               | 6.97 us                                                | 7.27 us: 1.04x slower                                     |
| xml_etree_iterparse  | 72.1 ms                                                | 75.5 ms: 1.05x slower                                     |
| unpickle             | 8.80 us                                                | 9.23 us: 1.05x slower                                     |
| pickle_dict          | 17.0 us                                                | 18.2 us: 1.07x slower                                     |
| pickle_list          | 2.74 us                                                | 2.99 us: 1.09x slower                                     |
| unpickle_list        | 2.69 us                                                | 3.10 us: 1.15x slower                                     |
| Geometric mean       | (ref)                                                  | 1.05x faster                                              |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-darwin-arm64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 13.6 ms: 1.25x slower                                     |
| python_startup_no_site | 7.91 ms                                                | 12.2 ms: 1.55x slower                                     |
| Geometric mean         | (ref)                                                  | 1.39x slower                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-darwin-arm64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|-----------|:------------------------------------------------------:|:---------------------------------------------------------:|
| mako      | 9.87 ms                                                | 7.78 ms: 1.27x faster                                     |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-darwin-arm64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|--------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 71.5 us: 4.52x faster                                     |
| deltablue                | 4.91 ms                                                | 2.45 ms: 2.01x faster                                     |
| raytrace                 | 301 ms                                                 | 176 ms: 1.71x faster                                      |
| logging_silent           | 117 ns                                                 | 70.5 ns: 1.66x faster                                     |
| asyncio_tcp              | 659 ms                                                 | 401 ms: 1.64x faster                                      |
| richards_super           | 57.8 ms                                                | 35.7 ms: 1.62x faster                                     |
| chaos                    | 65.8 ms                                                | 41.1 ms: 1.60x faster                                     |
| sqlglot_parse            | 1.24 ms                                                | 792 us: 1.57x faster                                      |
| async_tree_none          | 388 ms                                                 | 250 ms: 1.55x faster                                      |
| richards                 | 48.7 ms                                                | 32.0 ms: 1.52x faster                                     |
| sqlglot_transpile        | 1.44 ms                                                | 973 us: 1.48x faster                                      |
| crypto_pyaes             | 71.8 ms                                                | 48.8 ms: 1.47x faster                                     |
| async_tree_memoization   | 474 ms                                                 | 328 ms: 1.45x faster                                      |
| pickle_pure_python       | 281 us                                                 | 195 us: 1.44x faster                                      |
| async_tree_io            | 980 ms                                                 | 699 ms: 1.40x faster                                      |
| scimark_lu               | 103 ms                                                 | 74.6 ms: 1.38x faster                                     |
| unpack_sequence          | 39.0 ns                                                | 28.4 ns: 1.37x faster                                     |
| go                       | 151 ms                                                 | 110 ms: 1.37x faster                                      |
| scimark_monte_carlo      | 65.6 ms                                                | 48.6 ms: 1.35x faster                                     |
| comprehensions           | 16.9 us                                                | 12.7 us: 1.34x faster                                     |
| deepcopy_memo            | 34.7 us                                                | 26.3 us: 1.32x faster                                     |
| pyflate                  | 427 ms                                                 | 326 ms: 1.31x faster                                      |
| chameleon                | 6.26 ms                                                | 4.82 ms: 1.30x faster                                     |
| logging_format           | 4.83 us                                                | 3.76 us: 1.28x faster                                     |
| logging_simple           | 4.45 us                                                | 3.47 us: 1.28x faster                                     |
| mako                     | 9.87 ms                                                | 7.78 ms: 1.27x faster                                     |
| regex_compile            | 95.3 ms                                                | 75.2 ms: 1.27x faster                                     |
| pycparser                | 877 ms                                                 | 692 ms: 1.27x faster                                      |
| hexiom                   | 6.19 ms                                                | 4.91 ms: 1.26x faster                                     |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 518 ms: 1.25x faster                                      |
| pprint_safe_repr         | 641 ms                                                 | 513 ms: 1.25x faster                                      |
| pprint_pformat           | 1.30 sec                                               | 1.05 sec: 1.25x faster                                    |
| float                    | 69.0 ms                                                | 55.4 ms: 1.24x faster                                     |
| tornado_http             | 86.7 ms                                                | 69.7 ms: 1.24x faster                                     |
| json_dumps               | 8.11 ms                                                | 6.53 ms: 1.24x faster                                     |
| unpickle_pure_python     | 194 us                                                 | 158 us: 1.23x faster                                      |
| nbody                    | 93.0 ms                                                | 76.0 ms: 1.22x faster                                     |
| sympy_sum                | 92.2 ms                                                | 75.6 ms: 1.22x faster                                     |
| create_gc_cycles         | 860 us                                                 | 705 us: 1.22x faster                                      |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.31 sec: 1.22x faster                                    |
| scimark_sor              | 128 ms                                                 | 105 ms: 1.22x faster                                      |
| tomli_loads              | 1.71 sec                                               | 1.41 sec: 1.21x faster                                    |
| regex_dna                | 174 ms                                                 | 145 ms: 1.20x faster                                      |
| spectral_norm            | 94.8 ms                                                | 79.0 ms: 1.20x faster                                     |
| deepcopy                 | 272 us                                                 | 227 us: 1.20x faster                                      |
| dulwich_log              | 35.3 ms                                                | 29.7 ms: 1.19x faster                                     |
| sympy_integrate          | 13.1 ms                                                | 11.1 ms: 1.19x faster                                     |
| xml_etree_process        | 46.5 ms                                                | 39.3 ms: 1.18x faster                                     |
| docutils                 | 1.73 sec                                               | 1.47 sec: 1.18x faster                                    |
| sympy_str                | 165 ms                                                 | 141 ms: 1.17x faster                                      |
| deepcopy_reduce          | 2.33 us                                                | 1.99 us: 1.17x faster                                     |
| generators               | 32.3 ms                                                | 28.2 ms: 1.15x faster                                     |
| fannkuch                 | 303 ms                                                 | 266 ms: 1.14x faster                                      |
| dask                     | 253 ms                                                 | 223 ms: 1.13x faster                                      |
| coroutines               | 20.7 ms                                                | 18.5 ms: 1.12x faster                                     |
| sympy_expand             | 269 ms                                                 | 241 ms: 1.11x faster                                      |
| sqlglot_optimize         | 36.8 ms                                                | 34.5 ms: 1.07x faster                                     |
| scimark_fft              | 224 ms                                                 | 213 ms: 1.05x faster                                      |
| bench_thread_pool        | 527 us                                                 | 503 us: 1.05x faster                                      |
| json                     | 3.08 ms                                                | 2.95 ms: 1.04x faster                                     |
| meteor_contest           | 77.7 ms                                                | 74.5 ms: 1.04x faster                                     |
| sqlglot_normalize        | 190 ms                                                 | 183 ms: 1.04x faster                                      |
| nqueens                  | 63.8 ms                                                | 61.6 ms: 1.03x faster                                     |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 3.31 ms: 1.03x faster                                     |
| xml_etree_parse          | 108 ms                                                 | 106 ms: 1.02x faster                                      |
| regex_v8                 | 17.1 ms                                                | 16.9 ms: 1.01x faster                                     |
| mdp                      | 1.63 sec                                               | 1.61 sec: 1.01x faster                                    |
| 2to3                     | 192 ms                                                 | 191 ms: 1.00x faster                                      |
| gc_traversal             | 2.36 ms                                                | 2.39 ms: 1.01x slower                                     |
| json_loads               | 16.4 us                                                | 17.0 us: 1.03x slower                                     |
| xml_etree_generate       | 53.5 ms                                                | 55.7 ms: 1.04x slower                                     |
| pickle                   | 6.97 us                                                | 7.27 us: 1.04x slower                                     |
| xml_etree_iterparse      | 72.1 ms                                                | 75.5 ms: 1.05x slower                                     |
| unpickle                 | 8.80 us                                                | 9.23 us: 1.05x slower                                     |
| pickle_dict              | 17.0 us                                                | 18.2 us: 1.07x slower                                     |
| sqlite_synth             | 1.46 us                                                | 1.59 us: 1.09x slower                                     |
| pickle_list              | 2.74 us                                                | 2.99 us: 1.09x slower                                     |
| coverage                 | 41.5 ms                                                | 47.4 ms: 1.14x slower                                     |
| unpickle_list            | 2.69 us                                                | 3.10 us: 1.15x slower                                     |
| python_startup           | 10.9 ms                                                | 13.6 ms: 1.25x slower                                     |
| bench_mp_pool            | 37.4 ms                                                | 47.2 ms: 1.26x slower                                     |
| telco                    | 3.49 ms                                                | 4.56 ms: 1.31x slower                                     |
| async_generators         | 231 ms                                                 | 304 ms: 1.32x slower                                      |
| python_startup_no_site   | 7.91 ms                                                | 12.2 ms: 1.55x slower                                     |
| Geometric mean           | (ref)                                                  | 1.18x faster                                              |

Benchmark hidden because not significant (5): mypy2, pathlib, asyncio_websockets, regex_effbot, pidigits
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240215-3.13.0a3+-aaf8974-JIT/bm-20240215-darwin-arm64-mdboom-aa_test-3.13.0a3+-aaf8974.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.16x
- 95% likely to have a speedup of 1.14x
- 99% likely to have a speedup of 1.12x


# Memory

- memory change: 1.26x