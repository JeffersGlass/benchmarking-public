
# Results vs. 3.10.4

- fork: python
- ref: f9774e57d84162ff0cba
- machine: darwin-arm64
- commit hash: f9774e5
- commit date: 2023-03-07
- overall geometric mean: 1.16x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.13x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 165 ms: 1.16x faster                                                  |
| chameleon      | 6.26 ms                                                | 4.48 ms: 1.40x faster                                                 |
| docutils       | 1.73 sec                                               | 1.49 sec: 1.16x faster                                                |
| html5lib       | 42.4 ms                                                | 35.4 ms: 1.20x faster                                                 |
| tornado_http   | 86.7 ms                                                | 70.0 ms: 1.24x faster                                                 |
| Geometric mean | (ref)                                                  | 1.23x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_memoization  | 474 ms                                                 | 336 ms: 1.41x faster                                                  |
| async_tree_none         | 388 ms                                                 | 289 ms: 1.34x faster                                                  |
| async_tree_io           | 980 ms                                                 | 744 ms: 1.32x faster                                                  |
| async_tree_cpu_io_mixed | 649 ms                                                 | 547 ms: 1.19x faster                                                  |
| Geometric mean          | (ref)                                                  | 1.31x faster                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 66.1 ms: 1.41x faster                                                 |
| float          | 69.0 ms                                                | 53.5 ms: 1.29x faster                                                 |
| pidigits       | 282 ms                                                 | 281 ms: 1.00x faster                                                  |
| Geometric mean | (ref)                                                  | 1.22x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 75.4 ms: 1.26x faster                                                 |
| regex_dna      | 174 ms                                                 | 153 ms: 1.14x faster                                                  |
| regex_v8       | 17.1 ms                                                | 16.2 ms: 1.06x faster                                                 |
| regex_effbot   | 2.46 ms                                                | 2.69 ms: 1.10x slower                                                 |
| Geometric mean | (ref)                                                  | 1.09x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 191 us: 1.47x faster                                                  |
| unpickle_pure_python | 194 us                                                 | 145 us: 1.34x faster                                                  |
| json_dumps           | 8.11 ms                                                | 6.18 ms: 1.31x faster                                                 |
| xml_etree_process    | 46.5 ms                                                | 37.0 ms: 1.26x faster                                                 |
| xml_etree_parse      | 108 ms                                                 | 97.9 ms: 1.10x faster                                                 |
| xml_etree_generate   | 53.5 ms                                                | 51.1 ms: 1.05x faster                                                 |
| json_loads           | 16.4 us                                                | 16.1 us: 1.02x faster                                                 |
| unpickle_list        | 2.69 us                                                | 2.65 us: 1.02x faster                                                 |
| xml_etree_iterparse  | 72.1 ms                                                | 71.1 ms: 1.01x faster                                                 |
| pickle_list          | 2.74 us                                                | 2.83 us: 1.03x slower                                                 |
| pickle_dict          | 17.0 us                                                | 18.0 us: 1.06x slower                                                 |
| pickle               | 6.97 us                                                | 7.47 us: 1.07x slower                                                 |
| unpickle             | 8.80 us                                                | 9.71 us: 1.10x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.09x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 12.5 ms: 1.15x slower                                                 |
| python_startup_no_site | 7.91 ms                                                | 10.4 ms: 1.31x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.23x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 9.87 ms                                                | 7.44 ms: 1.33x faster                                                 |
| django_template | 26.4 ms                                                | 21.6 ms: 1.22x faster                                                 |
| genshi_text     | 17.3 ms                                                | 14.7 ms: 1.18x faster                                                 |
| genshi_xml      | 33.8 ms                                                | 29.2 ms: 1.16x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.22x faster                                                          |

