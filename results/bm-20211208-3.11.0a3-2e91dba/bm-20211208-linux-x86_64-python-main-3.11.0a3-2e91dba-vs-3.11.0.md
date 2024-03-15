
# Results vs. 3.11.0

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: 2e91dba
- commit date: 2021-12-08
- overall geometric mean: 1.01x slower \*
- HPT reliability: 96.38%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.97x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211208-linux-x86_64-python-main-3.11.0a3-2e91dba |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| 2to3           | 264 ms                                                 | 264 ms: 1.00x faster                                  |
| chameleon      | 6.70 ms                                                | 7.44 ms: 1.11x slower                                 |
| html5lib       | 64.8 ms                                                | 68.5 ms: 1.06x slower                                 |
| tornado_http   | 98.1 ms                                                | 108 ms: 1.10x slower                                  |
| Geometric mean | (ref)                                                  | 1.07x slower                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211208-linux-x86_64-python-main-3.11.0a3-2e91dba |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pidigits       | 194 ms                                                 | 198 ms: 1.02x slower                                  |
| Geometric mean | (ref)                                                  | 1.01x slower                                          |

Benchmark hidden because not significant (2): nbody, float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211208-linux-x86_64-python-main-3.11.0a3-2e91dba |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.21 ms: 1.09x faster                                 |
| regex_compile  | 141 ms                                                 | 139 ms: 1.02x faster                                  |
| regex_dna      | 205 ms                                                 | 212 ms: 1.04x slower                                  |
| regex_v8       | 22.9 ms                                                | 24.5 ms: 1.07x slower                                 |
| Geometric mean | (ref)                                                  | 1.00x faster                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211208-linux-x86_64-python-main-3.11.0a3-2e91dba |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pickle_dict          | 34.6 us                                                | 27.7 us: 1.25x faster                                 |
| json_loads           | 29.2 us                                                | 25.6 us: 1.14x faster                                 |
| pickle               | 11.0 us                                                | 9.95 us: 1.10x faster                                 |
| json_dumps           | 13.3 ms                                                | 12.6 ms: 1.06x faster                                 |
| xml_etree_parse      | 164 ms                                                 | 156 ms: 1.05x faster                                  |
| xml_etree_iterparse  | 108 ms                                                 | 105 ms: 1.03x faster                                  |
| xml_etree_generate   | 81.1 ms                                                | 80.8 ms: 1.00x faster                                 |
| xml_etree_process    | 56.9 ms                                                | 57.8 ms: 1.02x slower                                 |
| pickle_list          | 4.59 us                                                | 4.68 us: 1.02x slower                                 |
| unpickle_pure_python | 242 us                                                 | 251 us: 1.04x slower                                  |
| unpickle             | 13.8 us                                                | 14.6 us: 1.05x slower                                 |
| pickle_pure_python   | 320 us                                                 | 347 us: 1.08x slower                                  |
| Geometric mean       | (ref)                                                  | 1.03x faster                                          |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211208-linux-x86_64-python-main-3.11.0a3-2e91dba |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 8.00 ms: 1.07x faster                                 |
| python_startup_no_site | 6.01 ms                                                | 5.78 ms: 1.04x faster                                 |
| Geometric mean         | (ref)                                                  | 1.05x faster                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211208-linux-x86_64-python-main-3.11.0a3-2e91dba |
|-----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| django_template | 33.5 ms                                                | 36.5 ms: 1.09x slower                                 |
| mako            | 10.7 ms                                                | 11.9 ms: 1.12x slower                                 |
| Geometric mean  | (ref)                                                  | 1.10x slower                                          |

