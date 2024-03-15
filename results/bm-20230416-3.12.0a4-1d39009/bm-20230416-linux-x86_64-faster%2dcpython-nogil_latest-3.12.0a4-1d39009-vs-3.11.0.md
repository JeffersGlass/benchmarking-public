
# Results vs. 3.11.0

- fork: faster-cpython
- ref: nogil_latest
- machine: linux-x86_64
- commit hash: 1d39009
- commit date: 2023-04-16
- overall geometric mean: 1.01x slower \*
- HPT reliability: 99.82%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.35x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230416-linux-x86_64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 290 ms: 1.10x slower                                                    |
| chameleon      | 6.70 ms                                                | 7.81 ms: 1.17x slower                                                   |
| docutils       | 2.66 sec                                               | 3.15 sec: 1.18x slower                                                  |
| html5lib       | 64.8 ms                                                | 69.2 ms: 1.07x slower                                                   |
| Geometric mean | (ref)                                                  | 1.13x slower                                                            |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230416-linux-x86_64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|-------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| async_tree_io           | 1.29 sec                                               | 616 ms: 2.09x faster                                                    |
| async_tree_none         | 528 ms                                                 | 311 ms: 1.70x faster                                                    |
| async_tree_memoization  | 639 ms                                                 | 381 ms: 1.68x faster                                                    |
| async_tree_cpu_io_mixed | 749 ms                                                 | 534 ms: 1.40x faster                                                    |
| Geometric mean          | (ref)                                                  | 1.70x faster                                                            |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230416-linux-x86_64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| float          | 78.9 ms                                                | 65.9 ms: 1.20x faster                                                   |
| pidigits       | 194 ms                                                 | 186 ms: 1.04x faster                                                    |
| nbody          | 96.0 ms                                                | 107 ms: 1.12x slower                                                    |
| Geometric mean | (ref)                                                  | 1.04x faster                                                            |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230416-linux-x86_64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| regex_v8       | 22.9 ms                                                | 21.1 ms: 1.09x faster                                                   |
| regex_effbot   | 3.51 ms                                                | 3.46 ms: 1.01x faster                                                   |
| regex_dna      | 205 ms                                                 | 205 ms: 1.00x slower                                                    |
| regex_compile  | 141 ms                                                 | 152 ms: 1.08x slower                                                    |
| Geometric mean | (ref)                                                  | 1.00x faster                                                            |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230416-linux-x86_64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                   |
| xml_etree_parse      | 164 ms                                                 | 137 ms: 1.19x faster                                                    |
| pickle_dict          | 34.6 us                                                | 30.0 us: 1.15x faster                                                   |
| pickle               | 11.0 us                                                | 10.3 us: 1.07x faster                                                   |
| pickle_list          | 4.59 us                                                | 4.33 us: 1.06x faster                                                   |
| unpickle_pure_python | 242 us                                                 | 229 us: 1.06x faster                                                    |
| json_loads           | 29.2 us                                                | 28.0 us: 1.04x faster                                                   |
| unpickle_list        | 5.21 us                                                | 5.20 us: 1.00x faster                                                   |
| xml_etree_generate   | 81.1 ms                                                | 83.7 ms: 1.03x slower                                                   |
| xml_etree_iterparse  | 108 ms                                                 | 114 ms: 1.05x slower                                                    |
| xml_etree_process    | 56.9 ms                                                | 61.3 ms: 1.08x slower                                                   |
| unpickle             | 13.8 us                                                | 15.5 us: 1.12x slower                                                   |
| Geometric mean       | (ref)                                                  | 1.04x faster                                                            |

Benchmark hidden because not significant (1): pickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230416-linux-x86_64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 9.18 ms: 1.07x slower                                                   |
| python_startup_no_site | 6.01 ms                                                | 6.59 ms: 1.10x slower                                                   |
| Geometric mean         | (ref)                                                  | 1.08x slower                                                            |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230416-linux-x86_64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|-----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| genshi_xml      | 53.4 ms                                                | 52.0 ms: 1.03x faster                                                   |
| genshi_text     | 22.5 ms                                                | 24.4 ms: 1.08x slower                                                   |
| django_template | 33.5 ms                                                | 37.4 ms: 1.11x slower                                                   |
| mako            | 10.7 ms                                                | 13.2 ms: 1.24x slower                                                   |
| Geometric mean  | (ref)                                                  | 1.10x slower                                                            |

