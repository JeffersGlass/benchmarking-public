
# Results vs. 3.10.4

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: 9471106
- commit date: 2022-01-13
- overall geometric mean: 1.31x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.23x faster
- Memory change: 1.08x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220113-linux-x86_64-python-main-3.11.0a4-9471106 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| 2to3           | 348 ms                                                 | 264 ms: 1.32x faster                                  |
| chameleon      | 9.68 ms                                                | 7.55 ms: 1.28x faster                                 |
| html5lib       | 88.9 ms                                                | 68.1 ms: 1.31x faster                                 |
| tornado_http   | 136 ms                                                 | 107 ms: 1.28x faster                                  |
| Geometric mean | (ref)                                                  | 1.30x faster                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220113-linux-x86_64-python-main-3.11.0a4-9471106 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| nbody          | 154 ms                                                 | 95.1 ms: 1.61x faster                                 |
| float          | 117 ms                                                 | 78.0 ms: 1.50x faster                                 |
| pidigits       | 191 ms                                                 | 194 ms: 1.02x slower                                  |
| Geometric mean | (ref)                                                  | 1.34x faster                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220113-linux-x86_64-python-main-3.11.0a4-9471106 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 138 ms: 1.36x faster                                  |
| regex_effbot   | 3.63 ms                                                | 3.25 ms: 1.12x faster                                 |
| regex_v8       | 27.8 ms                                                | 24.8 ms: 1.12x faster                                 |
| regex_dna      | 227 ms                                                 | 212 ms: 1.07x faster                                  |
| Geometric mean | (ref)                                                  | 1.16x faster                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220113-linux-x86_64-python-main-3.11.0a4-9471106 |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 329 us: 1.47x faster                                  |
| xml_etree_process    | 79.1 ms                                                | 56.9 ms: 1.39x faster                                 |
| unpickle_pure_python | 331 us                                                 | 254 us: 1.30x faster                                  |
| json_loads           | 31.2 us                                                | 25.1 us: 1.24x faster                                 |
| xml_etree_generate   | 99.4 ms                                                | 80.2 ms: 1.24x faster                                 |
| pickle_list          | 5.08 us                                                | 4.37 us: 1.16x faster                                 |
| json_dumps           | 14.2 ms                                                | 12.4 ms: 1.15x faster                                 |
| pickle_dict          | 29.6 us                                                | 26.8 us: 1.10x faster                                 |
| xml_etree_parse      | 168 ms                                                 | 155 ms: 1.09x faster                                  |
| xml_etree_iterparse  | 115 ms                                                 | 107 ms: 1.08x faster                                  |
| pickle               | 10.7 us                                                | 9.95 us: 1.07x faster                                 |
| unpickle             | 14.4 us                                                | 14.3 us: 1.01x faster                                 |
| Geometric mean       | (ref)                                                  | 1.17x faster                                          |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220113-linux-x86_64-python-main-3.11.0a4-9471106 |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 8.07 ms: 1.81x faster                                 |
| python_startup_no_site | 5.93 ms                                                | 5.85 ms: 1.01x faster                                 |
| Geometric mean         | (ref)                                                  | 1.35x faster                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220113-linux-x86_64-python-main-3.11.0a4-9471106 |
|-----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| mako            | 16.3 ms                                                | 11.5 ms: 1.42x faster                                 |
| django_template | 48.2 ms                                                | 35.2 ms: 1.37x faster                                 |
| Geometric mean  | (ref)                                                  | 1.39x faster                                          |

