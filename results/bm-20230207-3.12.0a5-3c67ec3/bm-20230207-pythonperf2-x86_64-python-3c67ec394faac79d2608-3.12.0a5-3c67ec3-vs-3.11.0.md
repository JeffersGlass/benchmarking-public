
# Results vs. 3.11.0

- fork: python
- ref: 3c67ec394faac79d2608
- machine: linux-x86_64
- commit hash: 3c67ec3
- commit date: 2023-02-07
- overall geometric mean: 1.04x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 282 ms: 1.02x faster                                                        |
| chameleon      | 7.92 ms                                                      | 7.46 ms: 1.06x faster                                                       |
| docutils       | 2.85 sec                                                     | 2.78 sec: 1.02x faster                                                      |
| html5lib       | 72.2 ms                                                      | 65.3 ms: 1.11x faster                                                       |
| tornado_http   | 124 ms                                                       | 117 ms: 1.07x faster                                                        |
| Geometric mean | (ref)                                                        | 1.05x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_memoization  | 629 ms                                                       | 601 ms: 1.05x faster                                                        |
| async_tree_none         | 518 ms                                                       | 503 ms: 1.03x faster                                                        |
| async_tree_cpu_io_mixed | 753 ms                                                       | 737 ms: 1.02x faster                                                        |
| Geometric mean          | (ref)                                                        | 1.03x faster                                                                |

