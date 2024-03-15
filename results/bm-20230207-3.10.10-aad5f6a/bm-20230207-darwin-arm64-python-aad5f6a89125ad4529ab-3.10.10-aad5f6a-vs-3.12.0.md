
# Results vs. 3.12.0

- fork: python
- ref: aad5f6a89125ad4529ab
- machine: darwin-arm64
- commit hash: aad5f6a
- commit date: 2023-02-07
- overall geometric mean: 1.21x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.17x slower
- Memory change: 0.90x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-darwin-arm64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 203 ms: 1.20x slower                                                 |
| chameleon      | 4.70 ms                                                | 5.78 ms: 1.23x slower                                                |
| docutils       | 1.50 sec                                               | 1.79 sec: 1.19x slower                                               |
| tornado_http   | 69.3 ms                                                | 92.9 ms: 1.34x slower                                                |
| Geometric mean | (ref)                                                  | 1.24x slower                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-darwin-arm64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 526 ms                                                 | 667 ms: 1.27x slower                                                 |
| async_tree_none         | 266 ms                                                 | 400 ms: 1.51x slower                                                 |
| async_tree_io           | 668 ms                                                 | 1.02 sec: 1.52x slower                                               |
| async_tree_memoization  | 312 ms                                                 | 488 ms: 1.56x slower                                                 |
| Geometric mean          | (ref)                                                  | 1.46x slower                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-darwin-arm64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| float          | 55.8 ms                                                | 72.3 ms: 1.30x slower                                                |
| nbody          | 68.8 ms                                                | 94.1 ms: 1.37x slower                                                |
| Geometric mean | (ref)                                                  | 1.21x slower                                                         |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-darwin-arm64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_effbot   | 2.64 ms                                                | 2.75 ms: 1.04x slower                                                |
| regex_v8       | 16.0 ms                                                | 18.2 ms: 1.14x slower                                                |
| regex_dna      | 154 ms                                                 | 187 ms: 1.21x slower                                                 |
| regex_compile  | 77.9 ms                                                | 96.9 ms: 1.24x slower                                                |
| Geometric mean | (ref)                                                  | 1.16x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-darwin-arm64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| unpickle_list        | 3.02 us                                                | 2.68 us: 1.13x faster                                                |
| json_loads           | 17.2 us                                                | 16.9 us: 1.02x faster                                                |
| xml_etree_generate   | 55.8 ms                                                | 55.0 ms: 1.01x faster                                                |
| xml_etree_iterparse  | 74.0 ms                                                | 73.1 ms: 1.01x faster                                                |
| pickle_list          | 2.89 us                                                | 2.93 us: 1.01x slower                                                |
| pickle_dict          | 18.1 us                                                | 18.7 us: 1.04x slower                                                |
| pickle               | 7.23 us                                                | 7.54 us: 1.04x slower                                                |
| unpickle             | 9.12 us                                                | 9.86 us: 1.08x slower                                                |
| xml_etree_process    | 39.7 ms                                                | 45.0 ms: 1.14x slower                                                |
| json_dumps           | 6.22 ms                                                | 8.29 ms: 1.33x slower                                                |
| unpickle_pure_python | 151 us                                                 | 204 us: 1.35x slower                                                 |
| pickle_pure_python   | 200 us                                                 | 287 us: 1.44x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.09x slower                                                         |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-darwin-arm64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup_no_site | 9.37 ms                                                | 9.82 ms: 1.05x slower                                                |
| python_startup         | 11.4 ms                                                | 12.7 ms: 1.11x slower                                                |
| Geometric mean         | (ref)                                                  | 1.08x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-darwin-arm64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|-----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| django_template | 22.3 ms                                                | 27.2 ms: 1.22x slower                                                |
| mako            | 7.71 ms                                                | 10.5 ms: 1.37x slower                                                |
| Geometric mean  | (ref)                                                  | 1.29x slower                                                         |

All benchmarks:
===============