All benchmarks:
===============

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230416-linux-x86_64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|-------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| async_tree_io           | 1.29 sec                                               | 616 ms: 2.09x faster                                                    |
| async_tree_none         | 528 ms                                                 | 311 ms: 1.70x faster                                                    |
| async_tree_memoization  | 639 ms                                                 | 381 ms: 1.68x faster                                                    |
| asyncio_tcp             | 875 ms                                                 | 525 ms: 1.67x faster                                                    |
| async_tree_cpu_io_mixed | 749 ms                                                 | 534 ms: 1.40x faster                                                    |
| json_dumps              | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                   |
| float                   | 78.9 ms                                                | 65.9 ms: 1.20x faster                                                   |
| xml_etree_parse         | 164 ms                                                 | 137 ms: 1.19x faster                                                    |
| pickle_dict             | 34.6 us                                                | 30.0 us: 1.15x faster                                                   |
| gc_traversal            | 4.01 ms                                                | 3.67 ms: 1.09x faster                                                   |
| regex_v8                | 22.9 ms                                                | 21.1 ms: 1.09x faster                                                   |
| logging_silent          | 111 ns                                                 | 104 ns: 1.07x faster                                                    |
| pickle                  | 11.0 us                                                | 10.3 us: 1.07x faster                                                   |
| pickle_list             | 4.59 us                                                | 4.33 us: 1.06x faster                                                   |
| unpickle_pure_python    | 242 us                                                 | 229 us: 1.06x faster                                                    |
| pidigits                | 194 ms                                                 | 186 ms: 1.04x faster                                                    |
| json_loads              | 29.2 us                                                | 28.0 us: 1.04x faster                                                   |
| json                    | 5.24 ms                                                | 5.06 ms: 1.04x faster                                                   |
| pycparser               | 1.19 sec                                               | 1.15 sec: 1.03x faster                                                  |
| richards                | 49.8 ms                                                | 48.4 ms: 1.03x faster                                                   |
| genshi_xml              | 53.4 ms                                                | 52.0 ms: 1.03x faster                                                   |
| nqueens                 | 87.9 ms                                                | 85.8 ms: 1.02x faster                                                   |
| scimark_sparse_mat_mult | 5.03 ms                                                | 4.94 ms: 1.02x faster                                                   |
| pathlib                 | 18.5 ms                                                | 18.2 ms: 1.02x faster                                                   |
| go                      | 149 ms                                                 | 146 ms: 1.02x faster                                                    |
| regex_effbot            | 3.51 ms                                                | 3.46 ms: 1.01x faster                                                   |
| coroutines              | 27.0 ms                                                | 26.8 ms: 1.01x faster                                                   |
| bench_mp_pool           | 24.0 ms                                                | 23.8 ms: 1.01x faster                                                   |
| unpickle_list           | 5.21 us                                                | 5.20 us: 1.00x faster                                                   |
| regex_dna               | 205 ms                                                 | 205 ms: 1.00x slower                                                    |
| mdp                     | 2.77 sec                                               | 2.79 sec: 1.00x slower                                                  |
| async_generators        | 374 ms                                                 | 377 ms: 1.01x slower                                                    |
| scimark_sor             | 121 ms                                                 | 123 ms: 1.01x slower                                                    |
| sqlglot_normalize       | 113 ms                                                 | 115 ms: 1.02x slower                                                    |
| pprint_pformat          | 1.55 sec                                               | 1.58 sec: 1.02x slower                                                  |
| sqlite_synth            | 2.57 us                                                | 2.62 us: 1.02x slower                                                   |
| pprint_safe_repr        | 747 ms                                                 | 765 ms: 1.02x slower                                                    |
| deepcopy                | 365 us                                                 | 375 us: 1.03x slower                                                    |
| sqlglot_optimize        | 55.3 ms                                                | 57.1 ms: 1.03x slower                                                   |
| xml_etree_generate      | 81.1 ms                                                | 83.7 ms: 1.03x slower                                                   |
| spectral_norm           | 108 ms                                                 | 112 ms: 1.04x slower                                                    |
| chaos                   | 71.9 ms                                                | 74.6 ms: 1.04x slower                                                   |
| xml_etree_iterparse     | 108 ms                                                 | 114 ms: 1.05x slower                                                    |
| generators              | 74.9 ms                                                | 78.8 ms: 1.05x slower                                                   |
| dulwich_log             | 64.6 ms                                                | 68.1 ms: 1.05x slower                                                   |
| sympy_integrate         | 21.5 ms                                                | 22.8 ms: 1.06x slower                                                   |
| deepcopy_reduce         | 3.22 us                                                | 3.42 us: 1.06x slower                                                   |
| crypto_pyaes            | 76.7 ms                                                | 81.8 ms: 1.07x slower                                                   |
| html5lib                | 64.8 ms                                                | 69.2 ms: 1.07x slower                                                   |
| python_startup          | 8.56 ms                                                | 9.18 ms: 1.07x slower                                                   |
| fannkuch                | 405 ms                                                 | 436 ms: 1.08x slower                                                    |
| regex_compile           | 141 ms                                                 | 152 ms: 1.08x slower                                                    |
| xml_etree_process       | 56.9 ms                                                | 61.3 ms: 1.08x slower                                                   |
| scimark_monte_carlo     | 70.7 ms                                                | 76.4 ms: 1.08x slower                                                   |
| genshi_text             | 22.5 ms                                                | 24.4 ms: 1.08x slower                                                   |
| pyflate                 | 434 ms                                                 | 470 ms: 1.08x slower                                                    |
| thrift                  | 784 us                                                 | 851 us: 1.09x slower                                                    |
| python_startup_no_site  | 6.01 ms                                                | 6.59 ms: 1.10x slower                                                   |
| 2to3                    | 264 ms                                                 | 290 ms: 1.10x slower                                                    |
| scimark_lu              | 116 ms                                                 | 128 ms: 1.10x slower                                                    |
| sympy_str               | 297 ms                                                 | 329 ms: 1.11x slower                                                    |
| scimark_fft             | 345 ms                                                 | 383 ms: 1.11x slower                                                    |
| sympy_expand            | 484 ms                                                 | 537 ms: 1.11x slower                                                    |
| create_gc_cycles        | 1.43 ms                                                | 1.59 ms: 1.11x slower                                                   |
| django_template         | 33.5 ms                                                | 37.4 ms: 1.11x slower                                                   |
| nbody                   | 96.0 ms                                                | 107 ms: 1.12x slower                                                    |
| comprehensions          | 23.6 us                                                | 26.3 us: 1.12x slower                                                   |
| unpickle                | 13.8 us                                                | 15.5 us: 1.12x slower                                                   |
| raytrace                | 309 ms                                                 | 346 ms: 1.12x slower                                                    |
| logging_format          | 6.81 us                                                | 7.66 us: 1.13x slower                                                   |
| logging_simple          | 6.22 us                                                | 7.00 us: 1.13x slower                                                   |
| djangocms               | 33.5 us                                                | 37.9 us: 1.13x slower                                                   |
| sympy_sum               | 169 ms                                                 | 192 ms: 1.14x slower                                                    |
| meteor_contest          | 109 ms                                                 | 124 ms: 1.14x slower                                                    |
| chameleon               | 6.70 ms                                                | 7.81 ms: 1.17x slower                                                   |
| docutils                | 2.66 sec                                               | 3.15 sec: 1.18x slower                                                  |
| sqlglot_transpile       | 1.75 ms                                                | 2.10 ms: 1.20x slower                                                   |
| mako                    | 10.7 ms                                                | 13.2 ms: 1.24x slower                                                   |
| sqlglot_parse           | 1.43 ms                                                | 1.79 ms: 1.25x slower                                                   |
| unpack_sequence         | 43.5 ns                                                | 58.1 ns: 1.34x slower                                                   |
| coverage                | 78.8 ms                                                | 109 ms: 1.39x slower                                                    |
| bench_thread_pool       | 834 us                                                 | 1.64 ms: 1.97x slower                                                   |
| Geometric mean          | (ref)                                                  | 1.01x slower                                                            |

Benchmark hidden because not significant (5): deltablue, deepcopy_memo, hexiom, pickle_pure_python, telco
Ignored benchmarks (18) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, dask, flaskblogging, gunicorn, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols


# HPT report

- Reliability score: 99.82% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.35x