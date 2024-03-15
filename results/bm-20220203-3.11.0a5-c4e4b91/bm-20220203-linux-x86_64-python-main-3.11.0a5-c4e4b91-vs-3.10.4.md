
# Results vs. 3.10.4

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: c4e4b91
- commit date: 2022-02-03
- overall geometric mean: 1.31x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.23x faster
- Memory change: 1.08x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220203-linux-x86_64-python-main-3.11.0a5-c4e4b91 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| 2to3           | 348 ms                                                 | 267 ms: 1.31x faster                                  |
| chameleon      | 9.68 ms                                                | 6.95 ms: 1.39x faster                                 |
| html5lib       | 88.9 ms                                                | 67.9 ms: 1.31x faster                                 |
| tornado_http   | 136 ms                                                 | 106 ms: 1.29x faster                                  |
| Geometric mean | (ref)                                                  | 1.32x faster                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220203-linux-x86_64-python-main-3.11.0a5-c4e4b91 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| nbody          | 154 ms                                                 | 94.7 ms: 1.62x faster                                 |
| float          | 117 ms                                                 | 77.5 ms: 1.51x faster                                 |
| pidigits       | 191 ms                                                 | 190 ms: 1.01x faster                                  |
| Geometric mean | (ref)                                                  | 1.35x faster                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220203-linux-x86_64-python-main-3.11.0a5-c4e4b91 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 140 ms: 1.34x faster                                  |
| regex_v8       | 27.8 ms                                                | 24.0 ms: 1.16x faster                                 |
| regex_effbot   | 3.63 ms                                                | 3.14 ms: 1.15x faster                                 |
| regex_dna      | 227 ms                                                 | 213 ms: 1.07x faster                                  |
| Geometric mean | (ref)                                                  | 1.18x faster                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220203-linux-x86_64-python-main-3.11.0a5-c4e4b91 |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 334 us: 1.45x faster                                  |
| xml_etree_process    | 79.1 ms                                                | 57.0 ms: 1.39x faster                                 |
| unpickle_pure_python | 331 us                                                 | 249 us: 1.33x faster                                  |
| xml_etree_generate   | 99.4 ms                                                | 79.6 ms: 1.25x faster                                 |
| json_loads           | 31.2 us                                                | 26.7 us: 1.17x faster                                 |
| json_dumps           | 14.2 ms                                                | 12.2 ms: 1.16x faster                                 |
| pickle_list          | 5.08 us                                                | 4.47 us: 1.14x faster                                 |
| xml_etree_parse      | 168 ms                                                 | 153 ms: 1.10x faster                                  |
| xml_etree_iterparse  | 115 ms                                                 | 106 ms: 1.09x faster                                  |
| pickle               | 10.7 us                                                | 9.93 us: 1.07x faster                                 |
| unpickle             | 14.4 us                                                | 13.4 us: 1.07x faster                                 |
| pickle_dict          | 29.6 us                                                | 28.1 us: 1.05x faster                                 |
| Geometric mean       | (ref)                                                  | 1.17x faster                                          |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220203-linux-x86_64-python-main-3.11.0a5-c4e4b91 |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 8.13 ms: 1.79x faster                                 |
| python_startup_no_site | 5.93 ms                                                | 5.92 ms: 1.00x faster                                 |
| Geometric mean         | (ref)                                                  | 1.34x faster                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220203-linux-x86_64-python-main-3.11.0a5-c4e4b91 |
|-----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| mako            | 16.3 ms                                                | 10.5 ms: 1.56x faster                                 |
| django_template | 48.2 ms                                                | 35.4 ms: 1.36x faster                                 |
| Geometric mean  | (ref)                                                  | 1.46x faster                                          |

