# Results vs. base

- fork: mdboom
- ref: estimate_too_short
- machine: linux-x86_64
- commit hash: c3a9b5a
- commit date: 2024-03-14
- overall geometric mean: 1.00x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240314-linux-x86_64-python-2a54c4b25e05e30c50b9-3.13.0a5+-2a54c4b | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 282 ms                                                                 | 280 ms: 1.01x faster                                                 |
| chameleon      | 6.78 ms                                                                | 7.00 ms: 1.03x slower                                                |
| docutils       | 2.77 sec                                                               | 2.72 sec: 1.02x faster                                               |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                         |

Benchmark hidden because not significant (2): html5lib, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20240314-linux-x86_64-python-2a54c4b25e05e30c50b9-3.13.0a5+-2a54c4b | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|--------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none_tg | 461 ms                                                                 | 458 ms: 1.01x faster                                                 |
| async_tree_io      | 1.20 sec                                                               | 1.20 sec: 1.00x slower                                               |
| Geometric mean     | (ref)                                                                  | 1.00x faster                                                         |

Benchmark hidden because not significant (6): async_tree_none, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed, async_tree_memoization_tg, async_tree_io_tg, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240314-linux-x86_64-python-2a54c4b25e05e30c50b9-3.13.0a5+-2a54c4b | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| nbody          | 93.9 ms                                                                | 93.1 ms: 1.01x faster                                                |
| pidigits       | 190 ms                                                                 | 189 ms: 1.00x faster                                                 |
| float          | 80.3 ms                                                                | 81.3 ms: 1.01x slower                                                |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240314-linux-x86_64-python-2a54c4b25e05e30c50b9-3.13.0a5+-2a54c4b | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 144 ms                                                                 | 142 ms: 1.01x faster                                                 |
| regex_v8       | 25.5 ms                                                                | 25.7 ms: 1.01x slower                                                |
| regex_effbot   | 3.69 ms                                                                | 3.83 ms: 1.04x slower                                                |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                         |

Benchmark hidden because not significant (1): regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240314-linux-x86_64-python-2a54c4b25e05e30c50b9-3.13.0a5+-2a54c4b | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| xml_etree_generate   | 88.4 ms                                                                | 86.9 ms: 1.02x faster                                                |
| xml_etree_iterparse  | 108 ms                                                                 | 107 ms: 1.01x faster                                                 |
| unpickle_list        | 4.92 us                                                                | 4.88 us: 1.01x faster                                                |
| xml_etree_process    | 60.2 ms                                                                | 59.7 ms: 1.01x faster                                                |
| json_dumps           | 10.6 ms                                                                | 10.5 ms: 1.01x faster                                                |
| tomli_loads          | 2.07 sec                                                               | 2.05 sec: 1.01x faster                                               |
| unpickle_pure_python | 238 us                                                                 | 237 us: 1.00x faster                                                 |
| pickle_list          | 5.08 us                                                                | 5.10 us: 1.00x slower                                                |
| pickle_pure_python   | 300 us                                                                 | 304 us: 1.01x slower                                                 |
| unpickle             | 14.6 us                                                                | 15.0 us: 1.03x slower                                                |
| Geometric mean       | (ref)                                                                  | 1.00x faster                                                         |

Benchmark hidden because not significant (4): xml_etree_parse, pickle_dict, json_loads, pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240314-linux-x86_64-python-2a54c4b25e05e30c50b9-3.13.0a5+-2a54c4b | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup_no_site | 11.1 ms                                                                | 11.2 ms: 1.00x slower                                                |
| Geometric mean         | (ref)                                                                  | 1.00x slower                                                         |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20240314-linux-x86_64-python-2a54c4b25e05e30c50b9-3.13.0a5+-2a54c4b | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|-----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| genshi_xml      | 54.7 ms                                                                | 53.5 ms: 1.02x faster                                                |
| genshi_text     | 24.1 ms                                                                | 23.7 ms: 1.01x faster                                                |
| django_template | 34.2 ms                                                                | 33.9 ms: 1.01x faster                                                |
| mako            | 10.8 ms                                                                | 10.9 ms: 1.01x slower                                                |
| Geometric mean  | (ref)                                                                  | 1.01x faster                                                         |

