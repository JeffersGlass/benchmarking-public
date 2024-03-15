
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_continue
- machine: darwin-arm64
- commit hash: 6dafac2
- commit date: 2024-02-12
- overall geometric mean: 1.19x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.13x faster
- Memory change: 1.26x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 173 ms: 1.11x faster                                                    |
| chameleon      | 6.26 ms                                                | 4.77 ms: 1.31x faster                                                   |
| docutils       | 1.73 sec                                               | 1.47 sec: 1.18x faster                                                  |
| tornado_http   | 86.7 ms                                                | 69.2 ms: 1.25x faster                                                   |
| Geometric mean | (ref)                                                  | 1.21x faster                                                            |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|-------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 250 ms: 1.55x faster                                                    |
| async_tree_memoization  | 474 ms                                                 | 327 ms: 1.45x faster                                                    |
| async_tree_io           | 980 ms                                                 | 696 ms: 1.41x faster                                                    |
| async_tree_cpu_io_mixed | 649 ms                                                 | 517 ms: 1.26x faster                                                    |
| Geometric mean          | (ref)                                                  | 1.41x faster                                                            |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| float          | 69.0 ms                                                | 54.8 ms: 1.26x faster                                                   |
| nbody          | 93.0 ms                                                | 75.5 ms: 1.23x faster                                                   |
| Geometric mean | (ref)                                                  | 1.16x faster                                                            |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 74.6 ms: 1.28x faster                                                   |
| regex_dna      | 174 ms                                                 | 152 ms: 1.15x faster                                                    |
| regex_v8       | 17.1 ms                                                | 17.0 ms: 1.01x faster                                                   |
| regex_effbot   | 2.46 ms                                                | 2.55 ms: 1.04x slower                                                   |
| Geometric mean | (ref)                                                  | 1.09x faster                                                            |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 195 us: 1.44x faster                                                    |
| json_dumps           | 8.11 ms                                                | 6.48 ms: 1.25x faster                                                   |
| tomli_loads          | 1.71 sec                                               | 1.37 sec: 1.25x faster                                                  |
| unpickle_pure_python | 194 us                                                 | 158 us: 1.23x faster                                                    |
| xml_etree_process    | 46.5 ms                                                | 38.5 ms: 1.21x faster                                                   |
| xml_etree_parse      | 108 ms                                                 | 107 ms: 1.01x faster                                                    |
| xml_etree_iterparse  | 72.1 ms                                                | 74.9 ms: 1.04x slower                                                   |
| json_loads           | 16.4 us                                                | 17.1 us: 1.04x slower                                                   |
| pickle               | 6.97 us                                                | 7.27 us: 1.04x slower                                                   |
| unpickle             | 8.80 us                                                | 9.17 us: 1.04x slower                                                   |
| xml_etree_generate   | 53.5 ms                                                | 55.8 ms: 1.04x slower                                                   |
| pickle_dict          | 17.0 us                                                | 18.1 us: 1.07x slower                                                   |
| pickle_list          | 2.74 us                                                | 2.95 us: 1.08x slower                                                   |
| unpickle_list        | 2.69 us                                                | 3.09 us: 1.15x slower                                                   |
| Geometric mean       | (ref)                                                  | 1.05x faster                                                            |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 13.3 ms: 1.23x slower                                                   |
| python_startup_no_site | 7.91 ms                                                | 12.0 ms: 1.51x slower                                                   |
| Geometric mean         | (ref)                                                  | 1.36x slower                                                            |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|-----------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| mako      | 9.87 ms                                                | 7.47 ms: 1.32x faster                                                   |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|--------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 70.0 us: 4.62x faster                                                   |
| deltablue                | 4.91 ms                                                | 2.44 ms: 2.01x faster                                                   |
| raytrace                 | 301 ms                                                 | 176 ms: 1.71x faster                                                    |
| logging_silent           | 117 ns                                                 | 70.5 ns: 1.66x faster                                                   |
| richards_super           | 57.8 ms                                                | 35.6 ms: 1.63x faster                                                   |
| chaos                    | 65.8 ms                                                | 40.7 ms: 1.62x faster                                                   |
| asyncio_tcp              | 659 ms                                                 | 412 ms: 1.60x faster                                                    |
| sqlglot_parse            | 1.24 ms                                                | 785 us: 1.58x faster                                                    |
| async_tree_none          | 388 ms                                                 | 250 ms: 1.55x faster                                                    |
| richards                 | 48.7 ms                                                | 31.9 ms: 1.53x faster                                                   |
| crypto_pyaes             | 71.8 ms                                                | 48.4 ms: 1.48x faster                                                   |
| sqlglot_transpile        | 1.44 ms                                                | 972 us: 1.48x faster                                                    |
| async_tree_memoization   | 474 ms                                                 | 327 ms: 1.45x faster                                                    |
| pickle_pure_python       | 281 us                                                 | 195 us: 1.44x faster                                                    |
| comprehensions           | 16.9 us                                                | 12.0 us: 1.41x faster                                                   |
| async_tree_io            | 980 ms                                                 | 696 ms: 1.41x faster                                                    |
| go                       | 151 ms                                                 | 109 ms: 1.39x faster                                                    |
| scimark_lu               | 103 ms                                                 | 74.8 ms: 1.38x faster                                                   |
| scimark_monte_carlo      | 65.6 ms                                                | 47.8 ms: 1.37x faster                                                   |
| unpack_sequence          | 39.0 ns                                                | 28.5 ns: 1.37x faster                                                   |
| deepcopy_memo            | 34.7 us                                                | 25.8 us: 1.35x faster                                                   |
| pyflate                  | 427 ms                                                 | 321 ms: 1.33x faster                                                    |
| mako                     | 9.87 ms                                                | 7.47 ms: 1.32x faster                                                   |
| chameleon                | 6.26 ms                                                | 4.77 ms: 1.31x faster                                                   |
| hexiom                   | 6.19 ms                                                | 4.78 ms: 1.29x faster                                                   |
| pprint_pformat           | 1.30 sec                                               | 1.01 sec: 1.29x faster                                                  |
| logging_simple           | 4.45 us                                                | 3.46 us: 1.28x faster                                                   |
| pprint_safe_repr         | 641 ms                                                 | 501 ms: 1.28x faster                                                    |
| regex_compile            | 95.3 ms                                                | 74.6 ms: 1.28x faster                                                   |
| logging_format           | 4.83 us                                                | 3.79 us: 1.28x faster                                                   |
| pycparser                | 877 ms                                                 | 692 ms: 1.27x faster                                                    |
| float                    | 69.0 ms                                                | 54.8 ms: 1.26x faster                                                   |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 517 ms: 1.26x faster                                                    |
| tornado_http             | 86.7 ms                                                | 69.2 ms: 1.25x faster                                                   |
| json_dumps               | 8.11 ms                                                | 6.48 ms: 1.25x faster                                                   |
| tomli_loads              | 1.71 sec                                               | 1.37 sec: 1.25x faster                                                  |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.30 sec: 1.23x faster                                                  |
| sympy_sum                | 92.2 ms                                                | 74.8 ms: 1.23x faster                                                   |
| nbody                    | 93.0 ms                                                | 75.5 ms: 1.23x faster                                                   |
| unpickle_pure_python     | 194 us                                                 | 158 us: 1.23x faster                                                    |
| create_gc_cycles         | 860 us                                                 | 704 us: 1.22x faster                                                    |
| scimark_sor              | 128 ms                                                 | 106 ms: 1.22x faster                                                    |
| spectral_norm            | 94.8 ms                                                | 78.1 ms: 1.21x faster                                                   |
| xml_etree_process        | 46.5 ms                                                | 38.5 ms: 1.21x faster                                                   |
| deepcopy                 | 272 us                                                 | 226 us: 1.20x faster                                                    |
| dulwich_log              | 35.3 ms                                                | 29.7 ms: 1.19x faster                                                   |
| docutils                 | 1.73 sec                                               | 1.47 sec: 1.18x faster                                                  |
| sympy_integrate          | 13.1 ms                                                | 11.1 ms: 1.18x faster                                                   |
| deepcopy_reduce          | 2.33 us                                                | 1.99 us: 1.17x faster                                                   |
| sympy_str                | 165 ms                                                 | 141 ms: 1.17x faster                                                    |
| mypy2                    | 607 ms                                                 | 522 ms: 1.16x faster                                                    |
| fannkuch                 | 303 ms                                                 | 263 ms: 1.15x faster                                                    |
| regex_dna                | 174 ms                                                 | 152 ms: 1.15x faster                                                    |
| generators               | 32.3 ms                                                | 28.4 ms: 1.14x faster                                                   |
| dask                     | 253 ms                                                 | 224 ms: 1.13x faster                                                    |
| coroutines               | 20.7 ms                                                | 18.4 ms: 1.12x faster                                                   |
| sympy_expand             | 269 ms                                                 | 240 ms: 1.12x faster                                                    |
| 2to3                     | 192 ms                                                 | 173 ms: 1.11x faster                                                    |
| sqlglot_optimize         | 36.8 ms                                                | 34.2 ms: 1.07x faster                                                   |
| bench_thread_pool        | 527 us                                                 | 499 us: 1.06x faster                                                    |
| scimark_fft              | 224 ms                                                 | 213 ms: 1.05x faster                                                    |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 3.27 ms: 1.05x faster                                                   |
| meteor_contest           | 77.7 ms                                                | 74.3 ms: 1.05x faster                                                   |
| sqlglot_normalize        | 190 ms                                                 | 182 ms: 1.04x faster                                                    |
| pathlib                  | 24.5 ms                                                | 23.5 ms: 1.04x faster                                                   |
| json                     | 3.08 ms                                                | 2.97 ms: 1.04x faster                                                   |
| nqueens                  | 63.8 ms                                                | 61.5 ms: 1.04x faster                                                   |
| mdp                      | 1.63 sec                                               | 1.59 sec: 1.02x faster                                                  |
| xml_etree_parse          | 108 ms                                                 | 107 ms: 1.01x faster                                                    |
| regex_v8                 | 17.1 ms                                                | 17.0 ms: 1.01x faster                                                   |
| asyncio_websockets       | 410 ms                                                 | 408 ms: 1.00x faster                                                    |
| gc_traversal             | 2.36 ms                                                | 2.39 ms: 1.01x slower                                                   |
| regex_effbot             | 2.46 ms                                                | 2.55 ms: 1.04x slower                                                   |
| xml_etree_iterparse      | 72.1 ms                                                | 74.9 ms: 1.04x slower                                                   |
| json_loads               | 16.4 us                                                | 17.1 us: 1.04x slower                                                   |
| pickle                   | 6.97 us                                                | 7.27 us: 1.04x slower                                                   |
| unpickle                 | 8.80 us                                                | 9.17 us: 1.04x slower                                                   |
| xml_etree_generate       | 53.5 ms                                                | 55.8 ms: 1.04x slower                                                   |
| pickle_dict              | 17.0 us                                                | 18.1 us: 1.07x slower                                                   |
| pickle_list              | 2.74 us                                                | 2.95 us: 1.08x slower                                                   |
| sqlite_synth             | 1.46 us                                                | 1.58 us: 1.08x slower                                                   |
| coverage                 | 41.5 ms                                                | 47.5 ms: 1.15x slower                                                   |
| unpickle_list            | 2.69 us                                                | 3.09 us: 1.15x slower                                                   |
| python_startup           | 10.9 ms                                                | 13.3 ms: 1.23x slower                                                   |
| bench_mp_pool            | 37.4 ms                                                | 46.8 ms: 1.25x slower                                                   |
| telco                    | 3.49 ms                                                | 4.45 ms: 1.27x slower                                                   |
| async_generators         | 231 ms                                                 | 301 ms: 1.30x slower                                                    |
| python_startup_no_site   | 7.91 ms                                                | 12.0 ms: 1.51x slower                                                   |
| Geometric mean           | (ref)                                                  | 1.19x faster                                                            |

Benchmark hidden because not significant (1): pidigits
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240212-3.13.0a3+-6dafac2-JIT/bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-6dafac2.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.17x
- 95% likely to have a speedup of 1.15x
- 99% likely to have a speedup of 1.13x


# Memory

- memory change: 1.26x