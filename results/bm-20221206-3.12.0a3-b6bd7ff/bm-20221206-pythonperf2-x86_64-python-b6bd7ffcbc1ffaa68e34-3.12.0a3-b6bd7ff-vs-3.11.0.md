
# Results vs. 3.11.0

- fork: python
- ref: b6bd7ffcbc1ffaa68e34
- machine: linux-x86_64
- commit hash: b6bd7ff
- commit date: 2022-12-06
- overall geometric mean: 1.02x faster \*
- HPT reliability: 99.50%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 281 ms: 1.02x faster                                                        |
| chameleon      | 7.92 ms                                                      | 7.51 ms: 1.06x faster                                                       |
| docutils       | 2.85 sec                                                     | 2.76 sec: 1.03x faster                                                      |
| html5lib       | 72.2 ms                                                      | 66.2 ms: 1.09x faster                                                       |
| Geometric mean | (ref)                                                        | 1.05x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 753 ms                                                       | 767 ms: 1.02x slower                                                        |
| async_tree_none         | 518 ms                                                       | 531 ms: 1.03x slower                                                        |
| Geometric mean          | (ref)                                                        | 1.01x slower                                                                |

Benchmark hidden because not significant (2): async_tree_memoization, async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 74.9 ms                                                      | 73.2 ms: 1.02x faster                                                       |
| pidigits       | 251 ms                                                       | 250 ms: 1.00x faster                                                        |
| Geometric mean | (ref)                                                        | 1.00x faster                                                                |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_v8       | 24.4 ms                                                      | 22.3 ms: 1.09x faster                                                       |
| regex_compile  | 156 ms                                                       | 150 ms: 1.04x faster                                                        |
| regex_dna      | 227 ms                                                       | 233 ms: 1.02x slower                                                        |
| regex_effbot   | 3.34 ms                                                      | 3.44 ms: 1.03x slower                                                       |
| Geometric mean | (ref)                                                        | 1.02x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.3 ms: 1.28x faster                                                       |
| json_loads           | 28.9 us                                                      | 24.2 us: 1.20x faster                                                       |
| unpickle_pure_python | 238 us                                                       | 212 us: 1.12x faster                                                        |
| xml_etree_parse      | 155 ms                                                       | 141 ms: 1.10x faster                                                        |
| unpickle_list        | 4.60 us                                                      | 4.47 us: 1.03x faster                                                       |
| pickle_dict          | 32.3 us                                                      | 31.9 us: 1.01x faster                                                       |
| unpickle             | 13.3 us                                                      | 13.1 us: 1.01x faster                                                       |
| pickle_list          | 3.94 us                                                      | 3.90 us: 1.01x faster                                                       |
| xml_etree_generate   | 79.7 ms                                                      | 78.9 ms: 1.01x faster                                                       |
| pickle               | 9.89 us                                                      | 9.84 us: 1.01x faster                                                       |
| xml_etree_process    | 55.9 ms                                                      | 55.6 ms: 1.00x faster                                                       |
| Geometric mean       | (ref)                                                        | 1.06x faster                                                                |

