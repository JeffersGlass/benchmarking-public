
# Results vs. 3.11.0

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: 2e49bd0
- commit date: 2022-04-05
- overall geometric mean: 1.02x faster \*
- HPT reliability: 99.98%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.97x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220405-linux-x86_64-python-main-3.11.0a7-2e49bd0 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| chameleon      | 6.70 ms                                                | 6.87 ms: 1.03x slower                                 |
| tornado_http   | 98.1 ms                                                | 95.4 ms: 1.03x faster                                 |
| Geometric mean | (ref)                                                  | 1.00x slower                                          |

Benchmark hidden because not significant (2): 2to3, html5lib

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220405-linux-x86_64-python-main-3.11.0a7-2e49bd0 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| float          | 78.9 ms                                                | 74.4 ms: 1.06x faster                                 |
| nbody          | 96.0 ms                                                | 95.2 ms: 1.01x faster                                 |
| pidigits       | 194 ms                                                 | 197 ms: 1.01x slower                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220405-linux-x86_64-python-main-3.11.0a7-2e49bd0 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.34 ms: 1.05x faster                                 |
| regex_compile  | 141 ms                                                 | 137 ms: 1.03x faster                                  |
| regex_dna      | 205 ms                                                 | 231 ms: 1.13x slower                                  |
| regex_v8       | 22.9 ms                                                | 25.9 ms: 1.13x slower                                 |
| Geometric mean | (ref)                                                  | 1.04x slower                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220405-linux-x86_64-python-main-3.11.0a7-2e49bd0 |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pickle_dict          | 34.6 us                                                | 27.6 us: 1.25x faster                                 |
| pickle               | 11.0 us                                                | 9.55 us: 1.15x faster                                 |
| json_dumps           | 13.3 ms                                                | 12.5 ms: 1.07x faster                                 |
| unpickle_list        | 5.21 us                                                | 4.97 us: 1.05x faster                                 |
| unpickle_pure_python | 242 us                                                 | 231 us: 1.05x faster                                  |
| xml_etree_parse      | 164 ms                                                 | 157 ms: 1.05x faster                                  |
| xml_etree_iterparse  | 108 ms                                                 | 104 ms: 1.04x faster                                  |
| json_loads           | 29.2 us                                                | 28.1 us: 1.04x faster                                 |
| xml_etree_generate   | 81.1 ms                                                | 78.5 ms: 1.03x faster                                 |
| xml_etree_process    | 56.9 ms                                                | 55.2 ms: 1.03x faster                                 |
| pickle_pure_python   | 320 us                                                 | 311 us: 1.03x faster                                  |
| pickle_list          | 4.59 us                                                | 4.57 us: 1.00x faster                                 |
| Geometric mean       | (ref)                                                  | 1.06x faster                                          |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220405-linux-x86_64-python-main-3.11.0a7-2e49bd0 |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 8.07 ms: 1.06x faster                                 |
| python_startup_no_site | 6.01 ms                                                | 5.98 ms: 1.00x faster                                 |
| Geometric mean         | (ref)                                                  | 1.03x faster                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220405-linux-x86_64-python-main-3.11.0a7-2e49bd0 |
|-----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| mako            | 10.7 ms                                                | 10.2 ms: 1.05x faster                                 |
| django_template | 33.5 ms                                                | 34.3 ms: 1.02x slower                                 |
| Geometric mean  | (ref)                                                  | 1.01x faster                                          |

