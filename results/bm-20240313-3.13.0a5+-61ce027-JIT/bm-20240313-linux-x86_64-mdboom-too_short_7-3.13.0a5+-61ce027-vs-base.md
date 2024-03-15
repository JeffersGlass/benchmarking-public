# Results vs. base

- fork: mdboom
- ref: too_short_7
- machine: linux-x86_64
- commit hash: 61ce027
- commit date: 2024-03-13
- overall geometric mean: 1.00x faster
- HPT reliability: 98.91%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------:|
| 2to3           | 282 ms                                                                 | 281 ms: 1.00x faster                                          |
| chameleon      | 6.90 ms                                                                | 7.01 ms: 1.02x slower                                         |
| html5lib       | 65.7 ms                                                                | 68.1 ms: 1.04x slower                                         |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                  |

Benchmark hidden because not significant (2): docutils, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|--------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------:|
| async_tree_none_tg | 459 ms                                                                 | 458 ms: 1.00x faster                                          |
| Geometric mean     | (ref)                                                                  | 1.00x slower                                                  |

Benchmark hidden because not significant (7): async_tree_none, async_tree_io, async_tree_memoization, async_tree_io_tg, async_tree_memoization_tg, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------:|
| float          | 79.8 ms                                                                | 80.6 ms: 1.01x slower                                         |
| nbody          | 92.4 ms                                                                | 93.5 ms: 1.01x slower                                         |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                  |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------:|
| regex_dna      | 238 ms                                                                 | 232 ms: 1.03x faster                                          |
| regex_compile  | 144 ms                                                                 | 143 ms: 1.00x faster                                          |
| regex_v8       | 25.4 ms                                                                | 26.1 ms: 1.03x slower                                         |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                  |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|----------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------:|
| pickle_list          | 5.31 us                                                                | 4.95 us: 1.07x faster                                         |
| pickle_dict          | 35.4 us                                                                | 33.7 us: 1.05x faster                                         |
| pickle               | 12.0 us                                                                | 11.6 us: 1.03x faster                                         |
| unpickle             | 15.1 us                                                                | 14.8 us: 1.02x faster                                         |
| pickle_pure_python   | 302 us                                                                 | 298 us: 1.01x faster                                          |
| unpickle_list        | 4.93 us                                                                | 4.89 us: 1.01x faster                                         |
| unpickle_pure_python | 239 us                                                                 | 238 us: 1.00x faster                                          |
| json_loads           | 27.9 us                                                                | 28.0 us: 1.01x slower                                         |
| xml_etree_generate   | 86.8 ms                                                                | 87.4 ms: 1.01x slower                                         |
| json_dumps           | 10.4 ms                                                                | 10.5 ms: 1.01x slower                                         |
| Geometric mean       | (ref)                                                                  | 1.01x faster                                                  |

Benchmark hidden because not significant (4): xml_etree_process, xml_etree_iterparse, tomli_loads, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|------------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------:|
| python_startup_no_site | 11.2 ms                                                                | 11.1 ms: 1.00x faster                                         |
| python_startup         | 12.6 ms                                                                | 12.6 ms: 1.00x faster                                         |
| Geometric mean         | (ref)                                                                  | 1.00x faster                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|-----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------:|
| genshi_text     | 24.7 ms                                                                | 24.0 ms: 1.03x faster                                         |
| django_template | 34.4 ms                                                                | 34.8 ms: 1.01x slower                                         |
| mako            | 10.7 ms                                                                | 10.9 ms: 1.02x slower                                         |
| Geometric mean  | (ref)                                                                  | 1.00x faster                                                  |

Benchmark hidden because not significant (1): genshi_xml

All benchmarks:
===============

