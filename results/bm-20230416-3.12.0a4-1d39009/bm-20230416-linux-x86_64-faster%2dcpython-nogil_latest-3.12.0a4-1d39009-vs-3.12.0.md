
# Results vs. 3.12.0

- fork: faster-cpython
- ref: nogil_latest
- machine: linux-x86_64
- commit hash: 1d39009
- commit date: 2023-04-16
- overall geometric mean: 1.02x slower \*
- HPT reliability: 87.85%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.27x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230416-linux-x86_64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 290 ms: 1.06x slower                                                    |
| chameleon      | 7.41 ms                                                | 7.81 ms: 1.05x slower                                                   |
| docutils       | 2.77 sec                                               | 3.15 sec: 1.14x slower                                                  |
| Geometric mean | (ref)                                                  | 1.08x slower                                                            |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230416-linux-x86_64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|-------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| async_tree_io           | 1.16 sec                                               | 616 ms: 1.88x faster                                                    |
| async_tree_memoization  | 578 ms                                                 | 381 ms: 1.52x faster                                                    |
| async_tree_none         | 472 ms                                                 | 311 ms: 1.52x faster                                                    |
| async_tree_cpu_io_mixed | 726 ms                                                 | 534 ms: 1.36x faster                                                    |
| Geometric mean          | (ref)                                                  | 1.56x faster                                                            |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230416-linux-x86_64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| float          | 84.7 ms                                                | 65.9 ms: 1.29x faster                                                   |
| pidigits       | 187 ms                                                 | 186 ms: 1.01x faster                                                    |
| nbody          | 97.0 ms                                                | 107 ms: 1.10x slower                                                    |
| Geometric mean | (ref)                                                  | 1.05x faster                                                            |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230416-linux-x86_64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| regex_v8       | 23.1 ms                                                | 21.1 ms: 1.10x faster                                                   |
| regex_effbot   | 3.61 ms                                                | 3.46 ms: 1.04x faster                                                   |
| regex_dna      | 212 ms                                                 | 205 ms: 1.03x faster                                                    |
| regex_compile  | 148 ms                                                 | 152 ms: 1.02x slower                                                    |
| Geometric mean | (ref)                                                  | 1.04x faster                                                            |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230416-linux-x86_64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| pickle_dict          | 35.5 us                                                | 30.0 us: 1.18x faster                                                   |
| pickle_list          | 5.08 us                                                | 4.33 us: 1.18x faster                                                   |
| xml_etree_parse      | 159 ms                                                 | 137 ms: 1.16x faster                                                    |
| pickle               | 11.6 us                                                | 10.3 us: 1.13x faster                                                   |
| xml_etree_generate   | 89.2 ms                                                | 83.7 ms: 1.06x faster                                                   |
| unpickle             | 15.9 us                                                | 15.5 us: 1.02x faster                                                   |
| unpickle_list        | 5.29 us                                                | 5.20 us: 1.02x faster                                                   |
| json_loads           | 28.5 us                                                | 28.0 us: 1.02x faster                                                   |
| xml_etree_process    | 61.7 ms                                                | 61.3 ms: 1.01x faster                                                   |
| unpickle_pure_python | 230 us                                                 | 229 us: 1.01x faster                                                    |
| xml_etree_iterparse  | 107 ms                                                 | 114 ms: 1.06x slower                                                    |
| Geometric mean       | (ref)                                                  | 1.05x faster                                                            |

Benchmark hidden because not significant (2): pickle_pure_python, json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230416-linux-x86_64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| python_startup_no_site | 6.94 ms                                                | 6.59 ms: 1.05x faster                                                   |
| python_startup         | 9.55 ms                                                | 9.18 ms: 1.04x faster                                                   |
| Geometric mean         | (ref)                                                  | 1.05x faster                                                            |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230416-linux-x86_64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|-----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| django_template | 34.6 ms                                                | 37.4 ms: 1.08x slower                                                   |
| mako            | 11.9 ms                                                | 13.2 ms: 1.11x slower                                                   |
| Geometric mean  | (ref)                                                  | 1.10x slower                                                            |

