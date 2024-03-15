
# Results vs. 3.12.0

- fork: python
- ref: 7f5e3f04f838686d65f1
- machine: windows-amd64
- commit hash: 7f5e3f0
- commit date: 2024-02-21
- overall geometric mean: 1.02x slower \*
- HPT reliability: 87.12%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 228 ms: 1.05x slower                                                        |
| chameleon      | 4.98 ms                                                     | 4.93 ms: 1.01x faster                                                       |
| docutils       | 1.66 sec                                                    | 1.64 sec: 1.01x faster                                                      |
| tornado_http   | 89.5 ms                                                     | 85.6 ms: 1.05x faster                                                       |
| Geometric mean | (ref)                                                       | 1.01x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 261 ms: 1.12x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 445 ms: 1.10x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 459 ms: 1.09x faster                                                        |
| async_tree_none_tg         | 285 ms                                                      | 265 ms: 1.08x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 345 ms: 1.06x faster                                                        |
| async_tree_io_tg           | 771 ms                                                      | 745 ms: 1.03x faster                                                        |
| async_tree_io              | 731 ms                                                      | 718 ms: 1.02x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.06x faster                                                                |

Benchmark hidden because not significant (1): async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| nbody          | 71.9 ms                                                     | 59.9 ms: 1.20x faster                                                       |
| float          | 56.8 ms                                                     | 50.8 ms: 1.12x faster                                                       |
| Geometric mean | (ref)                                                       | 1.10x faster                                                                |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 119 ms: 1.06x faster                                                        |
| regex_effbot   | 1.62 ms                                                     | 1.59 ms: 1.02x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 15.2 ms: 1.07x slower                                                       |
| regex_compile  | 87.5 ms                                                     | 101 ms: 1.16x slower                                                        |
| Geometric mean | (ref)                                                       | 1.03x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 180 us: 1.09x faster                                                        |
| pickle_dict          | 18.4 us                                                     | 17.4 us: 1.06x faster                                                       |
| xml_etree_generate   | 55.8 ms                                                     | 53.6 ms: 1.04x faster                                                       |
| tomli_loads          | 1.37 sec                                                    | 1.34 sec: 1.02x faster                                                      |
| xml_etree_process    | 37.7 ms                                                     | 37.0 ms: 1.02x faster                                                       |
| json_dumps           | 5.70 ms                                                     | 5.67 ms: 1.01x faster                                                       |
| json_loads           | 13.9 us                                                     | 14.0 us: 1.01x slower                                                       |
| xml_etree_parse      | 93.0 ms                                                     | 93.8 ms: 1.01x slower                                                       |
| unpickle_list        | 2.75 us                                                     | 2.79 us: 1.01x slower                                                       |
| pickle               | 7.43 us                                                     | 7.57 us: 1.02x slower                                                       |
| unpickle_pure_python | 133 us                                                      | 144 us: 1.08x slower                                                        |
| unpickle             | 8.18 us                                                     | 9.04 us: 1.10x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.00x slower                                                                |