All benchmarks:
===============

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220113-linux-x86_64-python-main-3.11.0a4-9471106 |
|-------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| deltablue               | 7.91 ms                                                | 4.16 ms: 1.90x faster                                 |
| python_startup          | 14.6 ms                                                | 8.07 ms: 1.81x faster                                 |
| scimark_sor             | 220 ms                                                 | 124 ms: 1.77x faster                                  |
| spectral_norm           | 170 ms                                                 | 99.0 ms: 1.72x faster                                 |
| logging_silent          | 190 ns                                                 | 113 ns: 1.67x faster                                  |
| scimark_monte_carlo     | 118 ms                                                 | 72.7 ms: 1.63x faster                                 |
| go                      | 240 ms                                                 | 148 ms: 1.62x faster                                  |
| nbody                   | 154 ms                                                 | 95.1 ms: 1.61x faster                                 |
| pyflate                 | 716 ms                                                 | 444 ms: 1.61x faster                                  |
| chaos                   | 115 ms                                                 | 72.7 ms: 1.59x faster                                 |
| raytrace                | 507 ms                                                 | 320 ms: 1.58x faster                                  |
| hexiom                  | 10.4 ms                                                | 6.63 ms: 1.57x faster                                 |
| scimark_lu              | 176 ms                                                 | 114 ms: 1.55x faster                                  |
| richards                | 79.3 ms                                                | 51.5 ms: 1.54x faster                                 |
| crypto_pyaes            | 128 ms                                                 | 83.8 ms: 1.53x faster                                 |
| float                   | 117 ms                                                 | 78.0 ms: 1.50x faster                                 |
| pickle_pure_python      | 484 us                                                 | 329 us: 1.47x faster                                  |
| mako                    | 16.3 ms                                                | 11.5 ms: 1.42x faster                                 |
| scimark_fft             | 466 ms                                                 | 330 ms: 1.41x faster                                  |
| logging_format          | 9.09 us                                                | 6.51 us: 1.40x faster                                 |
| logging_simple          | 8.30 us                                                | 5.95 us: 1.40x faster                                 |
| xml_etree_process       | 79.1 ms                                                | 56.9 ms: 1.39x faster                                 |
| scimark_sparse_mat_mult | 6.47 ms                                                | 4.69 ms: 1.38x faster                                 |
| django_template         | 48.2 ms                                                | 35.2 ms: 1.37x faster                                 |
| regex_compile           | 188 ms                                                 | 138 ms: 1.36x faster                                  |
| fannkuch                | 532 ms                                                 | 392 ms: 1.36x faster                                  |
| pycparser               | 1.58 sec                                               | 1.17 sec: 1.35x faster                                |
| unpack_sequence         | 60.0 ns                                                | 44.8 ns: 1.34x faster                                 |
| 2to3                    | 348 ms                                                 | 264 ms: 1.32x faster                                  |
| thrift                  | 1.07 ms                                                | 812 us: 1.32x faster                                  |
| html5lib                | 88.9 ms                                                | 68.1 ms: 1.31x faster                                 |
| unpickle_pure_python    | 331 us                                                 | 254 us: 1.30x faster                                  |
| chameleon               | 9.68 ms                                                | 7.55 ms: 1.28x faster                                 |
| dulwich_log             | 84.3 ms                                                | 65.8 ms: 1.28x faster                                 |
| tornado_http            | 136 ms                                                 | 107 ms: 1.28x faster                                  |
| nqueens                 | 106 ms                                                 | 84.0 ms: 1.26x faster                                 |
| json_loads              | 31.2 us                                                | 25.1 us: 1.24x faster                                 |
| xml_etree_generate      | 99.4 ms                                                | 80.2 ms: 1.24x faster                                 |
| sympy_integrate         | 25.8 ms                                                | 21.4 ms: 1.21x faster                                 |
| json                    | 5.69 ms                                                | 4.74 ms: 1.20x faster                                 |
| meteor_contest          | 120 ms                                                 | 103 ms: 1.16x faster                                  |
| pickle_list             | 5.08 us                                                | 4.37 us: 1.16x faster                                 |
| sympy_sum               | 196 ms                                                 | 170 ms: 1.16x faster                                  |
| json_dumps              | 14.2 ms                                                | 12.4 ms: 1.15x faster                                 |
| sympy_str               | 346 ms                                                 | 302 ms: 1.15x faster                                  |
| regex_effbot            | 3.63 ms                                                | 3.25 ms: 1.12x faster                                 |
| regex_v8                | 27.8 ms                                                | 24.8 ms: 1.12x faster                                 |
| sympy_expand            | 566 ms                                                 | 506 ms: 1.12x faster                                  |
| sqlite_synth            | 3.02 us                                                | 2.73 us: 1.11x faster                                 |
| pickle_dict             | 29.6 us                                                | 26.8 us: 1.10x faster                                 |
| xml_etree_parse         | 168 ms                                                 | 155 ms: 1.09x faster                                  |
| telco                   | 7.27 ms                                                | 6.69 ms: 1.09x faster                                 |
| xml_etree_iterparse     | 115 ms                                                 | 107 ms: 1.08x faster                                  |
| pickle                  | 10.7 us                                                | 9.95 us: 1.07x faster                                 |
| pathlib                 | 20.5 ms                                                | 19.1 ms: 1.07x faster                                 |
| regex_dna               | 227 ms                                                 | 212 ms: 1.07x faster                                  |
| python_startup_no_site  | 5.93 ms                                                | 5.85 ms: 1.01x faster                                 |
| unpickle                | 14.4 us                                                | 14.3 us: 1.01x faster                                 |
| pidigits                | 191 ms                                                 | 194 ms: 1.02x slower                                  |
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