| Benchmark               | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|-------------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------:|
| pickle_list             | 5.31 us                                                                | 4.95 us: 1.07x faster                                         |
| gc_traversal            | 3.95 ms                                                                | 3.69 ms: 1.07x faster                                         |
| go                      | 158 ms                                                                 | 149 ms: 1.06x faster                                          |
| pickle_dict             | 35.4 us                                                                | 33.7 us: 1.05x faster                                         |
| mdp                     | 2.75 sec                                                               | 2.63 sec: 1.05x faster                                        |
| async_generators        | 469 ms                                                                 | 453 ms: 1.04x faster                                          |
| pprint_safe_repr        | 779 ms                                                                 | 755 ms: 1.03x faster                                          |
| unpack_sequence         | 90.6 ns                                                                | 87.8 ns: 1.03x faster                                         |
| pickle                  | 12.0 us                                                                | 11.6 us: 1.03x faster                                         |
| genshi_text             | 24.7 ms                                                                | 24.0 ms: 1.03x faster                                         |
| scimark_lu              | 132 ms                                                                 | 129 ms: 1.03x faster                                          |
| spectral_norm           | 118 ms                                                                 | 115 ms: 1.03x faster                                          |
| regex_dna               | 238 ms                                                                 | 232 ms: 1.03x faster                                          |
| thrift                  | 811 us                                                                 | 794 us: 1.02x faster                                          |
| unpickle                | 15.1 us                                                                | 14.8 us: 1.02x faster                                         |
| pyflate                 | 490 ms                                                                 | 482 ms: 1.02x faster                                          |
| pprint_pformat          | 1.58 sec                                                               | 1.56 sec: 1.02x faster                                        |
| coroutines              | 22.7 ms                                                                | 22.4 ms: 1.01x faster                                         |
| meteor_contest          | 110 ms                                                                 | 109 ms: 1.01x faster                                          |
| pickle_pure_python      | 302 us                                                                 | 298 us: 1.01x faster                                          |
| dulwich_log             | 70.5 ms                                                                | 69.7 ms: 1.01x faster                                         |
| create_gc_cycles        | 1.52 ms                                                                | 1.50 ms: 1.01x faster                                         |
| unpickle_list           | 4.93 us                                                                | 4.89 us: 1.01x faster                                         |
| raytrace                | 294 ms                                                                 | 291 ms: 1.01x faster                                          |
| scimark_sor             | 130 ms                                                                 | 128 ms: 1.01x faster                                          |
| scimark_sparse_mat_mult | 4.91 ms                                                                | 4.88 ms: 1.01x faster                                         |
| logging_silent          | 102 ns                                                                 | 101 ns: 1.01x faster                                          |
| json                    | 5.16 ms                                                                | 5.12 ms: 1.01x faster                                         |
| hexiom                  | 7.09 ms                                                                | 7.04 ms: 1.01x faster                                         |
| sympy_sum               | 163 ms                                                                 | 162 ms: 1.01x faster                                          |
| nqueens                 | 90.5 ms                                                                | 90.0 ms: 1.01x faster                                         |
| generators              | 29.7 ms                                                                | 29.6 ms: 1.00x faster                                         |
| sqlglot_optimize        | 56.6 ms                                                                | 56.4 ms: 1.00x faster                                         |
| sympy_expand            | 487 ms                                                                 | 485 ms: 1.00x faster                                          |
| 2to3                    | 282 ms                                                                 | 281 ms: 1.00x faster                                          |
| regex_compile           | 144 ms                                                                 | 143 ms: 1.00x faster                                          |
| python_startup_no_site  | 11.2 ms                                                                | 11.1 ms: 1.00x faster                                         |
| python_startup          | 12.6 ms                                                                | 12.6 ms: 1.00x faster                                         |
| async_tree_none_tg      | 459 ms                                                                 | 458 ms: 1.00x faster                                          |
| unpickle_pure_python    | 239 us                                                                 | 238 us: 1.00x faster                                          |
| sqlite_synth            | 2.83 us                                                                | 2.85 us: 1.00x slower                                         |
| deepcopy_memo           | 39.5 us                                                                | 39.7 us: 1.01x slower                                         |
| json_loads              | 27.9 us                                                                | 28.0 us: 1.01x slower                                         |
| richards_super          | 52.2 ms                                                                | 52.5 ms: 1.01x slower                                         |
| deepcopy                | 354 us                                                                 | 356 us: 1.01x slower                                          |
| xml_etree_generate      | 86.8 ms                                                                | 87.4 ms: 1.01x slower                                         |
| json_dumps              | 10.4 ms                                                                | 10.5 ms: 1.01x slower                                         |
| pycparser               | 1.25 sec                                                               | 1.27 sec: 1.01x slower                                        |
| django_template         | 34.4 ms                                                                | 34.8 ms: 1.01x slower                                         |
| logging_simple          | 5.86 us                                                                | 5.92 us: 1.01x slower                                         |
| float                   | 79.8 ms                                                                | 80.6 ms: 1.01x slower                                         |
| nbody                   | 92.4 ms                                                                | 93.5 ms: 1.01x slower                                         |
| scimark_monte_carlo     | 70.1 ms                                                                | 71.0 ms: 1.01x slower                                         |
| mako                    | 10.7 ms                                                                | 10.9 ms: 1.02x slower                                         |
| chameleon               | 6.90 ms                                                                | 7.01 ms: 1.02x slower                                         |
| logging_format          | 6.46 us                                                                | 6.56 us: 1.02x slower                                         |
| telco                   | 8.42 ms                                                                | 8.56 ms: 1.02x slower                                         |
| regex_v8                | 25.4 ms                                                                | 26.1 ms: 1.03x slower                                         |
| html5lib                | 65.7 ms                                                                | 68.1 ms: 1.04x slower                                         |
| Geometric mean          | (ref)                                                                  | 1.00x faster                                                  |

Benchmark hidden because not significant (43): async_tree_none, bench_mp_pool, sympy_str, deltablue, async_tree_io, fannkuch, xml_etree_process, xml_etree_iterparse, async_tree_memoization, mypy2, tomli_loads, sympy_integrate, xml_etree_parse, pylint, asyncio_websockets, asyncio_tcp_ssl, pidigits, dask, sqlglot_normalize, sqlglot_transpile, richards, docutils, asyncio_tcp, async_tree_io_tg, genshi_xml, pathlib, aiohttp, tornado_http, comprehensions, bench_thread_pool, regex_effbot, gunicorn, async_tree_memoization_tg, sqlglot_parse, crypto_pyaes, coverage, deepcopy_reduce, typing_runtime_protocols, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, scimark_fft, chaos, djangocms


# HPT report

- Reliability score: 98.91% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x