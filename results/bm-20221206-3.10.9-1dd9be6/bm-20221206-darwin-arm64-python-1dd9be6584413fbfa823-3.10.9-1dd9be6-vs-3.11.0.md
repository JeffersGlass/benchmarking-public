
# Results vs. 3.11.0

- fork: python
- ref: 1dd9be6584413fbfa823
- machine: darwin-arm64
- commit hash: 1dd9be6
- commit date: 2022-12-06
- overall geometric mean: 1.26x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.22x slower
- Memory change: 0.91x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 223 ms: 1.44x slower                                                |
| chameleon      | 4.30 ms                                                | 5.83 ms: 1.36x slower                                               |
| docutils       | 1.43 sec                                               | 1.77 sec: 1.24x slower                                              |
| html5lib       | 33.0 ms                                                | 46.5 ms: 1.41x slower                                               |
| tornado_http   | 69.1 ms                                                | 93.5 ms: 1.35x slower                                               |
| Geometric mean | (ref)                                                  | 1.36x slower                                                        |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6 |
|-------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 519 ms                                                 | 661 ms: 1.27x slower                                                |
| async_tree_none         | 282 ms                                                 | 394 ms: 1.40x slower                                                |
| async_tree_memoization  | 336 ms                                                 | 481 ms: 1.43x slower                                                |
| async_tree_io           | 697 ms                                                 | 1.00 sec: 1.44x slower                                              |
| Geometric mean          | (ref)                                                  | 1.38x slower                                                        |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 284 ms: 1.01x slower                                                |
| float          | 50.8 ms                                                | 72.1 ms: 1.42x slower                                               |
| nbody          | 61.7 ms                                                | 92.6 ms: 1.50x slower                                               |
| Geometric mean | (ref)                                                  | 1.29x slower                                                        |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| regex_effbot   | 2.43 ms                                                | 2.64 ms: 1.09x slower                                               |
| regex_v8       | 15.1 ms                                                | 18.3 ms: 1.21x slower                                               |
| regex_dna      | 148 ms                                                 | 180 ms: 1.22x slower                                                |
| regex_compile  | 72.8 ms                                                | 96.5 ms: 1.32x slower                                               |
| Geometric mean | (ref)                                                  | 1.21x slower                                                        |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6 |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| unpickle_list        | 2.69 us                                                | 2.66 us: 1.01x faster                                               |
| xml_etree_iterparse  | 68.3 ms                                                | 69.0 ms: 1.01x slower                                               |
| pickle               | 6.98 us                                                | 7.56 us: 1.08x slower                                               |
| json_dumps           | 7.53 ms                                                | 8.25 ms: 1.09x slower                                               |
| pickle_list          | 2.70 us                                                | 2.96 us: 1.10x slower                                               |
| pickle_dict          | 17.1 us                                                | 18.8 us: 1.10x slower                                               |
| json_loads           | 15.3 us                                                | 17.0 us: 1.11x slower                                               |
| xml_etree_generate   | 45.8 ms                                                | 54.3 ms: 1.19x slower                                               |
| unpickle             | 8.29 us                                                | 9.87 us: 1.19x slower                                               |
| xml_etree_process    | 33.6 ms                                                | 44.9 ms: 1.34x slower                                               |
| unpickle_pure_python | 149 us                                                 | 203 us: 1.37x slower                                                |
| pickle_pure_python   | 191 us                                                 | 284 us: 1.48x slower                                                |
| Geometric mean       | (ref)                                                  | 1.15x slower                                                        |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6 |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| python_startup_no_site | 8.57 ms                                                | 6.95 ms: 1.23x faster                                               |
| python_startup         | 10.8 ms                                                | 9.57 ms: 1.12x faster                                               |
| Geometric mean         | (ref)                                                  | 1.18x faster                                                        |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6 |
|-----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| genshi_text     | 14.4 ms                                                | 18.2 ms: 1.26x slower                                               |
| genshi_xml      | 28.5 ms                                                | 37.3 ms: 1.31x slower                                               |
| mako            | 7.93 ms                                                | 10.7 ms: 1.34x slower                                               |
| django_template | 20.1 ms                                                | 27.3 ms: 1.35x slower                                               |
| Geometric mean  | (ref)                                                  | 1.32x slower                                                        |

All benchmarks:
===============

| Benchmark               | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6 |
|-------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| python_startup_no_site  | 8.57 ms                                                | 6.95 ms: 1.23x faster                                               |
| python_startup          | 10.8 ms                                                | 9.57 ms: 1.12x faster                                               |
| coverage                | 43.9 ms                                                | 40.6 ms: 1.08x faster                                               |
| pathlib                 | 23.2 ms                                                | 22.0 ms: 1.06x faster                                               |
| unpickle_list           | 2.69 us                                                | 2.66 us: 1.01x faster                                               |
| xml_etree_iterparse     | 68.3 ms                                                | 69.0 ms: 1.01x slower                                               |
| pidigits                | 280 ms                                                 | 284 ms: 1.01x slower                                                |
| generators              | 30.3 ms                                                | 32.4 ms: 1.07x slower                                               |
| pickle                  | 6.98 us                                                | 7.56 us: 1.08x slower                                               |
| regex_effbot            | 2.43 ms                                                | 2.64 ms: 1.09x slower                                               |
| meteor_contest          | 71.1 ms                                                | 77.4 ms: 1.09x slower                                               |
| json_dumps              | 7.53 ms                                                | 8.25 ms: 1.09x slower                                               |
| pickle_list             | 2.70 us                                                | 2.96 us: 1.10x slower                                               |
| pickle_dict             | 17.1 us                                                | 18.8 us: 1.10x slower                                               |
| flaskblogging           | 2.35 ms                                                | 2.60 ms: 1.10x slower                                               |
| json_loads              | 15.3 us                                                | 17.0 us: 1.11x slower                                               |
| unpack_sequence         | 33.6 ns                                                | 37.4 ns: 1.11x slower                                               |
| bench_thread_pool       | 465 us                                                 | 518 us: 1.11x slower                                                |
| mdp                     | 1.48 sec                                               | 1.66 sec: 1.12x slower                                              |
| json                    | 2.75 ms                                                | 3.11 ms: 1.13x slower                                               |
| telco                   | 3.17 ms                                                | 3.64 ms: 1.15x slower                                               |
| gunicorn                | 1.10 ms                                                | 1.26 ms: 1.15x slower                                               |
| aiohttp                 | 1.02 ms                                                | 1.19 ms: 1.16x slower                                               |
| coroutines              | 17.2 ms                                                | 20.1 ms: 1.17x slower                                               |
| sympy_str               | 144 ms                                                 | 170 ms: 1.18x slower                                                |
| sqlite_synth            | 1.26 us                                                | 1.49 us: 1.18x slower                                               |
| xml_etree_generate      | 45.8 ms                                                | 54.3 ms: 1.19x slower                                               |
| sympy_integrate         | 11.3 ms                                                | 13.4 ms: 1.19x slower                                               |
| pylint                  | 253 ms                                                 | 300 ms: 1.19x slower                                                |
| sympy_sum               | 80.2 ms                                                | 95.4 ms: 1.19x slower                                               |
| unpickle                | 8.29 us                                                | 9.87 us: 1.19x slower                                               |
| async_generators        | 192 ms                                                 | 231 ms: 1.20x slower                                                |
| sympy_expand            | 229 ms                                                 | 276 ms: 1.21x slower                                                |
| regex_v8                | 15.1 ms                                                | 18.3 ms: 1.21x slower                                               |
| sqlglot_normalize       | 162 ms                                                 | 196 ms: 1.21x slower                                                |
| regex_dna               | 148 ms                                                 | 180 ms: 1.22x slower                                                |
| nqueens                 | 55.9 ms                                                | 68.1 ms: 1.22x slower                                               |
| scimark_sparse_mat_mult | 2.81 ms                                                | 3.46 ms: 1.23x slower                                               |
| docutils                | 1.43 sec                                               | 1.77 sec: 1.24x slower                                              |
| pprint_pformat          | 979 ms                                                 | 1.23 sec: 1.26x slower                                              |
| sqlalchemy_declarative  | 59.3 ms                                                | 74.5 ms: 1.26x slower                                               |
| pprint_safe_repr        | 478 ms                                                 | 603 ms: 1.26x slower                                                |
| genshi_text             | 14.4 ms                                                | 18.2 ms: 1.26x slower                                               |
| async_tree_cpu_io_mixed | 519 ms                                                 | 661 ms: 1.27x slower                                                |
| sqlglot_optimize        | 29.6 ms                                                | 37.9 ms: 1.28x slower                                               |
| dulwich_log             | 28.6 ms                                                | 36.7 ms: 1.28x slower                                               |
| sqlalchemy_imperative   | 6.98 ms                                                | 8.96 ms: 1.28x slower                                               |
| deepcopy                | 215 us                                                 | 280 us: 1.30x slower                                                |
| deepcopy_reduce         | 1.79 us                                                | 2.34 us: 1.30x slower                                               |
| genshi_xml              | 28.5 ms                                                | 37.3 ms: 1.31x slower                                               |
| regex_compile           | 72.8 ms                                                | 96.5 ms: 1.32x slower                                               |
| fannkuch                | 240 ms                                                 | 318 ms: 1.33x slower                                                |
| scimark_fft             | 173 ms                                                 | 230 ms: 1.33x slower                                                |
| xml_etree_process       | 33.6 ms                                                | 44.9 ms: 1.34x slower                                               |
| deepcopy_memo           | 25.7 us                                                | 34.5 us: 1.34x slower                                               |
| mako                    | 7.93 ms                                                | 10.7 ms: 1.34x slower                                               |
| tornado_http            | 69.1 ms                                                | 93.5 ms: 1.35x slower                                               |
| django_template         | 20.1 ms                                                | 27.3 ms: 1.35x slower                                               |
| chameleon               | 4.30 ms                                                | 5.83 ms: 1.36x slower                                               |
| logging_format          | 3.67 us                                                | 4.99 us: 1.36x slower                                               |
| logging_simple          | 3.41 us                                                | 4.63 us: 1.36x slower                                               |
| unpickle_pure_python    | 149 us                                                 | 203 us: 1.37x slower                                                |
| hexiom                  | 4.58 ms                                                | 6.30 ms: 1.38x slower                                               |
| pycparser               | 659 ms                                                 | 912 ms: 1.38x slower                                                |
| async_tree_none         | 282 ms                                                 | 394 ms: 1.40x slower                                                |
| chaos                   | 47.4 ms                                                | 66.6 ms: 1.41x slower                                               |
| html5lib                | 33.0 ms                                                | 46.5 ms: 1.41x slower                                               |
| thrift                  | 410 us                                                 | 582 us: 1.42x slower                                                |
| float                   | 50.8 ms                                                | 72.1 ms: 1.42x slower                                               |
| async_tree_memoization  | 336 ms                                                 | 481 ms: 1.43x slower                                                |
| async_tree_io           | 697 ms                                                 | 1.00 sec: 1.44x slower                                              |
| 2to3                    | 154 ms                                                 | 223 ms: 1.44x slower                                                |
| spectral_norm           | 65.7 ms                                                | 96.2 ms: 1.46x slower                                               |
| sqlglot_transpile       | 1.05 ms                                                | 1.55 ms: 1.47x slower                                               |
| pickle_pure_python      | 191 us                                                 | 284 us: 1.48x slower                                                |
| sqlglot_parse           | 890 us                                                 | 1.33 ms: 1.50x slower                                               |
| nbody                   | 61.7 ms                                                | 92.6 ms: 1.50x slower                                               |
| go                      | 105 ms                                                 | 165 ms: 1.57x slower                                                |
| raytrace                | 206 ms                                                 | 327 ms: 1.59x slower                                                |
| scimark_sor             | 79.2 ms                                                | 126 ms: 1.59x slower                                                |
| pyflate                 | 284 ms                                                 | 453 ms: 1.60x slower                                                |
| scimark_lu              | 67.7 ms                                                | 110 ms: 1.62x slower                                                |
| crypto_pyaes            | 47.5 ms                                                | 77.9 ms: 1.64x slower                                               |
| richards                | 31.1 ms                                                | 51.0 ms: 1.64x slower                                               |
| scimark_monte_carlo     | 43.5 ms                                                | 72.0 ms: 1.65x slower                                               |
| logging_silent          | 66.5 ns                                                | 118 ns: 1.78x slower                                                |
| deltablue               | 2.75 ms                                                | 5.15 ms: 1.87x slower                                               |
| Geometric mean          | (ref)                                                  | 1.26x slower                                                        |

Benchmark hidden because not significant (2): bench_mp_pool, xml_etree_parse
Ignored benchmarks (15) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, comprehensions, create_gc_cycles, dask, gc_traversal, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (1) of results/bm-20221206-3.10.9-1dd9be6/bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6.json: mypy


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.25x
- 95% likely to have a slowdown of 1.24x
- 99% likely to have a slowdown of 1.22x


# Memory

- memory change: 0.91x