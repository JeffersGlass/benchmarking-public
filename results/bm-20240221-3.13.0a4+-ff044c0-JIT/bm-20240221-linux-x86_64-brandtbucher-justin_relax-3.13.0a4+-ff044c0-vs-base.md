# Results vs. base

- fork: brandtbucher
- ref: justin_relax
- machine: linux-x86_64
- commit hash: ff044c0
- commit date: 2024-02-21
- overall geometric mean: 1.03x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.09x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240221-linux-x86_64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 289 ms                                                                 | 280 ms: 1.03x faster                                                 |
| docutils       | 2.76 sec                                                               | 2.72 sec: 1.01x faster                                               |
| tornado_http   | 97.4 ms                                                                | 96.9 ms: 1.01x faster                                                |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                         |

Benchmark hidden because not significant (1): chameleon

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20240221-linux-x86_64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|--------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none_tg | 450 ms                                                                 | 447 ms: 1.01x faster                                                 |
| Geometric mean     | (ref)                                                                  | 1.00x faster                                                         |

Benchmark hidden because not significant (7): async_tree_memoization, async_tree_memoization_tg, async_tree_none, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed, async_tree_io_tg, async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240221-linux-x86_64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| float          | 84.3 ms                                                                | 80.7 ms: 1.04x faster                                                |
| nbody          | 101 ms                                                                 | 97.7 ms: 1.03x faster                                                |
| pidigits       | 188 ms                                                                 | 187 ms: 1.00x faster                                                 |
| Geometric mean | (ref)                                                                  | 1.03x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240221-linux-x86_64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 165 ms                                                                 | 150 ms: 1.10x faster                                                 |
| regex_v8       | 25.9 ms                                                                | 24.7 ms: 1.04x faster                                                |
| regex_effbot   | 3.62 ms                                                                | 3.72 ms: 1.03x slower                                                |
| regex_dna      | 217 ms                                                                 | 224 ms: 1.03x slower                                                 |
| Geometric mean | (ref)                                                                  | 1.02x faster                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240221-linux-x86_64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| tomli_loads          | 2.31 sec                                                               | 2.17 sec: 1.06x faster                                               |
| unpickle_pure_python | 254 us                                                                 | 244 us: 1.04x faster                                                 |
| xml_etree_iterparse  | 109 ms                                                                 | 106 ms: 1.03x faster                                                 |
| json_loads           | 27.7 us                                                                | 27.3 us: 1.01x faster                                                |
| unpickle             | 15.3 us                                                                | 15.1 us: 1.01x faster                                                |
| xml_etree_process    | 59.5 ms                                                                | 59.1 ms: 1.01x faster                                                |
| unpickle_list        | 5.04 us                                                                | 5.01 us: 1.01x faster                                                |
| json_dumps           | 10.4 ms                                                                | 10.4 ms: 1.00x faster                                                |
| pickle_dict          | 34.9 us                                                                | 35.2 us: 1.01x slower                                                |
| Geometric mean       | (ref)                                                                  | 1.01x faster                                                         |

Benchmark hidden because not significant (5): xml_etree_parse, xml_etree_generate, pickle_pure_python, pickle_list, pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240221-linux-x86_64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 11.8 ms                                                                | 12.2 ms: 1.04x slower                                                |
| python_startup_no_site | 10.4 ms                                                                | 10.9 ms: 1.04x slower                                                |
| Geometric mean         | (ref)                                                                  | 1.04x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240221-linux-x86_64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 12.1 ms                                                                | 11.6 ms: 1.05x faster                                                |

All benchmarks:
===============

