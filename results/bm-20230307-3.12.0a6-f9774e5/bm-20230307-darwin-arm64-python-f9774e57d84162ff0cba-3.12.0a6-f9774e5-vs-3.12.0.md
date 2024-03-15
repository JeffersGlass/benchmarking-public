
# Results vs. 3.12.0

- fork: python
- ref: f9774e57d84162ff0cba
- machine: darwin-arm64
- commit hash: f9774e5
- commit date: 2023-03-07
- overall geometric mean: 1.01x slower \*
- HPT reliability: 61.93%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 165 ms: 1.03x faster                                                  |
| chameleon      | 4.70 ms                                                | 4.48 ms: 1.05x faster                                                 |
| docutils       | 1.50 sec                                               | 1.49 sec: 1.01x faster                                                |
| Geometric mean | (ref)                                                  | 1.02x faster                                                          |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 526 ms                                                 | 547 ms: 1.04x slower                                                  |
| async_tree_memoization  | 312 ms                                                 | 336 ms: 1.08x slower                                                  |
| async_tree_none         | 266 ms                                                 | 289 ms: 1.09x slower                                                  |
| async_tree_io           | 668 ms                                                 | 744 ms: 1.11x slower                                                  |
| Geometric mean          | (ref)                                                  | 1.08x slower                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| float          | 55.8 ms                                                | 53.5 ms: 1.04x faster                                                 |
| nbody          | 68.8 ms                                                | 66.1 ms: 1.04x faster                                                 |
| pidigits       | 282 ms                                                 | 281 ms: 1.00x faster                                                  |
| Geometric mean | (ref)                                                  | 1.03x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 77.9 ms                                                | 75.4 ms: 1.03x faster                                                 |
| regex_dna      | 154 ms                                                 | 153 ms: 1.01x faster                                                  |
| regex_v8       | 16.0 ms                                                | 16.2 ms: 1.01x slower                                                 |
| regex_effbot   | 2.64 ms                                                | 2.69 ms: 1.02x slower                                                 |
| Geometric mean | (ref)                                                  | 1.00x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| unpickle_list        | 3.02 us                                                | 2.65 us: 1.14x faster                                                 |
| xml_etree_generate   | 55.8 ms                                                | 51.1 ms: 1.09x faster                                                 |
| xml_etree_parse      | 106 ms                                                 | 97.9 ms: 1.09x faster                                                 |
| xml_etree_process    | 39.7 ms                                                | 37.0 ms: 1.07x faster                                                 |
| json_loads           | 17.2 us                                                | 16.1 us: 1.07x faster                                                 |
| pickle_pure_python   | 200 us                                                 | 191 us: 1.05x faster                                                  |
| xml_etree_iterparse  | 74.0 ms                                                | 71.1 ms: 1.04x faster                                                 |
| unpickle_pure_python | 151 us                                                 | 145 us: 1.04x faster                                                  |
| pickle_list          | 2.89 us                                                | 2.83 us: 1.02x faster                                                 |
| json_dumps           | 6.22 ms                                                | 6.18 ms: 1.01x faster                                                 |
| pickle_dict          | 18.1 us                                                | 18.0 us: 1.00x faster                                                 |
| pickle               | 7.23 us                                                | 7.47 us: 1.03x slower                                                 |
| unpickle             | 9.12 us                                                | 9.71 us: 1.06x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.04x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 12.5 ms: 1.09x slower                                                 |
| python_startup_no_site | 9.37 ms                                                | 10.4 ms: 1.11x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.10x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 7.71 ms                                                | 7.44 ms: 1.04x faster                                                 |
| django_template | 22.3 ms                                                | 21.6 ms: 1.03x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.03x faster                                                          |

All benchmarks:
===============

