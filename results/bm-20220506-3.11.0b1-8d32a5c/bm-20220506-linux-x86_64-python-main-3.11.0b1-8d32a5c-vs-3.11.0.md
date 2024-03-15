
# Results vs. 3.11.0

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: 8d32a5c
- commit date: 2022-05-06
- overall geometric mean: 1.06x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x faster
- Memory change: 0.95x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220506-linux-x86_64-python-main-3.11.0b1-8d32a5c |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| 2to3           | 264 ms                                                 | 256 ms: 1.03x faster                                  |
| chameleon      | 6.70 ms                                                | 6.57 ms: 1.02x faster                                 |
| html5lib       | 64.8 ms                                                | 60.1 ms: 1.08x faster                                 |
| tornado_http   | 98.1 ms                                                | 94.6 ms: 1.04x faster                                 |
| Geometric mean | (ref)                                                  | 1.04x faster                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220506-linux-x86_64-python-main-3.11.0b1-8d32a5c |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| float          | 78.9 ms                                                | 72.5 ms: 1.09x faster                                 |
| nbody          | 96.0 ms                                                | 93.1 ms: 1.03x faster                                 |
| pidigits       | 194 ms                                                 | 190 ms: 1.02x faster                                  |
| Geometric mean | (ref)                                                  | 1.05x faster                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220506-linux-x86_64-python-main-3.11.0b1-8d32a5c |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 2.93 ms: 1.20x faster                                 |
| regex_v8       | 22.9 ms                                                | 21.6 ms: 1.06x faster                                 |
| regex_compile  | 141 ms                                                 | 135 ms: 1.05x faster                                  |
| regex_dna      | 205 ms                                                 | 204 ms: 1.00x faster                                  |
| Geometric mean | (ref)                                                  | 1.07x faster                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220506-linux-x86_64-python-main-3.11.0b1-8d32a5c |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pickle_dict          | 34.6 us                                                | 25.6 us: 1.35x faster                                 |
| json_loads           | 29.2 us                                                | 25.4 us: 1.15x faster                                 |
| pickle               | 11.0 us                                                | 9.56 us: 1.15x faster                                 |
| json_dumps           | 13.3 ms                                                | 12.4 ms: 1.08x faster                                 |
| pickle_list          | 4.59 us                                                | 4.26 us: 1.08x faster                                 |
| xml_etree_process    | 56.9 ms                                                | 53.6 ms: 1.06x faster                                 |
| xml_etree_generate   | 81.1 ms                                                | 76.5 ms: 1.06x faster                                 |
| unpickle_pure_python | 242 us                                                 | 229 us: 1.06x faster                                  |
| pickle_pure_python   | 320 us                                                 | 305 us: 1.05x faster                                  |
| xml_etree_parse      | 164 ms                                                 | 157 ms: 1.04x faster                                  |
| unpickle             | 13.8 us                                                | 13.4 us: 1.04x faster                                 |
| xml_etree_iterparse  | 108 ms                                                 | 104 ms: 1.03x faster                                  |
| unpickle_list        | 5.21 us                                                | 5.05 us: 1.03x faster                                 |
| Geometric mean       | (ref)                                                  | 1.09x faster                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220506-linux-x86_64-python-main-3.11.0b1-8d32a5c |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 8.25 ms: 1.04x faster                                 |
| python_startup_no_site | 6.01 ms                                                | 6.16 ms: 1.02x slower                                 |
| Geometric mean         | (ref)                                                  | 1.01x faster                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220506-linux-x86_64-python-main-3.11.0b1-8d32a5c |
|-----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| mako            | 10.7 ms                                                | 9.88 ms: 1.08x faster                                 |
| django_template | 33.5 ms                                                | 32.8 ms: 1.02x faster                                 |
| Geometric mean  | (ref)                                                  | 1.05x faster                                          |

