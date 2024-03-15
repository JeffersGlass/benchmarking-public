# Results vs. base

- fork: brandtbucher
- ref: justin_relax
- machine: darwin-arm64
- commit hash: ff044c0
- commit date: 2024-02-21
- overall geometric mean: 1.01x faster
- HPT reliability: 95.14%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240221-darwin-arm64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 187 ms                                                                 | 185 ms: 1.01x faster                                                 |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                         |

Benchmark hidden because not significant (3): chameleon, docutils, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20240221-darwin-arm64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|-------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 527 ms                                                                 | 521 ms: 1.01x faster                                                 |
| async_tree_io           | 699 ms                                                                 | 701 ms: 1.00x slower                                                 |
| async_tree_io_tg        | 665 ms                                                                 | 668 ms: 1.00x slower                                                 |
| async_tree_none_tg      | 256 ms                                                                 | 258 ms: 1.00x slower                                                 |
| Geometric mean          | (ref)                                                                  | 1.00x slower                                                         |

Benchmark hidden because not significant (4): async_tree_none, async_tree_cpu_io_mixed_tg, async_tree_memoization, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240221-darwin-arm64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| nbody          | 74.7 ms                                                                | 69.9 ms: 1.07x faster                                                |
| float          | 54.0 ms                                                                | 53.2 ms: 1.02x faster                                                |
| pidigits       | 282 ms                                                                 | 282 ms: 1.00x slower                                                 |
| Geometric mean | (ref)                                                                  | 1.03x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240221-darwin-arm64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 88.0 ms                                                                | 84.7 ms: 1.04x faster                                                |
| regex_v8       | 17.0 ms                                                                | 17.1 ms: 1.00x slower                                                |
| regex_effbot   | 2.47 ms                                                                | 2.56 ms: 1.04x slower                                                |
| regex_dna      | 145 ms                                                                 | 152 ms: 1.05x slower                                                 |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240221-darwin-arm64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| unpickle_pure_python | 156 us                                                                 | 149 us: 1.05x faster                                                 |
| xml_etree_generate   | 56.6 ms                                                                | 55.6 ms: 1.02x faster                                                |
| tomli_loads          | 1.39 sec                                                               | 1.37 sec: 1.01x faster                                               |
| xml_etree_iterparse  | 75.6 ms                                                                | 74.7 ms: 1.01x faster                                                |
| xml_etree_process    | 39.2 ms                                                                | 38.9 ms: 1.01x faster                                                |
| pickle_dict          | 18.1 us                                                                | 18.1 us: 1.00x slower                                                |
| json_loads           | 17.0 us                                                                | 17.1 us: 1.00x slower                                                |
| pickle_pure_python   | 196 us                                                                 | 197 us: 1.00x slower                                                 |
| pickle_list          | 2.96 us                                                                | 2.98 us: 1.01x slower                                                |
| unpickle_list        | 3.02 us                                                                | 3.04 us: 1.01x slower                                                |
| Geometric mean       | (ref)                                                                  | 1.01x faster                                                         |

Benchmark hidden because not significant (4): unpickle, json_dumps, xml_etree_parse, pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240221-darwin-arm64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 18.0 ms                                                                | 18.0 ms: 1.00x faster                                                |
| python_startup_no_site | 16.5 ms                                                                | 16.5 ms: 1.00x faster                                                |
| Geometric mean         | (ref)                                                                  | 1.00x faster                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240221-darwin-arm64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 7.64 ms                                                                | 6.85 ms: 1.12x faster                                                |

All benchmarks:
===============