Benchmark hidden because not significant (1): async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 74.9 ms                                                      | 71.9 ms: 1.04x faster                                                       |
| nbody          | 92.9 ms                                                      | 101 ms: 1.09x slower                                                        |
| Geometric mean | (ref)                                                        | 1.01x slower                                                                |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 145 ms: 1.08x faster                                                        |
| regex_v8       | 24.4 ms                                                      | 22.7 ms: 1.08x faster                                                       |
| regex_effbot   | 3.34 ms                                                      | 3.50 ms: 1.05x slower                                                       |
| regex_dna      | 227 ms                                                       | 240 ms: 1.06x slower                                                        |
| Geometric mean | (ref)                                                        | 1.01x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.0 ms: 1.32x faster                                                       |
| json_loads           | 28.9 us                                                      | 23.8 us: 1.21x faster                                                       |
| unpickle_pure_python | 238 us                                                       | 204 us: 1.17x faster                                                        |
| xml_etree_parse      | 155 ms                                                       | 142 ms: 1.09x faster                                                        |
| xml_etree_iterparse  | 107 ms                                                       | 103 ms: 1.04x faster                                                        |
| unpickle             | 13.3 us                                                      | 12.8 us: 1.04x faster                                                       |
| pickle_list          | 3.94 us                                                      | 3.84 us: 1.03x faster                                                       |
| pickle_dict          | 32.3 us                                                      | 31.6 us: 1.02x faster                                                       |
| unpickle_list        | 4.60 us                                                      | 4.50 us: 1.02x faster                                                       |
| pickle_pure_python   | 316 us                                                       | 312 us: 1.01x faster                                                        |
| xml_etree_process    | 55.9 ms                                                      | 55.6 ms: 1.00x faster                                                       |
| xml_etree_generate   | 79.7 ms                                                      | 80.6 ms: 1.01x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.07x faster                                                                |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 11.2 ms: 1.04x slower                                                       |
| python_startup_no_site | 7.73 ms                                                      | 8.25 ms: 1.07x slower                                                       |
| Geometric mean         | (ref)                                                        | 1.05x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako            | 11.0 ms                                                      | 10.3 ms: 1.07x faster                                                       |
| genshi_xml      | 57.1 ms                                                      | 53.4 ms: 1.07x faster                                                       |
| genshi_text     | 25.5 ms                                                      | 24.6 ms: 1.04x faster                                                       |
| django_template | 39.3 ms                                                      | 40.5 ms: 1.03x slower                                                       |
| Geometric mean  | (ref)                                                        | 1.04x faster                                                                |

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| asyncio_tcp             | 747 ms                                                       | 388 ms: 1.92x faster                                                        |
| json_dumps              | 13.3 ms                                                      | 10.0 ms: 1.32x faster                                                       |
| json_loads              | 28.9 us                                                      | 23.8 us: 1.21x faster                                                       |
| comprehensions          | 25.1 us                                                      | 21.3 us: 1.18x faster                                                       |
| gc_traversal            | 4.15 ms                                                      | 3.55 ms: 1.17x faster                                                       |
| unpickle_pure_python    | 238 us                                                       | 204 us: 1.17x faster                                                        |
| json                    | 5.58 ms                                                      | 4.94 ms: 1.13x faster                                                       |
| scimark_sparse_mat_mult | 4.06 ms                                                      | 3.61 ms: 1.13x faster                                                       |
| html5lib                | 72.2 ms                                                      | 65.3 ms: 1.11x faster                                                       |
| deltablue               | 3.97 ms                                                      | 3.60 ms: 1.10x faster                                                       |
| scimark_lu              | 114 ms                                                       | 104 ms: 1.10x faster                                                        |
| nqueens                 | 103 ms                                                       | 94.2 ms: 1.09x faster                                                       |
| pprint_pformat          | 1.67 sec                                                     | 1.53 sec: 1.09x faster                                                      |
| xml_etree_parse         | 155 ms                                                       | 142 ms: 1.09x faster                                                        |
| logging_simple          | 7.24 us                                                      | 6.67 us: 1.09x faster                                                       |
| pprint_safe_repr        | 805 ms                                                       | 744 ms: 1.08x faster                                                        |
| regex_compile           | 156 ms                                                       | 145 ms: 1.08x faster                                                        |
| sympy_sum               | 186 ms                                                       | 172 ms: 1.08x faster                                                        |
| chaos                   | 74.9 ms                                                      | 69.6 ms: 1.08x faster                                                       |
| richards                | 49.7 ms                                                      | 46.1 ms: 1.08x faster                                                       |
| sympy_str               | 337 ms                                                       | 313 ms: 1.08x faster                                                        |
| regex_v8                | 24.4 ms                                                      | 22.7 ms: 1.08x faster                                                       |
| hexiom                  | 6.98 ms                                                      | 6.49 ms: 1.08x faster                                                       |
| mako                    | 11.0 ms                                                      | 10.3 ms: 1.07x faster                                                       |
| genshi_xml              | 57.1 ms                                                      | 53.4 ms: 1.07x faster                                                       |
| tornado_http            | 124 ms                                                       | 117 ms: 1.07x faster                                                        |
| chameleon               | 7.92 ms                                                      | 7.46 ms: 1.06x faster                                                       |
| sympy_integrate         | 25.8 ms                                                      | 24.3 ms: 1.06x faster                                                       |
| unpack_sequence         | 45.7 ns                                                      | 43.3 ns: 1.06x faster                                                       |
| sympy_expand            | 553 ms                                                       | 526 ms: 1.05x faster                                                        |
| pyflate                 | 449 ms                                                       | 428 ms: 1.05x faster                                                        |
| deepcopy_memo           | 37.5 us                                                      | 35.8 us: 1.05x faster                                                       |
| async_tree_memoization  | 629 ms                                                       | 601 ms: 1.05x faster                                                        |
| scimark_sor             | 110 ms                                                       | 105 ms: 1.04x faster                                                        |
| float                   | 74.9 ms                                                      | 71.9 ms: 1.04x faster                                                       |
| xml_etree_iterparse     | 107 ms                                                       | 103 ms: 1.04x faster                                                        |
| mdp                     | 2.77 sec                                                     | 2.66 sec: 1.04x faster                                                      |
| logging_silent          | 100 ns                                                       | 96.5 ns: 1.04x faster                                                       |
| logging_format          | 7.71 us                                                      | 7.43 us: 1.04x faster                                                       |
| go                      | 158 ms                                                       | 152 ms: 1.04x faster                                                        |
| unpickle                | 13.3 us                                                      | 12.8 us: 1.04x faster                                                       |
| genshi_text             | 25.5 ms                                                      | 24.6 ms: 1.04x faster                                                       |
| telco                   | 6.81 ms                                                      | 6.59 ms: 1.03x faster                                                       |
| bench_thread_pool       | 1.00 ms                                                      | 971 us: 1.03x faster                                                        |
| raytrace                | 309 ms                                                       | 301 ms: 1.03x faster                                                        |
| async_tree_none         | 518 ms                                                       | 503 ms: 1.03x faster                                                        |
| deepcopy_reduce         | 3.40 us                                                      | 3.30 us: 1.03x faster                                                       |
| pickle_list             | 3.94 us                                                      | 3.84 us: 1.03x faster                                                       |
| pycparser               | 1.31 sec                                                     | 1.28 sec: 1.03x faster                                                      |
| docutils                | 2.85 sec                                                     | 2.78 sec: 1.02x faster                                                      |
| pickle_dict             | 32.3 us                                                      | 31.6 us: 1.02x faster                                                       |
| async_tree_cpu_io_mixed | 753 ms                                                       | 737 ms: 1.02x faster                                                        |
| unpickle_list           | 4.60 us                                                      | 4.50 us: 1.02x faster                                                       |
| sqlglot_optimize        | 59.0 ms                                                      | 57.7 ms: 1.02x faster                                                       |
| deepcopy                | 391 us                                                       | 383 us: 1.02x faster                                                        |
| crypto_pyaes            | 83.3 ms                                                      | 81.8 ms: 1.02x faster                                                       |
| 2to3                    | 287 ms                                                       | 282 ms: 1.02x faster                                                        |
| meteor_contest          | 131 ms                                                       | 128 ms: 1.02x faster                                                        |
| fannkuch                | 416 ms                                                       | 409 ms: 1.02x faster                                                        |
| pickle_pure_python      | 316 us                                                       | 312 us: 1.01x faster                                                        |
| dulwich_log             | 67.4 ms                                                      | 66.6 ms: 1.01x faster                                                       |
| sqlglot_normalize       | 122 ms                                                       | 120 ms: 1.01x faster                                                        |
| xml_etree_process       | 55.9 ms                                                      | 55.6 ms: 1.00x faster                                                       |
| spectral_norm           | 95.1 ms                                                      | 95.4 ms: 1.00x slower                                                       |
| scimark_monte_carlo     | 69.8 ms                                                      | 70.2 ms: 1.01x slower                                                       |
| sqlglot_transpile       | 1.91 ms                                                      | 1.93 ms: 1.01x slower                                                       |
| async_generators        | 322 ms                                                       | 325 ms: 1.01x slower                                                        |
| pathlib                 | 18.9 ms                                                      | 19.1 ms: 1.01x slower                                                       |
| xml_etree_generate      | 79.7 ms                                                      | 80.6 ms: 1.01x slower                                                       |
| sqlite_synth            | 2.52 us                                                      | 2.58 us: 1.02x slower                                                       |
| sqlglot_parse           | 1.51 ms                                                      | 1.56 ms: 1.03x slower                                                       |
| django_template         | 39.3 ms                                                      | 40.5 ms: 1.03x slower                                                       |
| create_gc_cycles        | 1.58 ms                                                      | 1.64 ms: 1.04x slower                                                       |
| python_startup          | 10.7 ms                                                      | 11.2 ms: 1.04x slower                                                       |
| coroutines              | 27.8 ms                                                      | 29.1 ms: 1.05x slower                                                       |
| regex_effbot            | 3.34 ms                                                      | 3.50 ms: 1.05x slower                                                       |
| regex_dna               | 227 ms                                                       | 240 ms: 1.06x slower                                                        |
| python_startup_no_site  | 7.73 ms                                                      | 8.25 ms: 1.07x slower                                                       |
| nbody                   | 92.9 ms                                                      | 101 ms: 1.09x slower                                                        |
| generators              | 54.6 ms                                                      | 60.4 ms: 1.10x slower                                                       |
| coverage                | 66.1 ms                                                      | 86.0 ms: 1.30x slower                                                       |
| dask                    | 410 ms                                                       | 562 ms: 1.37x slower                                                        |
| Geometric mean          | (ref)                                                        | 1.04x faster                                                                |

Benchmark hidden because not significant (6): scimark_fft, async_tree_io, pickle, pidigits, bench_mp_pool, thrift
Ignored benchmarks (16) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, gunicorn, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 1.00x