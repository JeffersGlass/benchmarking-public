
# Results vs. 3.11.0

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: 9471106
- commit date: 2022-01-13
- overall geometric mean: 1.01x faster \*
- HPT reliability: 54.40%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220113-linux-x86_64-python-main-3.11.0a4-9471106 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| chameleon      | 6.70 ms                                                | 7.55 ms: 1.13x slower                                 |
| html5lib       | 64.8 ms                                                | 68.1 ms: 1.05x slower                                 |
| tornado_http   | 98.1 ms                                                | 107 ms: 1.09x slower                                  |
| Geometric mean | (ref)                                                  | 1.06x slower                                          |

Benchmark hidden because not significant (1): 2to3

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220113-linux-x86_64-python-main-3.11.0a4-9471106 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| float          | 78.9 ms                                                | 78.0 ms: 1.01x faster                                 |
| nbody          | 96.0 ms                                                | 95.1 ms: 1.01x faster                                 |
| pidigits       | 194 ms                                                 | 194 ms: 1.00x faster                                  |
| Geometric mean | (ref)                                                  | 1.01x faster                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220113-linux-x86_64-python-main-3.11.0a4-9471106 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.25 ms: 1.08x faster                                 |
| regex_compile  | 141 ms                                                 | 138 ms: 1.02x faster                                  |
| regex_dna      | 205 ms                                                 | 212 ms: 1.04x slower                                  |
| regex_v8       | 22.9 ms                                                | 24.8 ms: 1.09x slower                                 |
| Geometric mean | (ref)                                                  | 1.00x slower                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220113-linux-x86_64-python-main-3.11.0a4-9471106 |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pickle_dict          | 34.6 us                                                | 26.8 us: 1.29x faster                                 |
| json_loads           | 29.2 us                                                | 25.1 us: 1.16x faster                                 |
| pickle               | 11.0 us                                                | 9.95 us: 1.10x faster                                 |
| json_dumps           | 13.3 ms                                                | 12.4 ms: 1.08x faster                                 |
| xml_etree_parse      | 164 ms                                                 | 155 ms: 1.06x faster                                  |
| pickle_list          | 4.59 us                                                | 4.37 us: 1.05x faster                                 |
| xml_etree_generate   | 81.1 ms                                                | 80.2 ms: 1.01x faster                                 |
| xml_etree_iterparse  | 108 ms                                                 | 107 ms: 1.01x faster                                  |
| pickle_pure_python   | 320 us                                                 | 329 us: 1.03x slower                                  |
| unpickle             | 13.8 us                                                | 14.3 us: 1.03x slower                                 |
| unpickle_pure_python | 242 us                                                 | 254 us: 1.05x slower                                  |
| Geometric mean       | (ref)                                                  | 1.05x faster                                          |

Benchmark hidden because not significant (2): unpickle_list, xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220113-linux-x86_64-python-main-3.11.0a4-9471106 |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 8.07 ms: 1.06x faster                                 |
| python_startup_no_site | 6.01 ms                                                | 5.85 ms: 1.03x faster                                 |
| Geometric mean         | (ref)                                                  | 1.04x faster                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220113-linux-x86_64-python-main-3.11.0a4-9471106 |
|-----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| django_template | 33.5 ms                                                | 35.2 ms: 1.05x slower                                 |
| mako            | 10.7 ms                                                | 11.5 ms: 1.08x slower                                 |
| Geometric mean  | (ref)                                                  | 1.07x slower                                          |