All benchmarks:
===============

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220203-linux-x86_64-python-main-3.11.0a5-c4e4b91 |
|-------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| deltablue               | 7.91 ms                                                | 4.13 ms: 1.91x faster                                 |
| python_startup          | 14.6 ms                                                | 8.13 ms: 1.79x faster                                 |
| scimark_sor             | 220 ms                                                 | 129 ms: 1.70x faster                                  |
| logging_silent          | 190 ns                                                 | 113 ns: 1.68x faster                                  |
| scimark_monte_carlo     | 118 ms                                                 | 72.6 ms: 1.63x faster                                 |
| spectral_norm           | 170 ms                                                 | 104 ms: 1.63x faster                                  |
| go                      | 240 ms                                                 | 147 ms: 1.63x faster                                  |
| nbody                   | 154 ms                                                 | 94.7 ms: 1.62x faster                                 |
| raytrace                | 507 ms                                                 | 321 ms: 1.58x faster                                  |
| richards                | 79.3 ms                                                | 50.8 ms: 1.56x faster                                 |
| pyflate                 | 716 ms                                                 | 459 ms: 1.56x faster                                  |
| mako                    | 16.3 ms                                                | 10.5 ms: 1.56x faster                                 |
| chaos                   | 115 ms                                                 | 74.9 ms: 1.54x faster                                 |
| hexiom                  | 10.4 ms                                                | 6.76 ms: 1.54x faster                                 |
| crypto_pyaes            | 128 ms                                                 | 83.8 ms: 1.52x faster                                 |
| float                   | 117 ms                                                 | 77.5 ms: 1.51x faster                                 |
| scimark_lu              | 176 ms                                                 | 120 ms: 1.47x faster                                  |
| pickle_pure_python      | 484 us                                                 | 334 us: 1.45x faster                                  |
| logging_format          | 9.09 us                                                | 6.37 us: 1.43x faster                                 |
| logging_simple          | 8.30 us                                                | 5.84 us: 1.42x faster                                 |
| chameleon               | 9.68 ms                                                | 6.95 ms: 1.39x faster                                 |
| xml_etree_process       | 79.1 ms                                                | 57.0 ms: 1.39x faster                                 |
| django_template         | 48.2 ms                                                | 35.4 ms: 1.36x faster                                 |
| regex_compile           | 188 ms                                                 | 140 ms: 1.34x faster                                  |
| scimark_fft             | 466 ms                                                 | 347 ms: 1.34x faster                                  |
| fannkuch                | 532 ms                                                 | 400 ms: 1.33x faster                                  |
| unpickle_pure_python    | 331 us                                                 | 249 us: 1.33x faster                                  |
| pycparser               | 1.58 sec                                               | 1.19 sec: 1.32x faster                                |
| thrift                  | 1.07 ms                                                | 815 us: 1.31x faster                                  |
| html5lib                | 88.9 ms                                                | 67.9 ms: 1.31x faster                                 |
| 2to3                    | 348 ms                                                 | 267 ms: 1.31x faster                                  |
| unpack_sequence         | 60.0 ns                                                | 46.0 ns: 1.30x faster                                 |
| tornado_http            | 136 ms                                                 | 106 ms: 1.29x faster                                  |
| dulwich_log             | 84.3 ms                                                | 65.7 ms: 1.28x faster                                 |
| scimark_sparse_mat_mult | 6.47 ms                                                | 5.14 ms: 1.26x faster                                 |
| xml_etree_generate      | 99.4 ms                                                | 79.6 ms: 1.25x faster                                 |
| nqueens                 | 106 ms                                                 | 87.2 ms: 1.21x faster                                 |
| sympy_integrate         | 25.8 ms                                                | 21.3 ms: 1.21x faster                                 |
| json                    | 5.69 ms                                                | 4.84 ms: 1.17x faster                                 |
| json_loads              | 31.2 us                                                | 26.7 us: 1.17x faster                                 |
| json_dumps              | 14.2 ms                                                | 12.2 ms: 1.16x faster                                 |
| sympy_sum               | 196 ms                                                 | 170 ms: 1.16x faster                                  |
| regex_v8                | 27.8 ms                                                | 24.0 ms: 1.16x faster                                 |
| regex_effbot            | 3.63 ms                                                | 3.14 ms: 1.15x faster                                 |
| meteor_contest          | 120 ms                                                 | 105 ms: 1.14x faster                                  |
| sympy_str               | 346 ms                                                 | 304 ms: 1.14x faster                                  |
| pickle_list             | 5.08 us                                                | 4.47 us: 1.14x faster                                 |
| sympy_expand            | 566 ms                                                 | 503 ms: 1.12x faster                                  |
| sqlite_synth            | 3.02 us                                                | 2.71 us: 1.12x faster                                 |
| pathlib                 | 20.5 ms                                                | 18.5 ms: 1.11x faster                                 |
| xml_etree_parse         | 168 ms                                                 | 153 ms: 1.10x faster                                  |
| xml_etree_iterparse     | 115 ms                                                 | 106 ms: 1.09x faster                                  |
| telco                   | 7.27 ms                                                | 6.70 ms: 1.08x faster                                 |
| pickle                  | 10.7 us                                                | 9.93 us: 1.07x faster                                 |
| unpickle                | 14.4 us                                                | 13.4 us: 1.07x faster                                 |
| regex_dna               | 227 ms                                                 | 213 ms: 1.07x faster                                  |
| pickle_dict             | 29.6 us                                                | 28.1 us: 1.05x faster                                 |
| pidigits                | 191 ms                                                 | 190 ms: 1.01x faster                                  |
| python_startup_no_site  | 5.93 ms                                                | 5.92 ms: 1.00x faster                                 |
| Geometric mean          | (ref)                                                  | 1.31x faster                                          |

Benchmark hidden because not significant (1): unpickle_list
Ignored benchmarks (41) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, async_generators, async_tree_cpu_io_mixed, async_tree_io, async_tree_memoization, async_tree_none, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, bench_mp_pool, bench_thread_pool, comprehensions, coroutines, coverage, create_gc_cycles, dask, deepcopy, deepcopy_memo, deepcopy_reduce, djangocms, docutils, flaskblogging, gc_traversal, generators, genshi_text, genshi_xml, gunicorn, mdp, mypy2, pprint_pformat, pprint_safe_repr, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, sqlglot_normalize, sqlglot_optimize, sqlglot_parse, sqlglot_transpile, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.29x
- 95% likely to have a speedup of 1.28x
- 99% likely to have a speedup of 1.23x


# Memory

- memory change: 1.08x