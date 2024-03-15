
# Results vs. 3.11.0

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: 3ddfa55
- commit date: 2022-03-07
- overall geometric mean: 1.01x slower \*
- HPT reliability: 57.30%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220307-linux-x86_64-python-main-3.11.0a6-3ddfa55 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| 2to3           | 264 ms                                                 | 268 ms: 1.01x slower                                  |
| chameleon      | 6.70 ms                                                | 6.93 ms: 1.03x slower                                 |
| html5lib       | 64.8 ms                                                | 68.6 ms: 1.06x slower                                 |
| tornado_http   | 98.1 ms                                                | 99.2 ms: 1.01x slower                                 |
| Geometric mean | (ref)                                                  | 1.03x slower                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220307-linux-x86_64-python-main-3.11.0a6-3ddfa55 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| nbody          | 96.0 ms                                                | 97.7 ms: 1.02x slower                                 |
| pidigits       | 194 ms                                                 | 208 ms: 1.07x slower                                  |
| Geometric mean | (ref)                                                  | 1.03x slower                                          |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220307-linux-x86_64-python-main-3.11.0a6-3ddfa55 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 140 ms: 1.01x faster                                  |
| regex_effbot   | 3.51 ms                                                | 3.49 ms: 1.01x faster                                 |
| regex_v8       | 22.9 ms                                                | 23.0 ms: 1.00x slower                                 |
| regex_dna      | 205 ms                                                 | 221 ms: 1.08x slower                                  |
| Geometric mean | (ref)                                                  | 1.02x slower                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220307-linux-x86_64-python-main-3.11.0a6-3ddfa55 |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pickle_dict          | 34.6 us                                                | 28.1 us: 1.23x faster                                 |
| pickle               | 11.0 us                                                | 9.69 us: 1.13x faster                                 |
| unpickle_list        | 5.21 us                                                | 4.92 us: 1.06x faster                                 |
| json_dumps           | 13.3 ms                                                | 12.6 ms: 1.06x faster                                 |
| xml_etree_parse      | 164 ms                                                 | 156 ms: 1.05x faster                                  |
| json_loads           | 29.2 us                                                | 28.1 us: 1.04x faster                                 |
| xml_etree_iterparse  | 108 ms                                                 | 105 ms: 1.03x faster                                  |
| xml_etree_generate   | 81.1 ms                                                | 79.6 ms: 1.02x faster                                 |
| pickle_list          | 4.59 us                                                | 4.51 us: 1.02x faster                                 |
| xml_etree_process    | 56.9 ms                                                | 56.0 ms: 1.02x faster                                 |
| unpickle_pure_python | 242 us                                                 | 246 us: 1.02x slower                                  |
| pickle_pure_python   | 320 us                                                 | 335 us: 1.05x slower                                  |
| Geometric mean       | (ref)                                                  | 1.04x faster                                          |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220307-linux-x86_64-python-main-3.11.0a6-3ddfa55 |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 8.20 ms: 1.04x faster                                 |
| python_startup_no_site | 6.01 ms                                                | 6.07 ms: 1.01x slower                                 |
| Geometric mean         | (ref)                                                  | 1.02x faster                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220307-linux-x86_64-python-main-3.11.0a6-3ddfa55 |
|-----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| mako            | 10.7 ms                                                | 10.6 ms: 1.00x faster                                 |
| django_template | 33.5 ms                                                | 36.0 ms: 1.07x slower                                 |
| Geometric mean  | (ref)                                                  | 1.03x slower                                          |