All benchmarks:
===============

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220113-linux-x86_64-python-main-3.11.0a4-9471106 |
|-------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pickle_dict             | 34.6 us                                                | 26.8 us: 1.29x faster                                 |
| json_loads              | 29.2 us                                                | 25.1 us: 1.16x faster                                 |
| pickle                  | 11.0 us                                                | 9.95 us: 1.10x faster                                 |
| json                    | 5.24 ms                                                | 4.74 ms: 1.10x faster                                 |
| spectral_norm           | 108 ms                                                 | 99.0 ms: 1.09x faster                                 |
| regex_effbot            | 3.51 ms                                                | 3.25 ms: 1.08x faster                                 |
| json_dumps              | 13.3 ms                                                | 12.4 ms: 1.08x faster                                 |
| scimark_sparse_mat_mult | 5.03 ms                                                | 4.69 ms: 1.07x faster                                 |
| xml_etree_parse         | 164 ms                                                 | 155 ms: 1.06x faster                                  |
| meteor_contest          | 109 ms                                                 | 103 ms: 1.06x faster                                  |
| python_startup          | 8.56 ms                                                | 8.07 ms: 1.06x faster                                 |
| pickle_list             | 4.59 us                                                | 4.37 us: 1.05x faster                                 |
| scimark_fft             | 345 ms                                                 | 330 ms: 1.05x faster                                  |
| logging_format          | 6.81 us                                                | 6.51 us: 1.05x faster                                 |
| logging_simple          | 6.22 us                                                | 5.95 us: 1.05x faster                                 |
| nqueens                 | 87.9 ms                                                | 84.0 ms: 1.05x faster                                 |
| hexiom                  | 6.89 ms                                                | 6.63 ms: 1.04x faster                                 |
| fannkuch                | 405 ms                                                 | 392 ms: 1.03x faster                                  |
| python_startup_no_site  | 6.01 ms                                                | 5.85 ms: 1.03x faster                                 |
| telco                   | 6.86 ms                                                | 6.69 ms: 1.02x faster                                 |
| scimark_lu              | 116 ms                                                 | 114 ms: 1.02x faster                                  |
| regex_compile           | 141 ms                                                 | 138 ms: 1.02x faster                                  |
| pycparser               | 1.19 sec                                               | 1.17 sec: 1.02x faster                                |
| float                   | 78.9 ms                                                | 78.0 ms: 1.01x faster                                 |
| xml_etree_generate      | 81.1 ms                                                | 80.2 ms: 1.01x faster                                 |
| nbody                   | 96.0 ms                                                | 95.1 ms: 1.01x faster                                 |
| xml_etree_iterparse     | 108 ms                                                 | 107 ms: 1.01x faster                                  |
| sympy_integrate         | 21.5 ms                                                | 21.4 ms: 1.00x faster                                 |
| pidigits                | 194 ms                                                 | 194 ms: 1.00x faster                                  |
| sympy_sum               | 169 ms                                                 | 170 ms: 1.00x slower                                  |
| chaos                   | 71.9 ms                                                | 72.7 ms: 1.01x slower                                 |
| sympy_str               | 297 ms                                                 | 302 ms: 1.01x slower                                  |
| dulwich_log             | 64.6 ms                                                | 65.8 ms: 1.02x slower                                 |
| logging_silent          | 111 ns                                                 | 113 ns: 1.02x slower                                  |
| pyflate                 | 434 ms                                                 | 444 ms: 1.02x slower                                  |
| scimark_sor             | 121 ms                                                 | 124 ms: 1.02x slower                                  |
| scimark_monte_carlo     | 70.7 ms                                                | 72.7 ms: 1.03x slower                                 |
| pickle_pure_python      | 320 us                                                 | 329 us: 1.03x slower                                  |
| unpack_sequence         | 43.5 ns                                                | 44.8 ns: 1.03x slower                                 |
| pathlib                 | 18.5 ms                                                | 19.1 ms: 1.03x slower                                 |
| unpickle                | 13.8 us                                                | 14.3 us: 1.03x slower                                 |
| richards                | 49.8 ms                                                | 51.5 ms: 1.04x slower                                 |
| thrift                  | 784 us                                                 | 812 us: 1.04x slower                                  |
| regex_dna               | 205 ms                                                 | 212 ms: 1.04x slower                                  |
| raytrace                | 309 ms                                                 | 320 ms: 1.04x slower                                  |
| sympy_expand            | 484 ms                                                 | 506 ms: 1.04x slower                                  |
| unpickle_pure_python    | 242 us                                                 | 254 us: 1.05x slower                                  |
| django_template         | 33.5 ms                                                | 35.2 ms: 1.05x slower                                 |
| html5lib                | 64.8 ms                                                | 68.1 ms: 1.05x slower                                 |
| deltablue               | 3.92 ms                                                | 4.16 ms: 1.06x slower                                 |
| sqlite_synth            | 2.57 us                                                | 2.73 us: 1.06x slower                                 |
| mako                    | 10.7 ms                                                | 11.5 ms: 1.08x slower                                 |
| regex_v8                | 22.9 ms                                                | 24.8 ms: 1.09x slower                                 |
| tornado_http            | 98.1 ms                                                | 107 ms: 1.09x slower                                  |
| crypto_pyaes            | 76.7 ms                                                | 83.8 ms: 1.09x slower                                 |
| chameleon               | 6.70 ms                                                | 7.55 ms: 1.13x slower                                 |
| Geometric mean          | (ref)                                                  | 1.01x faster                                          |

Benchmark hidden because not significant (4): go, unpickle_list, 2to3, xml_etree_process
Ignored benchmarks (45) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_generators, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_io, async_tree_io_tg, async_tree_memoization, async_tree_memoization_tg, async_tree_none, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, bench_mp_pool, bench_thread_pool, comprehensions, coroutines, coverage, create_gc_cycles, dask, deepcopy, deepcopy_memo, deepcopy_reduce, djangocms, docutils, flaskblogging, gc_traversal, generators, genshi_text, genshi_xml, gunicorn, mdp, mypy2, pprint_pformat, pprint_safe_repr, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, sqlglot_normalize, sqlglot_optimize, sqlglot_parse, sqlglot_transpile, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 54.40% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.99x