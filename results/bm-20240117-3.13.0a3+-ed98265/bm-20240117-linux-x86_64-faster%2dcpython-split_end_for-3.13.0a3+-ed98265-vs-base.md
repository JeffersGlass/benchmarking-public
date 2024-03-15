# Results vs. base

- fork: faster-cpython
- ref: split_end_for
- machine: linux-x86_64
- commit hash: ed98265
- commit date: 2024-01-17
- overall geometric mean: 1.00x slower
- HPT reliability: 76.26%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| chameleon      | 6.86 ms                                                                | 6.74 ms: 1.02x faster                                                     |
| docutils       | 2.60 sec                                                               | 2.61 sec: 1.01x slower                                                    |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                              |

Benchmark hidden because not significant (2): 2to3, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark        | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_io_tg | 1.19 sec                                                               | 1.19 sec: 1.00x slower                                                    |
| async_tree_io    | 1.17 sec                                                               | 1.18 sec: 1.01x slower                                                    |
| Geometric mean   | (ref)                                                                  | 1.00x slower                                                              |

Benchmark hidden because not significant (6): async_tree_none_tg, async_tree_memoization_tg, async_tree_memoization, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| float          | 80.3 ms                                                                | 79.2 ms: 1.01x faster                                                     |
| pidigits       | 187 ms                                                                 | 188 ms: 1.00x slower                                                      |
| nbody          | 86.2 ms                                                                | 86.6 ms: 1.00x slower                                                     |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                                 | 129 ms: 1.00x faster                                                      |
| regex_v8       | 25.1 ms                                                                | 25.5 ms: 1.02x slower                                                     |
| regex_dna      | 219 ms                                                                 | 223 ms: 1.02x slower                                                      |
| regex_effbot   | 3.63 ms                                                                | 3.71 ms: 1.02x slower                                                     |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|----------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| unpickle_pure_python | 213 us                                                                 | 211 us: 1.01x faster                                                      |
| json_loads           | 28.3 us                                                                | 28.1 us: 1.00x faster                                                     |
| xml_etree_process    | 58.8 ms                                                                | 58.5 ms: 1.00x faster                                                     |
| pickle_dict          | 34.8 us                                                                | 34.9 us: 1.00x slower                                                     |
| tomli_loads          | 2.10 sec                                                               | 2.11 sec: 1.01x slower                                                    |
| json_dumps           | 10.3 ms                                                                | 10.5 ms: 1.01x slower                                                     |
| pickle               | 11.7 us                                                                | 11.8 us: 1.01x slower                                                     |
| pickle_list          | 5.17 us                                                                | 5.25 us: 1.02x slower                                                     |
| unpickle_list        | 5.04 us                                                                | 5.16 us: 1.02x slower                                                     |
| unpickle             | 15.0 us                                                                | 15.9 us: 1.06x slower                                                     |
| Geometric mean       | (ref)                                                                  | 1.01x slower                                                              |

Benchmark hidden because not significant (4): xml_etree_parse, xml_etree_iterparse, xml_etree_generate, pickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|------------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                | 10.1 ms: 1.00x faster                                                     |
| python_startup_no_site | 8.73 ms                                                                | 8.69 ms: 1.00x faster                                                     |
| Geometric mean         | (ref)                                                                  | 1.00x faster                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|-----------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| mako      | 11.1 ms                                                                | 11.2 ms: 1.01x slower                                                     |

All benchmarks:
===============