All benchmarks:
===============

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220307-linux-x86_64-python-main-3.11.0a6-3ddfa55 |
|-------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pickle_dict             | 34.6 us                                                | 28.1 us: 1.23x faster                                 |
| pickle                  | 11.0 us                                                | 9.69 us: 1.13x faster                                 |
| logging_simple          | 6.22 us                                                | 5.52 us: 1.13x faster                                 |
| logging_format          | 6.81 us                                                | 6.08 us: 1.12x faster                                 |
| unpickle_list           | 5.21 us                                                | 4.92 us: 1.06x faster                                 |
| json_dumps              | 13.3 ms                                                | 12.6 ms: 1.06x faster                                 |
| json                    | 5.24 ms                                                | 5.00 ms: 1.05x faster                                 |
| xml_etree_parse         | 164 ms                                                 | 156 ms: 1.05x faster                                  |
| python_startup          | 8.56 ms                                                | 8.20 ms: 1.04x faster                                 |
| scimark_sparse_mat_mult | 5.03 ms                                                | 4.82 ms: 1.04x faster                                 |
| json_loads              | 29.2 us                                                | 28.1 us: 1.04x faster                                 |
| sympy_sum               | 169 ms                                                 | 163 ms: 1.03x faster                                  |
| meteor_contest          | 109 ms                                                 | 106 ms: 1.03x faster                                  |
| xml_etree_iterparse     | 108 ms                                                 | 105 ms: 1.03x faster                                  |
| sympy_integrate         | 21.5 ms                                                | 20.9 ms: 1.03x faster                                 |
| sympy_str               | 297 ms                                                 | 289 ms: 1.03x faster                                  |
| scimark_fft             | 345 ms                                                 | 336 ms: 1.03x faster                                  |
| richards                | 49.8 ms                                                | 48.5 ms: 1.03x faster                                 |
| sqlite_synth            | 2.57 us                                                | 2.51 us: 1.03x faster                                 |
| pathlib                 | 18.5 ms                                                | 18.2 ms: 1.02x faster                                 |
| xml_etree_generate      | 81.1 ms                                                | 79.6 ms: 1.02x faster                                 |
| fannkuch                | 405 ms                                                 | 398 ms: 1.02x faster                                  |
| pickle_list             | 4.59 us                                                | 4.51 us: 1.02x faster                                 |
| xml_etree_process       | 56.9 ms                                                | 56.0 ms: 1.02x faster                                 |
| regex_compile           | 141 ms                                                 | 140 ms: 1.01x faster                                  |
| nqueens                 | 87.9 ms                                                | 87.0 ms: 1.01x faster                                 |
| go                      | 149 ms                                                 | 148 ms: 1.01x faster                                  |
| sympy_expand            | 484 ms                                                 | 481 ms: 1.01x faster                                  |
| regex_effbot            | 3.51 ms                                                | 3.49 ms: 1.01x faster                                 |
| mako                    | 10.7 ms                                                | 10.6 ms: 1.00x faster                                 |
| regex_v8                | 22.9 ms                                                | 23.0 ms: 1.00x slower                                 |
| telco                   | 6.86 ms                                                | 6.92 ms: 1.01x slower                                 |
| python_startup_no_site  | 6.01 ms                                                | 6.07 ms: 1.01x slower                                 |
| tornado_http            | 98.1 ms                                                | 99.2 ms: 1.01x slower                                 |
| 2to3                    | 264 ms                                                 | 268 ms: 1.01x slower                                  |
| logging_silent          | 111 ns                                                 | 113 ns: 1.01x slower                                  |
| unpickle_pure_python    | 242 us                                                 | 246 us: 1.02x slower                                  |
| scimark_sor             | 121 ms                                                 | 123 ms: 1.02x slower                                  |
| nbody                   | 96.0 ms                                                | 97.7 ms: 1.02x slower                                 |
| hexiom                  | 6.89 ms                                                | 7.04 ms: 1.02x slower                                 |
| chaos                   | 71.9 ms                                                | 73.5 ms: 1.02x slower                                 |
| pycparser               | 1.19 sec                                               | 1.21 sec: 1.02x slower                                |
| dulwich_log             | 64.6 ms                                                | 66.5 ms: 1.03x slower                                 |
| raytrace                | 309 ms                                                 | 318 ms: 1.03x slower                                  |
| scimark_monte_carlo     | 70.7 ms                                                | 72.9 ms: 1.03x slower                                 |
| chameleon               | 6.70 ms                                                | 6.93 ms: 1.03x slower                                 |
| pyflate                 | 434 ms                                                 | 453 ms: 1.04x slower                                  |
| pickle_pure_python      | 320 us                                                 | 335 us: 1.05x slower                                  |
| html5lib                | 64.8 ms                                                | 68.6 ms: 1.06x slower                                 |
| deltablue               | 3.92 ms                                                | 4.16 ms: 1.06x slower                                 |
| pidigits                | 194 ms                                                 | 208 ms: 1.07x slower                                  |
| django_template         | 33.5 ms                                                | 36.0 ms: 1.07x slower                                 |
| regex_dna               | 205 ms                                                 | 221 ms: 1.08x slower                                  |
| crypto_pyaes            | 76.7 ms                                                | 84.6 ms: 1.10x slower                                 |
| unpack_sequence         | 43.5 ns                                                | 131 ns: 3.01x slower                                  |
| Geometric mean          | (ref)                                                  | 1.01x slower                                          |

Benchmark hidden because not significant (5): scimark_lu, spectral_norm, float, thrift, unpickle
Ignored benchmarks (45) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_generators, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_io, async_tree_io_tg, async_tree_memoization, async_tree_memoization_tg, async_tree_none, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, bench_mp_pool, bench_thread_pool, comprehensions, coroutines, coverage, create_gc_cycles, dask, deepcopy, deepcopy_memo, deepcopy_reduce, djangocms, docutils, flaskblogging, gc_traversal, generators, genshi_text, genshi_xml, gunicorn, mdp, mypy2, pprint_pformat, pprint_safe_repr, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, sqlglot_normalize, sqlglot_optimize, sqlglot_parse, sqlglot_transpile, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 57.30% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.99x