# Results vs. base

- fork: faster-cpython
- ref: cold_exits
- machine: linux-x86_64
- commit hash: d73fe0a
- commit date: 2024-01-16
- overall geometric mean: 1.01x slower
- HPT reliability: 99.99%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 284 ms                                                                 | 290 ms: 1.02x slower                                                   |
| chameleon      | 7.37 ms                                                                | 7.32 ms: 1.01x faster                                                  |
| docutils       | 2.72 sec                                                               | 2.85 sec: 1.05x slower                                                 |
| Geometric mean | (ref)                                                                  | 1.02x slower                                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark        | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_io_tg | 1.21 sec                                                               | 1.21 sec: 1.00x slower                                                 |
| Geometric mean   | (ref)                                                                  | 1.00x slower                                                           |

Benchmark hidden because not significant (7): async_tree_memoization_tg, async_tree_cpu_io_mixed_tg, async_tree_none, async_tree_memoization, async_tree_io, async_tree_cpu_io_mixed, async_tree_none_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 131 ms                                                                 | 120 ms: 1.09x faster                                                   |
| float          | 100 ms                                                                 | 93.4 ms: 1.07x faster                                                  |
| pidigits       | 197 ms                                                                 | 189 ms: 1.04x faster                                                   |
| Geometric mean | (ref)                                                                  | 1.07x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 3.64 ms                                                                | 3.61 ms: 1.01x faster                                                  |
| regex_v8       | 24.9 ms                                                                | 25.2 ms: 1.01x slower                                                  |
| regex_dna      | 223 ms                                                                 | 227 ms: 1.02x slower                                                   |
| regex_compile  | 156 ms                                                                 | 172 ms: 1.10x slower                                                   |
| Geometric mean | (ref)                                                                  | 1.03x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|----------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| unpickle_list        | 5.51 us                                                                | 4.93 us: 1.12x faster                                                  |
| pickle               | 11.7 us                                                                | 11.4 us: 1.03x faster                                                  |
| pickle_pure_python   | 302 us                                                                 | 299 us: 1.01x faster                                                   |
| unpickle             | 14.9 us                                                                | 14.8 us: 1.01x faster                                                  |
| json_dumps           | 10.7 ms                                                                | 10.6 ms: 1.01x faster                                                  |
| json_loads           | 28.5 us                                                                | 28.4 us: 1.00x faster                                                  |
| xml_etree_generate   | 90.4 ms                                                                | 90.8 ms: 1.00x slower                                                  |
| xml_etree_process    | 61.8 ms                                                                | 62.2 ms: 1.01x slower                                                  |
| pickle_dict          | 34.9 us                                                                | 37.0 us: 1.06x slower                                                  |
| tomli_loads          | 2.54 sec                                                               | 2.73 sec: 1.07x slower                                                 |
| unpickle_pure_python | 240 us                                                                 | 278 us: 1.16x slower                                                   |
| Geometric mean       | (ref)                                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (3): xml_etree_iterparse, xml_etree_parse, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                | 10.1 ms: 1.00x slower                                                  |
| python_startup_no_site | 8.71 ms                                                                | 8.74 ms: 1.00x slower                                                  |
| Geometric mean         | (ref)                                                                  | 1.00x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|-----------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 15.0 ms                                                                | 14.0 ms: 1.07x faster                                                  |

All benchmarks:
===============

