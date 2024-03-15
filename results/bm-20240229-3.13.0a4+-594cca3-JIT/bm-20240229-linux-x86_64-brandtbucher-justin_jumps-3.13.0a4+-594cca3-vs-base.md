# Results vs. base

- fork: brandtbucher
- ref: justin_jumps
- machine: linux-x86_64
- commit hash: 594cca3
- commit date: 2024-02-29
- overall geometric mean: 1.02x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 280 ms                                                                 | 276 ms: 1.01x faster                                                 |
| chameleon      | 6.77 ms                                                                | 6.69 ms: 1.01x faster                                                |
| docutils       | 2.72 sec                                                               | 2.70 sec: 1.01x faster                                               |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                         |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 712 ms                                                                 | 702 ms: 1.02x faster                                                 |
| async_tree_memoization     | 566 ms                                                                 | 560 ms: 1.01x faster                                                 |
| async_tree_cpu_io_mixed_tg | 724 ms                                                                 | 716 ms: 1.01x faster                                                 |
| async_tree_io              | 1.19 sec                                                               | 1.18 sec: 1.01x faster                                               |
| async_tree_none_tg         | 449 ms                                                                 | 445 ms: 1.01x faster                                                 |
| async_tree_io_tg           | 1.21 sec                                                               | 1.20 sec: 1.00x faster                                               |
| Geometric mean             | (ref)                                                                  | 1.01x faster                                                         |

Benchmark hidden because not significant (2): async_tree_none, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| float          | 81.5 ms                                                                | 78.2 ms: 1.04x faster                                                |
| nbody          | 95.0 ms                                                                | 92.9 ms: 1.02x faster                                                |
| pidigits       | 188 ms                                                                 | 187 ms: 1.00x faster                                                 |
| Geometric mean | (ref)                                                                  | 1.02x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 151 ms                                                                 | 143 ms: 1.06x faster                                                 |
| regex_effbot   | 3.63 ms                                                                | 3.56 ms: 1.02x faster                                                |
| regex_v8       | 24.7 ms                                                                | 24.3 ms: 1.02x faster                                                |
| regex_dna      | 224 ms                                                                 | 224 ms: 1.00x slower                                                 |
| Geometric mean | (ref)                                                                  | 1.02x faster                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| tomli_loads          | 2.18 sec                                                               | 2.03 sec: 1.07x faster                                               |
| pickle_dict          | 35.2 us                                                                | 33.3 us: 1.06x faster                                                |
| pickle_list          | 5.26 us                                                                | 5.01 us: 1.05x faster                                                |
| unpickle_pure_python | 245 us                                                                 | 236 us: 1.04x faster                                                 |
| unpickle             | 15.0 us                                                                | 14.6 us: 1.03x faster                                                |
| pickle               | 11.6 us                                                                | 11.3 us: 1.03x faster                                                |
| pickle_pure_python   | 305 us                                                                 | 299 us: 1.02x faster                                                 |
| xml_etree_iterparse  | 108 ms                                                                 | 106 ms: 1.01x faster                                                 |
| xml_etree_parse      | 158 ms                                                                 | 156 ms: 1.01x faster                                                 |
| xml_etree_process    | 58.7 ms                                                                | 58.2 ms: 1.01x faster                                                |
| json_loads           | 27.3 us                                                                | 27.4 us: 1.00x slower                                                |
| unpickle_list        | 4.94 us                                                                | 5.05 us: 1.02x slower                                                |
| Geometric mean       | (ref)                                                                  | 1.02x faster                                                         |

Benchmark hidden because not significant (2): xml_etree_generate, json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup_no_site | 10.9 ms                                                                | 10.9 ms: 1.00x faster                                                |
| python_startup         | 12.3 ms                                                                | 12.2 ms: 1.00x faster                                                |
| Geometric mean         | (ref)                                                                  | 1.00x faster                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 11.6 ms                                                                | 10.8 ms: 1.07x faster                                                |

All benchmarks:
===============

| Benchmark                  | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| unpack_sequence            | 121 ns                                                                 | 84.9 ns: 1.43x faster                                                |
| pprint_pformat             | 1.67 sec                                                               | 1.55 sec: 1.08x faster                                               |
| scimark_monte_carlo        | 76.2 ms                                                                | 70.9 ms: 1.08x faster                                                |
| tomli_loads                | 2.18 sec                                                               | 2.03 sec: 1.07x faster                                               |
| hexiom                     | 7.53 ms                                                                | 7.02 ms: 1.07x faster                                                |
| mako                       | 11.6 ms                                                                | 10.8 ms: 1.07x faster                                                |
| pprint_safe_repr           | 794 ms                                                                 | 742 ms: 1.07x faster                                                 |
| fannkuch                   | 423 ms                                                                 | 396 ms: 1.07x faster                                                 |
| pyflate                    | 513 ms                                                                 | 484 ms: 1.06x faster                                                 |
| regex_compile              | 151 ms                                                                 | 143 ms: 1.06x faster                                                 |
| comprehensions             | 18.0 us                                                                | 17.0 us: 1.06x faster                                                |
| pickle_dict                | 35.2 us                                                                | 33.3 us: 1.06x faster                                                |
| mdp                        | 2.76 sec                                                               | 2.61 sec: 1.06x faster                                               |
| spectral_norm              | 119 ms                                                                 | 113 ms: 1.06x faster                                                 |
| scimark_fft                | 354 ms                                                                 | 337 ms: 1.05x faster                                                 |
| pickle_list                | 5.26 us                                                                | 5.01 us: 1.05x faster                                                |
| pycparser                  | 1.22 sec                                                               | 1.16 sec: 1.05x faster                                               |
| float                      | 81.5 ms                                                                | 78.2 ms: 1.04x faster                                                |
| unpickle_pure_python       | 245 us                                                                 | 236 us: 1.04x faster                                                 |
| telco                      | 8.66 ms                                                                | 8.37 ms: 1.04x faster                                                |
| crypto_pyaes               | 74.9 ms                                                                | 72.5 ms: 1.03x faster                                                |
| unpickle                   | 15.0 us                                                                | 14.6 us: 1.03x faster                                                |
| sqlglot_parse              | 1.32 ms                                                                | 1.29 ms: 1.03x faster                                                |
| chaos                      | 64.0 ms                                                                | 62.4 ms: 1.03x faster                                                |
| pickle                     | 11.6 us                                                                | 11.3 us: 1.03x faster                                                |
| scimark_sparse_mat_mult    | 5.04 ms                                                                | 4.93 ms: 1.02x faster                                                |
| scimark_sor                | 129 ms                                                                 | 126 ms: 1.02x faster                                                 |
| nbody                      | 95.0 ms                                                                | 92.9 ms: 1.02x faster                                                |
| regex_effbot               | 3.63 ms                                                                | 3.56 ms: 1.02x faster                                                |
| sqlglot_transpile          | 1.66 ms                                                                | 1.63 ms: 1.02x faster                                                |
| meteor_contest             | 110 ms                                                                 | 108 ms: 1.02x faster                                                 |
| pickle_pure_python         | 305 us                                                                 | 299 us: 1.02x faster                                                 |
| logging_simple             | 5.71 us                                                                | 5.61 us: 1.02x faster                                                |
| scimark_lu                 | 133 ms                                                                 | 131 ms: 1.02x faster                                                 |
| sqlglot_optimize           | 56.9 ms                                                                | 56.0 ms: 1.02x faster                                                |
| async_tree_cpu_io_mixed    | 712 ms                                                                 | 702 ms: 1.02x faster                                                 |
| raytrace                   | 293 ms                                                                 | 288 ms: 1.02x faster                                                 |
| regex_v8                   | 24.7 ms                                                                | 24.3 ms: 1.02x faster                                                |
| json                       | 5.08 ms                                                                | 5.00 ms: 1.01x faster                                                |
| nqueens                    | 92.0 ms                                                                | 90.7 ms: 1.01x faster                                                |
| richards_super             | 52.9 ms                                                                | 52.2 ms: 1.01x faster                                                |
| xml_etree_iterparse        | 108 ms                                                                 | 106 ms: 1.01x faster                                                 |
| logging_format             | 6.25 us                                                                | 6.17 us: 1.01x faster                                                |
| sympy_expand               | 484 ms                                                                 | 478 ms: 1.01x faster                                                 |
| richards                   | 47.3 ms                                                                | 46.7 ms: 1.01x faster                                                |
| 2to3                       | 280 ms                                                                 | 276 ms: 1.01x faster                                                 |
| chameleon                  | 6.77 ms                                                                | 6.69 ms: 1.01x faster                                                |
| deepcopy_memo              | 39.4 us                                                                | 38.9 us: 1.01x faster                                                |
| sympy_sum                  | 160 ms                                                                 | 158 ms: 1.01x faster                                                 |
| async_tree_memoization     | 566 ms                                                                 | 560 ms: 1.01x faster                                                 |
| async_tree_cpu_io_mixed_tg | 724 ms                                                                 | 716 ms: 1.01x faster                                                 |
| async_generators           | 462 ms                                                                 | 457 ms: 1.01x faster                                                 |
| xml_etree_parse            | 158 ms                                                                 | 156 ms: 1.01x faster                                                 |
| sympy_str                  | 284 ms                                                                 | 281 ms: 1.01x faster                                                 |
| async_tree_io              | 1.19 sec                                                               | 1.18 sec: 1.01x faster                                               |
| deltablue                  | 3.43 ms                                                                | 3.40 ms: 1.01x faster                                                |
| dulwich_log                | 69.3 ms                                                                | 68.7 ms: 1.01x faster                                                |
| deepcopy                   | 352 us                                                                 | 350 us: 1.01x faster                                                 |
| docutils                   | 2.72 sec                                                               | 2.70 sec: 1.01x faster                                               |
| async_tree_none_tg         | 449 ms                                                                 | 445 ms: 1.01x faster                                                 |
| xml_etree_process          | 58.7 ms                                                                | 58.2 ms: 1.01x faster                                                |
| sympy_integrate            | 21.0 ms                                                                | 20.9 ms: 1.01x faster                                                |
| create_gc_cycles           | 1.50 ms                                                                | 1.49 ms: 1.01x faster                                                |
| gc_traversal               | 3.77 ms                                                                | 3.75 ms: 1.01x faster                                                |
| sqlglot_normalize          | 108 ms                                                                 | 107 ms: 1.01x faster                                                 |
| go                         | 158 ms                                                                 | 157 ms: 1.01x faster                                                 |
| pidigits                   | 188 ms                                                                 | 187 ms: 1.00x faster                                                 |
| bench_thread_pool          | 850 us                                                                 | 846 us: 1.00x faster                                                 |
| pathlib                    | 18.6 ms                                                                | 18.5 ms: 1.00x faster                                                |
| python_startup_no_site     | 10.9 ms                                                                | 10.9 ms: 1.00x faster                                                |
| async_tree_io_tg           | 1.21 sec                                                               | 1.20 sec: 1.00x faster                                               |
| python_startup             | 12.3 ms                                                                | 12.2 ms: 1.00x faster                                                |
| asyncio_tcp_ssl            | 1.80 sec                                                               | 1.80 sec: 1.00x faster                                               |
| regex_dna                  | 224 ms                                                                 | 224 ms: 1.00x slower                                                 |
| json_loads                 | 27.3 us                                                                | 27.4 us: 1.00x slower                                                |
| generators                 | 29.1 ms                                                                | 29.3 ms: 1.01x slower                                                |
| typing_runtime_protocols   | 110 us                                                                 | 111 us: 1.01x slower                                                 |
| unpickle_list              | 4.94 us                                                                | 5.05 us: 1.02x slower                                                |
| coroutines                 | 22.3 ms                                                                | 22.9 ms: 1.03x slower                                                |
| Geometric mean             | (ref)                                                                  | 1.02x faster                                                         |

Benchmark hidden because not significant (13): async_tree_none, async_tree_memoization_tg, coverage, bench_mp_pool, mypy2, tornado_http, xml_etree_generate, sqlite_synth, json_dumps, logging_silent, asyncio_websockets, deepcopy_reduce, asyncio_tcp


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x