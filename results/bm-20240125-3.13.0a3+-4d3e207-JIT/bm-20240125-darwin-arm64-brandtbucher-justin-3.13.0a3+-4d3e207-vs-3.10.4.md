
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin
- machine: darwin-arm64
- commit hash: 4d3e207
- commit date: 2024-01-25
- overall geometric mean: 1.17x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.11x faster
- Memory change: 1.27x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-darwin-arm64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 174 ms: 1.10x faster                                           |
| chameleon      | 6.26 ms                                                | 4.91 ms: 1.27x faster                                          |
| docutils       | 1.73 sec                                               | 1.48 sec: 1.17x faster                                         |
| tornado_http   | 86.7 ms                                                | 70.7 ms: 1.23x faster                                          |
| Geometric mean | (ref)                                                  | 1.19x faster                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-darwin-arm64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 253 ms: 1.53x faster                                           |
| async_tree_memoization  | 474 ms                                                 | 328 ms: 1.44x faster                                           |
| async_tree_io           | 980 ms                                                 | 698 ms: 1.40x faster                                           |
| async_tree_cpu_io_mixed | 649 ms                                                 | 521 ms: 1.25x faster                                           |
| Geometric mean          | (ref)                                                  | 1.40x faster                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-darwin-arm64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| float          | 69.0 ms                                                | 56.2 ms: 1.23x faster                                          |
| nbody          | 93.0 ms                                                | 77.1 ms: 1.21x faster                                          |
| pidigits       | 282 ms                                                 | 283 ms: 1.00x slower                                           |
| Geometric mean | (ref)                                                  | 1.14x faster                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-darwin-arm64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 76.5 ms: 1.25x faster                                          |
| regex_dna      | 174 ms                                                 | 156 ms: 1.12x faster                                           |
| regex_v8       | 17.1 ms                                                | 17.9 ms: 1.04x slower                                          |
| regex_effbot   | 2.46 ms                                                | 2.75 ms: 1.12x slower                                          |
| Geometric mean | (ref)                                                  | 1.05x faster                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-darwin-arm64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 197 us: 1.42x faster                                           |
| json_dumps           | 8.11 ms                                                | 6.54 ms: 1.24x faster                                          |
| unpickle_pure_python | 194 us                                                 | 158 us: 1.23x faster                                           |
| tomli_loads          | 1.71 sec                                               | 1.41 sec: 1.21x faster                                         |
| xml_etree_process    | 46.5 ms                                                | 39.1 ms: 1.19x faster                                          |
| xml_etree_parse      | 108 ms                                                 | 106 ms: 1.02x faster                                           |
| unpickle             | 8.80 us                                                | 9.15 us: 1.04x slower                                          |
| pickle               | 6.97 us                                                | 7.26 us: 1.04x slower                                          |
| json_loads           | 16.4 us                                                | 17.2 us: 1.04x slower                                          |
| xml_etree_iterparse  | 72.1 ms                                                | 76.2 ms: 1.06x slower                                          |
| xml_etree_generate   | 53.5 ms                                                | 56.7 ms: 1.06x slower                                          |
| pickle_dict          | 17.0 us                                                | 18.1 us: 1.06x slower                                          |
| pickle_list          | 2.74 us                                                | 2.98 us: 1.09x slower                                          |
| unpickle_list        | 2.69 us                                                | 3.07 us: 1.14x slower                                          |
| Geometric mean       | (ref)                                                  | 1.05x faster                                                   |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-darwin-arm64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 12.9 ms: 1.19x slower                                          |
| python_startup_no_site | 7.91 ms                                                | 11.3 ms: 1.43x slower                                          |
| Geometric mean         | (ref)                                                  | 1.30x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-darwin-arm64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 9.87 ms                                                | 7.94 ms: 1.24x faster                                          |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-darwin-arm64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 71.9 us: 4.49x faster                                          |
| deltablue                | 4.91 ms                                                | 2.51 ms: 1.96x faster                                          |
| logging_silent           | 117 ns                                                 | 69.6 ns: 1.68x faster                                          |
| raytrace                 | 301 ms                                                 | 179 ms: 1.68x faster                                           |
| richards_super           | 57.8 ms                                                | 35.7 ms: 1.62x faster                                          |
| chaos                    | 65.8 ms                                                | 42.1 ms: 1.56x faster                                          |
| sqlglot_parse            | 1.24 ms                                                | 800 us: 1.55x faster                                           |
| async_tree_none          | 388 ms                                                 | 253 ms: 1.53x faster                                           |
| richards                 | 48.7 ms                                                | 31.8 ms: 1.53x faster                                          |
| asyncio_tcp              | 659 ms                                                 | 442 ms: 1.49x faster                                           |
| sqlglot_transpile        | 1.44 ms                                                | 980 us: 1.47x faster                                           |
| async_tree_memoization   | 474 ms                                                 | 328 ms: 1.44x faster                                           |
| crypto_pyaes             | 71.8 ms                                                | 50.4 ms: 1.42x faster                                          |
| pickle_pure_python       | 281 us                                                 | 197 us: 1.42x faster                                           |
| async_tree_io            | 980 ms                                                 | 698 ms: 1.40x faster                                           |
| scimark_lu               | 103 ms                                                 | 74.9 ms: 1.37x faster                                          |
| go                       | 151 ms                                                 | 110 ms: 1.37x faster                                           |
| deepcopy_memo            | 34.7 us                                                | 25.9 us: 1.34x faster                                          |
| scimark_monte_carlo      | 65.6 ms                                                | 49.1 ms: 1.33x faster                                          |
| unpack_sequence          | 39.0 ns                                                | 29.5 ns: 1.32x faster                                          |
| comprehensions           | 16.9 us                                                | 12.9 us: 1.31x faster                                          |
| pyflate                  | 427 ms                                                 | 329 ms: 1.30x faster                                           |
| logging_format           | 4.83 us                                                | 3.76 us: 1.28x faster                                          |
| logging_simple           | 4.45 us                                                | 3.47 us: 1.28x faster                                          |
| chameleon                | 6.26 ms                                                | 4.91 ms: 1.27x faster                                          |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.27 sec: 1.27x faster                                         |
| pycparser                | 877 ms                                                 | 699 ms: 1.25x faster                                           |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 521 ms: 1.25x faster                                           |
| regex_compile            | 95.3 ms                                                | 76.5 ms: 1.25x faster                                          |
| mako                     | 9.87 ms                                                | 7.94 ms: 1.24x faster                                          |
| json_dumps               | 8.11 ms                                                | 6.54 ms: 1.24x faster                                          |
| unpickle_pure_python     | 194 us                                                 | 158 us: 1.23x faster                                           |
| float                    | 69.0 ms                                                | 56.2 ms: 1.23x faster                                          |
| tornado_http             | 86.7 ms                                                | 70.7 ms: 1.23x faster                                          |
| create_gc_cycles         | 860 us                                                 | 705 us: 1.22x faster                                           |
| pprint_safe_repr         | 641 ms                                                 | 526 ms: 1.22x faster                                           |
| hexiom                   | 6.19 ms                                                | 5.10 ms: 1.21x faster                                          |
| tomli_loads              | 1.71 sec                                               | 1.41 sec: 1.21x faster                                         |
| scimark_sor              | 128 ms                                                 | 106 ms: 1.21x faster                                           |
| pprint_pformat           | 1.30 sec                                               | 1.08 sec: 1.21x faster                                         |
| nbody                    | 93.0 ms                                                | 77.1 ms: 1.21x faster                                          |
| deepcopy                 | 272 us                                                 | 225 us: 1.21x faster                                           |
| sympy_sum                | 92.2 ms                                                | 76.9 ms: 1.20x faster                                          |
| xml_etree_process        | 46.5 ms                                                | 39.1 ms: 1.19x faster                                          |
| dulwich_log              | 35.3 ms                                                | 30.1 ms: 1.18x faster                                          |
| deepcopy_reduce          | 2.33 us                                                | 1.99 us: 1.17x faster                                          |
| docutils                 | 1.73 sec                                               | 1.48 sec: 1.17x faster                                         |
| sympy_integrate          | 13.1 ms                                                | 11.3 ms: 1.16x faster                                          |
| sympy_str                | 165 ms                                                 | 143 ms: 1.16x faster                                           |
| spectral_norm            | 94.8 ms                                                | 82.0 ms: 1.16x faster                                          |
| generators               | 32.3 ms                                                | 28.0 ms: 1.16x faster                                          |
| mypy2                    | 607 ms                                                 | 526 ms: 1.15x faster                                           |
| regex_dna                | 174 ms                                                 | 156 ms: 1.12x faster                                           |
| dask                     | 253 ms                                                 | 226 ms: 1.12x faster                                           |
| sympy_expand             | 269 ms                                                 | 242 ms: 1.11x faster                                           |
| 2to3                     | 192 ms                                                 | 174 ms: 1.10x faster                                           |
| coroutines               | 20.7 ms                                                | 18.9 ms: 1.10x faster                                          |
| fannkuch                 | 303 ms                                                 | 278 ms: 1.09x faster                                           |
| sqlglot_optimize         | 36.8 ms                                                | 35.0 ms: 1.05x faster                                          |
| json                     | 3.08 ms                                                | 2.93 ms: 1.05x faster                                          |
| meteor_contest           | 77.7 ms                                                | 74.3 ms: 1.05x faster                                          |
| bench_thread_pool        | 527 us                                                 | 509 us: 1.04x faster                                           |
| sqlglot_normalize        | 190 ms                                                 | 186 ms: 1.03x faster                                           |
| scimark_fft              | 224 ms                                                 | 220 ms: 1.02x faster                                           |
| pathlib                  | 24.5 ms                                                | 24.0 ms: 1.02x faster                                          |
| xml_etree_parse          | 108 ms                                                 | 106 ms: 1.02x faster                                           |
| nqueens                  | 63.8 ms                                                | 62.8 ms: 1.02x faster                                          |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 3.38 ms: 1.01x faster                                          |
| mdp                      | 1.63 sec                                               | 1.62 sec: 1.01x faster                                         |
| pidigits                 | 282 ms                                                 | 283 ms: 1.00x slower                                           |
| gc_traversal             | 2.36 ms                                                | 2.40 ms: 1.02x slower                                          |
| unpickle                 | 8.80 us                                                | 9.15 us: 1.04x slower                                          |
| pickle                   | 6.97 us                                                | 7.26 us: 1.04x slower                                          |
| regex_v8                 | 17.1 ms                                                | 17.9 ms: 1.04x slower                                          |
| json_loads               | 16.4 us                                                | 17.2 us: 1.04x slower                                          |
| xml_etree_iterparse      | 72.1 ms                                                | 76.2 ms: 1.06x slower                                          |
| xml_etree_generate       | 53.5 ms                                                | 56.7 ms: 1.06x slower                                          |
| pickle_dict              | 17.0 us                                                | 18.1 us: 1.06x slower                                          |
| pickle_list              | 2.74 us                                                | 2.98 us: 1.09x slower                                          |
| sqlite_synth             | 1.46 us                                                | 1.60 us: 1.10x slower                                          |
| regex_effbot             | 2.46 ms                                                | 2.75 ms: 1.12x slower                                          |
| coverage                 | 41.5 ms                                                | 47.1 ms: 1.14x slower                                          |
| unpickle_list            | 2.69 us                                                | 3.07 us: 1.14x slower                                          |
| python_startup           | 10.9 ms                                                | 12.9 ms: 1.19x slower                                          |
| bench_mp_pool            | 37.4 ms                                                | 46.1 ms: 1.23x slower                                          |
| async_generators         | 231 ms                                                 | 303 ms: 1.31x slower                                           |
| telco                    | 3.49 ms                                                | 4.63 ms: 1.33x slower                                          |
| python_startup_no_site   | 7.91 ms                                                | 11.3 ms: 1.43x slower                                          |
| Geometric mean           | (ref)                                                  | 1.17x faster                                                   |

Benchmark hidden because not significant (1): asyncio_websockets
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240125-3.13.0a3+-4d3e207-JIT/bm-20240125-darwin-arm64-brandtbucher-justin-3.13.0a3+-4d3e207.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.15x
- 95% likely to have a speedup of 1.13x
- 99% likely to have a speedup of 1.11x


# Memory

- memory change: 1.27x