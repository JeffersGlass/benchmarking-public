
# Results vs. 3.11.0

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: c4e4b91
- commit date: 2022-02-03
- overall geometric mean: 1.00x faster \*
- HPT reliability: 81.74%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220203-linux-x86_64-python-main-3.11.0a5-c4e4b91 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| 2to3           | 264 ms                                                 | 267 ms: 1.01x slower                                  |
| chameleon      | 6.70 ms                                                | 6.95 ms: 1.04x slower                                 |
| html5lib       | 64.8 ms                                                | 67.9 ms: 1.05x slower                                 |
| tornado_http   | 98.1 ms                                                | 106 ms: 1.08x slower                                  |
| Geometric mean | (ref)                                                  | 1.04x slower                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220203-linux-x86_64-python-main-3.11.0a5-c4e4b91 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pidigits       | 194 ms                                                 | 190 ms: 1.02x faster                                  |
| float          | 78.9 ms                                                | 77.5 ms: 1.02x faster                                 |
| nbody          | 96.0 ms                                                | 94.7 ms: 1.01x faster                                 |
| Geometric mean | (ref)                                                  | 1.02x faster                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220203-linux-x86_64-python-main-3.11.0a5-c4e4b91 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.14 ms: 1.12x faster                                 |
| regex_compile  | 141 ms                                                 | 140 ms: 1.01x faster                                  |
| regex_dna      | 205 ms                                                 | 213 ms: 1.04x slower                                  |
| regex_v8       | 22.9 ms                                                | 24.0 ms: 1.05x slower                                 |
| Geometric mean | (ref)                                                  | 1.01x faster                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220203-linux-x86_64-python-main-3.11.0a5-c4e4b91 |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pickle_dict          | 34.6 us                                                | 28.1 us: 1.23x faster                                 |
| pickle               | 11.0 us                                                | 9.93 us: 1.11x faster                                 |
| json_loads           | 29.2 us                                                | 26.7 us: 1.09x faster                                 |
| json_dumps           | 13.3 ms                                                | 12.2 ms: 1.09x faster                                 |
| xml_etree_parse      | 164 ms                                                 | 153 ms: 1.07x faster                                  |
| unpickle             | 13.8 us                                                | 13.4 us: 1.03x faster                                 |
| pickle_list          | 4.59 us                                                | 4.47 us: 1.03x faster                                 |
| xml_etree_generate   | 81.1 ms                                                | 79.6 ms: 1.02x faster                                 |
| xml_etree_iterparse  | 108 ms                                                 | 106 ms: 1.02x faster                                  |
| unpickle_pure_python | 242 us                                                 | 249 us: 1.03x slower                                  |
| pickle_pure_python   | 320 us                                                 | 334 us: 1.04x slower                                  |
| Geometric mean       | (ref)                                                  | 1.04x faster                                          |

Benchmark hidden because not significant (2): xml_etree_process, unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220203-linux-x86_64-python-main-3.11.0a5-c4e4b91 |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 8.13 ms: 1.05x faster                                 |
| python_startup_no_site | 6.01 ms                                                | 5.92 ms: 1.02x faster                                 |
| Geometric mean         | (ref)                                                  | 1.03x faster                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220203-linux-x86_64-python-main-3.11.0a5-c4e4b91 |
|-----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| mako            | 10.7 ms                                                | 10.5 ms: 1.02x faster                                 |
| django_template | 33.5 ms                                                | 35.4 ms: 1.05x slower                                 |
| Geometric mean  | (ref)                                                  | 1.02x slower                                          |

