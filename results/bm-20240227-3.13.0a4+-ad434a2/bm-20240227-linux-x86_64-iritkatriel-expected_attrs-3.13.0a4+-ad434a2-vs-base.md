# Results vs. base

- fork: iritkatriel
- ref: expected_attrs
- machine: linux-x86_64
- commit hash: ad434a2
- commit date: 2024-02-27
- overall geometric mean: 1.00x faster
- HPT reliability: 97.18%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|----------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 263 ms                                                                 | 262 ms: 1.00x faster                                                  |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                          |

Benchmark hidden because not significant (3): chameleon, docutils, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|--------------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_none_tg | 444 ms                                                                 | 441 ms: 1.01x faster                                                  |
| async_tree_io_tg   | 1.19 sec                                                               | 1.19 sec: 1.00x slower                                                |
| Geometric mean     | (ref)                                                                  | 1.00x faster                                                          |

Benchmark hidden because not significant (6): async_tree_memoization_tg, async_tree_none, async_tree_memoization, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|----------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------------:|
| nbody          | 88.7 ms                                                                | 88.2 ms: 1.01x faster                                                 |
| pidigits       | 188 ms                                                                 | 187 ms: 1.00x faster                                                  |
| float          | 80.1 ms                                                                | 80.6 ms: 1.01x slower                                                 |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|----------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 130 ms                                                                 | 131 ms: 1.00x slower                                                  |
| regex_dna      | 214 ms                                                                 | 224 ms: 1.05x slower                                                  |
| regex_v8       | 24.6 ms                                                                | 26.3 ms: 1.07x slower                                                 |
| regex_effbot   | 3.49 ms                                                                | 3.81 ms: 1.09x slower                                                 |
| Geometric mean | (ref)                                                                  | 1.05x slower                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|----------------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------------:|
| pickle_list          | 5.21 us                                                                | 4.82 us: 1.08x faster                                                 |
| pickle_dict          | 35.8 us                                                                | 33.6 us: 1.06x faster                                                 |
| pickle               | 12.1 us                                                                | 11.4 us: 1.06x faster                                                 |
| xml_etree_iterparse  | 105 ms                                                                 | 103 ms: 1.01x faster                                                  |
| unpickle_list        | 4.98 us                                                                | 4.90 us: 1.01x faster                                                 |
| xml_etree_process    | 57.9 ms                                                                | 57.6 ms: 1.01x faster                                                 |
| unpickle_pure_python | 211 us                                                                 | 210 us: 1.00x faster                                                  |
| xml_etree_generate   | 84.3 ms                                                                | 84.0 ms: 1.00x faster                                                 |
| json_loads           | 27.4 us                                                                | 27.5 us: 1.00x slower                                                 |
| json_dumps           | 10.4 ms                                                                | 10.5 ms: 1.01x slower                                                 |
| pickle_pure_python   | 289 us                                                                 | 292 us: 1.01x slower                                                  |
| unpickle             | 14.9 us                                                                | 15.0 us: 1.01x slower                                                 |
| Geometric mean       | (ref)                                                                  | 1.02x faster                                                          |

Benchmark hidden because not significant (2): xml_etree_parse, tomli_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|------------------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                | 10.1 ms: 1.00x slower                                                 |
| python_startup_no_site | 8.73 ms                                                                | 8.76 ms: 1.00x slower                                                 |
| Geometric mean         | (ref)                                                                  | 1.00x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|-----------|:----------------------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako      | 10.7 ms                                                                | 10.9 ms: 1.02x slower                                                 |

All benchmarks:
===============

