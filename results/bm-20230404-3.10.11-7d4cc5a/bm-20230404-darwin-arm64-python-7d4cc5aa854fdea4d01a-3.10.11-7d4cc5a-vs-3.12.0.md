
# Results vs. 3.12.0

- fork: python
- ref: 7d4cc5aa854fdea4d01a
- machine: darwin-arm64
- commit hash: 7d4cc5a
- commit date: 2023-04-04
- overall geometric mean: 1.21x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.16x slower
- Memory change: 0.90x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-darwin-arm64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 203 ms: 1.20x slower                                                 |
| chameleon      | 4.70 ms                                                | 5.75 ms: 1.23x slower                                                |
| docutils       | 1.50 sec                                               | 1.79 sec: 1.19x slower                                               |
| tornado_http   | 69.3 ms                                                | 91.2 ms: 1.32x slower                                                |
| Geometric mean | (ref)                                                  | 1.23x slower                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-darwin-arm64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 526 ms                                                 | 668 ms: 1.27x slower                                                 |
| async_tree_none         | 266 ms                                                 | 399 ms: 1.50x slower                                                 |
| async_tree_io           | 668 ms                                                 | 1.02 sec: 1.52x slower                                               |
| async_tree_memoization  | 312 ms                                                 | 490 ms: 1.57x slower                                                 |
| Geometric mean          | (ref)                                                  | 1.46x slower                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-darwin-arm64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| float          | 55.8 ms                                                | 72.2 ms: 1.29x slower                                                |
| nbody          | 68.8 ms                                                | 94.0 ms: 1.37x slower                                                |
| Geometric mean | (ref)                                                  | 1.21x slower                                                         |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-darwin-arm64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_effbot   | 2.64 ms                                                | 2.69 ms: 1.02x slower                                                |
| regex_v8       | 16.0 ms                                                | 18.0 ms: 1.13x slower                                                |
| regex_dna      | 154 ms                                                 | 185 ms: 1.20x slower                                                 |
| regex_compile  | 77.9 ms                                                | 96.9 ms: 1.24x slower                                                |
| Geometric mean | (ref)                                                  | 1.14x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-darwin-arm64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| unpickle_list        | 3.02 us                                                | 2.69 us: 1.12x faster                                                |
| xml_etree_generate   | 55.8 ms                                                | 54.3 ms: 1.03x faster                                                |
| json_loads           | 17.2 us                                                | 16.8 us: 1.02x faster                                                |
| xml_etree_iterparse  | 74.0 ms                                                | 73.2 ms: 1.01x faster                                                |
| pickle_dict          | 18.1 us                                                | 18.8 us: 1.04x slower                                                |
| pickle               | 7.23 us                                                | 7.56 us: 1.05x slower                                                |
| unpickle             | 9.12 us                                                | 9.89 us: 1.08x slower                                                |
| xml_etree_process    | 39.7 ms                                                | 44.9 ms: 1.13x slower                                                |
| json_dumps           | 6.22 ms                                                | 8.27 ms: 1.33x slower                                                |
| unpickle_pure_python | 151 us                                                 | 204 us: 1.35x slower                                                 |
| pickle_pure_python   | 200 us                                                 | 285 us: 1.43x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.09x slower                                                         |

Benchmark hidden because not significant (2): pickle_list, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-darwin-arm64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup_no_site | 9.37 ms                                                | 9.13 ms: 1.03x faster                                                |
| python_startup         | 11.4 ms                                                | 12.1 ms: 1.06x slower                                                |
| Geometric mean         | (ref)                                                  | 1.02x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-darwin-arm64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| django_template | 22.3 ms                                                | 27.1 ms: 1.21x slower                                                |
| mako            | 7.71 ms                                                | 10.6 ms: 1.37x slower                                                |
| Geometric mean  | (ref)                                                  | 1.29x slower                                                         |

All benchmarks:
===============