Benchmark hidden because not significant (2): pickle_pure_python, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 10.8 ms: 1.00x slower                                                       |
| python_startup_no_site | 7.73 ms                                                      | 7.86 ms: 1.02x slower                                                       |
| Geometric mean         | (ref)                                                        | 1.01x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| genshi_xml      | 57.1 ms                                                      | 53.5 ms: 1.07x faster                                                       |
| mako            | 11.0 ms                                                      | 10.4 ms: 1.06x faster                                                       |
| django_template | 39.3 ms                                                      | 39.6 ms: 1.01x slower                                                       |
| genshi_text     | 25.5 ms                                                      | 25.8 ms: 1.01x slower                                                       |
| Geometric mean  | (ref)                                                        | 1.03x faster                                                                |

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps              | 13.3 ms                                                      | 10.3 ms: 1.28x faster                                                       |
| json_loads              | 28.9 us                                                      | 24.2 us: 1.20x faster                                                       |
| scimark_lu              | 114 ms                                                       | 100 ms: 1.14x faster                                                        |
| unpickle_pure_python    | 238 us                                                       | 212 us: 1.12x faster                                                        |
| xml_etree_parse         | 155 ms                                                       | 141 ms: 1.10x faster                                                        |
| gc_traversal            | 4.15 ms                                                      | 3.79 ms: 1.09x faster                                                       |
| regex_v8                | 24.4 ms                                                      | 22.3 ms: 1.09x faster                                                       |
| json                    | 5.58 ms                                                      | 5.11 ms: 1.09x faster                                                       |
| html5lib                | 72.2 ms                                                      | 66.2 ms: 1.09x faster                                                       |
| scimark_sparse_mat_mult | 4.06 ms                                                      | 3.73 ms: 1.09x faster                                                       |
| deltablue               | 3.97 ms                                                      | 3.67 ms: 1.08x faster                                                       |
| richards                | 49.7 ms                                                      | 46.1 ms: 1.08x faster                                                       |
| pprint_pformat          | 1.67 sec                                                     | 1.56 sec: 1.07x faster                                                      |
| genshi_xml              | 57.1 ms                                                      | 53.5 ms: 1.07x faster                                                       |
| mako                    | 11.0 ms                                                      | 10.4 ms: 1.06x faster                                                       |
| pprint_safe_repr        | 805 ms                                                       | 758 ms: 1.06x faster                                                        |
| chameleon               | 7.92 ms                                                      | 7.51 ms: 1.06x faster                                                       |
| bench_mp_pool           | 4.70 ms                                                      | 4.46 ms: 1.05x faster                                                       |
| fannkuch                | 416 ms                                                       | 398 ms: 1.04x faster                                                        |
| thrift                  | 931 us                                                       | 894 us: 1.04x faster                                                        |
| pycparser               | 1.31 sec                                                     | 1.26 sec: 1.04x faster                                                      |
| regex_compile           | 156 ms                                                       | 150 ms: 1.04x faster                                                        |
| hexiom                  | 6.98 ms                                                      | 6.73 ms: 1.04x faster                                                       |
| deepcopy_memo           | 37.5 us                                                      | 36.2 us: 1.04x faster                                                       |
| docutils                | 2.85 sec                                                     | 2.76 sec: 1.03x faster                                                      |
| telco                   | 6.81 ms                                                      | 6.60 ms: 1.03x faster                                                       |
| logging_simple          | 7.24 us                                                      | 7.03 us: 1.03x faster                                                       |
| deepcopy                | 391 us                                                       | 380 us: 1.03x faster                                                        |
| unpickle_list           | 4.60 us                                                      | 4.47 us: 1.03x faster                                                       |
| sympy_expand            | 553 ms                                                       | 539 ms: 1.03x faster                                                        |
| float                   | 74.9 ms                                                      | 73.2 ms: 1.02x faster                                                       |
| 2to3                    | 287 ms                                                       | 281 ms: 1.02x faster                                                        |
| pyflate                 | 449 ms                                                       | 440 ms: 1.02x faster                                                        |
| sqlglot_transpile       | 1.91 ms                                                      | 1.87 ms: 1.02x faster                                                       |
| crypto_pyaes            | 83.3 ms                                                      | 81.8 ms: 1.02x faster                                                       |
| sympy_str               | 337 ms                                                       | 331 ms: 1.02x faster                                                        |
| mdp                     | 2.77 sec                                                     | 2.73 sec: 1.01x faster                                                      |
| pickle_dict             | 32.3 us                                                      | 31.9 us: 1.01x faster                                                       |
| meteor_contest          | 131 ms                                                       | 129 ms: 1.01x faster                                                        |
| sympy_sum               | 186 ms                                                       | 183 ms: 1.01x faster                                                        |
| unpickle                | 13.3 us                                                      | 13.1 us: 1.01x faster                                                       |
| pickle_list             | 3.94 us                                                      | 3.90 us: 1.01x faster                                                       |
| dulwich_log             | 67.4 ms                                                      | 66.7 ms: 1.01x faster                                                       |
| xml_etree_generate      | 79.7 ms                                                      | 78.9 ms: 1.01x faster                                                       |
| sympy_integrate         | 25.8 ms                                                      | 25.6 ms: 1.01x faster                                                       |
| sqlglot_optimize        | 59.0 ms                                                      | 58.5 ms: 1.01x faster                                                       |
| deepcopy_reduce         | 3.40 us                                                      | 3.37 us: 1.01x faster                                                       |
| asyncio_tcp             | 747 ms                                                       | 743 ms: 1.01x faster                                                        |
| pickle                  | 9.89 us                                                      | 9.84 us: 1.01x faster                                                       |
| pidigits                | 251 ms                                                       | 250 ms: 1.00x faster                                                        |
| xml_etree_process       | 55.9 ms                                                      | 55.6 ms: 1.00x faster                                                       |
| pathlib                 | 18.9 ms                                                      | 19.0 ms: 1.00x slower                                                       |
| python_startup          | 10.7 ms                                                      | 10.8 ms: 1.00x slower                                                       |
| scimark_fft             | 281 ms                                                       | 282 ms: 1.01x slower                                                        |
| coroutines              | 27.8 ms                                                      | 28.0 ms: 1.01x slower                                                       |
| django_template         | 39.3 ms                                                      | 39.6 ms: 1.01x slower                                                       |
| go                      | 158 ms                                                       | 159 ms: 1.01x slower                                                        |
| spectral_norm           | 95.1 ms                                                      | 96.2 ms: 1.01x slower                                                       |
| genshi_text             | 25.5 ms                                                      | 25.8 ms: 1.01x slower                                                       |
| python_startup_no_site  | 7.73 ms                                                      | 7.86 ms: 1.02x slower                                                       |
| async_tree_cpu_io_mixed | 753 ms                                                       | 767 ms: 1.02x slower                                                        |
| regex_dna               | 227 ms                                                       | 233 ms: 1.02x slower                                                        |
| async_tree_none         | 518 ms                                                       | 531 ms: 1.03x slower                                                        |
| regex_effbot            | 3.34 ms                                                      | 3.44 ms: 1.03x slower                                                       |
| sqlite_synth            | 2.52 us                                                      | 2.60 us: 1.03x slower                                                       |
| scimark_monte_carlo     | 69.8 ms                                                      | 72.7 ms: 1.04x slower                                                       |
| async_generators        | 322 ms                                                       | 335 ms: 1.04x slower                                                        |
| chaos                   | 74.9 ms                                                      | 78.3 ms: 1.04x slower                                                       |
| raytrace                | 309 ms                                                       | 327 ms: 1.06x slower                                                        |
| comprehensions          | 25.1 us                                                      | 27.3 us: 1.09x slower                                                       |
| generators              | 54.6 ms                                                      | 60.8 ms: 1.11x slower                                                       |
| coverage                | 66.1 ms                                                      | 85.0 ms: 1.29x slower                                                       |
| Geometric mean          | (ref)                                                        | 1.02x faster                                                                |

Benchmark hidden because not significant (15): async_tree_memoization, logging_silent, nqueens, bench_thread_pool, unpack_sequence, sqlglot_normalize, scimark_sor, dask, pickle_pure_python, logging_format, sqlglot_parse, async_tree_io, xml_etree_iterparse, create_gc_cycles, nbody
Ignored benchmarks (17) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, gunicorn, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols


# HPT report

- Reliability score: 99.50% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.02x