All benchmarks:
===============

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220506-linux-x86_64-python-main-3.11.0b1-8d32a5c |
|-------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pickle_dict             | 34.6 us                                                | 25.6 us: 1.35x faster                                 |
| regex_effbot            | 3.51 ms                                                | 2.93 ms: 1.20x faster                                 |
| json_loads              | 29.2 us                                                | 25.4 us: 1.15x faster                                 |
| pickle                  | 11.0 us                                                | 9.56 us: 1.15x faster                                 |
| logging_silent          | 111 ns                                                 | 98.2 ns: 1.13x faster                                 |
| spectral_norm           | 108 ms                                                 | 97.6 ms: 1.11x faster                                 |
| scimark_sparse_mat_mult | 5.03 ms                                                | 4.57 ms: 1.10x faster                                 |
| hexiom                  | 6.89 ms                                                | 6.29 ms: 1.10x faster                                 |
| go                      | 149 ms                                                 | 136 ms: 1.09x faster                                  |
| float                   | 78.9 ms                                                | 72.5 ms: 1.09x faster                                 |
| deltablue               | 3.92 ms                                                | 3.61 ms: 1.09x faster                                 |
| json_dumps              | 13.3 ms                                                | 12.4 ms: 1.08x faster                                 |
| mako                    | 10.7 ms                                                | 9.88 ms: 1.08x faster                                 |
| html5lib                | 64.8 ms                                                | 60.1 ms: 1.08x faster                                 |
| pickle_list             | 4.59 us                                                | 4.26 us: 1.08x faster                                 |
| richards                | 49.8 ms                                                | 46.4 ms: 1.07x faster                                 |
| json                    | 5.24 ms                                                | 4.91 ms: 1.07x faster                                 |
| scimark_lu              | 116 ms                                                 | 109 ms: 1.07x faster                                  |
| scimark_monte_carlo     | 70.7 ms                                                | 66.5 ms: 1.06x faster                                 |
| scimark_fft             | 345 ms                                                 | 325 ms: 1.06x faster                                  |
| xml_etree_process       | 56.9 ms                                                | 53.6 ms: 1.06x faster                                 |
| xml_etree_generate      | 81.1 ms                                                | 76.5 ms: 1.06x faster                                 |
| scimark_sor             | 121 ms                                                 | 115 ms: 1.06x faster                                  |
| regex_v8                | 22.9 ms                                                | 21.6 ms: 1.06x faster                                 |
| unpickle_pure_python    | 242 us                                                 | 229 us: 1.06x faster                                  |
| thrift                  | 784 us                                                 | 741 us: 1.06x faster                                  |
| logging_format          | 6.81 us                                                | 6.44 us: 1.06x faster                                 |
| logging_simple          | 6.22 us                                                | 5.89 us: 1.06x faster                                 |
| pyflate                 | 434 ms                                                 | 411 ms: 1.06x faster                                  |
| fannkuch                | 405 ms                                                 | 385 ms: 1.05x faster                                  |
| regex_compile           | 141 ms                                                 | 135 ms: 1.05x faster                                  |
| sympy_sum               | 169 ms                                                 | 161 ms: 1.05x faster                                  |
| raytrace                | 309 ms                                                 | 294 ms: 1.05x faster                                  |
| sympy_integrate         | 21.5 ms                                                | 20.5 ms: 1.05x faster                                 |
| pickle_pure_python      | 320 us                                                 | 305 us: 1.05x faster                                  |
| sympy_str               | 297 ms                                                 | 284 ms: 1.05x faster                                  |
| chaos                   | 71.9 ms                                                | 68.6 ms: 1.05x faster                                 |
| xml_etree_parse         | 164 ms                                                 | 157 ms: 1.04x faster                                  |
| meteor_contest          | 109 ms                                                 | 105 ms: 1.04x faster                                  |
| nqueens                 | 87.9 ms                                                | 84.7 ms: 1.04x faster                                 |
| python_startup          | 8.56 ms                                                | 8.25 ms: 1.04x faster                                 |
| unpickle                | 13.8 us                                                | 13.4 us: 1.04x faster                                 |
| sympy_expand            | 484 ms                                                 | 468 ms: 1.04x faster                                  |
| tornado_http            | 98.1 ms                                                | 94.6 ms: 1.04x faster                                 |
| pathlib                 | 18.5 ms                                                | 17.9 ms: 1.04x faster                                 |
| xml_etree_iterparse     | 108 ms                                                 | 104 ms: 1.03x faster                                  |
| crypto_pyaes            | 76.7 ms                                                | 74.3 ms: 1.03x faster                                 |
| unpickle_list           | 5.21 us                                                | 5.05 us: 1.03x faster                                 |
| 2to3                    | 264 ms                                                 | 256 ms: 1.03x faster                                  |
| nbody                   | 96.0 ms                                                | 93.1 ms: 1.03x faster                                 |
| dulwich_log             | 64.6 ms                                                | 62.8 ms: 1.03x faster                                 |
| pidigits                | 194 ms                                                 | 190 ms: 1.02x faster                                  |
| django_template         | 33.5 ms                                                | 32.8 ms: 1.02x faster                                 |
| chameleon               | 6.70 ms                                                | 6.57 ms: 1.02x faster                                 |
| sqlite_synth            | 2.57 us                                                | 2.53 us: 1.02x faster                                 |
| regex_dna               | 205 ms                                                 | 204 ms: 1.00x faster                                  |
| unpack_sequence         | 43.5 ns                                                | 44.3 ns: 1.02x slower                                 |
| python_startup_no_site  | 6.01 ms                                                | 6.16 ms: 1.02x slower                                 |
| Geometric mean          | (ref)                                                  | 1.06x faster                                          |

Benchmark hidden because not significant (2): telco, pycparser
Ignored benchmarks (45) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_generators, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_io, async_tree_io_tg, async_tree_memoization, async_tree_memoization_tg, async_tree_none, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, bench_mp_pool, bench_thread_pool, comprehensions, coroutines, coverage, create_gc_cycles, dask, deepcopy, deepcopy_memo, deepcopy_reduce, djangocms, docutils, flaskblogging, gc_traversal, generators, genshi_text, genshi_xml, gunicorn, mdp, mypy2, pprint_pformat, pprint_safe_repr, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, sqlglot_normalize, sqlglot_optimize, sqlglot_parse, sqlglot_transpile, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.04x
- 95% likely to have a speedup of 1.04x
- 99% likely to have a speedup of 1.04x


# Memory

- memory change: 0.95x