| Benchmark               | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| sqlite_synth            | 1.57 us                                                | 1.37 us: 1.15x faster                                                 |
| unpickle_list           | 3.02 us                                                | 2.65 us: 1.14x faster                                                 |
| async_generators        | 304 ms                                                 | 272 ms: 1.12x faster                                                  |
| generators              | 31.1 ms                                                | 27.9 ms: 1.12x faster                                                 |
| json                    | 3.09 ms                                                | 2.79 ms: 1.11x faster                                                 |
| logging_silent          | 76.4 ns                                                | 69.3 ns: 1.10x faster                                                 |
| xml_etree_generate      | 55.8 ms                                                | 51.1 ms: 1.09x faster                                                 |
| xml_etree_parse         | 106 ms                                                 | 97.9 ms: 1.09x faster                                                 |
| xml_etree_process       | 39.7 ms                                                | 37.0 ms: 1.07x faster                                                 |
| json_loads              | 17.2 us                                                | 16.1 us: 1.07x faster                                                 |
| bench_thread_pool       | 504 us                                                 | 472 us: 1.07x faster                                                  |
| sqlglot_normalize       | 186 ms                                                 | 175 ms: 1.06x faster                                                  |
| coroutines              | 19.2 ms                                                | 18.1 ms: 1.06x faster                                                 |
| deepcopy_reduce         | 2.07 us                                                | 1.95 us: 1.06x faster                                                 |
| sqlglot_optimize        | 34.0 ms                                                | 32.1 ms: 1.06x faster                                                 |
| mdp                     | 1.58 sec                                               | 1.50 sec: 1.06x faster                                                |
| deepcopy                | 235 us                                                 | 222 us: 1.06x faster                                                  |
| telco                   | 3.68 ms                                                | 3.49 ms: 1.06x faster                                                 |
| richards                | 32.1 ms                                                | 30.5 ms: 1.05x faster                                                 |
| pickle_pure_python      | 200 us                                                 | 191 us: 1.05x faster                                                  |
| deepcopy_memo           | 27.7 us                                                | 26.4 us: 1.05x faster                                                 |
| chameleon               | 4.70 ms                                                | 4.48 ms: 1.05x faster                                                 |
| deltablue               | 2.71 ms                                                | 2.59 ms: 1.05x faster                                                 |
| pprint_pformat          | 1.01 sec                                               | 970 ms: 1.04x faster                                                  |
| pprint_safe_repr        | 497 ms                                                 | 477 ms: 1.04x faster                                                  |
| float                   | 55.8 ms                                                | 53.5 ms: 1.04x faster                                                 |
| nbody                   | 68.8 ms                                                | 66.1 ms: 1.04x faster                                                 |
| xml_etree_iterparse     | 74.0 ms                                                | 71.1 ms: 1.04x faster                                                 |
| unpickle_pure_python    | 151 us                                                 | 145 us: 1.04x faster                                                  |
| mako                    | 7.71 ms                                                | 7.44 ms: 1.04x faster                                                 |
| django_template         | 22.3 ms                                                | 21.6 ms: 1.03x faster                                                 |
| regex_compile           | 77.9 ms                                                | 75.4 ms: 1.03x faster                                                 |
| 2to3                    | 169 ms                                                 | 165 ms: 1.03x faster                                                  |
| scimark_lu              | 76.0 ms                                                | 74.2 ms: 1.02x faster                                                 |
| spectral_norm           | 76.4 ms                                                | 74.9 ms: 1.02x faster                                                 |
| hexiom                  | 4.54 ms                                                | 4.46 ms: 1.02x faster                                                 |
| pickle_list             | 2.89 us                                                | 2.83 us: 1.02x faster                                                 |
| dulwich_log             | 29.8 ms                                                | 29.6 ms: 1.01x faster                                                 |
| docutils                | 1.50 sec                                               | 1.49 sec: 1.01x faster                                                |
| logging_simple          | 3.69 us                                                | 3.66 us: 1.01x faster                                                 |
| logging_format          | 3.98 us                                                | 3.95 us: 1.01x faster                                                 |
| regex_dna               | 154 ms                                                 | 153 ms: 1.01x faster                                                  |
| json_dumps              | 6.22 ms                                                | 6.18 ms: 1.01x faster                                                 |
| pickle_dict             | 18.1 us                                                | 18.0 us: 1.00x faster                                                 |
| pidigits                | 282 ms                                                 | 281 ms: 1.00x faster                                                  |
| scimark_fft             | 195 ms                                                 | 196 ms: 1.00x slower                                                  |
| scimark_sor             | 87.4 ms                                                | 87.7 ms: 1.00x slower                                                 |
| scimark_sparse_mat_mult | 3.14 ms                                                | 3.17 ms: 1.01x slower                                                 |
| nqueens                 | 62.4 ms                                                | 63.1 ms: 1.01x slower                                                 |
| gc_traversal            | 2.40 ms                                                | 2.43 ms: 1.01x slower                                                 |
| regex_v8                | 16.0 ms                                                | 16.2 ms: 1.01x slower                                                 |
| meteor_contest          | 71.7 ms                                                | 72.9 ms: 1.02x slower                                                 |
| regex_effbot            | 2.64 ms                                                | 2.69 ms: 1.02x slower                                                 |
| sqlalchemy_declarative  | 62.3 ms                                                | 63.8 ms: 1.02x slower                                                 |
| sympy_integrate         | 11.4 ms                                                | 11.7 ms: 1.03x slower                                                 |
| sympy_expand            | 241 ms                                                 | 248 ms: 1.03x slower                                                  |
| crypto_pyaes            | 51.9 ms                                                | 53.5 ms: 1.03x slower                                                 |
| pickle                  | 7.23 us                                                | 7.47 us: 1.03x slower                                                 |
| bench_mp_pool           | 44.9 ms                                                | 46.5 ms: 1.04x slower                                                 |
| fannkuch                | 248 ms                                                 | 258 ms: 1.04x slower                                                  |
| async_tree_cpu_io_mixed | 526 ms                                                 | 547 ms: 1.04x slower                                                  |
| unpack_sequence         | 31.5 ns                                                | 32.9 ns: 1.05x slower                                                 |
| sympy_str               | 148 ms                                                 | 155 ms: 1.05x slower                                                  |
| pyflate                 | 316 ms                                                 | 331 ms: 1.05x slower                                                  |
| unpickle                | 9.12 us                                                | 9.71 us: 1.06x slower                                                 |
| async_tree_memoization  | 312 ms                                                 | 336 ms: 1.08x slower                                                  |
| raytrace                | 212 ms                                                 | 229 ms: 1.08x slower                                                  |
| sqlalchemy_imperative   | 6.68 ms                                                | 7.21 ms: 1.08x slower                                                 |
| async_tree_none         | 266 ms                                                 | 289 ms: 1.09x slower                                                  |
| go                      | 102 ms                                                 | 111 ms: 1.09x slower                                                  |
| python_startup          | 11.4 ms                                                | 12.5 ms: 1.09x slower                                                 |
| python_startup_no_site  | 9.37 ms                                                | 10.4 ms: 1.11x slower                                                 |
| async_tree_io           | 668 ms                                                 | 744 ms: 1.11x slower                                                  |
| chaos                   | 42.5 ms                                                | 47.8 ms: 1.12x slower                                                 |
| scimark_monte_carlo     | 45.0 ms                                                | 51.0 ms: 1.13x slower                                                 |
| pathlib                 | 24.2 ms                                                | 27.5 ms: 1.13x slower                                                 |
| sympy_sum               | 77.6 ms                                                | 88.2 ms: 1.14x slower                                                 |
| sqlglot_transpile       | 1.02 ms                                                | 1.22 ms: 1.20x slower                                                 |
| comprehensions          | 14.5 us                                                | 17.7 us: 1.22x slower                                                 |
| sqlglot_parse           | 848 us                                                 | 1.05 ms: 1.24x slower                                                 |
| dask                    | 222 ms                                                 | 325 ms: 1.46x slower                                                  |
| coverage                | 38.9 ms                                                | 59.6 ms: 1.53x slower                                                 |
| Geometric mean          | (ref)                                                  | 1.01x slower                                                          |

Benchmark hidden because not significant (4): pycparser, create_gc_cycles, tornado_http, asyncio_tcp
Ignored benchmarks (12) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, gunicorn, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (4) of results/bm-20230307-3.12.0a6-f9774e5/bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5.json: genshi_text, genshi_xml, html5lib, thrift


# HPT report

- Reliability score: 61.93% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.98x