| Benchmark               | bm-20240221-darwin-arm64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|-------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako                    | 7.64 ms                                                                | 6.85 ms: 1.12x faster                                                |
| nbody                   | 74.7 ms                                                                | 69.9 ms: 1.07x faster                                                |
| scimark_fft             | 210 ms                                                                 | 200 ms: 1.05x faster                                                 |
| unpickle_pure_python    | 156 us                                                                 | 149 us: 1.05x faster                                                 |
| hexiom                  | 5.48 ms                                                                | 5.27 ms: 1.04x faster                                                |
| scimark_sparse_mat_mult | 3.26 ms                                                                | 3.13 ms: 1.04x faster                                                |
| regex_compile           | 88.0 ms                                                                | 84.7 ms: 1.04x faster                                                |
| comprehensions          | 13.0 us                                                                | 12.6 us: 1.03x faster                                                |
| spectral_norm           | 76.4 ms                                                                | 74.0 ms: 1.03x faster                                                |
| sqlglot_optimize        | 36.3 ms                                                                | 35.5 ms: 1.02x faster                                                |
| pyflate                 | 345 ms                                                                 | 339 ms: 1.02x faster                                                 |
| go                      | 117 ms                                                                 | 115 ms: 1.02x faster                                                 |
| sqlglot_parse           | 843 us                                                                 | 827 us: 1.02x faster                                                 |
| xml_etree_generate      | 56.6 ms                                                                | 55.6 ms: 1.02x faster                                                |
| sqlglot_transpile       | 1.03 ms                                                                | 1.01 ms: 1.02x faster                                                |
| unpack_sequence         | 116 ns                                                                 | 115 ns: 1.02x faster                                                 |
| float                   | 54.0 ms                                                                | 53.2 ms: 1.02x faster                                                |
| tomli_loads             | 1.39 sec                                                               | 1.37 sec: 1.01x faster                                               |
| sqlglot_normalize       | 186 ms                                                                 | 184 ms: 1.01x faster                                                 |
| async_tree_cpu_io_mixed | 527 ms                                                                 | 521 ms: 1.01x faster                                                 |
| crypto_pyaes            | 48.4 ms                                                                | 47.8 ms: 1.01x faster                                                |
| xml_etree_iterparse     | 75.6 ms                                                                | 74.7 ms: 1.01x faster                                                |
| telco                   | 4.60 ms                                                                | 4.55 ms: 1.01x faster                                                |
| scimark_monte_carlo     | 46.6 ms                                                                | 46.1 ms: 1.01x faster                                                |
| chaos                   | 40.6 ms                                                                | 40.2 ms: 1.01x faster                                                |
| deepcopy_memo           | 26.6 us                                                                | 26.3 us: 1.01x faster                                                |
| deepcopy_reduce         | 2.01 us                                                                | 1.99 us: 1.01x faster                                                |
| sympy_str               | 145 ms                                                                 | 144 ms: 1.01x faster                                                 |
| raytrace                | 192 ms                                                                 | 191 ms: 1.01x faster                                                 |
| 2to3                    | 187 ms                                                                 | 185 ms: 1.01x faster                                                 |
| meteor_contest          | 74.6 ms                                                                | 74.0 ms: 1.01x faster                                                |
| deepcopy                | 228 us                                                                 | 226 us: 1.01x faster                                                 |
| xml_etree_process       | 39.2 ms                                                                | 38.9 ms: 1.01x faster                                                |
| sympy_expand            | 247 ms                                                                 | 246 ms: 1.01x faster                                                 |
| logging_simple          | 3.51 us                                                                | 3.49 us: 1.01x faster                                                |
| deltablue               | 2.56 ms                                                                | 2.55 ms: 1.00x faster                                                |
| scimark_lu              | 87.1 ms                                                                | 86.7 ms: 1.00x faster                                                |
| python_startup          | 18.0 ms                                                                | 18.0 ms: 1.00x faster                                                |
| python_startup_no_site  | 16.5 ms                                                                | 16.5 ms: 1.00x faster                                                |
| mdp                     | 1.64 sec                                                               | 1.63 sec: 1.00x faster                                               |
| coroutines              | 18.6 ms                                                                | 18.5 ms: 1.00x faster                                                |
| sympy_sum               | 76.9 ms                                                                | 76.6 ms: 1.00x faster                                                |
| generators              | 28.7 ms                                                                | 28.6 ms: 1.00x faster                                                |
| sympy_integrate         | 11.5 ms                                                                | 11.5 ms: 1.00x faster                                                |
| bench_thread_pool       | 519 us                                                                 | 517 us: 1.00x faster                                                 |
| logging_silent          | 70.9 ns                                                                | 70.7 ns: 1.00x faster                                                |
| sqlite_synth            | 1.59 us                                                                | 1.59 us: 1.00x faster                                                |
| pidigits                | 282 ms                                                                 | 282 ms: 1.00x slower                                                 |
| pickle_dict             | 18.1 us                                                                | 18.1 us: 1.00x slower                                                |
| json_loads              | 17.0 us                                                                | 17.1 us: 1.00x slower                                                |
| regex_v8                | 17.0 ms                                                                | 17.1 ms: 1.00x slower                                                |
| async_tree_io           | 699 ms                                                                 | 701 ms: 1.00x slower                                                 |
| dulwich_log             | 30.5 ms                                                                | 30.6 ms: 1.00x slower                                                |
| pickle_pure_python      | 196 us                                                                 | 197 us: 1.00x slower                                                 |
| pycparser               | 729 ms                                                                 | 732 ms: 1.00x slower                                                 |
| async_tree_io_tg        | 665 ms                                                                 | 668 ms: 1.00x slower                                                 |
| async_tree_none_tg      | 256 ms                                                                 | 258 ms: 1.00x slower                                                 |
| pickle_list             | 2.96 us                                                                | 2.98 us: 1.01x slower                                                |
| unpickle_list           | 3.02 us                                                                | 3.04 us: 1.01x slower                                                |
| gc_traversal            | 2.41 ms                                                                | 2.43 ms: 1.01x slower                                                |
| coverage                | 47.5 ms                                                                | 47.9 ms: 1.01x slower                                                |
| fannkuch                | 307 ms                                                                 | 311 ms: 1.01x slower                                                 |
| create_gc_cycles        | 710 us                                                                 | 723 us: 1.02x slower                                                 |
| richards_super          | 42.5 ms                                                                | 43.3 ms: 1.02x slower                                                |
| scimark_sor             | 113 ms                                                                 | 116 ms: 1.03x slower                                                 |
| regex_effbot            | 2.47 ms                                                                | 2.56 ms: 1.04x slower                                                |
| regex_dna               | 145 ms                                                                 | 152 ms: 1.05x slower                                                 |
| Geometric mean          | (ref)                                                                  | 1.01x faster                                                         |

Benchmark hidden because not significant (25): asyncio_tcp, tornado_http, asyncio_tcp_ssl, nqueens, unpickle, typing_runtime_protocols, async_generators, pprint_safe_repr, json_dumps, logging_format, xml_etree_parse, json, async_tree_none, pprint_pformat, pickle, asyncio_websockets, docutils, chameleon, async_tree_cpu_io_mixed_tg, bench_mp_pool, richards, async_tree_memoization, pathlib, async_tree_memoization_tg, mypy2


# HPT report

- Reliability score: 95.14% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.01x