# Results vs. base

- fork: gvanrossum
- ref: kenjin_tier2_inliner
- machine: linux-x86_64
- commit hash: 2f9539b
- commit date: 2024-03-05
- overall geometric mean: 1.00x slower
- HPT reliability: 56.30%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

Benchmark hidden because not significant (5): 2to3, chameleon, docutils, html5lib, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark        | bm-20240305-linux-x86_64-python-23db9c62272f7470aadf-3.13.0a4+-23db9c6 | bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4+-2f9539b |
|------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_io_tg | 1.18 sec                                                               | 1.21 sec: 1.02x slower                                                     |
| Geometric mean   | (ref)                                                                  | 1.00x slower                                                               |

Benchmark hidden because not significant (7): async_tree_memoization_tg, async_tree_cpu_io_mixed_tg, async_tree_none, async_tree_cpu_io_mixed, async_tree_none_tg, async_tree_io, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240305-linux-x86_64-python-23db9c62272f7470aadf-3.13.0a4+-23db9c6 | bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4+-2f9539b |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| float          | 78.8 ms                                                                | 78.2 ms: 1.01x faster                                                      |
| pidigits       | 187 ms                                                                 | 187 ms: 1.00x faster                                                       |
| nbody          | 92.2 ms                                                                | 95.8 ms: 1.04x slower                                                      |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240305-linux-x86_64-python-23db9c62272f7470aadf-3.13.0a4+-23db9c6 | bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4+-2f9539b |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_effbot   | 3.81 ms                                                                | 3.73 ms: 1.02x faster                                                      |
| regex_dna      | 223 ms                                                                 | 223 ms: 1.00x faster                                                       |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                               |

Benchmark hidden because not significant (2): regex_v8, regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240305-linux-x86_64-python-23db9c62272f7470aadf-3.13.0a4+-23db9c6 | bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4+-2f9539b |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle_pure_python   | 304 us                                                                 | 298 us: 1.02x faster                                                       |
| pickle               | 11.6 us                                                                | 11.5 us: 1.01x faster                                                      |
| xml_etree_process    | 58.6 ms                                                                | 59.0 ms: 1.01x slower                                                      |
| json_dumps           | 10.3 ms                                                                | 10.4 ms: 1.01x slower                                                      |
| unpickle_pure_python | 236 us                                                                 | 238 us: 1.01x slower                                                       |
| xml_etree_generate   | 85.8 ms                                                                | 86.8 ms: 1.01x slower                                                      |
| unpickle_list        | 4.91 us                                                                | 4.97 us: 1.01x slower                                                      |
| pickle_dict          | 34.0 us                                                                | 34.6 us: 1.02x slower                                                      |
| pickle_list          | 4.93 us                                                                | 5.23 us: 1.06x slower                                                      |
| Geometric mean       | (ref)                                                                  | 1.01x slower                                                               |

Benchmark hidden because not significant (5): xml_etree_parse, json_loads, xml_etree_iterparse, tomli_loads, unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240305-linux-x86_64-python-23db9c62272f7470aadf-3.13.0a4+-23db9c6 | bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4+-2f9539b |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 12.3 ms                                                                | 12.4 ms: 1.00x slower                                                      |
| python_startup_no_site | 10.9 ms                                                                | 11.0 ms: 1.01x slower                                                      |
| Geometric mean         | (ref)                                                                  | 1.01x slower                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark      | bm-20240305-linux-x86_64-python-23db9c62272f7470aadf-3.13.0a4+-23db9c6 | bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4+-2f9539b |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako           | 10.9 ms                                                                | 10.7 ms: 1.01x faster                                                      |
| genshi_text    | 24.1 ms                                                                | 24.0 ms: 1.01x faster                                                      |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                               |

Benchmark hidden because not significant (2): django_template, genshi_xml

All benchmarks:
===============