All benchmarks:
===============

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220405-linux-x86_64-python-main-3.11.0a7-2e49bd0 |
|-------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pickle_dict             | 34.6 us                                                | 27.6 us: 1.25x faster                                 |
| pickle                  | 11.0 us                                                | 9.55 us: 1.15x faster                                 |
| scimark_lu              | 116 ms                                                 | 108 ms: 1.07x faster                                  |
| logging_format          | 6.81 us                                                | 6.35 us: 1.07x faster                                 |
| logging_simple          | 6.22 us                                                | 5.80 us: 1.07x faster                                 |
| logging_silent          | 111 ns                                                 | 104 ns: 1.07x faster                                  |
| json_dumps              | 13.3 ms                                                | 12.5 ms: 1.07x faster                                 |
| python_startup          | 8.56 ms                                                | 8.07 ms: 1.06x faster                                 |
| float                   | 78.9 ms                                                | 74.4 ms: 1.06x faster                                 |
| deltablue               | 3.92 ms                                                | 3.70 ms: 1.06x faster                                 |
| sympy_sum               | 169 ms                                                 | 160 ms: 1.05x faster                                  |
| regex_effbot            | 3.51 ms                                                | 3.34 ms: 1.05x faster                                 |
| unpickle_list           | 5.21 us                                                | 4.97 us: 1.05x faster                                 |
| unpickle_pure_python    | 242 us                                                 | 231 us: 1.05x faster                                  |
| sympy_integrate         | 21.5 ms                                                | 20.5 ms: 1.05x faster                                 |
| richards                | 49.8 ms                                                | 47.5 ms: 1.05x faster                                 |
| mako                    | 10.7 ms                                                | 10.2 ms: 1.05x faster                                 |
| xml_etree_parse         | 164 ms                                                 | 157 ms: 1.05x faster                                  |
| xml_etree_iterparse     | 108 ms                                                 | 104 ms: 1.04x faster                                  |
| go                      | 149 ms                                                 | 143 ms: 1.04x faster                                  |
| telco                   | 6.86 ms                                                | 6.59 ms: 1.04x faster                                 |
| json_loads              | 29.2 us                                                | 28.1 us: 1.04x faster                                 |
| scimark_sparse_mat_mult | 5.03 ms                                                | 4.85 ms: 1.04x faster                                 |
| spectral_norm           | 108 ms                                                 | 105 ms: 1.03x faster                                  |
| sympy_str               | 297 ms                                                 | 287 ms: 1.03x faster                                  |
| json                    | 5.24 ms                                                | 5.07 ms: 1.03x faster                                 |
| xml_etree_generate      | 81.1 ms                                                | 78.5 ms: 1.03x faster                                 |
| scimark_fft             | 345 ms                                                 | 335 ms: 1.03x faster                                  |
| nqueens                 | 87.9 ms                                                | 85.2 ms: 1.03x faster                                 |
| xml_etree_process       | 56.9 ms                                                | 55.2 ms: 1.03x faster                                 |
| thrift                  | 784 us                                                 | 762 us: 1.03x faster                                  |
| tornado_http            | 98.1 ms                                                | 95.4 ms: 1.03x faster                                 |
| regex_compile           | 141 ms                                                 | 137 ms: 1.03x faster                                  |
| pickle_pure_python      | 320 us                                                 | 311 us: 1.03x faster                                  |
| sqlite_synth            | 2.57 us                                                | 2.51 us: 1.03x faster                                 |
| chaos                   | 71.9 ms                                                | 70.2 ms: 1.02x faster                                 |
| meteor_contest          | 109 ms                                                 | 107 ms: 1.02x faster                                  |
| sympy_expand            | 484 ms                                                 | 476 ms: 1.02x faster                                  |
| dulwich_log             | 64.6 ms                                                | 63.8 ms: 1.01x faster                                 |
| fannkuch                | 405 ms                                                 | 401 ms: 1.01x faster                                  |
| raytrace                | 309 ms                                                 | 306 ms: 1.01x faster                                  |
| nbody                   | 96.0 ms                                                | 95.2 ms: 1.01x faster                                 |
| hexiom                  | 6.89 ms                                                | 6.84 ms: 1.01x faster                                 |
| python_startup_no_site  | 6.01 ms                                                | 5.98 ms: 1.00x faster                                 |
| pickle_list             | 4.59 us                                                | 4.57 us: 1.00x faster                                 |
| pyflate                 | 434 ms                                                 | 438 ms: 1.01x slower                                  |
| scimark_sor             | 121 ms                                                 | 123 ms: 1.01x slower                                  |
| pidigits                | 194 ms                                                 | 197 ms: 1.01x slower                                  |
| django_template         | 33.5 ms                                                | 34.3 ms: 1.02x slower                                 |
| chameleon               | 6.70 ms                                                | 6.87 ms: 1.03x slower                                 |
| unpack_sequence         | 43.5 ns                                                | 44.9 ns: 1.03x slower                                 |
| pycparser               | 1.19 sec                                               | 1.24 sec: 1.05x slower                                |
| crypto_pyaes            | 76.7 ms                                                | 82.7 ms: 1.08x slower                                 |
| regex_dna               | 205 ms                                                 | 231 ms: 1.13x slower                                  |
| regex_v8                | 22.9 ms                                                | 25.9 ms: 1.13x slower                                 |
| Geometric mean          | (ref)                                                  | 1.02x faster                                          |

Benchmark hidden because not significant (5): pathlib, 2to3, scimark_monte_carlo, html5lib, unpickle
Ignored benchmarks (45) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_generators, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_io, async_tree_io_tg, async_tree_memoization, async_tree_memoization_tg, async_tree_none, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, bench_mp_pool, bench_thread_pool, comprehensions, coroutines, coverage, create_gc_cycles, dask, deepcopy, deepcopy_memo, deepcopy_reduce, djangocms, docutils, flaskblogging, gc_traversal, generators, genshi_text, genshi_xml, gunicorn, mdp, mypy2, pprint_pformat, pprint_safe_repr, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, sqlglot_normalize, sqlglot_optimize, sqlglot_parse, sqlglot_transpile, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 99.98% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.97x