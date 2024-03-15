# Results vs. base

- fork: brandtbucher
- ref: justin_relax
- machine: windows-amd64
- commit hash: ff044c0
- commit date: 2024-02-21
- overall geometric mean: 1.04x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 228 ms                                                                      | 223 ms: 1.02x faster                                                      |
| chameleon      | 4.93 ms                                                                     | 4.63 ms: 1.07x faster                                                     |
| docutils       | 1.64 sec                                                                    | 1.61 sec: 1.02x faster                                                    |
| tornado_http   | 85.6 ms                                                                     | 84.7 ms: 1.01x faster                                                     |
| Geometric mean | (ref)                                                                       | 1.03x faster                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed_tg | 459 ms                                                                      | 465 ms: 1.01x slower                                                      |
| Geometric mean             | (ref)                                                                       | 1.00x slower                                                              |

Benchmark hidden because not significant (7): async_tree_memoization_tg, async_tree_memoization, async_tree_io, async_tree_none, async_tree_none_tg, async_tree_io_tg, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| float          | 50.8 ms                                                                     | 48.5 ms: 1.05x faster                                                     |
| pidigits       | 152 ms                                                                      | 150 ms: 1.01x faster                                                      |
| Geometric mean | (ref)                                                                       | 1.02x faster                                                              |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_compile  | 101 ms                                                                      | 89.9 ms: 1.12x faster                                                     |
| regex_v8       | 15.2 ms                                                                     | 14.6 ms: 1.04x faster                                                     |
| regex_effbot   | 1.59 ms                                                                     | 1.55 ms: 1.02x faster                                                     |
| regex_dna      | 119 ms                                                                      | 118 ms: 1.01x faster                                                      |
| Geometric mean | (ref)                                                                       | 1.05x faster                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| unpickle_pure_python | 144 us                                                                      | 135 us: 1.07x faster                                                      |
| pickle               | 7.57 us                                                                     | 7.15 us: 1.06x faster                                                     |
| unpickle             | 9.04 us                                                                     | 8.59 us: 1.05x faster                                                     |
| tomli_loads          | 1.34 sec                                                                    | 1.30 sec: 1.04x faster                                                    |
| pickle_pure_python   | 180 us                                                                      | 175 us: 1.03x faster                                                      |
| json_dumps           | 5.67 ms                                                                     | 5.53 ms: 1.03x faster                                                     |
| xml_etree_iterparse  | 65.1 ms                                                                     | 63.6 ms: 1.02x faster                                                     |
| xml_etree_parse      | 93.8 ms                                                                     | 92.0 ms: 1.02x faster                                                     |
| json_loads           | 14.0 us                                                                     | 13.7 us: 1.02x faster                                                     |
| xml_etree_process    | 37.0 ms                                                                     | 36.4 ms: 1.02x faster                                                     |
| unpickle_list        | 2.79 us                                                                     | 2.82 us: 1.01x slower                                                     |
| Geometric mean       | (ref)                                                                       | 1.02x faster                                                              |

Benchmark hidden because not significant (3): pickle_list, pickle_dict, xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|------------------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup         | 23.2 ms                                                                     | 23.9 ms: 1.03x slower                                                     |
| python_startup_no_site | 20.8 ms                                                                     | 21.6 ms: 1.03x slower                                                     |
| Geometric mean         | (ref)                                                                       | 1.03x slower                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|-----------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| mako      | 6.37 ms                                                                     | 5.95 ms: 1.07x faster                                                     |

All benchmarks:
===============