| Benchmark                | bm-20240221-linux-x86_64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|--------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| unpack_sequence          | 161 ns                                                                 | 132 ns: 1.22x faster                                                 |
| hexiom                   | 8.72 ms                                                                | 7.54 ms: 1.16x faster                                                |
| pprint_pformat           | 1.82 sec                                                               | 1.60 sec: 1.13x faster                                               |
| pprint_safe_repr         | 868 ms                                                                 | 769 ms: 1.13x faster                                                 |
| gc_traversal             | 3.92 ms                                                                | 3.48 ms: 1.12x faster                                                |
| regex_compile            | 165 ms                                                                 | 150 ms: 1.10x faster                                                 |
| pyflate                  | 553 ms                                                                 | 508 ms: 1.09x faster                                                 |
| scimark_monte_carlo      | 82.2 ms                                                                | 76.1 ms: 1.08x faster                                                |
| spectral_norm            | 130 ms                                                                 | 120 ms: 1.08x faster                                                 |
| chaos                    | 69.6 ms                                                                | 64.8 ms: 1.07x faster                                                |
| comprehensions           | 19.0 us                                                                | 17.7 us: 1.07x faster                                                |
| nqueens                  | 97.8 ms                                                                | 91.4 ms: 1.07x faster                                                |
| raytrace                 | 319 ms                                                                 | 299 ms: 1.07x faster                                                 |
| tomli_loads              | 2.31 sec                                                               | 2.17 sec: 1.06x faster                                               |
| deltablue                | 3.64 ms                                                                | 3.44 ms: 1.06x faster                                                |
| scimark_sparse_mat_mult  | 5.42 ms                                                                | 5.15 ms: 1.05x faster                                                |
| mako                     | 12.1 ms                                                                | 11.6 ms: 1.05x faster                                                |
| regex_v8                 | 25.9 ms                                                                | 24.7 ms: 1.04x faster                                                |
| float                    | 84.3 ms                                                                | 80.7 ms: 1.04x faster                                                |
| unpickle_pure_python     | 254 us                                                                 | 244 us: 1.04x faster                                                 |
| scimark_fft              | 373 ms                                                                 | 359 ms: 1.04x faster                                                 |
| scimark_lu               | 136 ms                                                                 | 131 ms: 1.04x faster                                                 |
| typing_runtime_protocols | 113 us                                                                 | 108 us: 1.04x faster                                                 |
| json                     | 5.19 ms                                                                | 5.00 ms: 1.04x faster                                                |
| crypto_pyaes             | 78.3 ms                                                                | 75.5 ms: 1.04x faster                                                |
| fannkuch                 | 436 ms                                                                 | 421 ms: 1.04x faster                                                 |
| nbody                    | 101 ms                                                                 | 97.7 ms: 1.03x faster                                                |
| richards                 | 51.4 ms                                                                | 49.6 ms: 1.03x faster                                                |
| go                       | 164 ms                                                                 | 158 ms: 1.03x faster                                                 |
| logging_silent           | 102 ns                                                                 | 98.9 ns: 1.03x faster                                                |
| logging_format           | 6.56 us                                                                | 6.34 us: 1.03x faster                                                |
| 2to3                     | 289 ms                                                                 | 280 ms: 1.03x faster                                                 |
| telco                    | 8.69 ms                                                                | 8.44 ms: 1.03x faster                                                |
| richards_super           | 57.4 ms                                                                | 55.9 ms: 1.03x faster                                                |
| xml_etree_iterparse      | 109 ms                                                                 | 106 ms: 1.03x faster                                                 |
| coroutines               | 22.3 ms                                                                | 21.7 ms: 1.03x faster                                                |
| meteor_contest           | 111 ms                                                                 | 109 ms: 1.03x faster                                                 |
| sympy_str                | 291 ms                                                                 | 284 ms: 1.02x faster                                                 |
| create_gc_cycles         | 1.52 ms                                                                | 1.49 ms: 1.02x faster                                                |
| sqlglot_transpile        | 1.69 ms                                                                | 1.65 ms: 1.02x faster                                                |
| sympy_expand             | 493 ms                                                                 | 482 ms: 1.02x faster                                                 |
| dulwich_log              | 70.6 ms                                                                | 69.2 ms: 1.02x faster                                                |
| deepcopy_memo            | 39.5 us                                                                | 38.7 us: 1.02x faster                                                |
| sqlglot_parse            | 1.34 ms                                                                | 1.31 ms: 1.02x faster                                                |
| sqlglot_optimize         | 57.6 ms                                                                | 56.7 ms: 1.01x faster                                                |
| sympy_sum                | 161 ms                                                                 | 159 ms: 1.01x faster                                                 |
| docutils                 | 2.76 sec                                                               | 2.72 sec: 1.01x faster                                               |
| json_loads               | 27.7 us                                                                | 27.3 us: 1.01x faster                                                |
| scimark_sor              | 132 ms                                                                 | 130 ms: 1.01x faster                                                 |
| logging_simple           | 5.85 us                                                                | 5.77 us: 1.01x faster                                                |
| async_generators         | 469 ms                                                                 | 463 ms: 1.01x faster                                                 |
| coverage                 | 96.5 ms                                                                | 95.5 ms: 1.01x faster                                                |
| sympy_integrate          | 21.2 ms                                                                | 20.9 ms: 1.01x faster                                                |
| unpickle                 | 15.3 us                                                                | 15.1 us: 1.01x faster                                                |
| bench_thread_pool        | 859 us                                                                 | 851 us: 1.01x faster                                                 |
| sqlglot_normalize        | 110 ms                                                                 | 109 ms: 1.01x faster                                                 |
| pycparser                | 1.23 sec                                                               | 1.22 sec: 1.01x faster                                               |
| xml_etree_process        | 59.5 ms                                                                | 59.1 ms: 1.01x faster                                                |
| deepcopy                 | 352 us                                                                 | 350 us: 1.01x faster                                                 |
| async_tree_none_tg       | 450 ms                                                                 | 447 ms: 1.01x faster                                                 |
| unpickle_list            | 5.04 us                                                                | 5.01 us: 1.01x faster                                                |
| tornado_http             | 97.4 ms                                                                | 96.9 ms: 1.01x faster                                                |
| json_dumps               | 10.4 ms                                                                | 10.4 ms: 1.00x faster                                                |
| pidigits                 | 188 ms                                                                 | 187 ms: 1.00x faster                                                 |
| asyncio_tcp_ssl          | 1.79 sec                                                               | 1.80 sec: 1.00x slower                                               |
| mdp                      | 2.64 sec                                                               | 2.66 sec: 1.01x slower                                               |
| pickle_dict              | 34.9 us                                                                | 35.2 us: 1.01x slower                                                |
| deepcopy_reduce          | 3.10 us                                                                | 3.15 us: 1.01x slower                                                |
| regex_effbot             | 3.62 ms                                                                | 3.72 ms: 1.03x slower                                                |
| regex_dna                | 217 ms                                                                 | 224 ms: 1.03x slower                                                 |
| python_startup           | 11.8 ms                                                                | 12.2 ms: 1.04x slower                                                |
| python_startup_no_site   | 10.4 ms                                                                | 10.9 ms: 1.04x slower                                                |
| Geometric mean           | (ref)                                                                  | 1.03x faster                                                         |

Benchmark hidden because not significant (20): mypy2, async_tree_memoization, async_tree_memoization_tg, async_tree_none, xml_etree_parse, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed, bench_mp_pool, sqlite_synth, async_tree_io_tg, xml_etree_generate, pickle_pure_python, pickle_list, pathlib, pickle, asyncio_websockets, asyncio_tcp, generators, chameleon, async_tree_io


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.09x