
# Results vs. 3.10.4

- fork: python
- ref: 7d4cc5aa854fdea4d01a
- machine: darwin-arm64
- commit hash: 7d4cc5a
- commit date: 2023-04-04
- overall geometric mean: 1.04x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-darwin-arm64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 203 ms: 1.06x slower                                                 |
| chameleon      | 6.26 ms                                                | 5.75 ms: 1.09x faster                                                |
| docutils       | 1.73 sec                                               | 1.79 sec: 1.03x slower                                               |
| html5lib       | 42.4 ms                                                | 47.8 ms: 1.13x slower                                                |
| tornado_http   | 86.7 ms                                                | 91.2 ms: 1.05x slower                                                |
| Geometric mean | (ref)                                                  | 1.04x slower                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-darwin-arm64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 399 ms: 1.03x slower                                                 |
| async_tree_cpu_io_mixed | 649 ms                                                 | 668 ms: 1.03x slower                                                 |
| async_tree_memoization  | 474 ms                                                 | 490 ms: 1.03x slower                                                 |
| async_tree_io           | 980 ms                                                 | 1.02 sec: 1.04x slower                                               |
| Geometric mean          | (ref)                                                  | 1.03x slower                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-darwin-arm64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| pidigits       | 282 ms                                                 | 282 ms: 1.00x faster                                                 |
| nbody          | 93.0 ms                                                | 94.0 ms: 1.01x slower                                                |
| float          | 69.0 ms                                                | 72.2 ms: 1.05x slower                                                |
| Geometric mean | (ref)                                                  | 1.02x slower                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-darwin-arm64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 96.9 ms: 1.02x slower                                                |
| regex_v8       | 17.1 ms                                                | 18.0 ms: 1.05x slower                                                |
| regex_dna      | 174 ms                                                 | 185 ms: 1.06x slower                                                 |
| regex_effbot   | 2.46 ms                                                | 2.69 ms: 1.10x slower                                                |
| Geometric mean | (ref)                                                  | 1.05x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-darwin-arm64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| xml_etree_process    | 46.5 ms                                                | 44.9 ms: 1.04x faster                                                |
| xml_etree_iterparse  | 72.1 ms                                                | 73.2 ms: 1.02x slower                                                |
| xml_etree_generate   | 53.5 ms                                                | 54.3 ms: 1.02x slower                                                |
| pickle_pure_python   | 281 us                                                 | 285 us: 1.02x slower                                                 |
| json_dumps           | 8.11 ms                                                | 8.27 ms: 1.02x slower                                                |
| json_loads           | 16.4 us                                                | 16.8 us: 1.02x slower                                                |
| unpickle_pure_python | 194 us                                                 | 204 us: 1.05x slower                                                 |
| pickle_list          | 2.74 us                                                | 2.90 us: 1.06x slower                                                |
| pickle               | 6.97 us                                                | 7.56 us: 1.08x slower                                                |
| pickle_dict          | 17.0 us                                                | 18.8 us: 1.11x slower                                                |
| unpickle             | 8.80 us                                                | 9.89 us: 1.12x slower                                                |
| Geometric mean       | (ref)                                                  | 1.04x slower                                                         |

Benchmark hidden because not significant (2): unpickle_list, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-darwin-arm64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 12.1 ms: 1.12x slower                                                |
| python_startup_no_site | 7.91 ms                                                | 9.13 ms: 1.15x slower                                                |
| Geometric mean         | (ref)                                                  | 1.14x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-darwin-arm64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| django_template | 26.4 ms                                                | 27.1 ms: 1.03x slower                                                |
| genshi_text     | 17.3 ms                                                | 18.2 ms: 1.05x slower                                                |
| mako            | 9.87 ms                                                | 10.6 ms: 1.07x slower                                                |
| genshi_xml      | 33.8 ms                                                | 37.3 ms: 1.10x slower                                                |
| Geometric mean  | (ref)                                                  | 1.06x slower                                                         |