All benchmarks:
===============

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| deltablue               | 4.91 ms                                                | 2.59 ms: 1.90x faster                                                 |
| logging_silent          | 117 ns                                                 | 69.3 ns: 1.69x faster                                                 |
| richards                | 48.7 ms                                                | 30.5 ms: 1.60x faster                                                 |
| pickle_pure_python      | 281 us                                                 | 191 us: 1.47x faster                                                  |
| scimark_sor             | 128 ms                                                 | 87.7 ms: 1.46x faster                                                 |
| async_tree_memoization  | 474 ms                                                 | 336 ms: 1.41x faster                                                  |
| nbody                   | 93.0 ms                                                | 66.1 ms: 1.41x faster                                                 |
| chameleon               | 6.26 ms                                                | 4.48 ms: 1.40x faster                                                 |
| asyncio_tcp             | 659 ms                                                 | 473 ms: 1.39x faster                                                  |
| hexiom                  | 6.19 ms                                                | 4.46 ms: 1.39x faster                                                 |
| scimark_lu              | 103 ms                                                 | 74.2 ms: 1.39x faster                                                 |
| chaos                   | 65.8 ms                                                | 47.8 ms: 1.38x faster                                                 |
| go                      | 151 ms                                                 | 111 ms: 1.36x faster                                                  |
| pprint_pformat          | 1.30 sec                                               | 970 ms: 1.34x faster                                                  |
| pprint_safe_repr        | 641 ms                                                 | 477 ms: 1.34x faster                                                  |
| async_tree_none         | 388 ms                                                 | 289 ms: 1.34x faster                                                  |
| crypto_pyaes            | 71.8 ms                                                | 53.5 ms: 1.34x faster                                                 |
| unpickle_pure_python    | 194 us                                                 | 145 us: 1.34x faster                                                  |
| mako                    | 9.87 ms                                                | 7.44 ms: 1.33x faster                                                 |
| raytrace                | 301 ms                                                 | 229 ms: 1.32x faster                                                  |
| async_tree_io           | 980 ms                                                 | 744 ms: 1.32x faster                                                  |
| deepcopy_memo           | 34.7 us                                                | 26.4 us: 1.31x faster                                                 |
| json_dumps              | 8.11 ms                                                | 6.18 ms: 1.31x faster                                                 |
| pycparser               | 877 ms                                                 | 674 ms: 1.30x faster                                                  |
| float                   | 69.0 ms                                                | 53.5 ms: 1.29x faster                                                 |
| pyflate                 | 427 ms                                                 | 331 ms: 1.29x faster                                                  |
| scimark_monte_carlo     | 65.6 ms                                                | 51.0 ms: 1.29x faster                                                 |
| spectral_norm           | 94.8 ms                                                | 74.9 ms: 1.27x faster                                                 |
| thrift                  | 572 us                                                 | 453 us: 1.26x faster                                                  |
| regex_compile           | 95.3 ms                                                | 75.4 ms: 1.26x faster                                                 |
| xml_etree_process       | 46.5 ms                                                | 37.0 ms: 1.26x faster                                                 |
| tornado_http            | 86.7 ms                                                | 70.0 ms: 1.24x faster                                                 |
| sqlalchemy_imperative   | 8.86 ms                                                | 7.21 ms: 1.23x faster                                                 |
| create_gc_cycles        | 860 us                                                 | 702 us: 1.22x faster                                                  |
| deepcopy                | 272 us                                                 | 222 us: 1.22x faster                                                  |
| logging_format          | 4.83 us                                                | 3.95 us: 1.22x faster                                                 |
| django_template         | 26.4 ms                                                | 21.6 ms: 1.22x faster                                                 |
| logging_simple          | 4.45 us                                                | 3.66 us: 1.22x faster                                                 |
| html5lib                | 42.4 ms                                                | 35.4 ms: 1.20x faster                                                 |
| dulwich_log             | 35.3 ms                                                | 29.6 ms: 1.20x faster                                                 |
| deepcopy_reduce         | 2.33 us                                                | 1.95 us: 1.19x faster                                                 |
| async_tree_cpu_io_mixed | 649 ms                                                 | 547 ms: 1.19x faster                                                  |
| unpack_sequence         | 39.0 ns                                                | 32.9 ns: 1.19x faster                                                 |
| sqlglot_parse           | 1.24 ms                                                | 1.05 ms: 1.19x faster                                                 |
| genshi_text             | 17.3 ms                                                | 14.7 ms: 1.18x faster                                                 |
| sqlglot_transpile       | 1.44 ms                                                | 1.22 ms: 1.18x faster                                                 |
| fannkuch                | 303 ms                                                 | 258 ms: 1.17x faster                                                  |
| 2to3                    | 192 ms                                                 | 165 ms: 1.16x faster                                                  |
| docutils                | 1.73 sec                                               | 1.49 sec: 1.16x faster                                                |
| generators              | 32.3 ms                                                | 27.9 ms: 1.16x faster                                                 |
| genshi_xml              | 33.8 ms                                                | 29.2 ms: 1.16x faster                                                 |
| sqlalchemy_declarative  | 73.3 ms                                                | 63.8 ms: 1.15x faster                                                 |
| scimark_fft             | 224 ms                                                 | 196 ms: 1.15x faster                                                  |
| sqlglot_optimize        | 36.8 ms                                                | 32.1 ms: 1.14x faster                                                 |
| coroutines              | 20.7 ms                                                | 18.1 ms: 1.14x faster                                                 |
| regex_dna               | 174 ms                                                 | 153 ms: 1.14x faster                                                  |
| sympy_integrate         | 13.1 ms                                                | 11.7 ms: 1.13x faster                                                 |
| bench_thread_pool       | 527 us                                                 | 472 us: 1.12x faster                                                  |
| json                    | 3.08 ms                                                | 2.79 ms: 1.11x faster                                                 |
| xml_etree_parse         | 108 ms                                                 | 97.9 ms: 1.10x faster                                                 |
| mdp                     | 1.63 sec                                               | 1.50 sec: 1.09x faster                                                |
| sqlglot_normalize       | 190 ms                                                 | 175 ms: 1.09x faster                                                  |
| sympy_expand            | 269 ms                                                 | 248 ms: 1.08x faster                                                  |
| scimark_sparse_mat_mult | 3.42 ms                                                | 3.17 ms: 1.08x faster                                                 |
| sympy_str               | 165 ms                                                 | 155 ms: 1.07x faster                                                  |
| sqlite_synth            | 1.46 us                                                | 1.37 us: 1.07x faster                                                 |
| meteor_contest          | 77.7 ms                                                | 72.9 ms: 1.07x faster                                                 |
| regex_v8                | 17.1 ms                                                | 16.2 ms: 1.06x faster                                                 |
| xml_etree_generate      | 53.5 ms                                                | 51.1 ms: 1.05x faster                                                 |
| sympy_sum               | 92.2 ms                                                | 88.2 ms: 1.05x faster                                                 |
| json_loads              | 16.4 us                                                | 16.1 us: 1.02x faster                                                 |
| unpickle_list           | 2.69 us                                                | 2.65 us: 1.02x faster                                                 |
| xml_etree_iterparse     | 72.1 ms                                                | 71.1 ms: 1.01x faster                                                 |
| nqueens                 | 63.8 ms                                                | 63.1 ms: 1.01x faster                                                 |
| pidigits                | 282 ms                                                 | 281 ms: 1.00x faster                                                  |
| gc_traversal            | 2.36 ms                                                | 2.43 ms: 1.03x slower                                                 |
| pickle_list             | 2.74 us                                                | 2.83 us: 1.03x slower                                                 |
| comprehensions          | 16.9 us                                                | 17.7 us: 1.04x slower                                                 |
| pickle_dict             | 17.0 us                                                | 18.0 us: 1.06x slower                                                 |
| pickle                  | 6.97 us                                                | 7.47 us: 1.07x slower                                                 |
| regex_effbot            | 2.46 ms                                                | 2.69 ms: 1.10x slower                                                 |
| unpickle                | 8.80 us                                                | 9.71 us: 1.10x slower                                                 |
| pathlib                 | 24.5 ms                                                | 27.5 ms: 1.12x slower                                                 |
| python_startup          | 10.9 ms                                                | 12.5 ms: 1.15x slower                                                 |
| async_generators        | 231 ms                                                 | 272 ms: 1.17x slower                                                  |
| bench_mp_pool           | 37.4 ms                                                | 46.5 ms: 1.24x slower                                                 |
| dask                    | 253 ms                                                 | 325 ms: 1.28x slower                                                  |
| python_startup_no_site  | 7.91 ms                                                | 10.4 ms: 1.31x slower                                                 |
| coverage                | 41.5 ms                                                | 59.6 ms: 1.44x slower                                                 |
| Geometric mean          | (ref)                                                  | 1.16x faster                                                          |

Benchmark hidden because not significant (1): telco
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, gunicorn, mypy2, pylint, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.15x
- 95% likely to have a speedup of 1.14x
- 99% likely to have a speedup of 1.13x


# Memory

- memory change: 1.10x