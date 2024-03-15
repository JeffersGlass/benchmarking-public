
# Results vs. 3.10.4

- fork: python
- ref: aad5f6a89125ad4529ab
- machine: darwin-arm64
- commit hash: aad5f6a
- commit date: 2023-02-07
- overall geometric mean: 1.04x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-darwin-arm64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 203 ms: 1.06x slower                                                 |
| chameleon      | 6.26 ms                                                | 5.78 ms: 1.08x faster                                                |
| docutils       | 1.73 sec                                               | 1.79 sec: 1.03x slower                                               |
| html5lib       | 42.4 ms                                                | 47.8 ms: 1.13x slower                                                |
| tornado_http   | 86.7 ms                                                | 92.9 ms: 1.07x slower                                                |
| Geometric mean | (ref)                                                  | 1.04x slower                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-darwin-arm64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 649 ms                                                 | 667 ms: 1.03x slower                                                 |
| async_tree_none         | 388 ms                                                 | 400 ms: 1.03x slower                                                 |
| async_tree_memoization  | 474 ms                                                 | 488 ms: 1.03x slower                                                 |
| async_tree_io           | 980 ms                                                 | 1.02 sec: 1.04x slower                                               |
| Geometric mean          | (ref)                                                  | 1.03x slower                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-darwin-arm64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| pidigits       | 282 ms                                                 | 282 ms: 1.00x faster                                                 |
| nbody          | 93.0 ms                                                | 94.1 ms: 1.01x slower                                                |
| float          | 69.0 ms                                                | 72.3 ms: 1.05x slower                                                |
| Geometric mean | (ref)                                                  | 1.02x slower                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-darwin-arm64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 96.9 ms: 1.02x slower                                                |
| regex_v8       | 17.1 ms                                                | 18.2 ms: 1.06x slower                                                |
| regex_dna      | 174 ms                                                 | 187 ms: 1.07x slower                                                 |
| regex_effbot   | 2.46 ms                                                | 2.75 ms: 1.12x slower                                                |
| Geometric mean | (ref)                                                  | 1.07x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-darwin-arm64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| xml_etree_process    | 46.5 ms                                                | 45.0 ms: 1.03x faster                                                |
| unpickle_list        | 2.69 us                                                | 2.68 us: 1.00x faster                                                |
| xml_etree_iterparse  | 72.1 ms                                                | 73.1 ms: 1.01x slower                                                |
| json_dumps           | 8.11 ms                                                | 8.29 ms: 1.02x slower                                                |
| pickle_pure_python   | 281 us                                                 | 287 us: 1.02x slower                                                 |
| json_loads           | 16.4 us                                                | 16.9 us: 1.03x slower                                                |
| xml_etree_generate   | 53.5 ms                                                | 55.0 ms: 1.03x slower                                                |
| unpickle_pure_python | 194 us                                                 | 204 us: 1.05x slower                                                 |
| pickle_list          | 2.74 us                                                | 2.93 us: 1.07x slower                                                |
| pickle               | 6.97 us                                                | 7.54 us: 1.08x slower                                                |
| pickle_dict          | 17.0 us                                                | 18.7 us: 1.10x slower                                                |
| unpickle             | 8.80 us                                                | 9.86 us: 1.12x slower                                                |
| Geometric mean       | (ref)                                                  | 1.04x slower                                                         |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-darwin-arm64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 12.7 ms: 1.17x slower                                                |
| python_startup_no_site | 7.91 ms                                                | 9.82 ms: 1.24x slower                                                |
| Geometric mean         | (ref)                                                  | 1.20x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-darwin-arm64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|-----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| django_template | 26.4 ms                                                | 27.2 ms: 1.03x slower                                                |
| genshi_text     | 17.3 ms                                                | 18.2 ms: 1.05x slower                                                |
| mako            | 9.87 ms                                                | 10.5 ms: 1.07x slower                                                |
| genshi_xml      | 33.8 ms                                                | 37.3 ms: 1.10x slower                                                |
| Geometric mean  | (ref)                                                  | 1.06x slower                                                         |

