
# Results vs. 3.10.4

- fork: python
- ref: 1dd9be6584413fbfa823
- machine: darwin-arm64
- commit hash: 1dd9be6
- commit date: 2022-12-06
- overall geometric mean: 1.02x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 0.97x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 223 ms: 1.16x slower                                                |
| chameleon      | 6.26 ms                                                | 5.83 ms: 1.07x faster                                               |
| docutils       | 1.73 sec                                               | 1.77 sec: 1.02x slower                                              |
| html5lib       | 42.4 ms                                                | 46.5 ms: 1.10x slower                                               |
| tornado_http   | 86.7 ms                                                | 93.5 ms: 1.08x slower                                               |
| Geometric mean | (ref)                                                  | 1.06x slower                                                        |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6 |
|-------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| async_tree_memoization  | 474 ms                                                 | 481 ms: 1.02x slower                                                |
| async_tree_cpu_io_mixed | 649 ms                                                 | 661 ms: 1.02x slower                                                |
| async_tree_io           | 980 ms                                                 | 1.00 sec: 1.02x slower                                              |
| Geometric mean          | (ref)                                                  | 1.02x slower                                                        |

Benchmark hidden because not significant (1): async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 92.6 ms: 1.00x faster                                               |
| pidigits       | 282 ms                                                 | 284 ms: 1.00x slower                                                |
| float          | 69.0 ms                                                | 72.1 ms: 1.04x slower                                               |
| Geometric mean | (ref)                                                  | 1.01x slower                                                        |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 96.5 ms: 1.01x slower                                               |
| regex_dna      | 174 ms                                                 | 180 ms: 1.03x slower                                                |
| regex_v8       | 17.1 ms                                                | 18.3 ms: 1.07x slower                                               |
| regex_effbot   | 2.46 ms                                                | 2.64 ms: 1.07x slower                                               |
| Geometric mean | (ref)                                                  | 1.05x slower                                                        |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6 |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| xml_etree_parse      | 108 ms                                                 | 100 ms: 1.07x faster                                                |
| xml_etree_iterparse  | 72.1 ms                                                | 69.0 ms: 1.05x faster                                               |
| xml_etree_process    | 46.5 ms                                                | 44.9 ms: 1.04x faster                                               |
| unpickle_list        | 2.69 us                                                | 2.66 us: 1.01x faster                                               |
| pickle_pure_python   | 281 us                                                 | 284 us: 1.01x slower                                                |
| xml_etree_generate   | 53.5 ms                                                | 54.3 ms: 1.01x slower                                               |
| json_dumps           | 8.11 ms                                                | 8.25 ms: 1.02x slower                                               |
| json_loads           | 16.4 us                                                | 17.0 us: 1.03x slower                                               |
| unpickle_pure_python | 194 us                                                 | 203 us: 1.04x slower                                                |
| pickle_list          | 2.74 us                                                | 2.96 us: 1.08x slower                                               |
| pickle               | 6.97 us                                                | 7.56 us: 1.08x slower                                               |
| pickle_dict          | 17.0 us                                                | 18.8 us: 1.11x slower                                               |
| unpickle             | 8.80 us                                                | 9.87 us: 1.12x slower                                               |
| Geometric mean       | (ref)                                                  | 1.03x slower                                                        |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6 |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| python_startup_no_site | 7.91 ms                                                | 6.95 ms: 1.14x faster                                               |
| python_startup         | 10.9 ms                                                | 9.57 ms: 1.14x faster                                               |
| Geometric mean         | (ref)                                                  | 1.14x faster                                                        |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6 |
|-----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| django_template | 26.4 ms                                                | 27.3 ms: 1.03x slower                                               |
| genshi_text     | 17.3 ms                                                | 18.2 ms: 1.05x slower                                               |
| mako            | 9.87 ms                                                | 10.7 ms: 1.08x slower                                               |
| genshi_xml      | 33.8 ms                                                | 37.3 ms: 1.10x slower                                               |
| Geometric mean  | (ref)                                                  | 1.07x slower                                                        |

