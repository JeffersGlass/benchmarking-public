# Results vs. base

- fork: brandtbucher
- ref: justin_relax
- machine: linux-x86_64
- commit hash: d5b3dec
- commit date: 2024-02-14
- overall geometric mean: 1.02x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240212-linux-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 276 ms                                                                 | 270 ms: 1.02x faster                                                 |
| chameleon      | 6.89 ms                                                                | 6.82 ms: 1.01x faster                                                |
| docutils       | 2.64 sec                                                               | 2.63 sec: 1.00x faster                                               |
| tornado_http   | 97.2 ms                                                                | 95.6 ms: 1.02x faster                                                |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240212-linux-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_memoization_tg  | 594 ms                                                                 | 571 ms: 1.04x faster                                                 |
| async_tree_none_tg         | 457 ms                                                                 | 447 ms: 1.02x faster                                                 |
| async_tree_cpu_io_mixed    | 723 ms                                                                 | 709 ms: 1.02x faster                                                 |
| async_tree_memoization     | 572 ms                                                                 | 561 ms: 1.02x faster                                                 |
| async_tree_cpu_io_mixed_tg | 732 ms                                                                 | 717 ms: 1.02x faster                                                 |
| async_tree_io_tg           | 1.21 sec                                                               | 1.19 sec: 1.02x faster                                               |
| async_tree_io              | 1.20 sec                                                               | 1.18 sec: 1.02x faster                                               |
| Geometric mean             | (ref)                                                                  | 1.02x faster                                                         |

Benchmark hidden because not significant (1): async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240212-linux-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| float          | 86.6 ms                                                                | 81.8 ms: 1.06x faster                                                |
| nbody          | 102 ms                                                                 | 99.1 ms: 1.03x faster                                                |
| pidigits       | 188 ms                                                                 | 187 ms: 1.00x faster                                                 |
| Geometric mean | (ref)                                                                  | 1.03x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240212-linux-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                                 | 134 ms: 1.05x faster                                                 |
| regex_v8       | 25.4 ms                                                                | 25.3 ms: 1.00x faster                                                |
| regex_effbot   | 3.61 ms                                                                | 3.74 ms: 1.04x slower                                                |
| regex_dna      | 219 ms                                                                 | 231 ms: 1.05x slower                                                 |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240212-linux-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| tomli_loads          | 2.20 sec                                                               | 2.05 sec: 1.07x faster                                               |
| unpickle_pure_python | 226 us                                                                 | 219 us: 1.03x faster                                                 |
| pickle_pure_python   | 299 us                                                                 | 293 us: 1.02x faster                                                 |
| json_dumps           | 10.5 ms                                                                | 10.3 ms: 1.02x faster                                                |
| xml_etree_iterparse  | 108 ms                                                                 | 106 ms: 1.01x faster                                                 |
| xml_etree_parse      | 157 ms                                                                 | 155 ms: 1.01x faster                                                 |
| json_loads           | 27.5 us                                                                | 27.3 us: 1.01x faster                                                |
| xml_etree_process    | 58.0 ms                                                                | 58.5 ms: 1.01x slower                                                |
| pickle_dict          | 33.3 us                                                                | 33.6 us: 1.01x slower                                                |
| pickle               | 11.6 us                                                                | 11.7 us: 1.01x slower                                                |
| pickle_list          | 4.91 us                                                                | 4.99 us: 1.01x slower                                                |
| unpickle_list        | 4.85 us                                                                | 5.09 us: 1.05x slower                                                |
| unpickle             | 15.0 us                                                                | 16.1 us: 1.08x slower                                                |
| Geometric mean       | (ref)                                                                  | 1.00x faster                                                         |

Benchmark hidden because not significant (1): xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240212-linux-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 10.3 ms                                                                | 10.2 ms: 1.01x faster                                                |
| python_startup_no_site | 8.87 ms                                                                | 8.80 ms: 1.01x faster                                                |
| Geometric mean         | (ref)                                                                  | 1.01x faster                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240212-linux-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 12.5 ms                                                                | 11.3 ms: 1.11x faster                                                |

All benchmarks:
===============

| Benchmark                  | bm-20240212-linux-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| spectral_norm              | 136 ms                                                                 | 108 ms: 1.25x faster                                                 |
| hexiom                     | 8.00 ms                                                                | 6.81 ms: 1.17x faster                                                |
| chaos                      | 70.5 ms                                                                | 62.5 ms: 1.13x faster                                                |
| mako                       | 12.5 ms                                                                | 11.3 ms: 1.11x faster                                                |
| scimark_sparse_mat_mult    | 5.35 ms                                                                | 4.85 ms: 1.10x faster                                                |
| gc_traversal               | 3.85 ms                                                                | 3.50 ms: 1.10x faster                                                |
| pprint_pformat             | 1.64 sec                                                               | 1.50 sec: 1.09x faster                                               |
| tomli_loads                | 2.20 sec                                                               | 2.05 sec: 1.07x faster                                               |
| pprint_safe_repr           | 788 ms                                                                 | 736 ms: 1.07x faster                                                 |
| comprehensions             | 19.3 us                                                                | 18.1 us: 1.07x faster                                                |
| mdp                        | 2.78 sec                                                               | 2.61 sec: 1.07x faster                                               |
| scimark_monte_carlo        | 74.0 ms                                                                | 69.7 ms: 1.06x faster                                                |
| float                      | 86.6 ms                                                                | 81.8 ms: 1.06x faster                                                |
| nqueens                    | 90.3 ms                                                                | 85.4 ms: 1.06x faster                                                |
| crypto_pyaes               | 78.0 ms                                                                | 73.7 ms: 1.06x faster                                                |
| regex_compile              | 141 ms                                                                 | 134 ms: 1.05x faster                                                 |
| fannkuch                   | 422 ms                                                                 | 403 ms: 1.05x faster                                                 |
| scimark_fft                | 371 ms                                                                 | 355 ms: 1.05x faster                                                 |
| unpack_sequence            | 48.3 ns                                                                | 46.4 ns: 1.04x faster                                                |
| logging_format             | 6.31 us                                                                | 6.06 us: 1.04x faster                                                |
| raytrace                   | 280 ms                                                                 | 269 ms: 1.04x faster                                                 |
| async_tree_memoization_tg  | 594 ms                                                                 | 571 ms: 1.04x faster                                                 |
| pyflate                    | 496 ms                                                                 | 478 ms: 1.04x faster                                                 |
| sympy_sum                  | 160 ms                                                                 | 155 ms: 1.04x faster                                                 |
| deepcopy_reduce            | 3.08 us                                                                | 2.98 us: 1.03x faster                                                |
| nbody                      | 102 ms                                                                 | 99.1 ms: 1.03x faster                                                |
| unpickle_pure_python       | 226 us                                                                 | 219 us: 1.03x faster                                                 |
| meteor_contest             | 110 ms                                                                 | 107 ms: 1.03x faster                                                 |
| deltablue                  | 3.38 ms                                                                | 3.28 ms: 1.03x faster                                                |
| json                       | 5.14 ms                                                                | 5.00 ms: 1.03x faster                                                |
| sympy_expand               | 480 ms                                                                 | 467 ms: 1.03x faster                                                 |
| sqlglot_optimize           | 56.0 ms                                                                | 54.5 ms: 1.03x faster                                                |
| sympy_str                  | 284 ms                                                                 | 276 ms: 1.03x faster                                                 |
| logging_simple             | 5.67 us                                                                | 5.53 us: 1.03x faster                                                |
| sqlglot_transpile          | 1.62 ms                                                                | 1.58 ms: 1.02x faster                                                |
| dulwich_log                | 68.4 ms                                                                | 66.8 ms: 1.02x faster                                                |
| sqlglot_parse              | 1.29 ms                                                                | 1.26 ms: 1.02x faster                                                |
| 2to3                       | 276 ms                                                                 | 270 ms: 1.02x faster                                                 |
| create_gc_cycles           | 1.50 ms                                                                | 1.46 ms: 1.02x faster                                                |
| async_tree_none_tg         | 457 ms                                                                 | 447 ms: 1.02x faster                                                 |
| go                         | 147 ms                                                                 | 144 ms: 1.02x faster                                                 |
| async_tree_cpu_io_mixed    | 723 ms                                                                 | 709 ms: 1.02x faster                                                 |
| telco                      | 8.61 ms                                                                | 8.44 ms: 1.02x faster                                                |
| async_tree_memoization     | 572 ms                                                                 | 561 ms: 1.02x faster                                                 |
| async_tree_cpu_io_mixed_tg | 732 ms                                                                 | 717 ms: 1.02x faster                                                 |
| pickle_pure_python         | 299 us                                                                 | 293 us: 1.02x faster                                                 |
| deepcopy_memo              | 38.4 us                                                                | 37.7 us: 1.02x faster                                                |
| sympy_integrate            | 20.9 ms                                                                | 20.5 ms: 1.02x faster                                                |
| sqlglot_normalize          | 109 ms                                                                 | 108 ms: 1.02x faster                                                 |
| tornado_http               | 97.2 ms                                                                | 95.6 ms: 1.02x faster                                                |
| async_tree_io_tg           | 1.21 sec                                                               | 1.19 sec: 1.02x faster                                               |
| json_dumps                 | 10.5 ms                                                                | 10.3 ms: 1.02x faster                                                |
| async_tree_io              | 1.20 sec                                                               | 1.18 sec: 1.02x faster                                               |
| deepcopy                   | 346 us                                                                 | 341 us: 1.01x faster                                                 |
| xml_etree_iterparse        | 108 ms                                                                 | 106 ms: 1.01x faster                                                 |
| dask                       | 366 ms                                                                 | 361 ms: 1.01x faster                                                 |
| chameleon                  | 6.89 ms                                                                | 6.82 ms: 1.01x faster                                                |
| python_startup             | 10.3 ms                                                                | 10.2 ms: 1.01x faster                                                |
| bench_thread_pool          | 843 us                                                                 | 835 us: 1.01x faster                                                 |
| python_startup_no_site     | 8.87 ms                                                                | 8.80 ms: 1.01x faster                                                |
| xml_etree_parse            | 157 ms                                                                 | 155 ms: 1.01x faster                                                 |
| json_loads                 | 27.5 us                                                                | 27.3 us: 1.01x faster                                                |
| asyncio_tcp                | 494 ms                                                                 | 491 ms: 1.01x faster                                                 |
| coroutines                 | 22.7 ms                                                                | 22.6 ms: 1.00x faster                                                |
| docutils                   | 2.64 sec                                                               | 2.63 sec: 1.00x faster                                               |
| regex_v8                   | 25.4 ms                                                                | 25.3 ms: 1.00x faster                                                |
| pidigits                   | 188 ms                                                                 | 187 ms: 1.00x faster                                                 |
| asyncio_tcp_ssl            | 1.81 sec                                                               | 1.80 sec: 1.00x faster                                               |
| scimark_lu                 | 113 ms                                                                 | 113 ms: 1.01x slower                                                 |
| xml_etree_process          | 58.0 ms                                                                | 58.5 ms: 1.01x slower                                                |
| pickle_dict                | 33.3 us                                                                | 33.6 us: 1.01x slower                                                |
| pickle                     | 11.6 us                                                                | 11.7 us: 1.01x slower                                                |
| scimark_sor                | 119 ms                                                                 | 120 ms: 1.01x slower                                                 |
| pathlib                    | 18.1 ms                                                                | 18.4 ms: 1.01x slower                                                |
| pickle_list                | 4.91 us                                                                | 4.99 us: 1.01x slower                                                |
| pycparser                  | 1.17 sec                                                               | 1.19 sec: 1.02x slower                                               |
| richards_super             | 51.9 ms                                                                | 53.2 ms: 1.03x slower                                                |
| richards                   | 45.9 ms                                                                | 47.5 ms: 1.04x slower                                                |
| regex_effbot               | 3.61 ms                                                                | 3.74 ms: 1.04x slower                                                |
| unpickle_list              | 4.85 us                                                                | 5.09 us: 1.05x slower                                                |
| regex_dna                  | 219 ms                                                                 | 231 ms: 1.05x slower                                                 |
| unpickle                   | 15.0 us                                                                | 16.1 us: 1.08x slower                                                |
| Geometric mean             | (ref)                                                                  | 1.02x faster                                                         |

Benchmark hidden because not significant (11): mypy2, async_tree_none, coverage, logging_silent, typing_runtime_protocols, xml_etree_generate, bench_mp_pool, async_generators, asyncio_websockets, sqlite_synth, generators


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 1.01x