| Benchmark               | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-darwin-arm64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_generators        | 304 ms                                                 | 233 ms: 1.30x faster                                                 |
| unpickle_list           | 3.02 us                                                | 2.69 us: 1.12x faster                                                |
| bench_mp_pool           | 44.9 ms                                                | 40.2 ms: 1.12x faster                                                |
| sqlite_synth            | 1.57 us                                                | 1.48 us: 1.06x faster                                                |
| xml_etree_generate      | 55.8 ms                                                | 54.3 ms: 1.03x faster                                                |
| python_startup_no_site  | 9.37 ms                                                | 9.13 ms: 1.03x faster                                                |
| json_loads              | 17.2 us                                                | 16.8 us: 1.02x faster                                                |
| telco                   | 3.68 ms                                                | 3.63 ms: 1.01x faster                                                |
| xml_etree_iterparse     | 74.0 ms                                                | 73.2 ms: 1.01x faster                                                |
| json                    | 3.09 ms                                                | 3.06 ms: 1.01x faster                                                |
| gc_traversal            | 2.40 ms                                                | 2.39 ms: 1.00x faster                                                |
| regex_effbot            | 2.64 ms                                                | 2.69 ms: 1.02x slower                                                |
| pickle_dict             | 18.1 us                                                | 18.8 us: 1.04x slower                                                |
| pickle                  | 7.23 us                                                | 7.56 us: 1.05x slower                                                |
| coroutines              | 19.2 ms                                                | 20.1 ms: 1.05x slower                                                |
| generators              | 31.1 ms                                                | 32.7 ms: 1.05x slower                                                |
| mdp                     | 1.58 sec                                               | 1.67 sec: 1.05x slower                                               |
| sqlglot_normalize       | 186 ms                                                 | 196 ms: 1.05x slower                                                 |
| bench_thread_pool       | 504 us                                                 | 532 us: 1.06x slower                                                 |
| python_startup          | 11.4 ms                                                | 12.1 ms: 1.06x slower                                                |
| coverage                | 38.9 ms                                                | 41.9 ms: 1.08x slower                                                |
| unpickle                | 9.12 us                                                | 9.89 us: 1.08x slower                                                |
| meteor_contest          | 71.7 ms                                                | 78.0 ms: 1.09x slower                                                |
| nqueens                 | 62.4 ms                                                | 68.0 ms: 1.09x slower                                                |
| scimark_sparse_mat_mult | 3.14 ms                                                | 3.46 ms: 1.10x slower                                                |
| sqlglot_optimize        | 34.0 ms                                                | 38.0 ms: 1.12x slower                                                |
| regex_v8                | 16.0 ms                                                | 18.0 ms: 1.13x slower                                                |
| xml_etree_process       | 39.7 ms                                                | 44.9 ms: 1.13x slower                                                |
| sympy_expand            | 241 ms                                                 | 277 ms: 1.15x slower                                                 |
| deepcopy_reduce         | 2.07 us                                                | 2.38 us: 1.15x slower                                                |
| sympy_str               | 148 ms                                                 | 170 ms: 1.16x slower                                                 |
| dask                    | 222 ms                                                 | 257 ms: 1.16x slower                                                 |
| pathlib                 | 24.2 ms                                                | 28.3 ms: 1.17x slower                                                |
| aiohttp                 | 1.08 ms                                                | 1.26 ms: 1.17x slower                                                |
| gunicorn                | 1.15 ms                                                | 1.34 ms: 1.17x slower                                                |
| sympy_integrate         | 11.4 ms                                                | 13.4 ms: 1.18x slower                                                |
| scimark_fft             | 195 ms                                                 | 231 ms: 1.18x slower                                                 |
| deepcopy                | 235 us                                                 | 279 us: 1.19x slower                                                 |
| docutils                | 1.50 sec                                               | 1.79 sec: 1.19x slower                                               |
| regex_dna               | 154 ms                                                 | 185 ms: 1.20x slower                                                 |
| 2to3                    | 169 ms                                                 | 203 ms: 1.20x slower                                                 |
| sqlalchemy_declarative  | 62.3 ms                                                | 75.0 ms: 1.20x slower                                                |
| pprint_safe_repr        | 497 ms                                                 | 602 ms: 1.21x slower                                                 |
| django_template         | 22.3 ms                                                | 27.1 ms: 1.21x slower                                                |
| unpack_sequence         | 31.5 ns                                                | 38.3 ns: 1.22x slower                                                |
| pprint_pformat          | 1.01 sec                                               | 1.23 sec: 1.22x slower                                               |
| chameleon               | 4.70 ms                                                | 5.75 ms: 1.23x slower                                                |
| comprehensions          | 14.5 us                                                | 17.9 us: 1.23x slower                                                |
| dulwich_log             | 29.8 ms                                                | 36.9 ms: 1.24x slower                                                |
| sympy_sum               | 77.6 ms                                                | 96.4 ms: 1.24x slower                                                |
| regex_compile           | 77.9 ms                                                | 96.9 ms: 1.24x slower                                                |
| deepcopy_memo           | 27.7 us                                                | 34.5 us: 1.25x slower                                                |
| create_gc_cycles        | 701 us                                                 | 874 us: 1.25x slower                                                 |
| spectral_norm           | 76.4 ms                                                | 96.4 ms: 1.26x slower                                                |
| logging_simple          | 3.69 us                                                | 4.65 us: 1.26x slower                                                |
| logging_format          | 3.98 us                                                | 5.05 us: 1.27x slower                                                |
| async_tree_cpu_io_mixed | 526 ms                                                 | 668 ms: 1.27x slower                                                 |
| fannkuch                | 248 ms                                                 | 319 ms: 1.28x slower                                                 |
| float                   | 55.8 ms                                                | 72.2 ms: 1.29x slower                                                |
| tornado_http            | 69.3 ms                                                | 91.2 ms: 1.32x slower                                                |
| json_dumps              | 6.22 ms                                                | 8.27 ms: 1.33x slower                                                |
| pycparser               | 677 ms                                                 | 910 ms: 1.34x slower                                                 |
| sqlalchemy_imperative   | 6.68 ms                                                | 9.01 ms: 1.35x slower                                                |
| unpickle_pure_python    | 151 us                                                 | 204 us: 1.35x slower                                                 |
| nbody                   | 68.8 ms                                                | 94.0 ms: 1.37x slower                                                |
| mako                    | 7.71 ms                                                | 10.6 ms: 1.37x slower                                                |
| hexiom                  | 4.54 ms                                                | 6.33 ms: 1.39x slower                                                |
| pickle_pure_python      | 200 us                                                 | 285 us: 1.43x slower                                                 |
| pyflate                 | 316 ms                                                 | 455 ms: 1.44x slower                                                 |
| scimark_sor             | 87.4 ms                                                | 126 ms: 1.44x slower                                                 |
| scimark_lu              | 76.0 ms                                                | 110 ms: 1.45x slower                                                 |
| asyncio_tcp             | 449 ms                                                 | 669 ms: 1.49x slower                                                 |
| sqlglot_transpile       | 1.02 ms                                                | 1.53 ms: 1.50x slower                                                |
| async_tree_none         | 266 ms                                                 | 399 ms: 1.50x slower                                                 |
| crypto_pyaes            | 51.9 ms                                                | 78.3 ms: 1.51x slower                                                |
| async_tree_io           | 668 ms                                                 | 1.02 sec: 1.52x slower                                               |
| raytrace                | 212 ms                                                 | 331 ms: 1.56x slower                                                 |
| logging_silent          | 76.4 ns                                                | 120 ns: 1.56x slower                                                 |
| sqlglot_parse           | 848 us                                                 | 1.33 ms: 1.57x slower                                                |
| async_tree_memoization  | 312 ms                                                 | 490 ms: 1.57x slower                                                 |
| richards                | 32.1 ms                                                | 50.7 ms: 1.58x slower                                                |
| chaos                   | 42.5 ms                                                | 68.0 ms: 1.60x slower                                                |
| scimark_monte_carlo     | 45.0 ms                                                | 72.3 ms: 1.61x slower                                                |
| go                      | 102 ms                                                 | 165 ms: 1.62x slower                                                 |
| deltablue               | 2.71 ms                                                | 5.17 ms: 1.91x slower                                                |
| Geometric mean          | (ref)                                                  | 1.21x slower                                                         |

Benchmark hidden because not significant (3): pidigits, pickle_list, xml_etree_parse
Ignored benchmarks (10) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (6) of results/bm-20230404-3.10.11-7d4cc5a/bm-20230404-darwin-arm64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.19x
- 95% likely to have a slowdown of 1.18x
- 99% likely to have a slowdown of 1.16x


# Memory

- memory change: 0.90x