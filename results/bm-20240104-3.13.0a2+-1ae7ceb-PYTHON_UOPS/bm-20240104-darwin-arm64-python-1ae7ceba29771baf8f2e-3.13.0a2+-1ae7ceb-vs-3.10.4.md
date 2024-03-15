
# Results vs. 3.10.4

- fork: python
- ref: 1ae7ceba29771baf8f2e
- machine: darwin-arm64
- commit hash: 1ae7ceb
- commit date: 2024-01-04
- overall geometric mean: 1.11x faster
- HPT reliability: 99.98%
- HPT 99th percentile: 1.03x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 178 ms: 1.08x faster                                                   |
| chameleon      | 6.26 ms                                                | 4.93 ms: 1.27x faster                                                  |
| docutils       | 1.73 sec                                               | 1.53 sec: 1.13x faster                                                 |
| tornado_http   | 86.7 ms                                                | 71.7 ms: 1.21x faster                                                  |
| Geometric mean | (ref)                                                  | 1.17x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 259 ms: 1.50x faster                                                   |
| async_tree_memoization  | 474 ms                                                 | 337 ms: 1.40x faster                                                   |
| async_tree_io           | 980 ms                                                 | 715 ms: 1.37x faster                                                   |
| async_tree_cpu_io_mixed | 649 ms                                                 | 531 ms: 1.22x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.37x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 89.3 ms: 1.04x faster                                                  |
| pidigits       | 282 ms                                                 | 284 ms: 1.01x slower                                                   |
| float          | 69.0 ms                                                | 70.1 ms: 1.02x slower                                                  |
| Geometric mean | (ref)                                                  | 1.01x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_dna      | 174 ms                                                 | 148 ms: 1.18x faster                                                   |
| regex_compile  | 95.3 ms                                                | 84.4 ms: 1.13x faster                                                  |
| regex_v8       | 17.1 ms                                                | 17.0 ms: 1.01x faster                                                  |
| regex_effbot   | 2.46 ms                                                | 2.49 ms: 1.01x slower                                                  |
| Geometric mean | (ref)                                                  | 1.07x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 200 us: 1.40x faster                                                   |
| json_dumps           | 8.11 ms                                                | 6.68 ms: 1.21x faster                                                  |
| unpickle_pure_python | 194 us                                                 | 167 us: 1.16x faster                                                   |
| xml_etree_process    | 46.5 ms                                                | 41.8 ms: 1.11x faster                                                  |
| tomli_loads          | 1.71 sec                                               | 1.69 sec: 1.01x faster                                                 |
| unpickle             | 8.80 us                                                | 9.20 us: 1.05x slower                                                  |
| json_loads           | 16.4 us                                                | 17.3 us: 1.05x slower                                                  |
| pickle_list          | 2.74 us                                                | 2.88 us: 1.05x slower                                                  |
| pickle               | 6.97 us                                                | 7.42 us: 1.06x slower                                                  |
| pickle_dict          | 17.0 us                                                | 18.5 us: 1.09x slower                                                  |
| xml_etree_generate   | 53.5 ms                                                | 60.1 ms: 1.12x slower                                                  |
| xml_etree_iterparse  | 72.1 ms                                                | 81.2 ms: 1.13x slower                                                  |
| unpickle_list        | 2.69 us                                                | 3.18 us: 1.18x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.01x faster                                                           |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 13.2 ms: 1.22x slower                                                  |
| python_startup_no_site | 7.91 ms                                                | 11.8 ms: 1.49x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.35x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 9.87 ms                                                | 9.90 ms: 1.00x slower                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 76.3 us: 4.24x faster                                                  |
| logging_silent           | 117 ns                                                 | 72.4 ns: 1.62x faster                                                  |
| raytrace                 | 301 ms                                                 | 188 ms: 1.60x faster                                                   |
| richards_super           | 57.8 ms                                                | 36.7 ms: 1.58x faster                                                  |
| asyncio_tcp              | 659 ms                                                 | 431 ms: 1.53x faster                                                   |
| async_tree_none          | 388 ms                                                 | 259 ms: 1.50x faster                                                   |
| richards                 | 48.7 ms                                                | 32.7 ms: 1.49x faster                                                  |
| sqlglot_parse            | 1.24 ms                                                | 839 us: 1.48x faster                                                   |
| unpack_sequence          | 39.0 ns                                                | 26.4 ns: 1.48x faster                                                  |
| sqlglot_transpile        | 1.44 ms                                                | 1.03 ms: 1.41x faster                                                  |
| async_tree_memoization   | 474 ms                                                 | 337 ms: 1.40x faster                                                   |
| pickle_pure_python       | 281 us                                                 | 200 us: 1.40x faster                                                   |
| chaos                    | 65.8 ms                                                | 47.1 ms: 1.40x faster                                                  |
| async_tree_io            | 980 ms                                                 | 715 ms: 1.37x faster                                                   |
| go                       | 151 ms                                                 | 111 ms: 1.36x faster                                                   |
| deltablue                | 4.91 ms                                                | 3.64 ms: 1.35x faster                                                  |
| deepcopy_memo            | 34.7 us                                                | 26.2 us: 1.32x faster                                                  |
| scimark_lu               | 103 ms                                                 | 78.6 ms: 1.31x faster                                                  |
| generators               | 32.3 ms                                                | 24.8 ms: 1.31x faster                                                  |
| crypto_pyaes             | 71.8 ms                                                | 55.7 ms: 1.29x faster                                                  |
| chameleon                | 6.26 ms                                                | 4.93 ms: 1.27x faster                                                  |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.27 sec: 1.27x faster                                                 |
| pycparser                | 877 ms                                                 | 708 ms: 1.24x faster                                                   |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 531 ms: 1.22x faster                                                   |
| logging_simple           | 4.45 us                                                | 3.65 us: 1.22x faster                                                  |
| logging_format           | 4.83 us                                                | 3.96 us: 1.22x faster                                                  |
| create_gc_cycles         | 860 us                                                 | 707 us: 1.22x faster                                                   |
| json_dumps               | 8.11 ms                                                | 6.68 ms: 1.21x faster                                                  |
| tornado_http             | 86.7 ms                                                | 71.7 ms: 1.21x faster                                                  |
| scimark_sor              | 128 ms                                                 | 109 ms: 1.18x faster                                                   |
| regex_dna                | 174 ms                                                 | 148 ms: 1.18x faster                                                   |
| deepcopy                 | 272 us                                                 | 233 us: 1.17x faster                                                   |
| dulwich_log              | 35.3 ms                                                | 30.3 ms: 1.16x faster                                                  |
| unpickle_pure_python     | 194 us                                                 | 167 us: 1.16x faster                                                   |
| coroutines               | 20.7 ms                                                | 17.9 ms: 1.16x faster                                                  |
| pyflate                  | 427 ms                                                 | 374 ms: 1.14x faster                                                   |
| mypy2                    | 607 ms                                                 | 533 ms: 1.14x faster                                                   |
| docutils                 | 1.73 sec                                               | 1.53 sec: 1.13x faster                                                 |
| scimark_monte_carlo      | 65.6 ms                                                | 58.0 ms: 1.13x faster                                                  |
| regex_compile            | 95.3 ms                                                | 84.4 ms: 1.13x faster                                                  |
| deepcopy_reduce          | 2.33 us                                                | 2.08 us: 1.12x faster                                                  |
| sympy_sum                | 92.2 ms                                                | 82.5 ms: 1.12x faster                                                  |
| xml_etree_process        | 46.5 ms                                                | 41.8 ms: 1.11x faster                                                  |
| sympy_integrate          | 13.1 ms                                                | 11.9 ms: 1.10x faster                                                  |
| dask                     | 253 ms                                                 | 230 ms: 1.10x faster                                                   |
| pprint_safe_repr         | 641 ms                                                 | 583 ms: 1.10x faster                                                   |
| pprint_pformat           | 1.30 sec                                               | 1.20 sec: 1.09x faster                                                 |
| 2to3                     | 192 ms                                                 | 178 ms: 1.08x faster                                                   |
| sympy_str                | 165 ms                                                 | 156 ms: 1.06x faster                                                   |
| comprehensions           | 16.9 us                                                | 16.1 us: 1.05x faster                                                  |
| nbody                    | 93.0 ms                                                | 89.3 ms: 1.04x faster                                                  |
| hexiom                   | 6.19 ms                                                | 5.96 ms: 1.04x faster                                                  |
| sympy_expand             | 269 ms                                                 | 259 ms: 1.04x faster                                                   |
| json                     | 3.08 ms                                                | 3.00 ms: 1.03x faster                                                  |
| tomli_loads              | 1.71 sec                                               | 1.69 sec: 1.01x faster                                                 |
| bench_thread_pool        | 527 us                                                 | 521 us: 1.01x faster                                                   |
| regex_v8                 | 17.1 ms                                                | 17.0 ms: 1.01x faster                                                  |
| mako                     | 9.87 ms                                                | 9.90 ms: 1.00x slower                                                  |
| pidigits                 | 282 ms                                                 | 284 ms: 1.01x slower                                                   |
| sqlglot_optimize         | 36.8 ms                                                | 37.2 ms: 1.01x slower                                                  |
| regex_effbot             | 2.46 ms                                                | 2.49 ms: 1.01x slower                                                  |
| pathlib                  | 24.5 ms                                                | 24.9 ms: 1.01x slower                                                  |
| float                    | 69.0 ms                                                | 70.1 ms: 1.02x slower                                                  |
| meteor_contest           | 77.7 ms                                                | 79.2 ms: 1.02x slower                                                  |
| gc_traversal             | 2.36 ms                                                | 2.41 ms: 1.02x slower                                                  |
| sqlglot_normalize        | 190 ms                                                 | 196 ms: 1.03x slower                                                   |
| unpickle                 | 8.80 us                                                | 9.20 us: 1.05x slower                                                  |
| json_loads               | 16.4 us                                                | 17.3 us: 1.05x slower                                                  |
| pickle_list              | 2.74 us                                                | 2.88 us: 1.05x slower                                                  |
| pickle                   | 6.97 us                                                | 7.42 us: 1.06x slower                                                  |
| mdp                      | 1.63 sec                                               | 1.74 sec: 1.07x slower                                                 |
| nqueens                  | 63.8 ms                                                | 68.8 ms: 1.08x slower                                                  |
| pickle_dict              | 17.0 us                                                | 18.5 us: 1.09x slower                                                  |
| xml_etree_generate       | 53.5 ms                                                | 60.1 ms: 1.12x slower                                                  |
| xml_etree_iterparse      | 72.1 ms                                                | 81.2 ms: 1.13x slower                                                  |
| fannkuch                 | 303 ms                                                 | 341 ms: 1.13x slower                                                   |
| scimark_fft              | 224 ms                                                 | 257 ms: 1.14x slower                                                   |
| coverage                 | 41.5 ms                                                | 48.2 ms: 1.16x slower                                                  |
| spectral_norm            | 94.8 ms                                                | 110 ms: 1.16x slower                                                   |
| sqlite_synth             | 1.46 us                                                | 1.71 us: 1.17x slower                                                  |
| unpickle_list            | 2.69 us                                                | 3.18 us: 1.18x slower                                                  |
| python_startup           | 10.9 ms                                                | 13.2 ms: 1.22x slower                                                  |
| bench_mp_pool            | 37.4 ms                                                | 46.2 ms: 1.24x slower                                                  |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 4.30 ms: 1.26x slower                                                  |
| async_generators         | 231 ms                                                 | 305 ms: 1.32x slower                                                   |
| telco                    | 3.49 ms                                                | 4.96 ms: 1.42x slower                                                  |
| python_startup_no_site   | 7.91 ms                                                | 11.8 ms: 1.49x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.11x faster                                                           |

Benchmark hidden because not significant (2): xml_etree_parse, asyncio_websockets
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240104-3.13.0a2+-1ae7ceb-PYTHON_UOPS/bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 99.98% likely to be faster
- 90% likely to have a speedup of 1.06x
- 95% likely to have a speedup of 1.05x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: 1.10x