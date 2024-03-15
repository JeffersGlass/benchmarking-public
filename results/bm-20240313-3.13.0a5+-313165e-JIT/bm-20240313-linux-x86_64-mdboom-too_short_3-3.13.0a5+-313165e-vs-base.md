# Results vs. base

- fork: mdboom
- ref: too_short_3
- machine: linux-x86_64
- commit hash: 313165e
- commit date: 2024-03-13
- overall geometric mean: 1.00x faster
- HPT reliability: 93.58%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------:|
| docutils       | 2.77 sec                                                               | 2.79 sec: 1.01x slower                                        |
| html5lib       | 65.7 ms                                                                | 67.1 ms: 1.02x slower                                         |
| tornado_http   | 98.7 ms                                                                | 101 ms: 1.03x slower                                          |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                  |

Benchmark hidden because not significant (2): 2to3, chameleon

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|-------------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------:|
| async_tree_io           | 1.22 sec                                                               | 1.20 sec: 1.02x faster                                        |
| async_tree_io_tg        | 1.24 sec                                                               | 1.22 sec: 1.01x faster                                        |
| async_tree_none_tg      | 459 ms                                                                 | 456 ms: 1.01x faster                                          |
| async_tree_cpu_io_mixed | 724 ms                                                                 | 733 ms: 1.01x slower                                          |
| Geometric mean          | (ref)                                                                  | 1.00x faster                                                  |

Benchmark hidden because not significant (4): async_tree_memoization, async_tree_memoization_tg, async_tree_cpu_io_mixed_tg, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------:|
| pidigits       | 189 ms                                                                 | 190 ms: 1.00x slower                                          |
| nbody          | 92.4 ms                                                                | 94.0 ms: 1.02x slower                                         |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                  |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------:|
| regex_dna      | 238 ms                                                                 | 220 ms: 1.08x faster                                          |
| regex_effbot   | 3.82 ms                                                                | 3.59 ms: 1.07x faster                                         |
| regex_v8       | 25.4 ms                                                                | 24.1 ms: 1.05x faster                                         |
| regex_compile  | 144 ms                                                                 | 142 ms: 1.01x faster                                          |
| Geometric mean | (ref)                                                                  | 1.05x faster                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|----------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------:|
| pickle_list          | 5.31 us                                                                | 4.99 us: 1.06x faster                                         |
| pickle_dict          | 35.4 us                                                                | 33.9 us: 1.04x faster                                         |
| pickle               | 12.0 us                                                                | 11.6 us: 1.04x faster                                         |
| unpickle             | 15.1 us                                                                | 14.7 us: 1.03x faster                                         |
| unpickle_list        | 4.93 us                                                                | 4.91 us: 1.00x faster                                         |
| json_dumps           | 10.4 ms                                                                | 10.5 ms: 1.01x slower                                         |
| xml_etree_parse      | 159 ms                                                                 | 161 ms: 1.01x slower                                          |
| xml_etree_generate   | 86.8 ms                                                                | 87.8 ms: 1.01x slower                                         |
| xml_etree_iterparse  | 107 ms                                                                 | 108 ms: 1.01x slower                                          |
| unpickle_pure_python | 239 us                                                                 | 243 us: 1.02x slower                                          |
| tomli_loads          | 2.08 sec                                                               | 2.12 sec: 1.02x slower                                        |
| Geometric mean       | (ref)                                                                  | 1.01x faster                                                  |

Benchmark hidden because not significant (3): xml_etree_process, pickle_pure_python, json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|------------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------:|
| python_startup_no_site | 11.2 ms                                                                | 11.1 ms: 1.00x faster                                         |
| python_startup         | 12.6 ms                                                                | 12.6 ms: 1.00x faster                                         |
| Geometric mean         | (ref)                                                                  | 1.00x faster                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark      | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------:|
| genshi_text    | 24.7 ms                                                                | 24.2 ms: 1.02x faster                                         |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                  |

Benchmark hidden because not significant (3): genshi_xml, mako, django_template

All benchmarks:
===============