| Benchmark               | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|-------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| generators              | 36.4 ms                                                                | 29.4 ms: 1.24x faster                                                  |
| unpickle_list           | 5.51 us                                                                | 4.93 us: 1.12x faster                                                  |
| nbody                   | 131 ms                                                                 | 120 ms: 1.09x faster                                                   |
| spectral_norm           | 161 ms                                                                 | 149 ms: 1.08x faster                                                   |
| float                   | 100 ms                                                                 | 93.4 ms: 1.07x faster                                                  |
| mako                    | 15.0 ms                                                                | 14.0 ms: 1.07x faster                                                  |
| scimark_fft             | 480 ms                                                                 | 452 ms: 1.06x faster                                                   |
| scimark_sparse_mat_mult | 6.40 ms                                                                | 6.05 ms: 1.06x faster                                                  |
| gc_traversal            | 3.70 ms                                                                | 3.52 ms: 1.05x faster                                                  |
| comprehensions          | 22.9 us                                                                | 22.0 us: 1.04x faster                                                  |
| pidigits                | 197 ms                                                                 | 189 ms: 1.04x faster                                                   |
| crypto_pyaes            | 87.7 ms                                                                | 84.6 ms: 1.04x faster                                                  |
| chaos                   | 78.2 ms                                                                | 75.7 ms: 1.03x faster                                                  |
| pickle                  | 11.7 us                                                                | 11.4 us: 1.03x faster                                                  |
| deepcopy_memo           | 42.4 us                                                                | 41.3 us: 1.03x faster                                                  |
| regex_effbot            | 3.64 ms                                                                | 3.61 ms: 1.01x faster                                                  |
| pickle_pure_python      | 302 us                                                                 | 299 us: 1.01x faster                                                   |
| sqlite_synth            | 2.88 us                                                                | 2.86 us: 1.01x faster                                                  |
| meteor_contest          | 117 ms                                                                 | 116 ms: 1.01x faster                                                   |
| unpickle                | 14.9 us                                                                | 14.8 us: 1.01x faster                                                  |
| json_dumps              | 10.7 ms                                                                | 10.6 ms: 1.01x faster                                                  |
| chameleon               | 7.37 ms                                                                | 7.32 ms: 1.01x faster                                                  |
| json_loads              | 28.5 us                                                                | 28.4 us: 1.00x faster                                                  |
| async_tree_io_tg        | 1.21 sec                                                               | 1.21 sec: 1.00x slower                                                 |
| python_startup          | 10.1 ms                                                                | 10.1 ms: 1.00x slower                                                  |
| python_startup_no_site  | 8.71 ms                                                                | 8.74 ms: 1.00x slower                                                  |
| xml_etree_generate      | 90.4 ms                                                                | 90.8 ms: 1.00x slower                                                  |
| mdp                     | 2.65 sec                                                               | 2.66 sec: 1.00x slower                                                 |
| bench_thread_pool       | 851 us                                                                 | 855 us: 1.00x slower                                                   |
| deepcopy_reduce         | 3.13 us                                                                | 3.15 us: 1.00x slower                                                  |
| asyncio_tcp_ssl         | 1.80 sec                                                               | 1.81 sec: 1.01x slower                                                 |
| unpack_sequence         | 54.0 ns                                                                | 54.3 ns: 1.01x slower                                                  |
| xml_etree_process       | 61.8 ms                                                                | 62.2 ms: 1.01x slower                                                  |
| deltablue               | 5.11 ms                                                                | 5.14 ms: 1.01x slower                                                  |
| async_generators        | 454 ms                                                                 | 458 ms: 1.01x slower                                                   |
| fannkuch                | 479 ms                                                                 | 485 ms: 1.01x slower                                                   |
| create_gc_cycles        | 1.47 ms                                                                | 1.49 ms: 1.01x slower                                                  |
| regex_v8                | 24.9 ms                                                                | 25.2 ms: 1.01x slower                                                  |
| sympy_sum               | 162 ms                                                                 | 164 ms: 1.02x slower                                                   |
| pprint_pformat          | 1.77 sec                                                               | 1.80 sec: 1.02x slower                                                 |
| 2to3                    | 284 ms                                                                 | 290 ms: 1.02x slower                                                   |
| coroutines              | 22.0 ms                                                                | 22.4 ms: 1.02x slower                                                  |
| regex_dna               | 223 ms                                                                 | 227 ms: 1.02x slower                                                   |
| sympy_integrate         | 21.4 ms                                                                | 21.8 ms: 1.02x slower                                                  |
| sympy_expand            | 493 ms                                                                 | 503 ms: 1.02x slower                                                   |
| sympy_str               | 296 ms                                                                 | 302 ms: 1.02x slower                                                   |
| pycparser               | 1.25 sec                                                               | 1.28 sec: 1.02x slower                                                 |
| hexiom                  | 9.08 ms                                                                | 9.28 ms: 1.02x slower                                                  |
| raytrace                | 308 ms                                                                 | 316 ms: 1.02x slower                                                   |
| pathlib                 | 18.7 ms                                                                | 19.1 ms: 1.02x slower                                                  |
| pyflate                 | 562 ms                                                                 | 579 ms: 1.03x slower                                                   |
| dulwich_log             | 69.2 ms                                                                | 71.3 ms: 1.03x slower                                                  |
| pprint_safe_repr        | 845 ms                                                                 | 873 ms: 1.03x slower                                                   |
| scimark_monte_carlo     | 86.2 ms                                                                | 89.4 ms: 1.04x slower                                                  |
| sqlglot_normalize       | 115 ms                                                                 | 119 ms: 1.04x slower                                                   |
| docutils                | 2.72 sec                                                               | 2.85 sec: 1.05x slower                                                 |
| sqlglot_optimize        | 58.6 ms                                                                | 61.5 ms: 1.05x slower                                                  |
| sqlglot_transpile       | 1.66 ms                                                                | 1.75 ms: 1.05x slower                                                  |
| pickle_dict             | 34.9 us                                                                | 37.0 us: 1.06x slower                                                  |
| logging_simple          | 6.05 us                                                                | 6.44 us: 1.06x slower                                                  |
| sqlglot_parse           | 1.33 ms                                                                | 1.42 ms: 1.07x slower                                                  |
| tomli_loads             | 2.54 sec                                                               | 2.73 sec: 1.07x slower                                                 |
| logging_format          | 6.71 us                                                                | 7.24 us: 1.08x slower                                                  |
| go                      | 160 ms                                                                 | 176 ms: 1.10x slower                                                   |
| regex_compile           | 156 ms                                                                 | 172 ms: 1.10x slower                                                   |
| scimark_sor             | 132 ms                                                                 | 150 ms: 1.14x slower                                                   |
| unpickle_pure_python    | 240 us                                                                 | 278 us: 1.16x slower                                                   |
| scimark_lu              | 119 ms                                                                 | 152 ms: 1.28x slower                                                   |
| richards                | 48.9 ms                                                                | 68.4 ms: 1.40x slower                                                  |
| richards_super          | 55.2 ms                                                                | 77.6 ms: 1.41x slower                                                  |
| Geometric mean          | (ref)                                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (23): xml_etree_iterparse, coverage, nqueens, async_tree_memoization_tg, async_tree_cpu_io_mixed_tg, bench_mp_pool, async_tree_none, asyncio_tcp, json, asyncio_websockets, async_tree_memoization, async_tree_io, deepcopy, logging_silent, async_tree_cpu_io_mixed, xml_etree_parse, async_tree_none_tg, telco, pickle_list, tornado_http, typing_runtime_protocols, dask, mypy2


# HPT report

- Reliability score: 99.99% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.01x