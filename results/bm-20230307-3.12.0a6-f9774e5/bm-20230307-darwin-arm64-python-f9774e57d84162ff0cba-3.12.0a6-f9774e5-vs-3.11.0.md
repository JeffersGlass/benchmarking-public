
# Results vs. 3.11.0

- fork: python
- ref: f9774e57d84162ff0cba
- machine: darwin-arm64
- commit hash: f9774e5
- commit date: 2023-03-07
- overall geometric mean: 1.06x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x slower
- Memory change: 1.03x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 165 ms: 1.07x slower                                                  |
| chameleon      | 4.30 ms                                                | 4.48 ms: 1.04x slower                                                 |
| docutils       | 1.43 sec                                               | 1.49 sec: 1.04x slower                                                |
| html5lib       | 33.0 ms                                                | 35.4 ms: 1.07x slower                                                 |
| Geometric mean | (ref)                                                  | 1.05x slower                                                          |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_none         | 282 ms                                                 | 289 ms: 1.03x slower                                                  |
| async_tree_cpu_io_mixed | 519 ms                                                 | 547 ms: 1.06x slower                                                  |
| async_tree_io           | 697 ms                                                 | 744 ms: 1.07x slower                                                  |
| Geometric mean          | (ref)                                                  | 1.04x slower                                                          |

Benchmark hidden because not significant (1): async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 281 ms: 1.00x slower                                                  |
| float          | 50.8 ms                                                | 53.5 ms: 1.05x slower                                                 |
| nbody          | 61.7 ms                                                | 66.1 ms: 1.07x slower                                                 |
| Geometric mean | (ref)                                                  | 1.04x slower                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_dna      | 148 ms                                                 | 153 ms: 1.03x slower                                                  |
| regex_compile  | 72.8 ms                                                | 75.4 ms: 1.04x slower                                                 |
| regex_v8       | 15.1 ms                                                | 16.2 ms: 1.07x slower                                                 |
| regex_effbot   | 2.43 ms                                                | 2.69 ms: 1.11x slower                                                 |
| Geometric mean | (ref)                                                  | 1.06x slower                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.18 ms: 1.22x faster                                                 |
| xml_etree_parse      | 100 ms                                                 | 97.9 ms: 1.02x faster                                                 |
| unpickle_pure_python | 149 us                                                 | 145 us: 1.02x faster                                                  |
| unpickle_list        | 2.69 us                                                | 2.65 us: 1.01x faster                                                 |
| pickle_pure_python   | 191 us                                                 | 191 us: 1.01x faster                                                  |
| xml_etree_iterparse  | 68.3 ms                                                | 71.1 ms: 1.04x slower                                                 |
| json_loads           | 15.3 us                                                | 16.1 us: 1.05x slower                                                 |
| pickle_list          | 2.70 us                                                | 2.83 us: 1.05x slower                                                 |
| pickle_dict          | 17.1 us                                                | 18.0 us: 1.05x slower                                                 |
| pickle               | 6.98 us                                                | 7.47 us: 1.07x slower                                                 |
| xml_etree_process    | 33.6 ms                                                | 37.0 ms: 1.10x slower                                                 |
| xml_etree_generate   | 45.8 ms                                                | 51.1 ms: 1.12x slower                                                 |
| unpickle             | 8.29 us                                                | 9.71 us: 1.17x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.03x slower                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 12.5 ms: 1.16x slower                                                 |
| python_startup_no_site | 8.57 ms                                                | 10.4 ms: 1.21x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.18x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 7.93 ms                                                | 7.44 ms: 1.07x faster                                                 |
| genshi_text     | 14.4 ms                                                | 14.7 ms: 1.02x slower                                                 |
| genshi_xml      | 28.5 ms                                                | 29.2 ms: 1.02x slower                                                 |
| django_template | 20.1 ms                                                | 21.6 ms: 1.07x slower                                                 |
| Geometric mean  | (ref)                                                  | 1.01x slower                                                          |

All benchmarks:
===============