All benchmarks:
===============

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-darwin-arm64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| chameleon               | 6.26 ms                                                | 5.78 ms: 1.08x faster                                                |
| pprint_safe_repr        | 641 ms                                                 | 600 ms: 1.07x faster                                                 |
| pprint_pformat          | 1.30 sec                                               | 1.23 sec: 1.06x faster                                               |
| xml_etree_process       | 46.5 ms                                                | 45.0 ms: 1.03x faster                                                |
| coroutines              | 20.7 ms                                                | 20.2 ms: 1.03x faster                                                |
| unpack_sequence         | 39.0 ns                                                | 38.3 ns: 1.02x faster                                                |
| scimark_sor             | 128 ms                                                 | 126 ms: 1.01x faster                                                 |
| deepcopy_memo           | 34.7 us                                                | 34.4 us: 1.01x faster                                                |
| unpickle_list           | 2.69 us                                                | 2.68 us: 1.00x faster                                                |
| pidigits                | 282 ms                                                 | 282 ms: 1.00x faster                                                 |
| meteor_contest          | 77.7 ms                                                | 77.6 ms: 1.00x faster                                                |
| sqlite_synth            | 1.46 us                                                | 1.47 us: 1.01x slower                                                |
| coverage                | 41.5 ms                                                | 41.8 ms: 1.01x slower                                                |
| deepcopy_reduce         | 2.33 us                                                | 2.35 us: 1.01x slower                                                |
| generators              | 32.3 ms                                                | 32.7 ms: 1.01x slower                                                |
| nbody                   | 93.0 ms                                                | 94.1 ms: 1.01x slower                                                |
| bench_thread_pool       | 527 us                                                 | 534 us: 1.01x slower                                                 |
| async_generators        | 231 ms                                                 | 234 ms: 1.01x slower                                                 |
| xml_etree_iterparse     | 72.1 ms                                                | 73.1 ms: 1.01x slower                                                |
| gc_traversal            | 2.36 ms                                                | 2.40 ms: 1.02x slower                                                |
| scimark_sparse_mat_mult | 3.42 ms                                                | 3.48 ms: 1.02x slower                                                |
| spectral_norm           | 94.8 ms                                                | 96.3 ms: 1.02x slower                                                |
| regex_compile           | 95.3 ms                                                | 96.9 ms: 1.02x slower                                                |
| chaos                   | 65.8 ms                                                | 67.1 ms: 1.02x slower                                                |
| asyncio_tcp             | 659 ms                                                 | 673 ms: 1.02x slower                                                 |
| hexiom                  | 6.19 ms                                                | 6.32 ms: 1.02x slower                                                |
| sqlalchemy_declarative  | 73.3 ms                                                | 74.8 ms: 1.02x slower                                                |
| create_gc_cycles        | 860 us                                                 | 878 us: 1.02x slower                                                 |
| json_dumps              | 8.11 ms                                                | 8.29 ms: 1.02x slower                                                |
| pickle_pure_python      | 281 us                                                 | 287 us: 1.02x slower                                                 |
| sympy_integrate         | 13.1 ms                                                | 13.4 ms: 1.02x slower                                                |
| mdp                     | 1.63 sec                                               | 1.67 sec: 1.02x slower                                               |
| thrift                  | 572 us                                                 | 586 us: 1.03x slower                                                 |
| json_loads              | 16.4 us                                                | 16.9 us: 1.03x slower                                                |
| async_tree_cpu_io_mixed | 649 ms                                                 | 667 ms: 1.03x slower                                                 |
| sqlalchemy_imperative   | 8.86 ms                                                | 9.10 ms: 1.03x slower                                                |
| gunicorn                | 1.30 ms                                                | 1.34 ms: 1.03x slower                                                |
| xml_etree_generate      | 53.5 ms                                                | 55.0 ms: 1.03x slower                                                |
| django_template         | 26.4 ms                                                | 27.2 ms: 1.03x slower                                                |
| aiohttp                 | 1.22 ms                                                | 1.26 ms: 1.03x slower                                                |
| sqlglot_normalize       | 190 ms                                                 | 196 ms: 1.03x slower                                                 |
| async_tree_none         | 388 ms                                                 | 400 ms: 1.03x slower                                                 |
| docutils                | 1.73 sec                                               | 1.79 sec: 1.03x slower                                               |
| async_tree_memoization  | 474 ms                                                 | 488 ms: 1.03x slower                                                 |
| richards                | 48.7 ms                                                | 50.2 ms: 1.03x slower                                                |
| deepcopy                | 272 us                                                 | 280 us: 1.03x slower                                                 |
| scimark_fft             | 224 ms                                                 | 232 ms: 1.03x slower                                                 |
| sympy_expand            | 269 ms                                                 | 278 ms: 1.03x slower                                                 |
| sqlglot_optimize        | 36.8 ms                                                | 38.0 ms: 1.03x slower                                                |
| sympy_str               | 165 ms                                                 | 171 ms: 1.04x slower                                                 |
| flaskblogging           | 2.65 ms                                                | 2.74 ms: 1.04x slower                                                |
| async_tree_io           | 980 ms                                                 | 1.02 sec: 1.04x slower                                               |
| logging_format          | 4.83 us                                                | 5.01 us: 1.04x slower                                                |
| logging_simple          | 4.45 us                                                | 4.62 us: 1.04x slower                                                |
| pycparser               | 877 ms                                                 | 913 ms: 1.04x slower                                                 |
| fannkuch                | 303 ms                                                 | 317 ms: 1.05x slower                                                 |
| dask                    | 253 ms                                                 | 265 ms: 1.05x slower                                                 |
| unpickle_pure_python    | 194 us                                                 | 204 us: 1.05x slower                                                 |
| telco                   | 3.49 ms                                                | 3.65 ms: 1.05x slower                                                |
| comprehensions          | 16.9 us                                                | 17.7 us: 1.05x slower                                                |
| float                   | 69.0 ms                                                | 72.3 ms: 1.05x slower                                                |
| genshi_text             | 17.3 ms                                                | 18.2 ms: 1.05x slower                                                |
| sympy_sum               | 92.2 ms                                                | 96.8 ms: 1.05x slower                                                |
| dulwich_log             | 35.3 ms                                                | 37.2 ms: 1.05x slower                                                |
| deltablue               | 4.91 ms                                                | 5.18 ms: 1.05x slower                                                |
| 2to3                    | 192 ms                                                 | 203 ms: 1.06x slower                                                 |
| regex_v8                | 17.1 ms                                                | 18.2 ms: 1.06x slower                                                |
| pyflate                 | 427 ms                                                 | 455 ms: 1.07x slower                                                 |
| sqlglot_transpile       | 1.44 ms                                                | 1.54 ms: 1.07x slower                                                |
| mako                    | 9.87 ms                                                | 10.5 ms: 1.07x slower                                                |
| nqueens                 | 63.8 ms                                                | 68.1 ms: 1.07x slower                                                |
| pickle_list             | 2.74 us                                                | 2.93 us: 1.07x slower                                                |
| scimark_lu              | 103 ms                                                 | 110 ms: 1.07x slower                                                 |
| sqlglot_parse           | 1.24 ms                                                | 1.33 ms: 1.07x slower                                                |
| tornado_http            | 86.7 ms                                                | 92.9 ms: 1.07x slower                                                |
| regex_dna               | 174 ms                                                 | 187 ms: 1.07x slower                                                 |
| pickle                  | 6.97 us                                                | 7.54 us: 1.08x slower                                                |
| crypto_pyaes            | 71.8 ms                                                | 78.0 ms: 1.09x slower                                                |
| go                      | 151 ms                                                 | 165 ms: 1.09x slower                                                 |
| bench_mp_pool           | 37.4 ms                                                | 40.9 ms: 1.09x slower                                                |
| raytrace                | 301 ms                                                 | 330 ms: 1.10x slower                                                 |
| pickle_dict             | 17.0 us                                                | 18.7 us: 1.10x slower                                                |
| genshi_xml              | 33.8 ms                                                | 37.3 ms: 1.10x slower                                                |
| pylint                  | 277 ms                                                 | 307 ms: 1.11x slower                                                 |
| scimark_monte_carlo     | 65.6 ms                                                | 72.8 ms: 1.11x slower                                                |
| regex_effbot            | 2.46 ms                                                | 2.75 ms: 1.12x slower                                                |
| unpickle                | 8.80 us                                                | 9.86 us: 1.12x slower                                                |
| html5lib                | 42.4 ms                                                | 47.8 ms: 1.13x slower                                                |
| python_startup          | 10.9 ms                                                | 12.7 ms: 1.17x slower                                                |
| pathlib                 | 24.5 ms                                                | 28.7 ms: 1.17x slower                                                |
| python_startup_no_site  | 7.91 ms                                                | 9.82 ms: 1.24x slower                                                |
| Geometric mean          | (ref)                                                  | 1.04x slower                                                         |

Benchmark hidden because not significant (3): xml_etree_parse, json, logging_silent
Ignored benchmarks (6) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.03x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 0.99x