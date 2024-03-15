
# Results vs. 3.10.4

- fork: python
- ref: 2feec0fc7fd0b9caae7a
- machine: darwin-arm64
- commit hash: 2feec0f
- commit date: 2023-12-18
- overall geometric mean: 1.04x faster
- HPT reliability: 80.43%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 196 ms: 1.02x slower                                                   |
| chameleon      | 6.26 ms                                                | 5.51 ms: 1.14x faster                                                  |
| docutils       | 1.73 sec                                               | 1.67 sec: 1.03x faster                                                 |
| tornado_http   | 86.7 ms                                                | 83.4 ms: 1.04x faster                                                  |
| Geometric mean | (ref)                                                  | 1.05x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 279 ms: 1.39x faster                                                   |
| async_tree_memoization  | 474 ms                                                 | 360 ms: 1.32x faster                                                   |
| async_tree_io           | 980 ms                                                 | 767 ms: 1.28x faster                                                   |
| async_tree_cpu_io_mixed | 649 ms                                                 | 564 ms: 1.15x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.28x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 92.7 ms: 1.00x faster                                                  |
| pidigits       | 282 ms                                                 | 294 ms: 1.04x slower                                                   |
| float          | 69.0 ms                                                | 74.2 ms: 1.08x slower                                                  |
| Geometric mean | (ref)                                                  | 1.04x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_dna      | 174 ms                                                 | 161 ms: 1.09x faster                                                   |
| regex_compile  | 95.3 ms                                                | 89.4 ms: 1.07x faster                                                  |
| regex_v8       | 17.1 ms                                                | 18.4 ms: 1.08x slower                                                  |
| regex_effbot   | 2.46 ms                                                | 2.84 ms: 1.16x slower                                                  |
| Geometric mean | (ref)                                                  | 1.02x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 212 us: 1.32x faster                                                   |
| json_dumps           | 8.11 ms                                                | 6.97 ms: 1.16x faster                                                  |
| unpickle_pure_python | 194 us                                                 | 180 us: 1.08x faster                                                   |
| xml_etree_process    | 46.5 ms                                                | 44.4 ms: 1.05x faster                                                  |
| tomli_loads          | 1.71 sec                                               | 1.76 sec: 1.03x slower                                                 |
| xml_etree_parse      | 108 ms                                                 | 113 ms: 1.05x slower                                                   |
| unpickle             | 8.80 us                                                | 9.49 us: 1.08x slower                                                  |
| json_loads           | 16.4 us                                                | 17.9 us: 1.09x slower                                                  |
| pickle_dict          | 17.0 us                                                | 18.6 us: 1.09x slower                                                  |
| pickle               | 6.97 us                                                | 7.67 us: 1.10x slower                                                  |
| pickle_list          | 2.74 us                                                | 3.04 us: 1.11x slower                                                  |
| xml_etree_iterparse  | 72.1 ms                                                | 86.0 ms: 1.19x slower                                                  |
| xml_etree_generate   | 53.5 ms                                                | 64.3 ms: 1.20x slower                                                  |
| unpickle_list        | 2.69 us                                                | 3.27 us: 1.21x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.04x slower                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 15.6 ms: 1.43x slower                                                  |
| python_startup_no_site | 7.91 ms                                                | 14.0 ms: 1.77x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.59x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 9.87 ms                                                | 10.5 ms: 1.06x slower                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 80.6 us: 4.01x faster                                                  |
| logging_silent           | 117 ns                                                 | 77.5 ns: 1.51x faster                                                  |
| raytrace                 | 301 ms                                                 | 203 ms: 1.49x faster                                                   |
| richards_super           | 57.8 ms                                                | 39.9 ms: 1.45x faster                                                  |
| async_tree_none          | 388 ms                                                 | 279 ms: 1.39x faster                                                   |
| richards                 | 48.7 ms                                                | 35.9 ms: 1.36x faster                                                  |
| sqlglot_parse            | 1.24 ms                                                | 924 us: 1.35x faster                                                   |
| pickle_pure_python       | 281 us                                                 | 212 us: 1.32x faster                                                   |
| async_tree_memoization   | 474 ms                                                 | 360 ms: 1.32x faster                                                   |
| chaos                    | 65.8 ms                                                | 50.1 ms: 1.31x faster                                                  |
| unpack_sequence          | 39.0 ns                                                | 29.8 ns: 1.31x faster                                                  |
| deltablue                | 4.91 ms                                                | 3.83 ms: 1.28x faster                                                  |
| async_tree_io            | 980 ms                                                 | 767 ms: 1.28x faster                                                   |
| sqlglot_transpile        | 1.44 ms                                                | 1.13 ms: 1.28x faster                                                  |
| go                       | 151 ms                                                 | 119 ms: 1.27x faster                                                   |
| scimark_lu               | 103 ms                                                 | 81.4 ms: 1.26x faster                                                  |
| crypto_pyaes             | 71.8 ms                                                | 57.3 ms: 1.25x faster                                                  |
| deepcopy_memo            | 34.7 us                                                | 28.4 us: 1.22x faster                                                  |
| generators               | 32.3 ms                                                | 26.6 ms: 1.21x faster                                                  |
| json_dumps               | 8.11 ms                                                | 6.97 ms: 1.16x faster                                                  |
| create_gc_cycles         | 860 us                                                 | 740 us: 1.16x faster                                                   |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 564 ms: 1.15x faster                                                   |
| logging_format           | 4.83 us                                                | 4.22 us: 1.14x faster                                                  |
| logging_simple           | 4.45 us                                                | 3.89 us: 1.14x faster                                                  |
| pycparser                | 877 ms                                                 | 769 ms: 1.14x faster                                                   |
| chameleon                | 6.26 ms                                                | 5.51 ms: 1.14x faster                                                  |
| scimark_sor              | 128 ms                                                 | 114 ms: 1.13x faster                                                   |
| asyncio_tcp              | 659 ms                                                 | 595 ms: 1.11x faster                                                   |
| dulwich_log              | 35.3 ms                                                | 32.0 ms: 1.10x faster                                                  |
| deepcopy                 | 272 us                                                 | 247 us: 1.10x faster                                                   |
| regex_dna                | 174 ms                                                 | 161 ms: 1.09x faster                                                   |
| unpickle_pure_python     | 194 us                                                 | 180 us: 1.08x faster                                                   |
| scimark_monte_carlo      | 65.6 ms                                                | 61.4 ms: 1.07x faster                                                  |
| coroutines               | 20.7 ms                                                | 19.4 ms: 1.07x faster                                                  |
| regex_compile            | 95.3 ms                                                | 89.4 ms: 1.07x faster                                                  |
| deepcopy_reduce          | 2.33 us                                                | 2.19 us: 1.06x faster                                                  |
| sympy_sum                | 92.2 ms                                                | 87.7 ms: 1.05x faster                                                  |
| xml_etree_process        | 46.5 ms                                                | 44.4 ms: 1.05x faster                                                  |
| pprint_safe_repr         | 641 ms                                                 | 615 ms: 1.04x faster                                                   |
| tornado_http             | 86.7 ms                                                | 83.4 ms: 1.04x faster                                                  |
| pyflate                  | 427 ms                                                 | 411 ms: 1.04x faster                                                   |
| pprint_pformat           | 1.30 sec                                               | 1.26 sec: 1.04x faster                                                 |
| docutils                 | 1.73 sec                                               | 1.67 sec: 1.03x faster                                                 |
| sympy_integrate          | 13.1 ms                                                | 12.8 ms: 1.02x faster                                                  |
| nbody                    | 93.0 ms                                                | 92.7 ms: 1.00x faster                                                  |
| comprehensions           | 16.9 us                                                | 16.9 us: 1.00x faster                                                  |
| sympy_str                | 165 ms                                                 | 167 ms: 1.01x slower                                                   |
| hexiom                   | 6.19 ms                                                | 6.31 ms: 1.02x slower                                                  |
| sympy_expand             | 269 ms                                                 | 274 ms: 1.02x slower                                                   |
| 2to3                     | 192 ms                                                 | 196 ms: 1.02x slower                                                   |
| json                     | 3.08 ms                                                | 3.16 ms: 1.03x slower                                                  |
| tomli_loads              | 1.71 sec                                               | 1.76 sec: 1.03x slower                                                 |
| pidigits                 | 282 ms                                                 | 294 ms: 1.04x slower                                                   |
| xml_etree_parse          | 108 ms                                                 | 113 ms: 1.05x slower                                                   |
| mako                     | 9.87 ms                                                | 10.5 ms: 1.06x slower                                                  |
| asyncio_websockets       | 410 ms                                                 | 437 ms: 1.07x slower                                                   |
| regex_v8                 | 17.1 ms                                                | 18.4 ms: 1.08x slower                                                  |
| sqlglot_optimize         | 36.8 ms                                                | 39.5 ms: 1.08x slower                                                  |
| float                    | 69.0 ms                                                | 74.2 ms: 1.08x slower                                                  |
| meteor_contest           | 77.7 ms                                                | 83.9 ms: 1.08x slower                                                  |
| unpickle                 | 8.80 us                                                | 9.49 us: 1.08x slower                                                  |
| gc_traversal             | 2.36 ms                                                | 2.56 ms: 1.08x slower                                                  |
| json_loads               | 16.4 us                                                | 17.9 us: 1.09x slower                                                  |
| pickle_dict              | 17.0 us                                                | 18.6 us: 1.09x slower                                                  |
| pickle                   | 6.97 us                                                | 7.67 us: 1.10x slower                                                  |
| bench_thread_pool        | 527 us                                                 | 582 us: 1.10x slower                                                   |
| pickle_list              | 2.74 us                                                | 3.04 us: 1.11x slower                                                  |
| sqlglot_normalize        | 190 ms                                                 | 211 ms: 1.11x slower                                                   |
| spectral_norm            | 94.8 ms                                                | 106 ms: 1.12x slower                                                   |
| pathlib                  | 24.5 ms                                                | 27.5 ms: 1.12x slower                                                  |
| nqueens                  | 63.8 ms                                                | 72.2 ms: 1.13x slower                                                  |
| mdp                      | 1.63 sec                                               | 1.85 sec: 1.14x slower                                                 |
| regex_effbot             | 2.46 ms                                                | 2.84 ms: 1.16x slower                                                  |
| scimark_fft              | 224 ms                                                 | 261 ms: 1.16x slower                                                   |
| fannkuch                 | 303 ms                                                 | 360 ms: 1.19x slower                                                   |
| xml_etree_iterparse      | 72.1 ms                                                | 86.0 ms: 1.19x slower                                                  |
| coverage                 | 41.5 ms                                                | 49.9 ms: 1.20x slower                                                  |
| xml_etree_generate       | 53.5 ms                                                | 64.3 ms: 1.20x slower                                                  |
| unpickle_list            | 2.69 us                                                | 3.27 us: 1.21x slower                                                  |
| sqlite_synth             | 1.46 us                                                | 1.78 us: 1.22x slower                                                  |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 4.38 ms: 1.28x slower                                                  |
| bench_mp_pool            | 37.4 ms                                                | 51.6 ms: 1.38x slower                                                  |
| async_generators         | 231 ms                                                 | 322 ms: 1.39x slower                                                   |
| telco                    | 3.49 ms                                                | 4.95 ms: 1.42x slower                                                  |
| python_startup           | 10.9 ms                                                | 15.6 ms: 1.43x slower                                                  |
| python_startup_no_site   | 7.91 ms                                                | 14.0 ms: 1.77x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.04x faster                                                           |

Benchmark hidden because not significant (3): mypy2, dask, asyncio_tcp_ssl
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231218-3.13.0a2+-2feec0f-PYTHON_UOPS/bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 80.43% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.10x