| Benchmark               | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| asyncio_tcp             | 643 ms                                                 | 473 ms: 1.36x faster                                                  |
| json_dumps              | 7.53 ms                                                | 6.18 ms: 1.22x faster                                                 |
| generators              | 30.3 ms                                                | 27.9 ms: 1.09x faster                                                 |
| mako                    | 7.93 ms                                                | 7.44 ms: 1.07x faster                                                 |
| deltablue               | 2.75 ms                                                | 2.59 ms: 1.06x faster                                                 |
| hexiom                  | 4.58 ms                                                | 4.46 ms: 1.03x faster                                                 |
| xml_etree_parse         | 100 ms                                                 | 97.9 ms: 1.02x faster                                                 |
| unpickle_pure_python    | 149 us                                                 | 145 us: 1.02x faster                                                  |
| unpack_sequence         | 33.6 ns                                                | 32.9 ns: 1.02x faster                                                 |
| richards                | 31.1 ms                                                | 30.5 ms: 1.02x faster                                                 |
| unpickle_list           | 2.69 us                                                | 2.65 us: 1.01x faster                                                 |
| create_gc_cycles        | 711 us                                                 | 702 us: 1.01x faster                                                  |
| pprint_pformat          | 979 ms                                                 | 970 ms: 1.01x faster                                                  |
| pickle_pure_python      | 191 us                                                 | 191 us: 1.01x faster                                                  |
| pprint_safe_repr        | 478 ms                                                 | 477 ms: 1.00x faster                                                  |
| pidigits                | 280 ms                                                 | 281 ms: 1.00x slower                                                  |
| mdp                     | 1.48 sec                                               | 1.50 sec: 1.01x slower                                                |
| chaos                   | 47.4 ms                                                | 47.8 ms: 1.01x slower                                                 |
| json                    | 2.75 ms                                                | 2.79 ms: 1.01x slower                                                 |
| bench_thread_pool       | 465 us                                                 | 472 us: 1.01x slower                                                  |
| gc_traversal            | 2.38 ms                                                | 2.43 ms: 1.02x slower                                                 |
| genshi_text             | 14.4 ms                                                | 14.7 ms: 1.02x slower                                                 |
| pycparser               | 659 ms                                                 | 674 ms: 1.02x slower                                                  |
| genshi_xml              | 28.5 ms                                                | 29.2 ms: 1.02x slower                                                 |
| deepcopy_memo           | 25.7 us                                                | 26.4 us: 1.03x slower                                                 |
| async_tree_none         | 282 ms                                                 | 289 ms: 1.03x slower                                                  |
| meteor_contest          | 71.1 ms                                                | 72.9 ms: 1.03x slower                                                 |
| deepcopy                | 215 us                                                 | 222 us: 1.03x slower                                                  |
| sqlalchemy_imperative   | 6.98 ms                                                | 7.21 ms: 1.03x slower                                                 |
| dulwich_log             | 28.6 ms                                                | 29.6 ms: 1.03x slower                                                 |
| regex_dna               | 148 ms                                                 | 153 ms: 1.03x slower                                                  |
| sympy_integrate         | 11.3 ms                                                | 11.7 ms: 1.03x slower                                                 |
| regex_compile           | 72.8 ms                                                | 75.4 ms: 1.04x slower                                                 |
| xml_etree_iterparse     | 68.3 ms                                                | 71.1 ms: 1.04x slower                                                 |
| logging_silent          | 66.5 ns                                                | 69.3 ns: 1.04x slower                                                 |
| docutils                | 1.43 sec                                               | 1.49 sec: 1.04x slower                                                |
| chameleon               | 4.30 ms                                                | 4.48 ms: 1.04x slower                                                 |
| go                      | 105 ms                                                 | 111 ms: 1.05x slower                                                  |
| json_loads              | 15.3 us                                                | 16.1 us: 1.05x slower                                                 |
| pickle_list             | 2.70 us                                                | 2.83 us: 1.05x slower                                                 |
| pickle_dict             | 17.1 us                                                | 18.0 us: 1.05x slower                                                 |
| float                   | 50.8 ms                                                | 53.5 ms: 1.05x slower                                                 |
| coroutines              | 17.2 ms                                                | 18.1 ms: 1.05x slower                                                 |
| async_tree_cpu_io_mixed | 519 ms                                                 | 547 ms: 1.06x slower                                                  |
| async_tree_io           | 697 ms                                                 | 744 ms: 1.07x slower                                                  |
| 2to3                    | 154 ms                                                 | 165 ms: 1.07x slower                                                  |
| regex_v8                | 15.1 ms                                                | 16.2 ms: 1.07x slower                                                 |
| nbody                   | 61.7 ms                                                | 66.1 ms: 1.07x slower                                                 |
| pickle                  | 6.98 us                                                | 7.47 us: 1.07x slower                                                 |
| logging_simple          | 3.41 us                                                | 3.66 us: 1.07x slower                                                 |
| django_template         | 20.1 ms                                                | 21.6 ms: 1.07x slower                                                 |
| html5lib                | 33.0 ms                                                | 35.4 ms: 1.07x slower                                                 |
| sympy_str               | 144 ms                                                 | 155 ms: 1.07x slower                                                  |
| logging_format          | 3.67 us                                                | 3.95 us: 1.08x slower                                                 |
| sqlalchemy_declarative  | 59.3 ms                                                | 63.8 ms: 1.08x slower                                                 |
| fannkuch                | 240 ms                                                 | 258 ms: 1.08x slower                                                  |
| sqlglot_normalize       | 162 ms                                                 | 175 ms: 1.08x slower                                                  |
| sympy_expand            | 229 ms                                                 | 248 ms: 1.08x slower                                                  |
| sqlglot_optimize        | 29.6 ms                                                | 32.1 ms: 1.08x slower                                                 |
| sqlite_synth            | 1.26 us                                                | 1.37 us: 1.09x slower                                                 |
| deepcopy_reduce         | 1.79 us                                                | 1.95 us: 1.09x slower                                                 |
| scimark_lu              | 67.7 ms                                                | 74.2 ms: 1.10x slower                                                 |
| sympy_sum               | 80.2 ms                                                | 88.2 ms: 1.10x slower                                                 |
| telco                   | 3.17 ms                                                | 3.49 ms: 1.10x slower                                                 |
| xml_etree_process       | 33.6 ms                                                | 37.0 ms: 1.10x slower                                                 |
| thrift                  | 410 us                                                 | 453 us: 1.10x slower                                                  |
| scimark_sor             | 79.2 ms                                                | 87.7 ms: 1.11x slower                                                 |
| regex_effbot            | 2.43 ms                                                | 2.69 ms: 1.11x slower                                                 |
| raytrace                | 206 ms                                                 | 229 ms: 1.11x slower                                                  |
| xml_etree_generate      | 45.8 ms                                                | 51.1 ms: 1.12x slower                                                 |
| scimark_sparse_mat_mult | 2.81 ms                                                | 3.17 ms: 1.13x slower                                                 |
| crypto_pyaes            | 47.5 ms                                                | 53.5 ms: 1.13x slower                                                 |
| nqueens                 | 55.9 ms                                                | 63.1 ms: 1.13x slower                                                 |
| scimark_fft             | 173 ms                                                 | 196 ms: 1.13x slower                                                  |
| bench_mp_pool           | 41.0 ms                                                | 46.5 ms: 1.14x slower                                                 |
| spectral_norm           | 65.7 ms                                                | 74.9 ms: 1.14x slower                                                 |
| python_startup          | 10.8 ms                                                | 12.5 ms: 1.16x slower                                                 |
| sqlglot_transpile       | 1.05 ms                                                | 1.22 ms: 1.16x slower                                                 |
| pyflate                 | 284 ms                                                 | 331 ms: 1.17x slower                                                  |
| unpickle                | 8.29 us                                                | 9.71 us: 1.17x slower                                                 |
| scimark_monte_carlo     | 43.5 ms                                                | 51.0 ms: 1.17x slower                                                 |
| sqlglot_parse           | 890 us                                                 | 1.05 ms: 1.18x slower                                                 |
| pathlib                 | 23.2 ms                                                | 27.5 ms: 1.18x slower                                                 |
| python_startup_no_site  | 8.57 ms                                                | 10.4 ms: 1.21x slower                                                 |
| comprehensions          | 14.4 us                                                | 17.7 us: 1.22x slower                                                 |
| coverage                | 43.9 ms                                                | 59.6 ms: 1.36x slower                                                 |
| async_generators        | 192 ms                                                 | 272 ms: 1.41x slower                                                  |
| dask                    | 219 ms                                                 | 325 ms: 1.48x slower                                                  |
| Geometric mean          | (ref)                                                  | 1.06x slower                                                          |

Benchmark hidden because not significant (2): async_tree_memoization, tornado_http
Ignored benchmarks (14) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, gunicorn, mypy2, pylint, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.04x
- 95% likely to have a slowdown of 1.04x
- 99% likely to have a slowdown of 1.03x


# Memory

- memory change: 1.03x