All benchmarks:
===============

| Benchmark                | bm-20240314-linux-x86_64-python-2a54c4b25e05e30c50b9-3.13.0a5+-2a54c4b | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|--------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| gc_traversal             | 4.08 ms                                                                | 3.59 ms: 1.14x faster                                                |
| nqueens                  | 91.3 ms                                                                | 81.8 ms: 1.12x faster                                                |
| hexiom                   | 7.00 ms                                                                | 6.74 ms: 1.04x faster                                                |
| pycparser                | 1.26 sec                                                               | 1.21 sec: 1.04x faster                                               |
| deepcopy_memo            | 38.9 us                                                                | 37.5 us: 1.04x faster                                                |
| deepcopy_reduce          | 3.11 us                                                                | 3.01 us: 1.03x faster                                                |
| raytrace                 | 295 ms                                                                 | 286 ms: 1.03x faster                                                 |
| deepcopy                 | 352 us                                                                 | 342 us: 1.03x faster                                                 |
| telco                    | 8.58 ms                                                                | 8.33 ms: 1.03x faster                                                |
| djangocms                | 32.1 us                                                                | 31.3 us: 1.03x faster                                                |
| sqlglot_normalize        | 110 ms                                                                 | 107 ms: 1.02x faster                                                 |
| richards_super           | 53.2 ms                                                                | 52.0 ms: 1.02x faster                                                |
| genshi_xml               | 54.7 ms                                                                | 53.5 ms: 1.02x faster                                                |
| json                     | 5.26 ms                                                                | 5.14 ms: 1.02x faster                                                |
| docutils                 | 2.77 sec                                                               | 2.72 sec: 1.02x faster                                               |
| spectral_norm            | 114 ms                                                                 | 111 ms: 1.02x faster                                                 |
| xml_etree_generate       | 88.4 ms                                                                | 86.9 ms: 1.02x faster                                                |
| sympy_integrate          | 21.2 ms                                                                | 20.8 ms: 1.02x faster                                                |
| sqlglot_transpile        | 1.67 ms                                                                | 1.64 ms: 1.02x faster                                                |
| pathlib                  | 18.7 ms                                                                | 18.4 ms: 1.02x faster                                                |
| genshi_text              | 24.1 ms                                                                | 23.7 ms: 1.01x faster                                                |
| typing_runtime_protocols | 111 us                                                                 | 109 us: 1.01x faster                                                 |
| coverage                 | 97.2 ms                                                                | 96.0 ms: 1.01x faster                                                |
| richards                 | 46.5 ms                                                                | 45.9 ms: 1.01x faster                                                |
| xml_etree_iterparse      | 108 ms                                                                 | 107 ms: 1.01x faster                                                 |
| scimark_lu               | 132 ms                                                                 | 130 ms: 1.01x faster                                                 |
| regex_compile            | 144 ms                                                                 | 142 ms: 1.01x faster                                                 |
| sympy_str                | 286 ms                                                                 | 283 ms: 1.01x faster                                                 |
| sqlglot_optimize         | 56.7 ms                                                                | 56.2 ms: 1.01x faster                                                |
| dulwich_log              | 70.0 ms                                                                | 69.4 ms: 1.01x faster                                                |
| nbody                    | 93.9 ms                                                                | 93.1 ms: 1.01x faster                                                |
| django_template          | 34.2 ms                                                                | 33.9 ms: 1.01x faster                                                |
| bench_thread_pool        | 864 us                                                                 | 857 us: 1.01x faster                                                 |
| go                       | 157 ms                                                                 | 156 ms: 1.01x faster                                                 |
| unpickle_list            | 4.92 us                                                                | 4.88 us: 1.01x faster                                                |
| async_tree_none_tg       | 461 ms                                                                 | 458 ms: 1.01x faster                                                 |
| gunicorn                 | 1.30 ms                                                                | 1.29 ms: 1.01x faster                                                |
| xml_etree_process        | 60.2 ms                                                                | 59.7 ms: 1.01x faster                                                |
| 2to3                     | 282 ms                                                                 | 280 ms: 1.01x faster                                                 |
| sympy_sum                | 161 ms                                                                 | 160 ms: 1.01x faster                                                 |
| sqlglot_parse            | 1.32 ms                                                                | 1.31 ms: 1.01x faster                                                |
| json_dumps               | 10.6 ms                                                                | 10.5 ms: 1.01x faster                                                |
| comprehensions           | 17.3 us                                                                | 17.2 us: 1.01x faster                                                |
| tomli_loads              | 2.07 sec                                                               | 2.05 sec: 1.01x faster                                               |
| chaos                    | 63.9 ms                                                                | 63.6 ms: 1.01x faster                                                |
| unpickle_pure_python     | 238 us                                                                 | 237 us: 1.00x faster                                                 |
| sympy_expand             | 486 ms                                                                 | 484 ms: 1.00x faster                                                 |
| asyncio_tcp              | 512 ms                                                                 | 510 ms: 1.00x faster                                                 |
| pidigits                 | 190 ms                                                                 | 189 ms: 1.00x faster                                                 |
| python_startup_no_site   | 11.1 ms                                                                | 11.2 ms: 1.00x slower                                                |
| async_tree_io            | 1.20 sec                                                               | 1.20 sec: 1.00x slower                                               |
| pickle_list              | 5.08 us                                                                | 5.10 us: 1.00x slower                                                |
| meteor_contest           | 110 ms                                                                 | 110 ms: 1.00x slower                                                 |
| regex_v8                 | 25.5 ms                                                                | 25.7 ms: 1.01x slower                                                |
| create_gc_cycles         | 1.51 ms                                                                | 1.52 ms: 1.01x slower                                                |
| mako                     | 10.8 ms                                                                | 10.9 ms: 1.01x slower                                                |
| unpack_sequence          | 91.9 ns                                                                | 92.9 ns: 1.01x slower                                                |
| logging_simple           | 5.80 us                                                                | 5.86 us: 1.01x slower                                                |
| sqlite_synth             | 2.86 us                                                                | 2.89 us: 1.01x slower                                                |
| float                    | 80.3 ms                                                                | 81.3 ms: 1.01x slower                                                |
| logging_format           | 6.44 us                                                                | 6.53 us: 1.01x slower                                                |
| scimark_fft              | 343 ms                                                                 | 347 ms: 1.01x slower                                                 |
| pickle_pure_python       | 300 us                                                                 | 304 us: 1.01x slower                                                 |
| pyflate                  | 484 ms                                                                 | 492 ms: 1.02x slower                                                 |
| fannkuch                 | 395 ms                                                                 | 401 ms: 1.02x slower                                                 |
| unpickle                 | 14.6 us                                                                | 15.0 us: 1.03x slower                                                |
| logging_silent           | 98.7 ns                                                                | 102 ns: 1.03x slower                                                 |
| chameleon                | 6.78 ms                                                                | 7.00 ms: 1.03x slower                                                |
| mdp                      | 2.64 sec                                                               | 2.74 sec: 1.04x slower                                               |
| regex_effbot             | 3.69 ms                                                                | 3.83 ms: 1.04x slower                                                |
| scimark_sor              | 126 ms                                                                 | 138 ms: 1.09x slower                                                 |
| deltablue                | 3.43 ms                                                                | 3.75 ms: 1.09x slower                                                |
| Geometric mean           | (ref)                                                                  | 1.00x faster                                                         |

Benchmark hidden because not significant (30): pprint_safe_repr, pylint, async_tree_none, mypy2, aiohttp, pprint_pformat, tornado_http, xml_etree_parse, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed, coroutines, dask, crypto_pyaes, regex_dna, async_tree_memoization_tg, pickle_dict, asyncio_tcp_ssl, json_loads, async_tree_io_tg, asyncio_websockets, bench_mp_pool, html5lib, python_startup, async_generators, generators, thrift, scimark_sparse_mat_mult, pickle, scimark_monte_carlo, async_tree_memoization


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.99x