All benchmarks:
===============

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6 |
|-------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| python_startup_no_site  | 7.91 ms                                                | 6.95 ms: 1.14x faster                                               |
| python_startup          | 10.9 ms                                                | 9.57 ms: 1.14x faster                                               |
| pathlib                 | 24.5 ms                                                | 22.0 ms: 1.12x faster                                               |
| xml_etree_parse         | 108 ms                                                 | 100 ms: 1.07x faster                                                |
| chameleon               | 6.26 ms                                                | 5.83 ms: 1.07x faster                                               |
| pprint_safe_repr        | 641 ms                                                 | 603 ms: 1.06x faster                                                |
| pprint_pformat          | 1.30 sec                                               | 1.23 sec: 1.06x faster                                              |
| xml_etree_iterparse     | 72.1 ms                                                | 69.0 ms: 1.05x faster                                               |
| unpack_sequence         | 39.0 ns                                                | 37.4 ns: 1.04x faster                                               |
| xml_etree_process       | 46.5 ms                                                | 44.9 ms: 1.04x faster                                               |
| gunicorn                | 1.30 ms                                                | 1.26 ms: 1.03x faster                                               |
| aiohttp                 | 1.22 ms                                                | 1.19 ms: 1.03x faster                                               |
| coroutines              | 20.7 ms                                                | 20.1 ms: 1.03x faster                                               |
| coverage                | 41.5 ms                                                | 40.6 ms: 1.02x faster                                               |
| flaskblogging           | 2.65 ms                                                | 2.60 ms: 1.02x faster                                               |
| bench_thread_pool       | 527 us                                                 | 518 us: 1.02x faster                                                |
| scimark_sor             | 128 ms                                                 | 126 ms: 1.02x faster                                                |
| unpickle_list           | 2.69 us                                                | 2.66 us: 1.01x faster                                               |
| deepcopy_memo           | 34.7 us                                                | 34.5 us: 1.01x faster                                               |
| meteor_contest          | 77.7 ms                                                | 77.4 ms: 1.00x faster                                               |
| nbody                   | 93.0 ms                                                | 92.6 ms: 1.00x faster                                               |
| deepcopy_reduce         | 2.33 us                                                | 2.34 us: 1.00x slower                                               |
| pidigits                | 282 ms                                                 | 284 ms: 1.00x slower                                                |
| json                    | 3.08 ms                                                | 3.11 ms: 1.01x slower                                               |
| sqlalchemy_imperative   | 8.86 ms                                                | 8.96 ms: 1.01x slower                                               |
| pickle_pure_python      | 281 us                                                 | 284 us: 1.01x slower                                                |
| scimark_sparse_mat_mult | 3.42 ms                                                | 3.46 ms: 1.01x slower                                               |
| chaos                   | 65.8 ms                                                | 66.6 ms: 1.01x slower                                               |
| regex_compile           | 95.3 ms                                                | 96.5 ms: 1.01x slower                                               |
| spectral_norm           | 94.8 ms                                                | 96.2 ms: 1.01x slower                                               |
| xml_etree_generate      | 53.5 ms                                                | 54.3 ms: 1.01x slower                                               |
| async_tree_memoization  | 474 ms                                                 | 481 ms: 1.02x slower                                                |
| thrift                  | 572 us                                                 | 582 us: 1.02x slower                                                |
| sqlalchemy_declarative  | 73.3 ms                                                | 74.5 ms: 1.02x slower                                               |
| json_dumps              | 8.11 ms                                                | 8.25 ms: 1.02x slower                                               |
| async_tree_cpu_io_mixed | 649 ms                                                 | 661 ms: 1.02x slower                                                |
| hexiom                  | 6.19 ms                                                | 6.30 ms: 1.02x slower                                               |
| sympy_integrate         | 13.1 ms                                                | 13.4 ms: 1.02x slower                                               |
| sqlite_synth            | 1.46 us                                                | 1.49 us: 1.02x slower                                               |
| mdp                     | 1.63 sec                                               | 1.66 sec: 1.02x slower                                              |
| docutils                | 1.73 sec                                               | 1.77 sec: 1.02x slower                                              |
| async_tree_io           | 980 ms                                                 | 1.00 sec: 1.02x slower                                              |
| scimark_fft             | 224 ms                                                 | 230 ms: 1.02x slower                                                |
| sympy_expand            | 269 ms                                                 | 276 ms: 1.03x slower                                                |
| sympy_str               | 165 ms                                                 | 170 ms: 1.03x slower                                                |
| deepcopy                | 272 us                                                 | 280 us: 1.03x slower                                                |
| sqlglot_normalize       | 190 ms                                                 | 196 ms: 1.03x slower                                                |
| sqlglot_optimize        | 36.8 ms                                                | 37.9 ms: 1.03x slower                                               |
| regex_dna               | 174 ms                                                 | 180 ms: 1.03x slower                                                |
| django_template         | 26.4 ms                                                | 27.3 ms: 1.03x slower                                               |
| logging_format          | 4.83 us                                                | 4.99 us: 1.03x slower                                               |
| sympy_sum               | 92.2 ms                                                | 95.4 ms: 1.03x slower                                               |
| json_loads              | 16.4 us                                                | 17.0 us: 1.03x slower                                               |
| dulwich_log             | 35.3 ms                                                | 36.7 ms: 1.04x slower                                               |
| pycparser               | 877 ms                                                 | 912 ms: 1.04x slower                                                |
| logging_simple          | 4.45 us                                                | 4.63 us: 1.04x slower                                               |
| telco                   | 3.49 ms                                                | 3.64 ms: 1.04x slower                                               |
| unpickle_pure_python    | 194 us                                                 | 203 us: 1.04x slower                                                |
| float                   | 69.0 ms                                                | 72.1 ms: 1.04x slower                                               |
| genshi_text             | 17.3 ms                                                | 18.2 ms: 1.05x slower                                               |
| deltablue               | 4.91 ms                                                | 5.15 ms: 1.05x slower                                               |
| richards                | 48.7 ms                                                | 51.0 ms: 1.05x slower                                               |
| fannkuch                | 303 ms                                                 | 318 ms: 1.05x slower                                                |
| pyflate                 | 427 ms                                                 | 453 ms: 1.06x slower                                                |
| scimark_lu              | 103 ms                                                 | 110 ms: 1.07x slower                                                |
| regex_v8                | 17.1 ms                                                | 18.3 ms: 1.07x slower                                               |
| nqueens                 | 63.8 ms                                                | 68.1 ms: 1.07x slower                                               |
| sqlglot_transpile       | 1.44 ms                                                | 1.55 ms: 1.07x slower                                               |
| regex_effbot            | 2.46 ms                                                | 2.64 ms: 1.07x slower                                               |
| sqlglot_parse           | 1.24 ms                                                | 1.33 ms: 1.07x slower                                               |
| tornado_http            | 86.7 ms                                                | 93.5 ms: 1.08x slower                                               |
| mako                    | 9.87 ms                                                | 10.7 ms: 1.08x slower                                               |
| pickle_list             | 2.74 us                                                | 2.96 us: 1.08x slower                                               |
| crypto_pyaes            | 71.8 ms                                                | 77.9 ms: 1.08x slower                                               |
| pickle                  | 6.97 us                                                | 7.56 us: 1.08x slower                                               |
| raytrace                | 301 ms                                                 | 327 ms: 1.09x slower                                                |
| pylint                  | 277 ms                                                 | 300 ms: 1.09x slower                                                |
| bench_mp_pool           | 37.4 ms                                                | 40.8 ms: 1.09x slower                                               |
| go                      | 151 ms                                                 | 165 ms: 1.10x slower                                                |
| scimark_monte_carlo     | 65.6 ms                                                | 72.0 ms: 1.10x slower                                               |
| html5lib                | 42.4 ms                                                | 46.5 ms: 1.10x slower                                               |
| genshi_xml              | 33.8 ms                                                | 37.3 ms: 1.10x slower                                               |
| pickle_dict             | 17.0 us                                                | 18.8 us: 1.11x slower                                               |
| unpickle                | 8.80 us                                                | 9.87 us: 1.12x slower                                               |
| 2to3                    | 192 ms                                                 | 223 ms: 1.16x slower                                                |
| Geometric mean          | (ref)                                                  | 1.02x slower                                                        |

Benchmark hidden because not significant (4): async_generators, generators, logging_silent, async_tree_none
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, comprehensions, create_gc_cycles, dask, gc_traversal, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (1) of results/bm-20221206-3.10.9-1dd9be6/bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6.json: mypy


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 0.97x