| Benchmark                  | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| unpack_sequence            | 89.7 ns                                                                     | 57.6 ns: 1.56x faster                                                     |
| scimark_monte_carlo        | 59.6 ms                                                                     | 45.6 ms: 1.31x faster                                                     |
| scimark_sor                | 104 ms                                                                      | 84.4 ms: 1.23x faster                                                     |
| hexiom                     | 6.01 ms                                                                     | 5.00 ms: 1.20x faster                                                     |
| spectral_norm              | 62.0 ms                                                                     | 54.6 ms: 1.14x faster                                                     |
| go                         | 111 ms                                                                      | 98.1 ms: 1.13x faster                                                     |
| regex_compile              | 101 ms                                                                      | 89.9 ms: 1.12x faster                                                     |
| pyflate                    | 331 ms                                                                      | 296 ms: 1.12x faster                                                      |
| scimark_sparse_mat_mult    | 2.60 ms                                                                     | 2.33 ms: 1.12x faster                                                     |
| async_generators           | 251 ms                                                                      | 233 ms: 1.08x faster                                                      |
| mdp                        | 1.63 sec                                                                    | 1.52 sec: 1.07x faster                                                    |
| mako                       | 6.37 ms                                                                     | 5.95 ms: 1.07x faster                                                     |
| unpickle_pure_python       | 144 us                                                                      | 135 us: 1.07x faster                                                      |
| chameleon                  | 4.93 ms                                                                     | 4.63 ms: 1.07x faster                                                     |
| sympy_expand               | 304 ms                                                                      | 286 ms: 1.06x faster                                                      |
| crypto_pyaes               | 46.5 ms                                                                     | 43.9 ms: 1.06x faster                                                     |
| pickle                     | 7.57 us                                                                     | 7.15 us: 1.06x faster                                                     |
| meteor_contest             | 78.0 ms                                                                     | 73.7 ms: 1.06x faster                                                     |
| raytrace                   | 191 ms                                                                      | 181 ms: 1.06x faster                                                      |
| comprehensions             | 11.4 us                                                                     | 10.8 us: 1.06x faster                                                     |
| scimark_fft                | 188 ms                                                                      | 179 ms: 1.05x faster                                                      |
| sympy_str                  | 175 ms                                                                      | 166 ms: 1.05x faster                                                      |
| unpickle                   | 9.04 us                                                                     | 8.59 us: 1.05x faster                                                     |
| coroutines                 | 13.6 ms                                                                     | 13.0 ms: 1.05x faster                                                     |
| float                      | 50.8 ms                                                                     | 48.5 ms: 1.05x faster                                                     |
| deltablue                  | 2.21 ms                                                                     | 2.11 ms: 1.05x faster                                                     |
| scimark_lu                 | 77.6 ms                                                                     | 74.5 ms: 1.04x faster                                                     |
| chaos                      | 42.5 ms                                                                     | 40.8 ms: 1.04x faster                                                     |
| sympy_integrate            | 13.8 ms                                                                     | 13.2 ms: 1.04x faster                                                     |
| sympy_sum                  | 91.2 ms                                                                     | 87.8 ms: 1.04x faster                                                     |
| regex_v8                   | 15.2 ms                                                                     | 14.6 ms: 1.04x faster                                                     |
| tomli_loads                | 1.34 sec                                                                    | 1.30 sec: 1.04x faster                                                    |
| deepcopy_memo              | 22.6 us                                                                     | 21.9 us: 1.03x faster                                                     |
| sqlglot_optimize           | 36.0 ms                                                                     | 34.8 ms: 1.03x faster                                                     |
| deepcopy                   | 227 us                                                                      | 220 us: 1.03x faster                                                      |
| sqlglot_parse              | 828 us                                                                      | 801 us: 1.03x faster                                                      |
| sqlglot_normalize          | 180 ms                                                                      | 175 ms: 1.03x faster                                                      |
| mypy2                      | 445 ms                                                                      | 433 ms: 1.03x faster                                                      |
| pickle_pure_python         | 180 us                                                                      | 175 us: 1.03x faster                                                      |
| json_dumps                 | 5.67 ms                                                                     | 5.53 ms: 1.03x faster                                                     |
| regex_effbot               | 1.59 ms                                                                     | 1.55 ms: 1.02x faster                                                     |
| xml_etree_iterparse        | 65.1 ms                                                                     | 63.6 ms: 1.02x faster                                                     |
| 2to3                       | 228 ms                                                                      | 223 ms: 1.02x faster                                                      |
| deepcopy_reduce            | 1.98 us                                                                     | 1.94 us: 1.02x faster                                                     |
| docutils                   | 1.64 sec                                                                    | 1.61 sec: 1.02x faster                                                    |
| xml_etree_parse            | 93.8 ms                                                                     | 92.0 ms: 1.02x faster                                                     |
| json_loads                 | 14.0 us                                                                     | 13.7 us: 1.02x faster                                                     |
| sqlglot_transpile          | 1.05 ms                                                                     | 1.03 ms: 1.02x faster                                                     |
| dulwich_log                | 42.0 ms                                                                     | 41.3 ms: 1.02x faster                                                     |
| xml_etree_process          | 37.0 ms                                                                     | 36.4 ms: 1.02x faster                                                     |
| logging_silent             | 56.7 ns                                                                     | 55.7 ns: 1.02x faster                                                     |
| sqlite_synth               | 1.58 us                                                                     | 1.55 us: 1.02x faster                                                     |
| pidigits                   | 152 ms                                                                      | 150 ms: 1.01x faster                                                      |
| typing_runtime_protocols   | 71.8 us                                                                     | 70.9 us: 1.01x faster                                                     |
| nqueens                    | 62.3 ms                                                                     | 61.5 ms: 1.01x faster                                                     |
| pprint_safe_repr           | 512 ms                                                                      | 506 ms: 1.01x faster                                                      |
| tornado_http               | 85.6 ms                                                                     | 84.7 ms: 1.01x faster                                                     |
| logging_simple             | 5.96 us                                                                     | 5.90 us: 1.01x faster                                                     |
| logging_format             | 6.47 us                                                                     | 6.41 us: 1.01x faster                                                     |
| regex_dna                  | 119 ms                                                                      | 118 ms: 1.01x faster                                                      |
| bench_thread_pool          | 846 us                                                                      | 839 us: 1.01x faster                                                      |
| richards_super             | 35.4 ms                                                                     | 35.2 ms: 1.01x faster                                                     |
| richards                   | 31.9 ms                                                                     | 31.7 ms: 1.00x faster                                                     |
| pprint_pformat             | 1.04 sec                                                                    | 1.04 sec: 1.01x slower                                                    |
| telco                      | 4.53 ms                                                                     | 4.57 ms: 1.01x slower                                                     |
| bench_mp_pool              | 69.5 ms                                                                     | 70.3 ms: 1.01x slower                                                     |
| unpickle_list              | 2.79 us                                                                     | 2.82 us: 1.01x slower                                                     |
| async_tree_cpu_io_mixed_tg | 459 ms                                                                      | 465 ms: 1.01x slower                                                      |
| fannkuch                   | 256 ms                                                                      | 259 ms: 1.01x slower                                                      |
| gc_traversal               | 1.49 ms                                                                     | 1.51 ms: 1.01x slower                                                     |
| python_startup             | 23.2 ms                                                                     | 23.9 ms: 1.03x slower                                                     |
| python_startup_no_site     | 20.8 ms                                                                     | 21.6 ms: 1.03x slower                                                     |
| Geometric mean             | (ref)                                                                       | 1.04x faster                                                              |

Benchmark hidden because not significant (19): pycparser, asyncio_tcp, pickle_list, async_tree_memoization_tg, nbody, create_gc_cycles, coverage, async_tree_memoization, pickle_dict, generators, xml_etree_generate, async_tree_io, async_tree_none, asyncio_tcp_ssl, pathlib, async_tree_none_tg, async_tree_io_tg, async_tree_cpu_io_mixed, json


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: unknown