Benchmark hidden because not significant (2): pickle_list, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 23.2 ms: 1.19x slower                                                       |
| python_startup_no_site | 16.2 ms                                                     | 20.8 ms: 1.28x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.24x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 6.37 ms: 1.11x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 71.8 us: 1.32x faster                                                       |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.65 sec: 1.27x faster                                                      |
| comprehensions             | 14.1 us                                                     | 11.4 us: 1.24x faster                                                       |
| nbody                      | 71.9 ms                                                     | 59.9 ms: 1.20x faster                                                       |
| mypy2                      | 509 ms                                                      | 445 ms: 1.15x faster                                                        |
| float                      | 56.8 ms                                                     | 50.8 ms: 1.12x faster                                                       |
| async_tree_none            | 291 ms                                                      | 261 ms: 1.12x faster                                                        |
| sqlite_synth               | 1.76 us                                                     | 1.58 us: 1.12x faster                                                       |
| mako                       | 7.09 ms                                                     | 6.37 ms: 1.11x faster                                                       |
| generators                 | 22.5 ms                                                     | 20.3 ms: 1.11x faster                                                       |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 445 ms: 1.10x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 459 ms: 1.09x faster                                                        |
| pickle_pure_python         | 195 us                                                      | 180 us: 1.09x faster                                                        |
| spectral_norm              | 66.9 ms                                                     | 62.0 ms: 1.08x faster                                                       |
| async_tree_none_tg         | 285 ms                                                      | 265 ms: 1.08x faster                                                        |
| logging_silent             | 60.5 ns                                                     | 56.7 ns: 1.07x faster                                                       |
| async_tree_memoization_tg  | 367 ms                                                      | 345 ms: 1.06x faster                                                        |
| regex_dna                  | 126 ms                                                      | 119 ms: 1.06x faster                                                        |
| pathlib                    | 80.5 ms                                                     | 75.9 ms: 1.06x faster                                                       |
| pickle_dict                | 18.4 us                                                     | 17.4 us: 1.06x faster                                                       |
| deepcopy_reduce            | 2.09 us                                                     | 1.98 us: 1.06x faster                                                       |
| dulwich_log                | 44.3 ms                                                     | 42.0 ms: 1.05x faster                                                       |
| logging_simple             | 6.28 us                                                     | 5.96 us: 1.05x faster                                                       |
| deepcopy_memo              | 23.7 us                                                     | 22.6 us: 1.05x faster                                                       |
| deepcopy                   | 238 us                                                      | 227 us: 1.05x faster                                                        |
| tornado_http               | 89.5 ms                                                     | 85.6 ms: 1.05x faster                                                       |
| coroutines                 | 14.3 ms                                                     | 13.6 ms: 1.05x faster                                                       |
| crypto_pyaes               | 48.5 ms                                                     | 46.5 ms: 1.04x faster                                                       |
| xml_etree_generate         | 55.8 ms                                                     | 53.6 ms: 1.04x faster                                                       |
| logging_format             | 6.72 us                                                     | 6.47 us: 1.04x faster                                                       |
| sqlglot_normalize          | 187 ms                                                      | 180 ms: 1.04x faster                                                        |
| async_tree_io_tg           | 771 ms                                                      | 745 ms: 1.03x faster                                                        |
| asyncio_tcp                | 487 ms                                                      | 475 ms: 1.03x faster                                                        |
| gc_traversal               | 1.52 ms                                                     | 1.49 ms: 1.02x faster                                                       |
| chaos                      | 43.3 ms                                                     | 42.5 ms: 1.02x faster                                                       |
| async_tree_io              | 731 ms                                                      | 718 ms: 1.02x faster                                                        |
| tomli_loads                | 1.37 sec                                                    | 1.34 sec: 1.02x faster                                                      |
| xml_etree_process          | 37.7 ms                                                     | 37.0 ms: 1.02x faster                                                       |
| regex_effbot               | 1.62 ms                                                     | 1.59 ms: 1.02x faster                                                       |
| docutils                   | 1.66 sec                                                    | 1.64 sec: 1.01x faster                                                      |
| chameleon                  | 4.98 ms                                                     | 4.93 ms: 1.01x faster                                                       |
| pprint_pformat             | 1.05 sec                                                    | 1.04 sec: 1.01x faster                                                      |
| nqueens                    | 62.8 ms                                                     | 62.3 ms: 1.01x faster                                                       |
| raytrace                   | 192 ms                                                      | 191 ms: 1.01x faster                                                        |
| json_dumps                 | 5.70 ms                                                     | 5.67 ms: 1.01x faster                                                       |
| json_loads                 | 13.9 us                                                     | 14.0 us: 1.01x slower                                                       |
| xml_etree_parse            | 93.0 ms                                                     | 93.8 ms: 1.01x slower                                                       |
| unpickle_list              | 2.75 us                                                     | 2.79 us: 1.01x slower                                                       |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.60 ms: 1.02x slower                                                       |
| pickle                     | 7.43 us                                                     | 7.57 us: 1.02x slower                                                       |
| scimark_fft                | 184 ms                                                      | 188 ms: 1.02x slower                                                        |
| deltablue                  | 2.16 ms                                                     | 2.21 ms: 1.02x slower                                                       |
| sqlglot_parse              | 804 us                                                      | 828 us: 1.03x slower                                                        |
| sqlglot_transpile          | 1.02 ms                                                     | 1.05 ms: 1.03x slower                                                       |
| fannkuch                   | 247 ms                                                      | 256 ms: 1.04x slower                                                        |
| sqlglot_optimize           | 34.5 ms                                                     | 36.0 ms: 1.04x slower                                                       |
| meteor_contest             | 74.6 ms                                                     | 78.0 ms: 1.05x slower                                                       |
| 2to3                       | 218 ms                                                      | 228 ms: 1.05x slower                                                        |
| async_generators           | 239 ms                                                      | 251 ms: 1.05x slower                                                        |
| pycparser                  | 699 ms                                                      | 741 ms: 1.06x slower                                                        |
| sympy_integrate            | 13.0 ms                                                     | 13.8 ms: 1.06x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 15.2 ms: 1.07x slower                                                       |
| sympy_expand               | 284 ms                                                      | 304 ms: 1.07x slower                                                        |
| unpickle_pure_python       | 133 us                                                      | 144 us: 1.08x slower                                                        |
| telco                      | 4.13 ms                                                     | 4.53 ms: 1.10x slower                                                       |
| richards_super             | 32.1 ms                                                     | 35.4 ms: 1.10x slower                                                       |
| unpickle                   | 8.18 us                                                     | 9.04 us: 1.10x slower                                                       |
| json                       | 3.05 ms                                                     | 3.38 ms: 1.11x slower                                                       |
| richards                   | 28.4 ms                                                     | 31.9 ms: 1.12x slower                                                       |
| pyflate                    | 295 ms                                                      | 331 ms: 1.12x slower                                                        |
| regex_compile              | 87.5 ms                                                     | 101 ms: 1.16x slower                                                        |
| coverage                   | 40.8 ms                                                     | 48.1 ms: 1.18x slower                                                       |
| mdp                        | 1.37 sec                                                    | 1.63 sec: 1.19x slower                                                      |
| python_startup             | 19.5 ms                                                     | 23.2 ms: 1.19x slower                                                       |
| go                         | 91.6 ms                                                     | 111 ms: 1.21x slower                                                        |
| python_startup_no_site     | 16.2 ms                                                     | 20.8 ms: 1.28x slower                                                       |
| scimark_lu                 | 58.9 ms                                                     | 77.6 ms: 1.32x slower                                                       |
| scimark_sor                | 78.8 ms                                                     | 104 ms: 1.32x slower                                                        |
| scimark_monte_carlo        | 43.7 ms                                                     | 59.6 ms: 1.36x slower                                                       |
| hexiom                     | 4.10 ms                                                     | 6.01 ms: 1.47x slower                                                       |
| unpack_sequence            | 37.5 ns                                                     | 89.7 ns: 2.40x slower                                                       |
| Geometric mean             | (ref)                                                       | 1.02x slower                                                                |

Benchmark hidden because not significant (10): async_tree_memoization, bench_thread_pool, create_gc_cycles, pickle_list, sympy_sum, sympy_str, pprint_safe_repr, xml_etree_iterparse, pidigits, bench_mp_pool
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 87.12% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown