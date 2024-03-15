
# Results vs. 3.12.0

- fork: python
- ref: 1dd9be6584413fbfa823
- machine: darwin-arm64
- commit hash: 1dd9be6
- commit date: 2022-12-06
- overall geometric mean: 1.19x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.14x slower
- Memory change: 0.87x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 223 ms: 1.31x slower                                                |
| chameleon      | 4.70 ms                                                | 5.83 ms: 1.24x slower                                               |
| docutils       | 1.50 sec                                               | 1.77 sec: 1.18x slower                                              |
| tornado_http   | 69.3 ms                                                | 93.5 ms: 1.35x slower                                               |
| Geometric mean | (ref)                                                  | 1.27x slower                                                        |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6 |
|-------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 526 ms                                                 | 661 ms: 1.26x slower                                                |
| async_tree_none         | 266 ms                                                 | 394 ms: 1.48x slower                                                |
| async_tree_io           | 668 ms                                                 | 1.00 sec: 1.50x slower                                              |
| async_tree_memoization  | 312 ms                                                 | 481 ms: 1.54x slower                                                |
| Geometric mean          | (ref)                                                  | 1.44x slower                                                        |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| pidigits       | 282 ms                                                 | 284 ms: 1.01x slower                                                |
| float          | 55.8 ms                                                | 72.1 ms: 1.29x slower                                               |
| nbody          | 68.8 ms                                                | 92.6 ms: 1.34x slower                                               |
| Geometric mean | (ref)                                                  | 1.20x slower                                                        |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| regex_effbot   | 2.64 ms                                                | 2.64 ms: 1.00x faster                                               |
| regex_v8       | 16.0 ms                                                | 18.3 ms: 1.15x slower                                               |
| regex_dna      | 154 ms                                                 | 180 ms: 1.17x slower                                                |
| regex_compile  | 77.9 ms                                                | 96.5 ms: 1.24x slower                                               |
| Geometric mean | (ref)                                                  | 1.13x slower                                                        |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6 |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| unpickle_list        | 3.02 us                                                | 2.66 us: 1.13x faster                                               |
| xml_etree_iterparse  | 74.0 ms                                                | 69.0 ms: 1.07x faster                                               |
| xml_etree_parse      | 106 ms                                                 | 100 ms: 1.06x faster                                                |
| xml_etree_generate   | 55.8 ms                                                | 54.3 ms: 1.03x faster                                               |
| json_loads           | 17.2 us                                                | 17.0 us: 1.01x faster                                               |
| pickle_list          | 2.89 us                                                | 2.96 us: 1.02x slower                                               |
| pickle_dict          | 18.1 us                                                | 18.8 us: 1.04x slower                                               |
| pickle               | 7.23 us                                                | 7.56 us: 1.05x slower                                               |
| unpickle             | 9.12 us                                                | 9.87 us: 1.08x slower                                               |
| xml_etree_process    | 39.7 ms                                                | 44.9 ms: 1.13x slower                                               |
| json_dumps           | 6.22 ms                                                | 8.25 ms: 1.33x slower                                               |
| unpickle_pure_python | 151 us                                                 | 203 us: 1.35x slower                                                |
| pickle_pure_python   | 200 us                                                 | 284 us: 1.42x slower                                                |
| Geometric mean       | (ref)                                                  | 1.08x slower                                                        |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6 |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| python_startup_no_site | 9.37 ms                                                | 6.95 ms: 1.35x faster                                               |
| python_startup         | 11.4 ms                                                | 9.57 ms: 1.19x faster                                               |
| Geometric mean         | (ref)                                                  | 1.27x faster                                                        |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6 |
|-----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| django_template | 22.3 ms                                                | 27.3 ms: 1.22x slower                                               |
| mako            | 7.71 ms                                                | 10.7 ms: 1.38x slower                                               |
| Geometric mean  | (ref)                                                  | 1.30x slower                                                        |

All benchmarks:
===============

| Benchmark               | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6 |
|-------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| python_startup_no_site  | 9.37 ms                                                | 6.95 ms: 1.35x faster                                               |
| async_generators        | 304 ms                                                 | 231 ms: 1.32x faster                                                |
| python_startup          | 11.4 ms                                                | 9.57 ms: 1.19x faster                                               |
| unpickle_list           | 3.02 us                                                | 2.66 us: 1.13x faster                                               |
| pathlib                 | 24.2 ms                                                | 22.0 ms: 1.10x faster                                               |
| bench_mp_pool           | 44.9 ms                                                | 40.8 ms: 1.10x faster                                               |
| xml_etree_iterparse     | 74.0 ms                                                | 69.0 ms: 1.07x faster                                               |
| xml_etree_parse         | 106 ms                                                 | 100 ms: 1.06x faster                                                |
| sqlite_synth            | 1.57 us                                                | 1.49 us: 1.06x faster                                               |
| xml_etree_generate      | 55.8 ms                                                | 54.3 ms: 1.03x faster                                               |
| json_loads              | 17.2 us                                                | 17.0 us: 1.01x faster                                               |
| telco                   | 3.68 ms                                                | 3.64 ms: 1.01x faster                                               |
| regex_effbot            | 2.64 ms                                                | 2.64 ms: 1.00x faster                                               |
| pidigits                | 282 ms                                                 | 284 ms: 1.01x slower                                                |
| json                    | 3.09 ms                                                | 3.11 ms: 1.01x slower                                               |
| pickle_list             | 2.89 us                                                | 2.96 us: 1.02x slower                                               |
| bench_thread_pool       | 504 us                                                 | 518 us: 1.03x slower                                                |
| pickle_dict             | 18.1 us                                                | 18.8 us: 1.04x slower                                               |
| generators              | 31.1 ms                                                | 32.4 ms: 1.04x slower                                               |
| coverage                | 38.9 ms                                                | 40.6 ms: 1.05x slower                                               |
| pickle                  | 7.23 us                                                | 7.56 us: 1.05x slower                                               |
| coroutines              | 19.2 ms                                                | 20.1 ms: 1.05x slower                                               |
| mdp                     | 1.58 sec                                               | 1.66 sec: 1.05x slower                                              |
| sqlglot_normalize       | 186 ms                                                 | 196 ms: 1.05x slower                                                |
| meteor_contest          | 71.7 ms                                                | 77.4 ms: 1.08x slower                                               |
| unpickle                | 9.12 us                                                | 9.87 us: 1.08x slower                                               |
| nqueens                 | 62.4 ms                                                | 68.1 ms: 1.09x slower                                               |
| gunicorn                | 1.15 ms                                                | 1.26 ms: 1.10x slower                                               |
| aiohttp                 | 1.08 ms                                                | 1.19 ms: 1.10x slower                                               |
| scimark_sparse_mat_mult | 3.14 ms                                                | 3.46 ms: 1.11x slower                                               |
| sqlglot_optimize        | 34.0 ms                                                | 37.9 ms: 1.11x slower                                               |
| deepcopy_reduce         | 2.07 us                                                | 2.34 us: 1.13x slower                                               |
| xml_etree_process       | 39.7 ms                                                | 44.9 ms: 1.13x slower                                               |
| sympy_expand            | 241 ms                                                 | 276 ms: 1.15x slower                                                |
| regex_v8                | 16.0 ms                                                | 18.3 ms: 1.15x slower                                               |
| sympy_str               | 148 ms                                                 | 170 ms: 1.15x slower                                                |
| regex_dna               | 154 ms                                                 | 180 ms: 1.17x slower                                                |
| scimark_fft             | 195 ms                                                 | 230 ms: 1.18x slower                                                |
| sympy_integrate         | 11.4 ms                                                | 13.4 ms: 1.18x slower                                               |
| docutils                | 1.50 sec                                               | 1.77 sec: 1.18x slower                                              |
| unpack_sequence         | 31.5 ns                                                | 37.4 ns: 1.19x slower                                               |
| deepcopy                | 235 us                                                 | 280 us: 1.19x slower                                                |
| sqlalchemy_declarative  | 62.3 ms                                                | 74.5 ms: 1.20x slower                                               |
| pprint_safe_repr        | 497 ms                                                 | 603 ms: 1.21x slower                                                |
| pprint_pformat          | 1.01 sec                                               | 1.23 sec: 1.22x slower                                              |
| django_template         | 22.3 ms                                                | 27.3 ms: 1.22x slower                                               |
| sympy_sum               | 77.6 ms                                                | 95.4 ms: 1.23x slower                                               |
| dulwich_log             | 29.8 ms                                                | 36.7 ms: 1.23x slower                                               |
| regex_compile           | 77.9 ms                                                | 96.5 ms: 1.24x slower                                               |
| chameleon               | 4.70 ms                                                | 5.83 ms: 1.24x slower                                               |
| deepcopy_memo           | 27.7 us                                                | 34.5 us: 1.25x slower                                               |
| logging_format          | 3.98 us                                                | 4.99 us: 1.25x slower                                               |
| logging_simple          | 3.69 us                                                | 4.63 us: 1.26x slower                                               |
| async_tree_cpu_io_mixed | 526 ms                                                 | 661 ms: 1.26x slower                                                |
| spectral_norm           | 76.4 ms                                                | 96.2 ms: 1.26x slower                                               |
| fannkuch                | 248 ms                                                 | 318 ms: 1.28x slower                                                |
| float                   | 55.8 ms                                                | 72.1 ms: 1.29x slower                                               |
| 2to3                    | 169 ms                                                 | 223 ms: 1.31x slower                                                |
| json_dumps              | 6.22 ms                                                | 8.25 ms: 1.33x slower                                               |
| sqlalchemy_imperative   | 6.68 ms                                                | 8.96 ms: 1.34x slower                                               |
| nbody                   | 68.8 ms                                                | 92.6 ms: 1.34x slower                                               |
| unpickle_pure_python    | 151 us                                                 | 203 us: 1.35x slower                                                |
| pycparser               | 677 ms                                                 | 912 ms: 1.35x slower                                                |
| tornado_http            | 69.3 ms                                                | 93.5 ms: 1.35x slower                                               |
| mako                    | 7.71 ms                                                | 10.7 ms: 1.38x slower                                               |
| hexiom                  | 4.54 ms                                                | 6.30 ms: 1.39x slower                                               |
| pickle_pure_python      | 200 us                                                 | 284 us: 1.42x slower                                                |
| pyflate                 | 316 ms                                                 | 453 ms: 1.44x slower                                                |
| scimark_lu              | 76.0 ms                                                | 110 ms: 1.44x slower                                                |
| scimark_sor             | 87.4 ms                                                | 126 ms: 1.44x slower                                                |
| async_tree_none         | 266 ms                                                 | 394 ms: 1.48x slower                                                |
| async_tree_io           | 668 ms                                                 | 1.00 sec: 1.50x slower                                              |
| crypto_pyaes            | 51.9 ms                                                | 77.9 ms: 1.50x slower                                               |
| sqlglot_transpile       | 1.02 ms                                                | 1.55 ms: 1.52x slower                                               |
| async_tree_memoization  | 312 ms                                                 | 481 ms: 1.54x slower                                                |
| raytrace                | 212 ms                                                 | 327 ms: 1.54x slower                                                |
| logging_silent          | 76.4 ns                                                | 118 ns: 1.55x slower                                                |
| chaos                   | 42.5 ms                                                | 66.6 ms: 1.57x slower                                               |
| sqlglot_parse           | 848 us                                                 | 1.33 ms: 1.57x slower                                               |
| richards                | 32.1 ms                                                | 51.0 ms: 1.59x slower                                               |
| scimark_monte_carlo     | 45.0 ms                                                | 72.0 ms: 1.60x slower                                               |
| go                      | 102 ms                                                 | 165 ms: 1.63x slower                                                |
| deltablue               | 2.71 ms                                                | 5.15 ms: 1.90x slower                                               |
| Geometric mean          | (ref)                                                  | 1.19x slower                                                        |
Ignored benchmarks (15) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, comprehensions, create_gc_cycles, dask, gc_traversal, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (7) of results/bm-20221206-3.10.9-1dd9be6/bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6.json: flaskblogging, genshi_text, genshi_xml, html5lib, mypy, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.17x
- 95% likely to have a slowdown of 1.17x
- 99% likely to have a slowdown of 1.14x


# Memory

- memory change: 0.87x