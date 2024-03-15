
# Results vs. 3.11.0

- fork: python
- ref: 7d4cc5aa854fdea4d01a
- machine: darwin-arm64
- commit hash: 7d4cc5a
- commit date: 2023-04-04
- overall geometric mean: 1.27x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.23x slower
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-darwin-arm64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 203 ms: 1.32x slower                                                 |
| chameleon      | 4.30 ms                                                | 5.75 ms: 1.34x slower                                                |
| docutils       | 1.43 sec                                               | 1.79 sec: 1.25x slower                                               |
| html5lib       | 33.0 ms                                                | 47.8 ms: 1.45x slower                                                |
| tornado_http   | 69.1 ms                                                | 91.2 ms: 1.32x slower                                                |
| Geometric mean | (ref)                                                  | 1.33x slower                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-darwin-arm64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 519 ms                                                 | 668 ms: 1.29x slower                                                 |
| async_tree_none         | 282 ms                                                 | 399 ms: 1.42x slower                                                 |
| async_tree_memoization  | 336 ms                                                 | 490 ms: 1.46x slower                                                 |
| async_tree_io           | 697 ms                                                 | 1.02 sec: 1.46x slower                                               |
| Geometric mean          | (ref)                                                  | 1.40x slower                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-darwin-arm64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 282 ms: 1.01x slower                                                 |
| float          | 50.8 ms                                                | 72.2 ms: 1.42x slower                                                |
| nbody          | 61.7 ms                                                | 94.0 ms: 1.52x slower                                                |
| Geometric mean | (ref)                                                  | 1.30x slower                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-darwin-arm64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_effbot   | 2.43 ms                                                | 2.69 ms: 1.11x slower                                                |
| regex_v8       | 15.1 ms                                                | 18.0 ms: 1.19x slower                                                |
| regex_dna      | 148 ms                                                 | 185 ms: 1.25x slower                                                 |
| regex_compile  | 72.8 ms                                                | 96.9 ms: 1.33x slower                                                |
| Geometric mean | (ref)                                                  | 1.22x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-darwin-arm64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| xml_etree_iterparse  | 68.3 ms                                                | 73.2 ms: 1.07x slower                                                |
| pickle_list          | 2.70 us                                                | 2.90 us: 1.07x slower                                                |
| pickle               | 6.98 us                                                | 7.56 us: 1.08x slower                                                |
| json_dumps           | 7.53 ms                                                | 8.27 ms: 1.10x slower                                                |
| json_loads           | 15.3 us                                                | 16.8 us: 1.10x slower                                                |
| pickle_dict          | 17.1 us                                                | 18.8 us: 1.10x slower                                                |
| xml_etree_parse      | 100 ms                                                 | 113 ms: 1.13x slower                                                 |
| xml_etree_generate   | 45.8 ms                                                | 54.3 ms: 1.19x slower                                                |
| unpickle             | 8.29 us                                                | 9.89 us: 1.19x slower                                                |
| xml_etree_process    | 33.6 ms                                                | 44.9 ms: 1.34x slower                                                |
| unpickle_pure_python | 149 us                                                 | 204 us: 1.37x slower                                                 |
| pickle_pure_python   | 191 us                                                 | 285 us: 1.49x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.16x slower                                                         |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-darwin-arm64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup_no_site | 8.57 ms                                                | 9.13 ms: 1.07x slower                                                |
| python_startup         | 10.8 ms                                                | 12.1 ms: 1.13x slower                                                |
| Geometric mean         | (ref)                                                  | 1.10x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-darwin-arm64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| genshi_text     | 14.4 ms                                                | 18.2 ms: 1.27x slower                                                |
| genshi_xml      | 28.5 ms                                                | 37.3 ms: 1.31x slower                                                |
| mako            | 7.93 ms                                                | 10.6 ms: 1.33x slower                                                |
| django_template | 20.1 ms                                                | 27.1 ms: 1.35x slower                                                |
| Geometric mean  | (ref)                                                  | 1.31x slower                                                         |

All benchmarks:
===============

