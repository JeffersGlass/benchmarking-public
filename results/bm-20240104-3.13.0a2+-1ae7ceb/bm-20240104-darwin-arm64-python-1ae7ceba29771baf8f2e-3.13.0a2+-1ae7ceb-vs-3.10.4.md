
# Results vs. 3.10.4

- fork: python
- ref: 1ae7ceba29771baf8f2e
- machine: darwin-arm64
- commit hash: 1ae7ceb
- commit date: 2024-01-04
- overall geometric mean: 1.18x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.11x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 173 ms: 1.11x faster                                                   |
| chameleon      | 6.26 ms                                                | 4.81 ms: 1.30x faster                                                  |
| docutils       | 1.73 sec                                               | 1.49 sec: 1.16x faster                                                 |
| tornado_http   | 86.7 ms                                                | 69.4 ms: 1.25x faster                                                  |
| Geometric mean | (ref)                                                  | 1.20x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 250 ms: 1.55x faster                                                   |
| async_tree_memoization  | 474 ms                                                 | 328 ms: 1.45x faster                                                   |
| async_tree_io           | 980 ms                                                 | 709 ms: 1.38x faster                                                   |
| async_tree_cpu_io_mixed | 649 ms                                                 | 522 ms: 1.24x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.40x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| float          | 69.0 ms                                                | 57.9 ms: 1.19x faster                                                  |
| nbody          | 93.0 ms                                                | 79.0 ms: 1.18x faster                                                  |
| Geometric mean | (ref)                                                  | 1.12x faster                                                           |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 73.9 ms: 1.29x faster                                                  |
| regex_dna      | 174 ms                                                 | 148 ms: 1.18x faster                                                   |
| regex_v8       | 17.1 ms                                                | 16.9 ms: 1.02x faster                                                  |
| regex_effbot   | 2.46 ms                                                | 2.49 ms: 1.01x slower                                                  |
| Geometric mean | (ref)                                                  | 1.11x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 198 us: 1.42x faster                                                   |
| unpickle_pure_python | 194 us                                                 | 157 us: 1.24x faster                                                   |
| json_dumps           | 8.11 ms                                                | 6.60 ms: 1.23x faster                                                  |
| xml_etree_process    | 46.5 ms                                                | 40.0 ms: 1.16x faster                                                  |
| tomli_loads          | 1.71 sec                                               | 1.58 sec: 1.08x faster                                                 |
| xml_etree_parse      | 108 ms                                                 | 107 ms: 1.01x faster                                                   |
| json_loads           | 16.4 us                                                | 17.3 us: 1.05x slower                                                  |
| pickle_list          | 2.74 us                                                | 2.88 us: 1.05x slower                                                  |
| xml_etree_iterparse  | 72.1 ms                                                | 76.1 ms: 1.05x slower                                                  |
| pickle_dict          | 17.0 us                                                | 17.9 us: 1.06x slower                                                  |
| xml_etree_generate   | 53.5 ms                                                | 56.7 ms: 1.06x slower                                                  |
| unpickle             | 8.80 us                                                | 9.33 us: 1.06x slower                                                  |
| pickle               | 6.97 us                                                | 7.49 us: 1.07x slower                                                  |
| unpickle_list        | 2.69 us                                                | 3.15 us: 1.17x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 13.4 ms: 1.23x slower                                                  |
| python_startup_no_site | 7.91 ms                                                | 12.0 ms: 1.51x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.36x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 9.87 ms                                                | 7.61 ms: 1.30x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 73.6 us: 4.39x faster                                                  |
| deltablue                | 4.91 ms                                                | 2.47 ms: 1.99x faster                                                  |
| raytrace                 | 301 ms                                                 | 174 ms: 1.73x faster                                                   |
| logging_silent           | 117 ns                                                 | 71.1 ns: 1.65x faster                                                  |
| chaos                    | 65.8 ms                                                | 40.0 ms: 1.64x faster                                                  |
| async_tree_none          | 388 ms                                                 | 250 ms: 1.55x faster                                                   |
| richards_super           | 57.8 ms                                                | 37.5 ms: 1.54x faster                                                  |
| asyncio_tcp              | 659 ms                                                 | 428 ms: 1.54x faster                                                   |
| sqlglot_parse            | 1.24 ms                                                | 818 us: 1.52x faster                                                   |
| crypto_pyaes             | 71.8 ms                                                | 48.2 ms: 1.49x faster                                                  |
| unpack_sequence          | 39.0 ns                                                | 26.6 ns: 1.47x faster                                                  |
| async_tree_memoization   | 474 ms                                                 | 328 ms: 1.45x faster                                                   |
| sqlglot_transpile        | 1.44 ms                                                | 1000 us: 1.44x faster                                                  |
| go                       | 151 ms                                                 | 104 ms: 1.44x faster                                                   |
| richards                 | 48.7 ms                                                | 34.0 ms: 1.43x faster                                                  |
| pickle_pure_python       | 281 us                                                 | 198 us: 1.42x faster                                                   |
| deepcopy_memo            | 34.7 us                                                | 24.9 us: 1.39x faster                                                  |
| comprehensions           | 16.9 us                                                | 12.2 us: 1.38x faster                                                  |
| async_tree_io            | 980 ms                                                 | 709 ms: 1.38x faster                                                   |
| hexiom                   | 6.19 ms                                                | 4.49 ms: 1.38x faster                                                  |
| scimark_monte_carlo      | 65.6 ms                                                | 47.7 ms: 1.37x faster                                                  |
| scimark_lu               | 103 ms                                                 | 75.9 ms: 1.36x faster                                                  |
| generators               | 32.3 ms                                                | 24.8 ms: 1.30x faster                                                  |
| chameleon                | 6.26 ms                                                | 4.81 ms: 1.30x faster                                                  |
| mako                     | 9.87 ms                                                | 7.61 ms: 1.30x faster                                                  |
| regex_compile            | 95.3 ms                                                | 73.9 ms: 1.29x faster                                                  |
| spectral_norm            | 94.8 ms                                                | 74.0 ms: 1.28x faster                                                  |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.27 sec: 1.27x faster                                                 |
| logging_simple           | 4.45 us                                                | 3.53 us: 1.26x faster                                                  |
| logging_format           | 4.83 us                                                | 3.84 us: 1.26x faster                                                  |
| tornado_http             | 86.7 ms                                                | 69.4 ms: 1.25x faster                                                  |
| pycparser                | 877 ms                                                 | 702 ms: 1.25x faster                                                   |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 522 ms: 1.24x faster                                                   |
| pyflate                  | 427 ms                                                 | 343 ms: 1.24x faster                                                   |
| unpickle_pure_python     | 194 us                                                 | 157 us: 1.24x faster                                                   |
| json_dumps               | 8.11 ms                                                | 6.60 ms: 1.23x faster                                                  |
| sympy_sum                | 92.2 ms                                                | 75.1 ms: 1.23x faster                                                  |
| create_gc_cycles         | 860 us                                                 | 702 us: 1.22x faster                                                   |
| pprint_pformat           | 1.30 sec                                               | 1.07 sec: 1.22x faster                                                 |
| pprint_safe_repr         | 641 ms                                                 | 529 ms: 1.21x faster                                                   |
| scimark_sor              | 128 ms                                                 | 107 ms: 1.20x faster                                                   |
| sympy_integrate          | 13.1 ms                                                | 11.0 ms: 1.19x faster                                                  |
| dulwich_log              | 35.3 ms                                                | 29.6 ms: 1.19x faster                                                  |
| float                    | 69.0 ms                                                | 57.9 ms: 1.19x faster                                                  |
| deepcopy                 | 272 us                                                 | 229 us: 1.19x faster                                                   |
| nbody                    | 93.0 ms                                                | 79.0 ms: 1.18x faster                                                  |
| regex_dna                | 174 ms                                                 | 148 ms: 1.18x faster                                                   |
| mypy2                    | 607 ms                                                 | 521 ms: 1.17x faster                                                   |
| coroutines               | 20.7 ms                                                | 17.8 ms: 1.16x faster                                                  |
| xml_etree_process        | 46.5 ms                                                | 40.0 ms: 1.16x faster                                                  |
| docutils                 | 1.73 sec                                               | 1.49 sec: 1.16x faster                                                 |
| sympy_str                | 165 ms                                                 | 145 ms: 1.14x faster                                                   |
| deepcopy_reduce          | 2.33 us                                                | 2.06 us: 1.13x faster                                                  |
| dask                     | 253 ms                                                 | 227 ms: 1.12x faster                                                   |
| 2to3                     | 192 ms                                                 | 173 ms: 1.11x faster                                                   |
| scimark_fft              | 224 ms                                                 | 205 ms: 1.09x faster                                                   |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 3.14 ms: 1.09x faster                                                  |
| tomli_loads              | 1.71 sec                                               | 1.58 sec: 1.08x faster                                                 |
| sympy_expand             | 269 ms                                                 | 251 ms: 1.07x faster                                                   |
| sqlglot_optimize         | 36.8 ms                                                | 34.9 ms: 1.05x faster                                                  |
| meteor_contest           | 77.7 ms                                                | 74.0 ms: 1.05x faster                                                  |
| nqueens                  | 63.8 ms                                                | 61.0 ms: 1.05x faster                                                  |
| fannkuch                 | 303 ms                                                 | 295 ms: 1.03x faster                                                   |
| bench_thread_pool        | 527 us                                                 | 514 us: 1.03x faster                                                   |
| sqlglot_normalize        | 190 ms                                                 | 187 ms: 1.02x faster                                                   |
| json                     | 3.08 ms                                                | 3.03 ms: 1.02x faster                                                  |
| regex_v8                 | 17.1 ms                                                | 16.9 ms: 1.02x faster                                                  |
| xml_etree_parse          | 108 ms                                                 | 107 ms: 1.01x faster                                                   |
| regex_effbot             | 2.46 ms                                                | 2.49 ms: 1.01x slower                                                  |
| gc_traversal             | 2.36 ms                                                | 2.40 ms: 1.02x slower                                                  |
| json_loads               | 16.4 us                                                | 17.3 us: 1.05x slower                                                  |
| pickle_list              | 2.74 us                                                | 2.88 us: 1.05x slower                                                  |
| xml_etree_iterparse      | 72.1 ms                                                | 76.1 ms: 1.05x slower                                                  |
| pickle_dict              | 17.0 us                                                | 17.9 us: 1.06x slower                                                  |
| xml_etree_generate       | 53.5 ms                                                | 56.7 ms: 1.06x slower                                                  |
| unpickle                 | 8.80 us                                                | 9.33 us: 1.06x slower                                                  |
| pickle                   | 6.97 us                                                | 7.49 us: 1.07x slower                                                  |
| sqlite_synth             | 1.46 us                                                | 1.66 us: 1.14x slower                                                  |
| unpickle_list            | 2.69 us                                                | 3.15 us: 1.17x slower                                                  |
| coverage                 | 41.5 ms                                                | 49.3 ms: 1.19x slower                                                  |
| bench_mp_pool            | 37.4 ms                                                | 45.6 ms: 1.22x slower                                                  |
| python_startup           | 10.9 ms                                                | 13.4 ms: 1.23x slower                                                  |
| async_generators         | 231 ms                                                 | 302 ms: 1.31x slower                                                   |
| telco                    | 3.49 ms                                                | 4.74 ms: 1.36x slower                                                  |
| python_startup_no_site   | 7.91 ms                                                | 12.0 ms: 1.51x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.18x faster                                                           |

Benchmark hidden because not significant (4): asyncio_websockets, pidigits, mdp, pathlib
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240104-3.13.0a2+-1ae7ceb/bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.15x
- 95% likely to have a speedup of 1.14x
- 99% likely to have a speedup of 1.11x


# Memory

- memory change: 1.10x