| Benchmark               | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-darwin-arm64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_generators        | 304 ms                                                 | 234 ms: 1.30x faster                                                 |
| unpickle_list           | 3.02 us                                                | 2.68 us: 1.13x faster                                                |
| bench_mp_pool           | 44.9 ms                                                | 40.9 ms: 1.10x faster                                                |
| sqlite_synth            | 1.57 us                                                | 1.47 us: 1.07x faster                                                |
| json_loads              | 17.2 us                                                | 16.9 us: 1.02x faster                                                |
| xml_etree_generate      | 55.8 ms                                                | 55.0 ms: 1.01x faster                                                |
| xml_etree_iterparse     | 74.0 ms                                                | 73.1 ms: 1.01x faster                                                |
| telco                   | 3.68 ms                                                | 3.65 ms: 1.01x faster                                                |
| pickle_list             | 2.89 us                                                | 2.93 us: 1.01x slower                                                |
| pickle_dict             | 18.1 us                                                | 18.7 us: 1.04x slower                                                |
| regex_effbot            | 2.64 ms                                                | 2.75 ms: 1.04x slower                                                |
| pickle                  | 7.23 us                                                | 7.54 us: 1.04x slower                                                |
| python_startup_no_site  | 9.37 ms                                                | 9.82 ms: 1.05x slower                                                |
| coroutines              | 19.2 ms                                                | 20.2 ms: 1.05x slower                                                |
| generators              | 31.1 ms                                                | 32.7 ms: 1.05x slower                                                |
| sqlglot_normalize       | 186 ms                                                 | 196 ms: 1.06x slower                                                 |
| mdp                     | 1.58 sec                                               | 1.67 sec: 1.06x slower                                               |
| bench_thread_pool       | 504 us                                                 | 534 us: 1.06x slower                                                 |
| coverage                | 38.9 ms                                                | 41.8 ms: 1.08x slower                                                |
| unpickle                | 9.12 us                                                | 9.86 us: 1.08x slower                                                |
| meteor_contest          | 71.7 ms                                                | 77.6 ms: 1.08x slower                                                |
| nqueens                 | 62.4 ms                                                | 68.1 ms: 1.09x slower                                                |
| scimark_sparse_mat_mult | 3.14 ms                                                | 3.48 ms: 1.11x slower                                                |
| python_startup          | 11.4 ms                                                | 12.7 ms: 1.11x slower                                                |
| sqlglot_optimize        | 34.0 ms                                                | 38.0 ms: 1.12x slower                                                |
| xml_etree_process       | 39.7 ms                                                | 45.0 ms: 1.14x slower                                                |
| deepcopy_reduce         | 2.07 us                                                | 2.35 us: 1.14x slower                                                |
| regex_v8                | 16.0 ms                                                | 18.2 ms: 1.14x slower                                                |
| sympy_expand            | 241 ms                                                 | 278 ms: 1.15x slower                                                 |
| sympy_str               | 148 ms                                                 | 171 ms: 1.16x slower                                                 |
| gunicorn                | 1.15 ms                                                | 1.34 ms: 1.17x slower                                                |
| aiohttp                 | 1.08 ms                                                | 1.26 ms: 1.17x slower                                                |
| sympy_integrate         | 11.4 ms                                                | 13.4 ms: 1.18x slower                                                |
| pathlib                 | 24.2 ms                                                | 28.7 ms: 1.19x slower                                                |
| scimark_fft             | 195 ms                                                 | 232 ms: 1.19x slower                                                 |
| docutils                | 1.50 sec                                               | 1.79 sec: 1.19x slower                                               |
| dask                    | 222 ms                                                 | 265 ms: 1.19x slower                                                 |
| deepcopy                | 235 us                                                 | 280 us: 1.19x slower                                                 |
| 2to3                    | 169 ms                                                 | 203 ms: 1.20x slower                                                 |
| sqlalchemy_declarative  | 62.3 ms                                                | 74.8 ms: 1.20x slower                                                |
| pprint_safe_repr        | 497 ms                                                 | 600 ms: 1.21x slower                                                 |
| regex_dna               | 154 ms                                                 | 187 ms: 1.21x slower                                                 |
| django_template         | 22.3 ms                                                | 27.2 ms: 1.22x slower                                                |
| pprint_pformat          | 1.01 sec                                               | 1.23 sec: 1.22x slower                                               |
| unpack_sequence         | 31.5 ns                                                | 38.3 ns: 1.22x slower                                                |
| comprehensions          | 14.5 us                                                | 17.7 us: 1.22x slower                                                |
| chameleon               | 4.70 ms                                                | 5.78 ms: 1.23x slower                                                |
| deepcopy_memo           | 27.7 us                                                | 34.4 us: 1.24x slower                                                |
| regex_compile           | 77.9 ms                                                | 96.9 ms: 1.24x slower                                                |
| sympy_sum               | 77.6 ms                                                | 96.8 ms: 1.25x slower                                                |
| dulwich_log             | 29.8 ms                                                | 37.2 ms: 1.25x slower                                                |
| create_gc_cycles        | 701 us                                                 | 878 us: 1.25x slower                                                 |
| logging_simple          | 3.69 us                                                | 4.62 us: 1.25x slower                                                |
| logging_format          | 3.98 us                                                | 5.01 us: 1.26x slower                                                |
| spectral_norm           | 76.4 ms                                                | 96.3 ms: 1.26x slower                                                |
| async_tree_cpu_io_mixed | 526 ms                                                 | 667 ms: 1.27x slower                                                 |
| fannkuch                | 248 ms                                                 | 317 ms: 1.27x slower                                                 |
| float                   | 55.8 ms                                                | 72.3 ms: 1.30x slower                                                |
| json_dumps              | 6.22 ms                                                | 8.29 ms: 1.33x slower                                                |
| tornado_http            | 69.3 ms                                                | 92.9 ms: 1.34x slower                                                |
| pycparser               | 677 ms                                                 | 913 ms: 1.35x slower                                                 |
| unpickle_pure_python    | 151 us                                                 | 204 us: 1.35x slower                                                 |
| sqlalchemy_imperative   | 6.68 ms                                                | 9.10 ms: 1.36x slower                                                |
| mako                    | 7.71 ms                                                | 10.5 ms: 1.37x slower                                                |
| nbody                   | 68.8 ms                                                | 94.1 ms: 1.37x slower                                                |
| hexiom                  | 4.54 ms                                                | 6.32 ms: 1.39x slower                                                |
| pickle_pure_python      | 200 us                                                 | 287 us: 1.44x slower                                                 |
| pyflate                 | 316 ms                                                 | 455 ms: 1.44x slower                                                 |
| scimark_sor             | 87.4 ms                                                | 126 ms: 1.45x slower                                                 |
| scimark_lu              | 76.0 ms                                                | 110 ms: 1.45x slower                                                 |
| asyncio_tcp             | 449 ms                                                 | 673 ms: 1.50x slower                                                 |
| crypto_pyaes            | 51.9 ms                                                | 78.0 ms: 1.50x slower                                                |
| async_tree_none         | 266 ms                                                 | 400 ms: 1.51x slower                                                 |
| sqlglot_transpile       | 1.02 ms                                                | 1.54 ms: 1.51x slower                                                |
| async_tree_io           | 668 ms                                                 | 1.02 sec: 1.52x slower                                               |
| logging_silent          | 76.4 ns                                                | 118 ns: 1.54x slower                                                 |
| raytrace                | 212 ms                                                 | 330 ms: 1.56x slower                                                 |
| richards                | 32.1 ms                                                | 50.2 ms: 1.56x slower                                                |
| async_tree_memoization  | 312 ms                                                 | 488 ms: 1.56x slower                                                 |
| sqlglot_parse           | 848 us                                                 | 1.33 ms: 1.57x slower                                                |
| chaos                   | 42.5 ms                                                | 67.1 ms: 1.58x slower                                                |
| scimark_monte_carlo     | 45.0 ms                                                | 72.8 ms: 1.62x slower                                                |
| go                      | 102 ms                                                 | 165 ms: 1.62x slower                                                 |
| deltablue               | 2.71 ms                                                | 5.18 ms: 1.91x slower                                                |
| Geometric mean          | (ref)                                                  | 1.21x slower                                                         |

Benchmark hidden because not significant (4): json, gc_traversal, pidigits, xml_etree_parse
Ignored benchmarks (10) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (6) of results/bm-20230207-3.10.10-aad5f6a/bm-20230207-darwin-arm64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.19x
- 95% likely to have a slowdown of 1.18x
- 99% likely to have a slowdown of 1.17x


# Memory

- memory change: 0.90x