| Benchmark                | bm-20240305-linux-x86_64-python-23db9c62272f7470aadf-3.13.0a4+-23db9c6 | bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4+-2f9539b |
|--------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_effbot             | 3.81 ms                                                                | 3.73 ms: 1.02x faster                                                      |
| pickle_pure_python       | 304 us                                                                 | 298 us: 1.02x faster                                                       |
| coroutines               | 22.9 ms                                                                | 22.5 ms: 1.02x faster                                                      |
| pprint_safe_repr         | 756 ms                                                                 | 745 ms: 1.02x faster                                                       |
| logging_simple           | 5.71 us                                                                | 5.64 us: 1.01x faster                                                      |
| mdp                      | 2.63 sec                                                               | 2.60 sec: 1.01x faster                                                     |
| mako                     | 10.9 ms                                                                | 10.7 ms: 1.01x faster                                                      |
| aiohttp                  | 1.18 ms                                                                | 1.16 ms: 1.01x faster                                                      |
| sqlglot_parse            | 1.29 ms                                                                | 1.28 ms: 1.01x faster                                                      |
| pathlib                  | 18.7 ms                                                                | 18.4 ms: 1.01x faster                                                      |
| sqlglot_transpile        | 1.64 ms                                                                | 1.62 ms: 1.01x faster                                                      |
| pickle                   | 11.6 us                                                                | 11.5 us: 1.01x faster                                                      |
| sympy_sum                | 158 ms                                                                 | 157 ms: 1.01x faster                                                       |
| sympy_str                | 282 ms                                                                 | 279 ms: 1.01x faster                                                       |
| float                    | 78.8 ms                                                                | 78.2 ms: 1.01x faster                                                      |
| sqlite_synth             | 2.83 us                                                                | 2.81 us: 1.01x faster                                                      |
| genshi_text              | 24.1 ms                                                                | 24.0 ms: 1.01x faster                                                      |
| sympy_expand             | 477 ms                                                                 | 474 ms: 1.01x faster                                                       |
| sympy_integrate          | 21.0 ms                                                                | 20.9 ms: 1.01x faster                                                      |
| sqlglot_optimize         | 55.8 ms                                                                | 55.6 ms: 1.00x faster                                                      |
| create_gc_cycles         | 1.50 ms                                                                | 1.50 ms: 1.00x faster                                                      |
| regex_dna                | 223 ms                                                                 | 223 ms: 1.00x faster                                                       |
| pidigits                 | 187 ms                                                                 | 187 ms: 1.00x faster                                                       |
| asyncio_tcp              | 488 ms                                                                 | 487 ms: 1.00x faster                                                       |
| bench_thread_pool        | 844 us                                                                 | 846 us: 1.00x slower                                                       |
| python_startup           | 12.3 ms                                                                | 12.4 ms: 1.00x slower                                                      |
| async_generators         | 460 ms                                                                 | 463 ms: 1.01x slower                                                       |
| sqlglot_normalize        | 106 ms                                                                 | 107 ms: 1.01x slower                                                       |
| python_startup_no_site   | 10.9 ms                                                                | 11.0 ms: 1.01x slower                                                      |
| xml_etree_process        | 58.6 ms                                                                | 59.0 ms: 1.01x slower                                                      |
| meteor_contest           | 107 ms                                                                 | 107 ms: 1.01x slower                                                       |
| richards_super           | 51.5 ms                                                                | 51.8 ms: 1.01x slower                                                      |
| dulwich_log              | 68.5 ms                                                                | 68.9 ms: 1.01x slower                                                      |
| hexiom                   | 6.95 ms                                                                | 7.00 ms: 1.01x slower                                                      |
| json_dumps               | 10.3 ms                                                                | 10.4 ms: 1.01x slower                                                      |
| unpickle_pure_python     | 236 us                                                                 | 238 us: 1.01x slower                                                       |
| deepcopy                 | 350 us                                                                 | 353 us: 1.01x slower                                                       |
| xml_etree_generate       | 85.8 ms                                                                | 86.8 ms: 1.01x slower                                                      |
| scimark_monte_carlo      | 69.8 ms                                                                | 70.6 ms: 1.01x slower                                                      |
| spectral_norm            | 112 ms                                                                 | 113 ms: 1.01x slower                                                       |
| unpickle_list            | 4.91 us                                                                | 4.97 us: 1.01x slower                                                      |
| scimark_lu               | 128 ms                                                                 | 130 ms: 1.02x slower                                                       |
| pickle_dict              | 34.0 us                                                                | 34.6 us: 1.02x slower                                                      |
| async_tree_io_tg         | 1.18 sec                                                               | 1.21 sec: 1.02x slower                                                     |
| comprehensions           | 17.1 us                                                                | 17.5 us: 1.02x slower                                                      |
| scimark_fft              | 334 ms                                                                 | 342 ms: 1.02x slower                                                       |
| typing_runtime_protocols | 109 us                                                                 | 112 us: 1.03x slower                                                       |
| telco                    | 8.24 ms                                                                | 8.48 ms: 1.03x slower                                                      |
| unpack_sequence          | 93.7 ns                                                                | 96.7 ns: 1.03x slower                                                      |
| scimark_sor              | 126 ms                                                                 | 130 ms: 1.03x slower                                                       |
| pycparser                | 1.17 sec                                                               | 1.22 sec: 1.04x slower                                                     |
| nbody                    | 92.2 ms                                                                | 95.8 ms: 1.04x slower                                                      |
| scimark_sparse_mat_mult  | 4.81 ms                                                                | 5.02 ms: 1.04x slower                                                      |
| pickle_list              | 4.93 us                                                                | 5.23 us: 1.06x slower                                                      |
| gc_traversal             | 3.76 ms                                                                | 4.03 ms: 1.07x slower                                                      |
| Geometric mean           | (ref)                                                                  | 1.00x slower                                                               |

Benchmark hidden because not significant (47): nqueens, async_tree_memoization_tg, djangocms, async_tree_cpu_io_mixed_tg, deepcopy_reduce, async_tree_none, tornado_http, async_tree_cpu_io_mixed, html5lib, fannkuch, pyflate, gunicorn, crypto_pyaes, django_template, pylint, raytrace, logging_format, richards, xml_etree_parse, regex_v8, json_loads, 2to3, pprint_pformat, asyncio_websockets, regex_compile, go, asyncio_tcp_ssl, xml_etree_iterparse, tomli_loads, bench_mp_pool, coverage, docutils, dask, async_tree_none_tg, mypy2, genshi_xml, generators, deepcopy_memo, unpickle, chaos, chameleon, async_tree_io, thrift, deltablue, logging_silent, async_tree_memoization, json


# HPT report

- Reliability score: 56.30% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x