| Benchmark                | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|--------------------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------------:|
| unpack_sequence          | 55.0 ns                                                                | 42.9 ns: 1.28x faster                                                 |
| pickle_list              | 5.21 us                                                                | 4.82 us: 1.08x faster                                                 |
| pickle_dict              | 35.8 us                                                                | 33.6 us: 1.06x faster                                                 |
| pickle                   | 12.1 us                                                                | 11.4 us: 1.06x faster                                                 |
| scimark_sor              | 122 ms                                                                 | 116 ms: 1.05x faster                                                  |
| pyflate                  | 458 ms                                                                 | 439 ms: 1.04x faster                                                  |
| spectral_norm            | 109 ms                                                                 | 105 ms: 1.04x faster                                                  |
| crypto_pyaes             | 70.5 ms                                                                | 69.0 ms: 1.02x faster                                                 |
| generators               | 29.2 ms                                                                | 28.7 ms: 1.02x faster                                                 |
| hexiom                   | 5.99 ms                                                                | 5.89 ms: 1.02x faster                                                 |
| typing_runtime_protocols | 111 us                                                                 | 109 us: 1.02x faster                                                  |
| xml_etree_iterparse      | 105 ms                                                                 | 103 ms: 1.01x faster                                                  |
| unpickle_list            | 4.98 us                                                                | 4.90 us: 1.01x faster                                                 |
| fannkuch                 | 381 ms                                                                 | 376 ms: 1.01x faster                                                  |
| sympy_str                | 268 ms                                                                 | 264 ms: 1.01x faster                                                  |
| telco                    | 8.34 ms                                                                | 8.25 ms: 1.01x faster                                                 |
| pathlib                  | 18.1 ms                                                                | 17.9 ms: 1.01x faster                                                 |
| pprint_safe_repr         | 720 ms                                                                 | 713 ms: 1.01x faster                                                  |
| sympy_sum                | 147 ms                                                                 | 146 ms: 1.01x faster                                                  |
| async_tree_none_tg       | 444 ms                                                                 | 441 ms: 1.01x faster                                                  |
| sympy_integrate          | 19.5 ms                                                                | 19.3 ms: 1.01x faster                                                 |
| coroutines               | 22.0 ms                                                                | 21.9 ms: 1.01x faster                                                 |
| sqlglot_optimize         | 53.0 ms                                                                | 52.7 ms: 1.01x faster                                                 |
| xml_etree_process        | 57.9 ms                                                                | 57.6 ms: 1.01x faster                                                 |
| nbody                    | 88.7 ms                                                                | 88.2 ms: 1.01x faster                                                 |
| go                       | 135 ms                                                                 | 135 ms: 1.01x faster                                                  |
| meteor_contest           | 107 ms                                                                 | 106 ms: 1.01x faster                                                  |
| asyncio_tcp              | 484 ms                                                                 | 482 ms: 1.01x faster                                                  |
| unpickle_pure_python     | 211 us                                                                 | 210 us: 1.00x faster                                                  |
| 2to3                     | 263 ms                                                                 | 262 ms: 1.00x faster                                                  |
| xml_etree_generate       | 84.3 ms                                                                | 84.0 ms: 1.00x faster                                                 |
| pidigits                 | 188 ms                                                                 | 187 ms: 1.00x faster                                                  |
| asyncio_tcp_ssl          | 1.79 sec                                                               | 1.78 sec: 1.00x faster                                                |
| dulwich_log              | 65.2 ms                                                                | 65.1 ms: 1.00x faster                                                 |
| python_startup           | 10.1 ms                                                                | 10.1 ms: 1.00x slower                                                 |
| regex_compile            | 130 ms                                                                 | 131 ms: 1.00x slower                                                  |
| json_loads               | 27.4 us                                                                | 27.5 us: 1.00x slower                                                 |
| async_tree_io_tg         | 1.19 sec                                                               | 1.19 sec: 1.00x slower                                                |
| python_startup_no_site   | 8.73 ms                                                                | 8.76 ms: 1.00x slower                                                 |
| nqueens                  | 80.0 ms                                                                | 80.3 ms: 1.00x slower                                                 |
| deltablue                | 3.13 ms                                                                | 3.14 ms: 1.00x slower                                                 |
| gc_traversal             | 3.83 ms                                                                | 3.84 ms: 1.00x slower                                                 |
| float                    | 80.1 ms                                                                | 80.6 ms: 1.01x slower                                                 |
| json_dumps               | 10.4 ms                                                                | 10.5 ms: 1.01x slower                                                 |
| comprehensions           | 16.2 us                                                                | 16.3 us: 1.01x slower                                                 |
| pickle_pure_python       | 289 us                                                                 | 292 us: 1.01x slower                                                  |
| coverage                 | 94.4 ms                                                                | 95.2 ms: 1.01x slower                                                 |
| unpickle                 | 14.9 us                                                                | 15.0 us: 1.01x slower                                                 |
| sqlite_synth             | 2.81 us                                                                | 2.84 us: 1.01x slower                                                 |
| pycparser                | 1.15 sec                                                               | 1.16 sec: 1.01x slower                                                |
| deepcopy_reduce          | 2.98 us                                                                | 3.01 us: 1.01x slower                                                 |
| deepcopy                 | 337 us                                                                 | 341 us: 1.01x slower                                                  |
| logging_silent           | 97.0 ns                                                                | 98.1 ns: 1.01x slower                                                 |
| scimark_fft              | 352 ms                                                                 | 357 ms: 1.01x slower                                                  |
| richards_super           | 52.5 ms                                                                | 53.2 ms: 1.01x slower                                                 |
| mako                     | 10.7 ms                                                                | 10.9 ms: 1.02x slower                                                 |
| json                     | 4.98 ms                                                                | 5.08 ms: 1.02x slower                                                 |
| richards                 | 46.3 ms                                                                | 47.2 ms: 1.02x slower                                                 |
| logging_simple           | 5.61 us                                                                | 5.76 us: 1.03x slower                                                 |
| logging_format           | 6.16 us                                                                | 6.35 us: 1.03x slower                                                 |
| deepcopy_memo            | 36.2 us                                                                | 37.3 us: 1.03x slower                                                 |
| regex_dna                | 214 ms                                                                 | 224 ms: 1.05x slower                                                  |
| scimark_sparse_mat_mult  | 4.54 ms                                                                | 4.82 ms: 1.06x slower                                                 |
| regex_v8                 | 24.6 ms                                                                | 26.3 ms: 1.07x slower                                                 |
| regex_effbot             | 3.49 ms                                                                | 3.81 ms: 1.09x slower                                                 |
| Geometric mean           | (ref)                                                                  | 1.00x faster                                                          |

Benchmark hidden because not significant (27): scimark_lu, mypy2, async_tree_memoization_tg, chameleon, xml_etree_parse, async_tree_none, async_tree_memoization, sqlglot_transpile, create_gc_cycles, async_tree_cpu_io_mixed, async_generators, docutils, sqlglot_normalize, async_tree_cpu_io_mixed_tg, sympy_expand, bench_thread_pool, chaos, sqlglot_parse, raytrace, asyncio_websockets, async_tree_io, bench_mp_pool, tornado_http, tomli_loads, mdp, pprint_pformat, scimark_monte_carlo


# HPT report

- Reliability score: 97.18% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x