| Benchmark                | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|--------------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| gc_traversal             | 3.86 ms                                                                | 3.47 ms: 1.11x faster                                                     |
| hexiom                   | 6.09 ms                                                                | 5.97 ms: 1.02x faster                                                     |
| pyflate                  | 457 ms                                                                 | 448 ms: 1.02x faster                                                      |
| chameleon                | 6.86 ms                                                                | 6.74 ms: 1.02x faster                                                     |
| pprint_safe_repr         | 728 ms                                                                 | 717 ms: 1.02x faster                                                      |
| pprint_pformat           | 1.49 sec                                                               | 1.47 sec: 1.02x faster                                                    |
| create_gc_cycles         | 1.49 ms                                                                | 1.47 ms: 1.02x faster                                                     |
| unpack_sequence          | 44.9 ns                                                                | 44.3 ns: 1.01x faster                                                     |
| float                    | 80.3 ms                                                                | 79.2 ms: 1.01x faster                                                     |
| raytrace                 | 260 ms                                                                 | 258 ms: 1.01x faster                                                      |
| logging_format           | 6.27 us                                                                | 6.20 us: 1.01x faster                                                     |
| dulwich_log              | 65.5 ms                                                                | 64.8 ms: 1.01x faster                                                     |
| meteor_contest           | 107 ms                                                                 | 106 ms: 1.01x faster                                                      |
| sqlglot_normalize        | 108 ms                                                                 | 107 ms: 1.01x faster                                                      |
| unpickle_pure_python     | 213 us                                                                 | 211 us: 1.01x faster                                                      |
| sqlglot_parse            | 1.25 ms                                                                | 1.24 ms: 1.01x faster                                                     |
| json                     | 5.16 ms                                                                | 5.12 ms: 1.01x faster                                                     |
| logging_simple           | 5.70 us                                                                | 5.65 us: 1.01x faster                                                     |
| pathlib                  | 18.2 ms                                                                | 18.1 ms: 1.01x faster                                                     |
| bench_thread_pool        | 828 us                                                                 | 823 us: 1.01x faster                                                      |
| coroutines               | 22.7 ms                                                                | 22.6 ms: 1.01x faster                                                     |
| sqlglot_transpile        | 1.57 ms                                                                | 1.56 ms: 1.01x faster                                                     |
| go                       | 138 ms                                                                 | 137 ms: 1.01x faster                                                      |
| async_generators         | 446 ms                                                                 | 443 ms: 1.01x faster                                                      |
| pycparser                | 1.20 sec                                                               | 1.20 sec: 1.01x faster                                                    |
| python_startup           | 10.1 ms                                                                | 10.1 ms: 1.00x faster                                                     |
| json_loads               | 28.3 us                                                                | 28.1 us: 1.00x faster                                                     |
| sqlglot_optimize         | 54.1 ms                                                                | 53.8 ms: 1.00x faster                                                     |
| python_startup_no_site   | 8.73 ms                                                                | 8.69 ms: 1.00x faster                                                     |
| xml_etree_process        | 58.8 ms                                                                | 58.5 ms: 1.00x faster                                                     |
| sympy_sum                | 148 ms                                                                 | 147 ms: 1.00x faster                                                      |
| regex_compile            | 129 ms                                                                 | 129 ms: 1.00x faster                                                      |
| asyncio_tcp_ssl          | 1.79 sec                                                               | 1.78 sec: 1.00x faster                                                    |
| asyncio_tcp              | 481 ms                                                                 | 482 ms: 1.00x slower                                                      |
| pickle_dict              | 34.8 us                                                                | 34.9 us: 1.00x slower                                                     |
| pidigits                 | 187 ms                                                                 | 188 ms: 1.00x slower                                                      |
| async_tree_io_tg         | 1.19 sec                                                               | 1.19 sec: 1.00x slower                                                    |
| nbody                    | 86.2 ms                                                                | 86.6 ms: 1.00x slower                                                     |
| tomli_loads              | 2.10 sec                                                               | 2.11 sec: 1.01x slower                                                    |
| coverage                 | 94.9 ms                                                                | 95.5 ms: 1.01x slower                                                     |
| async_tree_io            | 1.17 sec                                                               | 1.18 sec: 1.01x slower                                                    |
| chaos                    | 58.5 ms                                                                | 58.8 ms: 1.01x slower                                                     |
| docutils                 | 2.60 sec                                                               | 2.61 sec: 1.01x slower                                                    |
| deepcopy_reduce          | 3.04 us                                                                | 3.06 us: 1.01x slower                                                     |
| fannkuch                 | 400 ms                                                                 | 403 ms: 1.01x slower                                                      |
| comprehensions           | 16.1 us                                                                | 16.2 us: 1.01x slower                                                     |
| scimark_lu               | 110 ms                                                                 | 111 ms: 1.01x slower                                                      |
| deepcopy                 | 342 us                                                                 | 345 us: 1.01x slower                                                      |
| crypto_pyaes             | 71.1 ms                                                                | 71.7 ms: 1.01x slower                                                     |
| scimark_sor              | 127 ms                                                                 | 128 ms: 1.01x slower                                                      |
| mako                     | 11.1 ms                                                                | 11.2 ms: 1.01x slower                                                     |
| typing_runtime_protocols | 109 us                                                                 | 110 us: 1.01x slower                                                      |
| json_dumps               | 10.3 ms                                                                | 10.5 ms: 1.01x slower                                                     |
| deepcopy_memo            | 37.4 us                                                                | 37.9 us: 1.01x slower                                                     |
| pickle                   | 11.7 us                                                                | 11.8 us: 1.01x slower                                                     |
| regex_v8                 | 25.1 ms                                                                | 25.5 ms: 1.02x slower                                                     |
| nqueens                  | 79.6 ms                                                                | 80.8 ms: 1.02x slower                                                     |
| regex_dna                | 219 ms                                                                 | 223 ms: 1.02x slower                                                      |
| sympy_str                | 270 ms                                                                 | 275 ms: 1.02x slower                                                      |
| sympy_expand             | 458 ms                                                                 | 465 ms: 1.02x slower                                                      |
| pickle_list              | 5.17 us                                                                | 5.25 us: 1.02x slower                                                     |
| regex_effbot             | 3.63 ms                                                                | 3.71 ms: 1.02x slower                                                     |
| telco                    | 8.24 ms                                                                | 8.43 ms: 1.02x slower                                                     |
| unpickle_list            | 5.04 us                                                                | 5.16 us: 1.02x slower                                                     |
| scimark_fft              | 350 ms                                                                 | 362 ms: 1.03x slower                                                      |
| spectral_norm            | 108 ms                                                                 | 112 ms: 1.04x slower                                                      |
| scimark_sparse_mat_mult  | 4.51 ms                                                                | 4.71 ms: 1.04x slower                                                     |
| unpickle                 | 15.0 us                                                                | 15.9 us: 1.06x slower                                                     |
| Geometric mean           | (ref)                                                                  | 1.00x slower                                                              |

Benchmark hidden because not significant (25): sqlite_synth, tornado_http, generators, async_tree_none_tg, xml_etree_parse, mypy2, bench_mp_pool, asyncio_websockets, xml_etree_iterparse, async_tree_memoization_tg, xml_etree_generate, richards_super, 2to3, sympy_integrate, scimark_monte_carlo, dask, logging_silent, mdp, deltablue, richards, pickle_pure_python, async_tree_memoization, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed, async_tree_none


# HPT report

- Reliability score: 76.26% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x