| Benchmark               | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-darwin-arm64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| coverage                | 43.9 ms                                                | 41.9 ms: 1.05x faster                                                |
| bench_mp_pool           | 41.0 ms                                                | 40.2 ms: 1.02x faster                                                |
| gc_traversal            | 2.38 ms                                                | 2.39 ms: 1.00x slower                                                |
| pidigits                | 280 ms                                                 | 282 ms: 1.01x slower                                                 |
| asyncio_tcp             | 643 ms                                                 | 669 ms: 1.04x slower                                                 |
| python_startup_no_site  | 8.57 ms                                                | 9.13 ms: 1.07x slower                                                |
| xml_etree_iterparse     | 68.3 ms                                                | 73.2 ms: 1.07x slower                                                |
| pickle_list             | 2.70 us                                                | 2.90 us: 1.07x slower                                                |
| generators              | 30.3 ms                                                | 32.7 ms: 1.08x slower                                                |
| pickle                  | 6.98 us                                                | 7.56 us: 1.08x slower                                                |
| json_dumps              | 7.53 ms                                                | 8.27 ms: 1.10x slower                                                |
| meteor_contest          | 71.1 ms                                                | 78.0 ms: 1.10x slower                                                |
| json_loads              | 15.3 us                                                | 16.8 us: 1.10x slower                                                |
| pickle_dict             | 17.1 us                                                | 18.8 us: 1.10x slower                                                |
| regex_effbot            | 2.43 ms                                                | 2.69 ms: 1.11x slower                                                |
| json                    | 2.75 ms                                                | 3.06 ms: 1.11x slower                                                |
| mdp                     | 1.48 sec                                               | 1.67 sec: 1.12x slower                                               |
| xml_etree_parse         | 100 ms                                                 | 113 ms: 1.13x slower                                                 |
| python_startup          | 10.8 ms                                                | 12.1 ms: 1.13x slower                                                |
| unpack_sequence         | 33.6 ns                                                | 38.3 ns: 1.14x slower                                                |
| bench_thread_pool       | 465 us                                                 | 532 us: 1.14x slower                                                 |
| telco                   | 3.17 ms                                                | 3.63 ms: 1.14x slower                                                |
| coroutines              | 17.2 ms                                                | 20.1 ms: 1.17x slower                                                |
| flaskblogging           | 2.35 ms                                                | 2.76 ms: 1.17x slower                                                |
| dask                    | 219 ms                                                 | 257 ms: 1.17x slower                                                 |
| sqlite_synth            | 1.26 us                                                | 1.48 us: 1.18x slower                                                |
| sympy_str               | 144 ms                                                 | 170 ms: 1.19x slower                                                 |
| xml_etree_generate      | 45.8 ms                                                | 54.3 ms: 1.19x slower                                                |
| sympy_integrate         | 11.3 ms                                                | 13.4 ms: 1.19x slower                                                |
| regex_v8                | 15.1 ms                                                | 18.0 ms: 1.19x slower                                                |
| unpickle                | 8.29 us                                                | 9.89 us: 1.19x slower                                                |
| sympy_sum               | 80.2 ms                                                | 96.4 ms: 1.20x slower                                                |
| sympy_expand            | 229 ms                                                 | 277 ms: 1.21x slower                                                 |
| sqlglot_normalize       | 162 ms                                                 | 196 ms: 1.21x slower                                                 |
| async_generators        | 192 ms                                                 | 233 ms: 1.21x slower                                                 |
| pylint                  | 253 ms                                                 | 307 ms: 1.22x slower                                                 |
| nqueens                 | 55.9 ms                                                | 68.0 ms: 1.22x slower                                                |
| pathlib                 | 23.2 ms                                                | 28.3 ms: 1.22x slower                                                |
| gunicorn                | 1.10 ms                                                | 1.34 ms: 1.23x slower                                                |
| scimark_sparse_mat_mult | 2.81 ms                                                | 3.46 ms: 1.23x slower                                                |
| create_gc_cycles        | 711 us                                                 | 874 us: 1.23x slower                                                 |
| aiohttp                 | 1.02 ms                                                | 1.26 ms: 1.23x slower                                                |
| comprehensions          | 14.4 us                                                | 17.9 us: 1.24x slower                                                |
| regex_dna               | 148 ms                                                 | 185 ms: 1.25x slower                                                 |
| docutils                | 1.43 sec                                               | 1.79 sec: 1.25x slower                                               |
| pprint_pformat          | 979 ms                                                 | 1.23 sec: 1.26x slower                                               |
| pprint_safe_repr        | 478 ms                                                 | 602 ms: 1.26x slower                                                 |
| sqlalchemy_declarative  | 59.3 ms                                                | 75.0 ms: 1.27x slower                                                |
| genshi_text             | 14.4 ms                                                | 18.2 ms: 1.27x slower                                                |
| sqlglot_optimize        | 29.6 ms                                                | 38.0 ms: 1.28x slower                                                |
| async_tree_cpu_io_mixed | 519 ms                                                 | 668 ms: 1.29x slower                                                 |
| dulwich_log             | 28.6 ms                                                | 36.9 ms: 1.29x slower                                                |
| sqlalchemy_imperative   | 6.98 ms                                                | 9.01 ms: 1.29x slower                                                |
| deepcopy                | 215 us                                                 | 279 us: 1.29x slower                                                 |
| genshi_xml              | 28.5 ms                                                | 37.3 ms: 1.31x slower                                                |
| 2to3                    | 154 ms                                                 | 203 ms: 1.32x slower                                                 |
| tornado_http            | 69.1 ms                                                | 91.2 ms: 1.32x slower                                                |
| deepcopy_reduce         | 1.79 us                                                | 2.38 us: 1.33x slower                                                |
| fannkuch                | 240 ms                                                 | 319 ms: 1.33x slower                                                 |
| regex_compile           | 72.8 ms                                                | 96.9 ms: 1.33x slower                                                |
| mako                    | 7.93 ms                                                | 10.6 ms: 1.33x slower                                                |
| xml_etree_process       | 33.6 ms                                                | 44.9 ms: 1.34x slower                                                |
| chameleon               | 4.30 ms                                                | 5.75 ms: 1.34x slower                                                |
| scimark_fft             | 173 ms                                                 | 231 ms: 1.34x slower                                                 |
| deepcopy_memo           | 25.7 us                                                | 34.5 us: 1.34x slower                                                |
| django_template         | 20.1 ms                                                | 27.1 ms: 1.35x slower                                                |
| logging_simple          | 3.41 us                                                | 4.65 us: 1.36x slower                                                |
| unpickle_pure_python    | 149 us                                                 | 204 us: 1.37x slower                                                 |
| logging_format          | 3.67 us                                                | 5.05 us: 1.38x slower                                                |
| pycparser               | 659 ms                                                 | 910 ms: 1.38x slower                                                 |
| hexiom                  | 4.58 ms                                                | 6.33 ms: 1.38x slower                                                |
| thrift                  | 410 us                                                 | 580 us: 1.41x slower                                                 |
| async_tree_none         | 282 ms                                                 | 399 ms: 1.42x slower                                                 |
| float                   | 50.8 ms                                                | 72.2 ms: 1.42x slower                                                |
| chaos                   | 47.4 ms                                                | 68.0 ms: 1.43x slower                                                |
| html5lib                | 33.0 ms                                                | 47.8 ms: 1.45x slower                                                |
| sqlglot_transpile       | 1.05 ms                                                | 1.53 ms: 1.46x slower                                                |
| async_tree_memoization  | 336 ms                                                 | 490 ms: 1.46x slower                                                 |
| async_tree_io           | 697 ms                                                 | 1.02 sec: 1.46x slower                                               |
| spectral_norm           | 65.7 ms                                                | 96.4 ms: 1.47x slower                                                |
| pickle_pure_python      | 191 us                                                 | 285 us: 1.49x slower                                                 |
| sqlglot_parse           | 890 us                                                 | 1.33 ms: 1.49x slower                                                |
| nbody                   | 61.7 ms                                                | 94.0 ms: 1.52x slower                                                |
| go                      | 105 ms                                                 | 165 ms: 1.56x slower                                                 |
| scimark_sor             | 79.2 ms                                                | 126 ms: 1.59x slower                                                 |
| pyflate                 | 284 ms                                                 | 455 ms: 1.60x slower                                                 |
| raytrace                | 206 ms                                                 | 331 ms: 1.61x slower                                                 |
| scimark_lu              | 67.7 ms                                                | 110 ms: 1.62x slower                                                 |
| richards                | 31.1 ms                                                | 50.7 ms: 1.63x slower                                                |
| crypto_pyaes            | 47.5 ms                                                | 78.3 ms: 1.65x slower                                                |
| scimark_monte_carlo     | 43.5 ms                                                | 72.3 ms: 1.66x slower                                                |
| logging_silent          | 66.5 ns                                                | 120 ns: 1.80x slower                                                 |
| deltablue               | 2.75 ms                                                | 5.17 ms: 1.88x slower                                                |
| Geometric mean          | (ref)                                                  | 1.27x slower                                                         |

Benchmark hidden because not significant (1): unpickle_list
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.25x
- 95% likely to have a slowdown of 1.24x
- 99% likely to have a slowdown of 1.23x


# Memory

- memory change: 0.93x