All benchmarks:
===============

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230416-linux-x86_64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|-------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| async_tree_io           | 1.16 sec                                               | 616 ms: 1.88x faster                                                    |
| async_tree_memoization  | 578 ms                                                 | 381 ms: 1.52x faster                                                    |
| async_tree_none         | 472 ms                                                 | 311 ms: 1.52x faster                                                    |
| async_tree_cpu_io_mixed | 726 ms                                                 | 534 ms: 1.36x faster                                                    |
| float                   | 84.7 ms                                                | 65.9 ms: 1.29x faster                                                   |
| async_generators        | 463 ms                                                 | 377 ms: 1.23x faster                                                    |
| pickle_dict             | 35.5 us                                                | 30.0 us: 1.18x faster                                                   |
| pickle_list             | 5.08 us                                                | 4.33 us: 1.18x faster                                                   |
| xml_etree_parse         | 159 ms                                                 | 137 ms: 1.16x faster                                                    |
| pickle                  | 11.6 us                                                | 10.3 us: 1.13x faster                                                   |
| regex_v8                | 23.1 ms                                                | 21.1 ms: 1.10x faster                                                   |
| sqlite_synth            | 2.83 us                                                | 2.62 us: 1.08x faster                                                   |
| xml_etree_generate      | 89.2 ms                                                | 83.7 ms: 1.06x faster                                                   |
| pathlib                 | 19.3 ms                                                | 18.2 ms: 1.06x faster                                                   |
| python_startup_no_site  | 6.94 ms                                                | 6.59 ms: 1.05x faster                                                   |
| scimark_sor             | 129 ms                                                 | 123 ms: 1.05x faster                                                    |
| regex_effbot            | 3.61 ms                                                | 3.46 ms: 1.04x faster                                                   |
| python_startup          | 9.55 ms                                                | 9.18 ms: 1.04x faster                                                   |
| json                    | 5.26 ms                                                | 5.06 ms: 1.04x faster                                                   |
| gc_traversal            | 3.79 ms                                                | 3.67 ms: 1.04x faster                                                   |
| regex_dna               | 212 ms                                                 | 205 ms: 1.03x faster                                                    |
| pyflate                 | 482 ms                                                 | 470 ms: 1.03x faster                                                    |
| telco                   | 7.10 ms                                                | 6.92 ms: 1.03x faster                                                   |
| unpickle                | 15.9 us                                                | 15.5 us: 1.02x faster                                                   |
| spectral_norm           | 115 ms                                                 | 112 ms: 1.02x faster                                                    |
| scimark_sparse_mat_mult | 5.06 ms                                                | 4.94 ms: 1.02x faster                                                   |
| pycparser               | 1.18 sec                                               | 1.15 sec: 1.02x faster                                                  |
| unpickle_list           | 5.29 us                                                | 5.20 us: 1.02x faster                                                   |
| json_loads              | 28.5 us                                                | 28.0 us: 1.02x faster                                                   |
| deepcopy_memo           | 40.7 us                                                | 40.1 us: 1.02x faster                                                   |
| pprint_safe_repr        | 776 ms                                                 | 765 ms: 1.01x faster                                                    |
| logging_silent          | 104 ns                                                 | 104 ns: 1.01x faster                                                    |
| bench_mp_pool           | 24.0 ms                                                | 23.8 ms: 1.01x faster                                                   |
| pidigits                | 187 ms                                                 | 186 ms: 1.01x faster                                                    |
| xml_etree_process       | 61.7 ms                                                | 61.3 ms: 1.01x faster                                                   |
| dulwich_log             | 68.5 ms                                                | 68.1 ms: 1.01x faster                                                   |
| unpickle_pure_python    | 230 us                                                 | 229 us: 1.01x faster                                                    |
| pprint_pformat          | 1.57 sec                                               | 1.58 sec: 1.01x slower                                                  |
| deepcopy                | 371 us                                                 | 375 us: 1.01x slower                                                    |
| scimark_monte_carlo     | 75.1 ms                                                | 76.4 ms: 1.02x slower                                                   |
| deepcopy_reduce         | 3.35 us                                                | 3.42 us: 1.02x slower                                                   |
| regex_compile           | 148 ms                                                 | 152 ms: 1.02x slower                                                    |
| nqueens                 | 83.3 ms                                                | 85.8 ms: 1.03x slower                                                   |
| sqlglot_normalize       | 110 ms                                                 | 115 ms: 1.04x slower                                                    |
| sqlglot_optimize        | 54.8 ms                                                | 57.1 ms: 1.04x slower                                                   |
| fannkuch                | 417 ms                                                 | 436 ms: 1.05x slower                                                    |
| go                      | 139 ms                                                 | 146 ms: 1.05x slower                                                    |
| deltablue               | 3.72 ms                                                | 3.91 ms: 1.05x slower                                                   |
| chameleon               | 7.41 ms                                                | 7.81 ms: 1.05x slower                                                   |
| richards                | 45.8 ms                                                | 48.4 ms: 1.06x slower                                                   |
| 2to3                    | 274 ms                                                 | 290 ms: 1.06x slower                                                    |
| mdp                     | 2.63 sec                                               | 2.79 sec: 1.06x slower                                                  |
| logging_format          | 7.23 us                                                | 7.66 us: 1.06x slower                                                   |
| xml_etree_iterparse     | 107 ms                                                 | 114 ms: 1.06x slower                                                    |
| sympy_integrate         | 21.4 ms                                                | 22.8 ms: 1.07x slower                                                   |
| asyncio_tcp             | 491 ms                                                 | 525 ms: 1.07x slower                                                    |
| hexiom                  | 6.41 ms                                                | 6.89 ms: 1.08x slower                                                   |
| unpack_sequence         | 54.0 ns                                                | 58.1 ns: 1.08x slower                                                   |
| create_gc_cycles        | 1.48 ms                                                | 1.59 ms: 1.08x slower                                                   |
| django_template         | 34.6 ms                                                | 37.4 ms: 1.08x slower                                                   |
| scimark_lu              | 118 ms                                                 | 128 ms: 1.08x slower                                                    |
| logging_simple          | 6.46 us                                                | 7.00 us: 1.08x slower                                                   |
| sympy_str               | 300 ms                                                 | 329 ms: 1.10x slower                                                    |
| nbody                   | 97.0 ms                                                | 107 ms: 1.10x slower                                                    |
| raytrace                | 312 ms                                                 | 346 ms: 1.11x slower                                                    |
| meteor_contest          | 112 ms                                                 | 124 ms: 1.11x slower                                                    |
| mako                    | 11.9 ms                                                | 13.2 ms: 1.11x slower                                                   |
| chaos                   | 67.0 ms                                                | 74.6 ms: 1.11x slower                                                   |
| sympy_expand            | 478 ms                                                 | 537 ms: 1.12x slower                                                    |
| docutils                | 2.77 sec                                               | 3.15 sec: 1.14x slower                                                  |
| sympy_sum               | 169 ms                                                 | 192 ms: 1.14x slower                                                    |
| coroutines              | 23.2 ms                                                | 26.8 ms: 1.16x slower                                                   |
| comprehensions          | 21.8 us                                                | 26.3 us: 1.21x slower                                                   |
| sqlglot_transpile       | 1.68 ms                                                | 2.10 ms: 1.25x slower                                                   |
| sqlglot_parse           | 1.36 ms                                                | 1.79 ms: 1.31x slower                                                   |
| coverage                | 72.7 ms                                                | 109 ms: 1.50x slower                                                    |
| bench_thread_pool       | 842 us                                                 | 1.64 ms: 1.95x slower                                                   |
| generators              | 31.2 ms                                                | 78.8 ms: 2.52x slower                                                   |
| Geometric mean          | (ref)                                                  | 1.02x slower                                                            |

Benchmark hidden because not significant (4): pickle_pure_python, crypto_pyaes, json_dumps, scimark_fft
Ignored benchmarks (16) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, dask, gunicorn, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
Ignored benchmarks (5) of results/bm-20230416-3.12.0a4-1d39009/bm-20230416-linux-x86_64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009.json: djangocms, genshi_text, genshi_xml, html5lib, thrift


# HPT report

- Reliability score: 87.85% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.27x