All benchmarks:
===============

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211208-linux-x86_64-python-main-3.11.0a3-2e91dba |
|-------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pickle_dict             | 34.6 us                                                | 27.7 us: 1.25x faster                                 |
| json_loads              | 29.2 us                                                | 25.6 us: 1.14x faster                                 |
| pickle                  | 11.0 us                                                | 9.95 us: 1.10x faster                                 |
| regex_effbot            | 3.51 ms                                                | 3.21 ms: 1.09x faster                                 |
| json                    | 5.24 ms                                                | 4.83 ms: 1.08x faster                                 |
| python_startup          | 8.56 ms                                                | 8.00 ms: 1.07x faster                                 |
| json_dumps              | 13.3 ms                                                | 12.6 ms: 1.06x faster                                 |
| xml_etree_parse         | 164 ms                                                 | 156 ms: 1.05x faster                                  |
| scimark_sparse_mat_mult | 5.03 ms                                                | 4.77 ms: 1.05x faster                                 |
| logging_format          | 6.81 us                                                | 6.49 us: 1.05x faster                                 |
| fannkuch                | 405 ms                                                 | 386 ms: 1.05x faster                                  |
| telco                   | 6.86 ms                                                | 6.56 ms: 1.05x faster                                 |
| spectral_norm           | 108 ms                                                 | 104 ms: 1.04x faster                                  |
| meteor_contest          | 109 ms                                                 | 104 ms: 1.04x faster                                  |
| logging_simple          | 6.22 us                                                | 5.97 us: 1.04x faster                                 |
| scimark_lu              | 116 ms                                                 | 112 ms: 1.04x faster                                  |
| python_startup_no_site  | 6.01 ms                                                | 5.78 ms: 1.04x faster                                 |
| scimark_fft             | 345 ms                                                 | 332 ms: 1.04x faster                                  |
| nqueens                 | 87.9 ms                                                | 84.6 ms: 1.04x faster                                 |
| xml_etree_iterparse     | 108 ms                                                 | 105 ms: 1.03x faster                                  |
| regex_compile           | 141 ms                                                 | 139 ms: 1.02x faster                                  |
| hexiom                  | 6.89 ms                                                | 6.77 ms: 1.02x faster                                 |
| logging_silent          | 111 ns                                                 | 110 ns: 1.01x faster                                  |
| xml_etree_generate      | 81.1 ms                                                | 80.8 ms: 1.00x faster                                 |
| 2to3                    | 264 ms                                                 | 264 ms: 1.00x faster                                  |
| sympy_integrate         | 21.5 ms                                                | 21.7 ms: 1.01x slower                                 |
| xml_etree_process       | 56.9 ms                                                | 57.8 ms: 1.02x slower                                 |
| sympy_sum               | 169 ms                                                 | 172 ms: 1.02x slower                                  |
| pickle_list             | 4.59 us                                                | 4.68 us: 1.02x slower                                 |
| pidigits                | 194 ms                                                 | 198 ms: 1.02x slower                                  |
| chaos                   | 71.9 ms                                                | 73.9 ms: 1.03x slower                                 |
| regex_dna               | 205 ms                                                 | 212 ms: 1.04x slower                                  |
| sympy_str               | 297 ms                                                 | 308 ms: 1.04x slower                                  |
| thrift                  | 784 us                                                 | 814 us: 1.04x slower                                  |
| unpickle_pure_python    | 242 us                                                 | 251 us: 1.04x slower                                  |
| dulwich_log             | 64.6 ms                                                | 67.2 ms: 1.04x slower                                 |
| pycparser               | 1.19 sec                                               | 1.24 sec: 1.04x slower                                |
| scimark_monte_carlo     | 70.7 ms                                                | 74.0 ms: 1.05x slower                                 |
| pathlib                 | 18.5 ms                                                | 19.4 ms: 1.05x slower                                 |
| sympy_expand            | 484 ms                                                 | 509 ms: 1.05x slower                                  |
| unpickle                | 13.8 us                                                | 14.6 us: 1.05x slower                                 |
| html5lib                | 64.8 ms                                                | 68.5 ms: 1.06x slower                                 |
| go                      | 149 ms                                                 | 158 ms: 1.06x slower                                  |
| sqlite_synth            | 2.57 us                                                | 2.74 us: 1.06x slower                                 |
| regex_v8                | 22.9 ms                                                | 24.5 ms: 1.07x slower                                 |
| scimark_sor             | 121 ms                                                 | 130 ms: 1.07x slower                                  |
| raytrace                | 309 ms                                                 | 333 ms: 1.08x slower                                  |
| pickle_pure_python      | 320 us                                                 | 347 us: 1.08x slower                                  |
| django_template         | 33.5 ms                                                | 36.5 ms: 1.09x slower                                 |
| richards                | 49.8 ms                                                | 54.5 ms: 1.10x slower                                 |
| pyflate                 | 434 ms                                                 | 477 ms: 1.10x slower                                  |
| tornado_http            | 98.1 ms                                                | 108 ms: 1.10x slower                                  |
| chameleon               | 6.70 ms                                                | 7.44 ms: 1.11x slower                                 |
| mako                    | 10.7 ms                                                | 11.9 ms: 1.12x slower                                 |
| unpack_sequence         | 43.5 ns                                                | 49.2 ns: 1.13x slower                                 |
| crypto_pyaes            | 76.7 ms                                                | 88.1 ms: 1.15x slower                                 |
| deltablue               | 3.92 ms                                                | 4.54 ms: 1.16x slower                                 |
| Geometric mean          | (ref)                                                  | 1.01x slower                                          |

Benchmark hidden because not significant (3): unpickle_list, nbody, float
Ignored benchmarks (45) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_generators, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_io, async_tree_io_tg, async_tree_memoization, async_tree_memoization_tg, async_tree_none, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, bench_mp_pool, bench_thread_pool, comprehensions, coroutines, coverage, create_gc_cycles, dask, deepcopy, deepcopy_memo, deepcopy_reduce, djangocms, docutils, flaskblogging, gc_traversal, generators, genshi_text, genshi_xml, gunicorn, mdp, mypy2, pprint_pformat, pprint_safe_repr, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, sqlglot_normalize, sqlglot_optimize, sqlglot_parse, sqlglot_transpile, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 96.38% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.97x