All benchmarks:
===============

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-darwin-arm64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| chameleon               | 6.26 ms                                                | 5.75 ms: 1.09x faster                                                |
| pprint_safe_repr        | 641 ms                                                 | 602 ms: 1.06x faster                                                 |
| pprint_pformat          | 1.30 sec                                               | 1.23 sec: 1.06x faster                                               |
| xml_etree_process       | 46.5 ms                                                | 44.9 ms: 1.04x faster                                                |
| coroutines              | 20.7 ms                                                | 20.1 ms: 1.03x faster                                                |
| unpack_sequence         | 39.0 ns                                                | 38.3 ns: 1.02x faster                                                |
| scimark_sor             | 128 ms                                                 | 126 ms: 1.02x faster                                                 |
| json                    | 3.08 ms                                                | 3.06 ms: 1.01x faster                                                |
| deepcopy_memo           | 34.7 us                                                | 34.5 us: 1.01x faster                                                |
| pidigits                | 282 ms                                                 | 282 ms: 1.00x faster                                                 |
| meteor_contest          | 77.7 ms                                                | 78.0 ms: 1.00x slower                                                |
| async_generators        | 231 ms                                                 | 233 ms: 1.01x slower                                                 |
| coverage                | 41.5 ms                                                | 41.9 ms: 1.01x slower                                                |
| bench_thread_pool       | 527 us                                                 | 532 us: 1.01x slower                                                 |
| scimark_sparse_mat_mult | 3.42 ms                                                | 3.46 ms: 1.01x slower                                                |
| generators              | 32.3 ms                                                | 32.7 ms: 1.01x slower                                                |
| nbody                   | 93.0 ms                                                | 94.0 ms: 1.01x slower                                                |
| sqlite_synth            | 1.46 us                                                | 1.48 us: 1.01x slower                                                |
| gc_traversal            | 2.36 ms                                                | 2.39 ms: 1.01x slower                                                |
| thrift                  | 572 us                                                 | 580 us: 1.01x slower                                                 |
| asyncio_tcp             | 659 ms                                                 | 669 ms: 1.01x slower                                                 |
| xml_etree_iterparse     | 72.1 ms                                                | 73.2 ms: 1.02x slower                                                |
| xml_etree_generate      | 53.5 ms                                                | 54.3 ms: 1.02x slower                                                |
| pickle_pure_python      | 281 us                                                 | 285 us: 1.02x slower                                                 |
| spectral_norm           | 94.8 ms                                                | 96.4 ms: 1.02x slower                                                |
| dask                    | 253 ms                                                 | 257 ms: 1.02x slower                                                 |
| create_gc_cycles        | 860 us                                                 | 874 us: 1.02x slower                                                 |
| sqlalchemy_imperative   | 8.86 ms                                                | 9.01 ms: 1.02x slower                                                |
| regex_compile           | 95.3 ms                                                | 96.9 ms: 1.02x slower                                                |
| sympy_integrate         | 13.1 ms                                                | 13.4 ms: 1.02x slower                                                |
| logging_silent          | 117 ns                                                 | 120 ns: 1.02x slower                                                 |
| json_dumps              | 8.11 ms                                                | 8.27 ms: 1.02x slower                                                |
| deepcopy_reduce         | 2.33 us                                                | 2.38 us: 1.02x slower                                                |
| mdp                     | 1.63 sec                                               | 1.67 sec: 1.02x slower                                               |
| hexiom                  | 6.19 ms                                                | 6.33 ms: 1.02x slower                                                |
| sqlalchemy_declarative  | 73.3 ms                                                | 75.0 ms: 1.02x slower                                                |
| json_loads              | 16.4 us                                                | 16.8 us: 1.02x slower                                                |
| deepcopy                | 272 us                                                 | 279 us: 1.03x slower                                                 |
| async_tree_none         | 388 ms                                                 | 399 ms: 1.03x slower                                                 |
| django_template         | 26.4 ms                                                | 27.1 ms: 1.03x slower                                                |
| async_tree_cpu_io_mixed | 649 ms                                                 | 668 ms: 1.03x slower                                                 |
| sqlglot_normalize       | 190 ms                                                 | 196 ms: 1.03x slower                                                 |
| sympy_expand            | 269 ms                                                 | 277 ms: 1.03x slower                                                 |
| scimark_fft             | 224 ms                                                 | 231 ms: 1.03x slower                                                 |
| aiohttp                 | 1.22 ms                                                | 1.26 ms: 1.03x slower                                                |
| sympy_str               | 165 ms                                                 | 170 ms: 1.03x slower                                                 |
| gunicorn                | 1.30 ms                                                | 1.34 ms: 1.03x slower                                                |
| sqlglot_optimize        | 36.8 ms                                                | 38.0 ms: 1.03x slower                                                |
| docutils                | 1.73 sec                                               | 1.79 sec: 1.03x slower                                               |
| chaos                   | 65.8 ms                                                | 68.0 ms: 1.03x slower                                                |
| async_tree_memoization  | 474 ms                                                 | 490 ms: 1.03x slower                                                 |
| pycparser               | 877 ms                                                 | 910 ms: 1.04x slower                                                 |
| async_tree_io           | 980 ms                                                 | 1.02 sec: 1.04x slower                                               |
| telco                   | 3.49 ms                                                | 3.63 ms: 1.04x slower                                                |
| richards                | 48.7 ms                                                | 50.7 ms: 1.04x slower                                                |
| flaskblogging           | 2.65 ms                                                | 2.76 ms: 1.04x slower                                                |
| dulwich_log             | 35.3 ms                                                | 36.9 ms: 1.04x slower                                                |
| sympy_sum               | 92.2 ms                                                | 96.4 ms: 1.05x slower                                                |
| logging_simple          | 4.45 us                                                | 4.65 us: 1.05x slower                                                |
| float                   | 69.0 ms                                                | 72.2 ms: 1.05x slower                                                |
| logging_format          | 4.83 us                                                | 5.05 us: 1.05x slower                                                |
| unpickle_pure_python    | 194 us                                                 | 204 us: 1.05x slower                                                 |
| regex_v8                | 17.1 ms                                                | 18.0 ms: 1.05x slower                                                |
| tornado_http            | 86.7 ms                                                | 91.2 ms: 1.05x slower                                                |
| genshi_text             | 17.3 ms                                                | 18.2 ms: 1.05x slower                                                |
| fannkuch                | 303 ms                                                 | 319 ms: 1.05x slower                                                 |
| deltablue               | 4.91 ms                                                | 5.17 ms: 1.05x slower                                                |
| comprehensions          | 16.9 us                                                | 17.9 us: 1.06x slower                                                |
| pickle_list             | 2.74 us                                                | 2.90 us: 1.06x slower                                                |
| regex_dna               | 174 ms                                                 | 185 ms: 1.06x slower                                                 |
| 2to3                    | 192 ms                                                 | 203 ms: 1.06x slower                                                 |
| sqlglot_transpile       | 1.44 ms                                                | 1.53 ms: 1.06x slower                                                |
| pyflate                 | 427 ms                                                 | 455 ms: 1.07x slower                                                 |
| nqueens                 | 63.8 ms                                                | 68.0 ms: 1.07x slower                                                |
| scimark_lu              | 103 ms                                                 | 110 ms: 1.07x slower                                                 |
| sqlglot_parse           | 1.24 ms                                                | 1.33 ms: 1.07x slower                                                |
| mako                    | 9.87 ms                                                | 10.6 ms: 1.07x slower                                                |
| bench_mp_pool           | 37.4 ms                                                | 40.2 ms: 1.08x slower                                                |
| pickle                  | 6.97 us                                                | 7.56 us: 1.08x slower                                                |
| crypto_pyaes            | 71.8 ms                                                | 78.3 ms: 1.09x slower                                                |
| go                      | 151 ms                                                 | 165 ms: 1.09x slower                                                 |
| regex_effbot            | 2.46 ms                                                | 2.69 ms: 1.10x slower                                                |
| raytrace                | 301 ms                                                 | 331 ms: 1.10x slower                                                 |
| scimark_monte_carlo     | 65.6 ms                                                | 72.3 ms: 1.10x slower                                                |
| genshi_xml              | 33.8 ms                                                | 37.3 ms: 1.10x slower                                                |
| pickle_dict             | 17.0 us                                                | 18.8 us: 1.11x slower                                                |
| pylint                  | 277 ms                                                 | 307 ms: 1.11x slower                                                 |
| python_startup          | 10.9 ms                                                | 12.1 ms: 1.12x slower                                                |
| unpickle                | 8.80 us                                                | 9.89 us: 1.12x slower                                                |
| html5lib                | 42.4 ms                                                | 47.8 ms: 1.13x slower                                                |
| pathlib                 | 24.5 ms                                                | 28.3 ms: 1.15x slower                                                |
| python_startup_no_site  | 7.91 ms                                                | 9.13 ms: 1.15x slower                                                |
| Geometric mean          | (ref)                                                  | 1.04x slower                                                         |

Benchmark hidden because not significant (2): unpickle_list, xml_etree_parse
Ignored benchmarks (6) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 0.99x