| Benchmark                | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|--------------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------:|
| regex_dna                | 238 ms                                                                 | 220 ms: 1.08x faster                                          |
| gc_traversal             | 3.95 ms                                                                | 3.69 ms: 1.07x faster                                         |
| regex_effbot             | 3.82 ms                                                                | 3.59 ms: 1.07x faster                                         |
| pickle_list              | 5.31 us                                                                | 4.99 us: 1.06x faster                                         |
| regex_v8                 | 25.4 ms                                                                | 24.1 ms: 1.05x faster                                         |
| mdp                      | 2.75 sec                                                               | 2.62 sec: 1.05x faster                                        |
| pickle_dict              | 35.4 us                                                                | 33.9 us: 1.04x faster                                         |
| pickle                   | 12.0 us                                                                | 11.6 us: 1.04x faster                                         |
| unpack_sequence          | 90.6 ns                                                                | 87.5 ns: 1.04x faster                                         |
| spectral_norm            | 118 ms                                                                 | 114 ms: 1.04x faster                                          |
| pycparser                | 1.25 sec                                                               | 1.22 sec: 1.03x faster                                        |
| unpickle                 | 15.1 us                                                                | 14.7 us: 1.03x faster                                         |
| thrift                   | 811 us                                                                 | 794 us: 1.02x faster                                          |
| genshi_text              | 24.7 ms                                                                | 24.2 ms: 1.02x faster                                         |
| djangocms                | 32.2 us                                                                | 31.6 us: 1.02x faster                                         |
| scimark_sparse_mat_mult  | 4.91 ms                                                                | 4.83 ms: 1.02x faster                                         |
| async_tree_io            | 1.22 sec                                                               | 1.20 sec: 1.02x faster                                        |
| pprint_pformat           | 1.58 sec                                                               | 1.56 sec: 1.02x faster                                        |
| raytrace                 | 294 ms                                                                 | 290 ms: 1.01x faster                                          |
| pyflate                  | 490 ms                                                                 | 486 ms: 1.01x faster                                          |
| async_tree_io_tg         | 1.24 sec                                                               | 1.22 sec: 1.01x faster                                        |
| regex_compile            | 144 ms                                                                 | 142 ms: 1.01x faster                                          |
| deepcopy_memo            | 39.5 us                                                                | 39.1 us: 1.01x faster                                         |
| nqueens                  | 90.5 ms                                                                | 89.7 ms: 1.01x faster                                         |
| logging_format           | 6.46 us                                                                | 6.40 us: 1.01x faster                                         |
| scimark_lu               | 132 ms                                                                 | 131 ms: 1.01x faster                                          |
| async_tree_none_tg       | 459 ms                                                                 | 456 ms: 1.01x faster                                          |
| unpickle_list            | 4.93 us                                                                | 4.91 us: 1.00x faster                                         |
| dulwich_log              | 70.5 ms                                                                | 70.2 ms: 1.00x faster                                         |
| deepcopy                 | 354 us                                                                 | 352 us: 1.00x faster                                          |
| create_gc_cycles         | 1.52 ms                                                                | 1.51 ms: 1.00x faster                                         |
| asyncio_tcp_ssl          | 1.85 sec                                                               | 1.85 sec: 1.00x faster                                        |
| hexiom                   | 7.09 ms                                                                | 7.06 ms: 1.00x faster                                         |
| generators               | 29.7 ms                                                                | 29.6 ms: 1.00x faster                                         |
| coroutines               | 22.7 ms                                                                | 22.7 ms: 1.00x faster                                         |
| python_startup_no_site   | 11.2 ms                                                                | 11.1 ms: 1.00x faster                                         |
| python_startup           | 12.6 ms                                                                | 12.6 ms: 1.00x faster                                         |
| bench_thread_pool        | 862 us                                                                 | 866 us: 1.00x slower                                          |
| pidigits                 | 189 ms                                                                 | 190 ms: 1.00x slower                                          |
| meteor_contest           | 110 ms                                                                 | 111 ms: 1.01x slower                                          |
| sqlglot_optimize         | 56.6 ms                                                                | 56.9 ms: 1.01x slower                                         |
| docutils                 | 2.77 sec                                                               | 2.79 sec: 1.01x slower                                        |
| gunicorn                 | 1.30 ms                                                                | 1.30 ms: 1.01x slower                                         |
| async_generators         | 469 ms                                                                 | 472 ms: 1.01x slower                                          |
| json_dumps               | 10.4 ms                                                                | 10.5 ms: 1.01x slower                                         |
| deltablue                | 3.44 ms                                                                | 3.47 ms: 1.01x slower                                         |
| aiohttp                  | 1.20 ms                                                                | 1.21 ms: 1.01x slower                                         |
| xml_etree_parse          | 159 ms                                                                 | 161 ms: 1.01x slower                                          |
| deepcopy_reduce          | 3.09 us                                                                | 3.12 us: 1.01x slower                                         |
| xml_etree_generate       | 86.8 ms                                                                | 87.8 ms: 1.01x slower                                         |
| xml_etree_iterparse      | 107 ms                                                                 | 108 ms: 1.01x slower                                          |
| async_tree_cpu_io_mixed  | 724 ms                                                                 | 733 ms: 1.01x slower                                          |
| logging_silent           | 102 ns                                                                 | 103 ns: 1.01x slower                                          |
| sqlglot_normalize        | 108 ms                                                                 | 110 ms: 1.02x slower                                          |
| chaos                    | 64.1 ms                                                                | 65.1 ms: 1.02x slower                                         |
| typing_runtime_protocols | 110 us                                                                 | 112 us: 1.02x slower                                          |
| unpickle_pure_python     | 239 us                                                                 | 243 us: 1.02x slower                                          |
| nbody                    | 92.4 ms                                                                | 94.0 ms: 1.02x slower                                         |
| sympy_integrate          | 21.2 ms                                                                | 21.6 ms: 1.02x slower                                         |
| html5lib                 | 65.7 ms                                                                | 67.1 ms: 1.02x slower                                         |
| richards_super           | 52.2 ms                                                                | 53.3 ms: 1.02x slower                                         |
| tomli_loads              | 2.08 sec                                                               | 2.12 sec: 1.02x slower                                        |
| scimark_monte_carlo      | 70.1 ms                                                                | 71.8 ms: 1.03x slower                                         |
| tornado_http             | 98.7 ms                                                                | 101 ms: 1.03x slower                                          |
| richards                 | 46.5 ms                                                                | 48.0 ms: 1.03x slower                                         |
| Geometric mean           | (ref)                                                                  | 1.00x faster                                                  |

Benchmark hidden because not significant (37): async_tree_memoization, async_tree_memoization_tg, chameleon, pprint_safe_repr, genshi_xml, scimark_sor, bench_mp_pool, scimark_fft, asyncio_websockets, async_tree_cpu_io_mixed_tg, telco, coverage, sympy_sum, go, dask, xml_etree_process, asyncio_tcp, 2to3, logging_simple, pickle_pure_python, sqlglot_transpile, sympy_expand, mako, float, sqlite_synth, sympy_str, pathlib, crypto_pyaes, django_template, fannkuch, sqlglot_parse, mypy2, comprehensions, pylint, json_loads, async_tree_none, json


# HPT report

- Reliability score: 93.58% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x