All benchmarks:
===============

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220203-linux-x86_64-python-main-3.11.0a5-c4e4b91 |
|-------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pickle_dict             | 34.6 us                                                | 28.1 us: 1.23x faster                                 |
| regex_effbot            | 3.51 ms                                                | 3.14 ms: 1.12x faster                                 |
| pickle                  | 11.0 us                                                | 9.93 us: 1.11x faster                                 |
| json_loads              | 29.2 us                                                | 26.7 us: 1.09x faster                                 |
| json_dumps              | 13.3 ms                                                | 12.2 ms: 1.09x faster                                 |
| json                    | 5.24 ms                                                | 4.84 ms: 1.08x faster                                 |
| xml_etree_parse         | 164 ms                                                 | 153 ms: 1.07x faster                                  |
| logging_format          | 6.81 us                                                | 6.37 us: 1.07x faster                                 |
| logging_simple          | 6.22 us                                                | 5.84 us: 1.07x faster                                 |
| python_startup          | 8.56 ms                                                | 8.13 ms: 1.05x faster                                 |
| meteor_contest          | 109 ms                                                 | 105 ms: 1.04x faster                                  |
| spectral_norm           | 108 ms                                                 | 104 ms: 1.04x faster                                  |
| unpickle                | 13.8 us                                                | 13.4 us: 1.03x faster                                 |
| pickle_list             | 4.59 us                                                | 4.47 us: 1.03x faster                                 |
| telco                   | 6.86 ms                                                | 6.70 ms: 1.02x faster                                 |
| pidigits                | 194 ms                                                 | 190 ms: 1.02x faster                                  |
| hexiom                  | 6.89 ms                                                | 6.76 ms: 1.02x faster                                 |
| xml_etree_generate      | 81.1 ms                                                | 79.6 ms: 1.02x faster                                 |
| float                   | 78.9 ms                                                | 77.5 ms: 1.02x faster                                 |
| mako                    | 10.7 ms                                                | 10.5 ms: 1.02x faster                                 |
| xml_etree_iterparse     | 108 ms                                                 | 106 ms: 1.02x faster                                  |
| python_startup_no_site  | 6.01 ms                                                | 5.92 ms: 1.02x faster                                 |
| nbody                   | 96.0 ms                                                | 94.7 ms: 1.01x faster                                 |
| fannkuch                | 405 ms                                                 | 400 ms: 1.01x faster                                  |
| sympy_integrate         | 21.5 ms                                                | 21.3 ms: 1.01x faster                                 |
| nqueens                 | 87.9 ms                                                | 87.2 ms: 1.01x faster                                 |
| regex_compile           | 141 ms                                                 | 140 ms: 1.01x faster                                  |
| go                      | 149 ms                                                 | 147 ms: 1.01x faster                                  |
| scimark_fft             | 345 ms                                                 | 347 ms: 1.00x slower                                  |
| sympy_sum               | 169 ms                                                 | 170 ms: 1.01x slower                                  |
| 2to3                    | 264 ms                                                 | 267 ms: 1.01x slower                                  |
| logging_silent          | 111 ns                                                 | 113 ns: 1.02x slower                                  |
| dulwich_log             | 64.6 ms                                                | 65.7 ms: 1.02x slower                                 |
| richards                | 49.8 ms                                                | 50.8 ms: 1.02x slower                                 |
| scimark_sparse_mat_mult | 5.03 ms                                                | 5.14 ms: 1.02x slower                                 |
| sympy_str               | 297 ms                                                 | 304 ms: 1.02x slower                                  |
| scimark_monte_carlo     | 70.7 ms                                                | 72.6 ms: 1.03x slower                                 |
| unpickle_pure_python    | 242 us                                                 | 249 us: 1.03x slower                                  |
| scimark_lu              | 116 ms                                                 | 120 ms: 1.03x slower                                  |
| chameleon               | 6.70 ms                                                | 6.95 ms: 1.04x slower                                 |
| sympy_expand            | 484 ms                                                 | 503 ms: 1.04x slower                                  |
| raytrace                | 309 ms                                                 | 321 ms: 1.04x slower                                  |
| regex_dna               | 205 ms                                                 | 213 ms: 1.04x slower                                  |
| thrift                  | 784 us                                                 | 815 us: 1.04x slower                                  |
| chaos                   | 71.9 ms                                                | 74.9 ms: 1.04x slower                                 |
| pickle_pure_python      | 320 us                                                 | 334 us: 1.04x slower                                  |
| html5lib                | 64.8 ms                                                | 67.9 ms: 1.05x slower                                 |
| regex_v8                | 22.9 ms                                                | 24.0 ms: 1.05x slower                                 |
| sqlite_synth            | 2.57 us                                                | 2.71 us: 1.05x slower                                 |
| deltablue               | 3.92 ms                                                | 4.13 ms: 1.05x slower                                 |
| django_template         | 33.5 ms                                                | 35.4 ms: 1.05x slower                                 |
| pyflate                 | 434 ms                                                 | 459 ms: 1.06x slower                                  |
| unpack_sequence         | 43.5 ns                                                | 46.0 ns: 1.06x slower                                 |
| scimark_sor             | 121 ms                                                 | 129 ms: 1.06x slower                                  |
| tornado_http            | 98.1 ms                                                | 106 ms: 1.08x slower                                  |
| crypto_pyaes            | 76.7 ms                                                | 83.8 ms: 1.09x slower                                 |
| Geometric mean          | (ref)                                                  | 1.00x faster                                          |

Benchmark hidden because not significant (4): pathlib, xml_etree_process, pycparser, unpickle_list
Ignored benchmarks (45) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_generators, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_io, async_tree_io_tg, async_tree_memoization, async_tree_memoization_tg, async_tree_none, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, bench_mp_pool, bench_thread_pool, comprehensions, coroutines, coverage, create_gc_cycles, dask, deepcopy, deepcopy_memo, deepcopy_reduce, djangocms, docutils, flaskblogging, gc_traversal, generators, genshi_text, genshi_xml, gunicorn, mdp, mypy2, pprint_pformat, pprint_safe_repr, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, sqlglot_normalize, sqlglot_optimize, sqlglot_parse, sqlglot_transpile, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 81.74% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x