
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin
- machine: darwin-arm64
- commit hash: b63610e
- commit date: 2023-12-19
- overall geometric mean: 1.13x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.07x faster
- Memory change: 1.27x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 182 ms: 1.05x faster                                           |
| chameleon      | 6.26 ms                                                | 5.12 ms: 1.22x faster                                          |
| docutils       | 1.73 sec                                               | 1.54 sec: 1.13x faster                                         |
| tornado_http   | 86.7 ms                                                | 72.8 ms: 1.19x faster                                          |
| Geometric mean | (ref)                                                  | 1.15x faster                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 258 ms: 1.50x faster                                           |
| async_tree_memoization  | 474 ms                                                 | 334 ms: 1.42x faster                                           |
| async_tree_io           | 980 ms                                                 | 714 ms: 1.37x faster                                           |
| async_tree_cpu_io_mixed | 649 ms                                                 | 530 ms: 1.22x faster                                           |
| Geometric mean          | (ref)                                                  | 1.38x faster                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| float          | 69.0 ms                                                | 58.3 ms: 1.18x faster                                          |
| nbody          | 93.0 ms                                                | 79.4 ms: 1.17x faster                                          |
| pidigits       | 282 ms                                                 | 284 ms: 1.00x slower                                           |
| Geometric mean | (ref)                                                  | 1.11x faster                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 80.6 ms: 1.18x faster                                          |
| regex_dna      | 174 ms                                                 | 153 ms: 1.14x faster                                           |
| regex_v8       | 17.1 ms                                                | 17.8 ms: 1.04x slower                                          |
| regex_effbot   | 2.46 ms                                                | 2.71 ms: 1.10x slower                                          |
| Geometric mean | (ref)                                                  | 1.04x faster                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 207 us: 1.35x faster                                           |
| json_dumps           | 8.11 ms                                                | 6.68 ms: 1.21x faster                                          |
| unpickle_pure_python | 194 us                                                 | 169 us: 1.15x faster                                           |
| xml_etree_process    | 46.5 ms                                                | 41.3 ms: 1.13x faster                                          |
| tomli_loads          | 1.71 sec                                               | 1.53 sec: 1.11x faster                                         |
| unpickle             | 8.80 us                                                | 9.16 us: 1.04x slower                                          |
| json_loads           | 16.4 us                                                | 17.3 us: 1.05x slower                                          |
| pickle_dict          | 17.0 us                                                | 17.9 us: 1.06x slower                                          |
| pickle_list          | 2.74 us                                                | 2.93 us: 1.07x slower                                          |
| xml_etree_iterparse  | 72.1 ms                                                | 77.6 ms: 1.08x slower                                          |
| pickle               | 6.97 us                                                | 7.51 us: 1.08x slower                                          |
| xml_etree_generate   | 53.5 ms                                                | 58.6 ms: 1.10x slower                                          |
| unpickle_list        | 2.69 us                                                | 3.11 us: 1.16x slower                                          |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                   |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 13.3 ms: 1.23x slower                                          |
| python_startup_no_site | 7.91 ms                                                | 12.0 ms: 1.51x slower                                          |
| Geometric mean         | (ref)                                                  | 1.36x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 9.87 ms                                                | 8.10 ms: 1.22x faster                                          |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 75.8 us: 4.26x faster                                          |
| deltablue                | 4.91 ms                                                | 2.62 ms: 1.88x faster                                          |
| raytrace                 | 301 ms                                                 | 188 ms: 1.60x faster                                           |
| logging_silent           | 117 ns                                                 | 73.6 ns: 1.59x faster                                          |
| asyncio_tcp              | 659 ms                                                 | 430 ms: 1.53x faster                                           |
| richards_super           | 57.8 ms                                                | 38.0 ms: 1.52x faster                                          |
| chaos                    | 65.8 ms                                                | 43.6 ms: 1.51x faster                                          |
| async_tree_none          | 388 ms                                                 | 258 ms: 1.50x faster                                           |
| richards                 | 48.7 ms                                                | 34.1 ms: 1.43x faster                                          |
| async_tree_memoization   | 474 ms                                                 | 334 ms: 1.42x faster                                           |
| sqlglot_parse            | 1.24 ms                                                | 878 us: 1.42x faster                                           |
| crypto_pyaes             | 71.8 ms                                                | 50.9 ms: 1.41x faster                                          |
| async_tree_io            | 980 ms                                                 | 714 ms: 1.37x faster                                           |
| pickle_pure_python       | 281 us                                                 | 207 us: 1.35x faster                                           |
| sqlglot_transpile        | 1.44 ms                                                | 1.07 ms: 1.35x faster                                          |
| unpack_sequence          | 39.0 ns                                                | 29.0 ns: 1.35x faster                                          |
| deepcopy_memo            | 34.7 us                                                | 26.5 us: 1.31x faster                                          |
| go                       | 151 ms                                                 | 115 ms: 1.31x faster                                           |
| scimark_lu               | 103 ms                                                 | 80.4 ms: 1.28x faster                                          |
| generators               | 32.3 ms                                                | 25.7 ms: 1.26x faster                                          |
| scimark_monte_carlo      | 65.6 ms                                                | 52.1 ms: 1.26x faster                                          |
| comprehensions           | 16.9 us                                                | 13.7 us: 1.24x faster                                          |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.31 sec: 1.23x faster                                         |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 530 ms: 1.22x faster                                           |
| chameleon                | 6.26 ms                                                | 5.12 ms: 1.22x faster                                          |
| create_gc_cycles         | 860 us                                                 | 704 us: 1.22x faster                                           |
| mako                     | 9.87 ms                                                | 8.10 ms: 1.22x faster                                          |
| pyflate                  | 427 ms                                                 | 351 ms: 1.22x faster                                           |
| json_dumps               | 8.11 ms                                                | 6.68 ms: 1.21x faster                                          |
| pycparser                | 877 ms                                                 | 725 ms: 1.21x faster                                           |
| logging_format           | 4.83 us                                                | 4.00 us: 1.21x faster                                          |
| logging_simple           | 4.45 us                                                | 3.69 us: 1.21x faster                                          |
| tornado_http             | 86.7 ms                                                | 72.8 ms: 1.19x faster                                          |
| float                    | 69.0 ms                                                | 58.3 ms: 1.18x faster                                          |
| regex_compile            | 95.3 ms                                                | 80.6 ms: 1.18x faster                                          |
| scimark_sor              | 128 ms                                                 | 109 ms: 1.17x faster                                           |
| pprint_safe_repr         | 641 ms                                                 | 546 ms: 1.17x faster                                           |
| pprint_pformat           | 1.30 sec                                               | 1.11 sec: 1.17x faster                                         |
| nbody                    | 93.0 ms                                                | 79.4 ms: 1.17x faster                                          |
| dulwich_log              | 35.3 ms                                                | 30.5 ms: 1.16x faster                                          |
| unpickle_pure_python     | 194 us                                                 | 169 us: 1.15x faster                                           |
| spectral_norm            | 94.8 ms                                                | 82.8 ms: 1.15x faster                                          |
| regex_dna                | 174 ms                                                 | 153 ms: 1.14x faster                                           |
| sympy_sum                | 92.2 ms                                                | 80.8 ms: 1.14x faster                                          |
| hexiom                   | 6.19 ms                                                | 5.43 ms: 1.14x faster                                          |
| deepcopy                 | 272 us                                                 | 238 us: 1.14x faster                                           |
| xml_etree_process        | 46.5 ms                                                | 41.3 ms: 1.13x faster                                          |
| docutils                 | 1.73 sec                                               | 1.54 sec: 1.13x faster                                         |
| tomli_loads              | 1.71 sec                                               | 1.53 sec: 1.11x faster                                         |
| deepcopy_reduce          | 2.33 us                                                | 2.13 us: 1.09x faster                                          |
| sympy_integrate          | 13.1 ms                                                | 12.0 ms: 1.09x faster                                          |
| coroutines               | 20.7 ms                                                | 19.0 ms: 1.09x faster                                          |
| dask                     | 253 ms                                                 | 234 ms: 1.08x faster                                           |
| sympy_str                | 165 ms                                                 | 153 ms: 1.08x faster                                           |
| 2to3                     | 192 ms                                                 | 182 ms: 1.05x faster                                           |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 3.31 ms: 1.03x faster                                          |
| sympy_expand             | 269 ms                                                 | 260 ms: 1.03x faster                                           |
| json                     | 3.08 ms                                                | 3.02 ms: 1.02x faster                                          |
| scimark_fft              | 224 ms                                                 | 222 ms: 1.01x faster                                           |
| meteor_contest           | 77.7 ms                                                | 77.4 ms: 1.00x faster                                          |
| sqlglot_optimize         | 36.8 ms                                                | 36.9 ms: 1.00x slower                                          |
| pidigits                 | 282 ms                                                 | 284 ms: 1.00x slower                                           |
| bench_thread_pool        | 527 us                                                 | 531 us: 1.01x slower                                           |
| gc_traversal             | 2.36 ms                                                | 2.40 ms: 1.01x slower                                          |
| pathlib                  | 24.5 ms                                                | 24.9 ms: 1.02x slower                                          |
| sqlglot_normalize        | 190 ms                                                 | 195 ms: 1.02x slower                                           |
| regex_v8                 | 17.1 ms                                                | 17.8 ms: 1.04x slower                                          |
| nqueens                  | 63.8 ms                                                | 66.2 ms: 1.04x slower                                          |
| unpickle                 | 8.80 us                                                | 9.16 us: 1.04x slower                                          |
| mdp                      | 1.63 sec                                               | 1.70 sec: 1.04x slower                                         |
| json_loads               | 16.4 us                                                | 17.3 us: 1.05x slower                                          |
| pickle_dict              | 17.0 us                                                | 17.9 us: 1.06x slower                                          |
| pickle_list              | 2.74 us                                                | 2.93 us: 1.07x slower                                          |
| xml_etree_iterparse      | 72.1 ms                                                | 77.6 ms: 1.08x slower                                          |
| pickle                   | 6.97 us                                                | 7.51 us: 1.08x slower                                          |
| xml_etree_generate       | 53.5 ms                                                | 58.6 ms: 1.10x slower                                          |
| regex_effbot             | 2.46 ms                                                | 2.71 ms: 1.10x slower                                          |
| sqlite_synth             | 1.46 us                                                | 1.67 us: 1.15x slower                                          |
| coverage                 | 41.5 ms                                                | 47.8 ms: 1.15x slower                                          |
| unpickle_list            | 2.69 us                                                | 3.11 us: 1.16x slower                                          |
| python_startup           | 10.9 ms                                                | 13.3 ms: 1.23x slower                                          |
| bench_mp_pool            | 37.4 ms                                                | 47.8 ms: 1.28x slower                                          |
| telco                    | 3.49 ms                                                | 4.69 ms: 1.34x slower                                          |
| async_generators         | 231 ms                                                 | 315 ms: 1.36x slower                                           |
| python_startup_no_site   | 7.91 ms                                                | 12.0 ms: 1.51x slower                                          |
| Geometric mean           | (ref)                                                  | 1.13x faster                                                   |

Benchmark hidden because not significant (4): mypy2, asyncio_websockets, fannkuch, xml_etree_parse
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231219-3.13.0a2+-b63610e-JIT/bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.11x
- 95% likely to have a speedup of 1.09x
- 99% likely to have a speedup of 1.07x


# Memory

- memory change: 1.27x