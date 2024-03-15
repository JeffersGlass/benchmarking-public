
# Results vs. 3.11.0

- fork: python
- ref: 7f5e3f04f838686d65f1
- machine: windows-amd64
- commit hash: 7f5e3f0
- commit date: 2024-02-21
- overall geometric mean: 1.04x faster \*
- HPT reliability: 97.82%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 228 ms: 1.07x slower                                                        |
| chameleon      | 5.26 ms                                                     | 4.93 ms: 1.07x faster                                                       |
| tornado_http   | 92.8 ms                                                     | 85.6 ms: 1.08x faster                                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                                |

Benchmark hidden because not significant (1): docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 261 ms: 1.27x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 335 ms: 1.19x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 445 ms: 1.19x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 345 ms: 1.17x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 265 ms: 1.16x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 459 ms: 1.14x faster                                                        |
| async_tree_io              | 808 ms                                                      | 718 ms: 1.13x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 745 ms: 1.11x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.17x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 59.9 ms: 1.17x faster                                                       |
| float          | 54.4 ms                                                     | 50.8 ms: 1.07x faster                                                       |
| pidigits       | 150 ms                                                      | 152 ms: 1.01x slower                                                        |
| Geometric mean | (ref)                                                       | 1.07x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 116 ms                                                      | 119 ms: 1.03x slower                                                        |
| regex_effbot   | 1.50 ms                                                     | 1.59 ms: 1.06x slower                                                       |
| regex_v8       | 14.2 ms                                                     | 15.2 ms: 1.07x slower                                                       |
| regex_compile  | 91.0 ms                                                     | 101 ms: 1.11x slower                                                        |
| Geometric mean | (ref)                                                       | 1.07x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.67 ms: 1.43x faster                                                       |
| pickle_pure_python   | 208 us                                                      | 180 us: 1.16x faster                                                        |
| unpickle_pure_python | 157 us                                                      | 144 us: 1.09x faster                                                        |
| tomli_loads          | 1.46 sec                                                    | 1.34 sec: 1.08x faster                                                      |
| pickle_dict          | 18.5 us                                                     | 17.4 us: 1.06x faster                                                       |
| xml_etree_parse      | 97.6 ms                                                     | 93.8 ms: 1.04x faster                                                       |
| xml_etree_generate   | 52.5 ms                                                     | 53.6 ms: 1.02x slower                                                       |
| pickle_list          | 2.70 us                                                     | 2.82 us: 1.04x slower                                                       |
| json_loads           | 13.0 us                                                     | 14.0 us: 1.08x slower                                                       |
| unpickle_list        | 2.59 us                                                     | 2.79 us: 1.08x slower                                                       |
| pickle               | 6.64 us                                                     | 7.57 us: 1.14x slower                                                       |
| unpickle             | 7.57 us                                                     | 9.04 us: 1.19x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.02x faster                                                                |

Benchmark hidden because not significant (2): xml_etree_iterparse, xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 23.2 ms: 1.18x slower                                                       |
| python_startup_no_site | 16.8 ms                                                     | 20.8 ms: 1.24x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.21x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 6.37 ms: 1.19x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 71.8 us: 4.54x faster                                                       |
| generators                 | 34.0 ms                                                     | 20.3 ms: 1.67x faster                                                       |
| asyncio_tcp                | 726 ms                                                      | 475 ms: 1.53x faster                                                        |
| json_dumps                 | 8.09 ms                                                     | 5.67 ms: 1.43x faster                                                       |
| comprehensions             | 15.6 us                                                     | 11.4 us: 1.38x faster                                                       |
| async_tree_none            | 332 ms                                                      | 261 ms: 1.27x faster                                                        |
| logging_silent             | 71.8 ns                                                     | 56.7 ns: 1.27x faster                                                       |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.65 sec: 1.23x faster                                                      |
| deltablue                  | 2.70 ms                                                     | 2.21 ms: 1.22x faster                                                       |
| async_tree_memoization     | 399 ms                                                      | 335 ms: 1.19x faster                                                        |
| mako                       | 7.58 ms                                                     | 6.37 ms: 1.19x faster                                                       |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 445 ms: 1.19x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 345 ms: 1.17x faster                                                        |
| nbody                      | 70.3 ms                                                     | 59.9 ms: 1.17x faster                                                       |
| async_tree_none_tg         | 309 ms                                                      | 265 ms: 1.16x faster                                                        |
| pickle_pure_python         | 208 us                                                      | 180 us: 1.16x faster                                                        |
| logging_simple             | 6.86 us                                                     | 5.96 us: 1.15x faster                                                       |
| sqlglot_parse              | 953 us                                                      | 828 us: 1.15x faster                                                        |
| deepcopy_memo              | 26.0 us                                                     | 22.6 us: 1.15x faster                                                       |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 459 ms: 1.14x faster                                                        |
| chaos                      | 48.4 ms                                                     | 42.5 ms: 1.14x faster                                                       |
| async_tree_io              | 808 ms                                                      | 718 ms: 1.13x faster                                                        |
| sqlite_synth               | 1.77 us                                                     | 1.58 us: 1.12x faster                                                       |
| raytrace                   | 213 ms                                                      | 191 ms: 1.12x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 745 ms: 1.11x faster                                                        |
| logging_format             | 7.16 us                                                     | 6.47 us: 1.11x faster                                                       |
| sqlglot_transpile          | 1.16 ms                                                     | 1.05 ms: 1.11x faster                                                       |
| dulwich_log                | 46.4 ms                                                     | 42.0 ms: 1.10x faster                                                       |
| spectral_norm              | 68.3 ms                                                     | 62.0 ms: 1.10x faster                                                       |
| sympy_sum                  | 100 ms                                                      | 91.2 ms: 1.10x faster                                                       |
| coroutines                 | 15.0 ms                                                     | 13.6 ms: 1.10x faster                                                       |
| nqueens                    | 68.3 ms                                                     | 62.3 ms: 1.10x faster                                                       |
| richards_super             | 38.7 ms                                                     | 35.4 ms: 1.09x faster                                                       |
| unpickle_pure_python       | 157 us                                                      | 144 us: 1.09x faster                                                        |
| deepcopy                   | 246 us                                                      | 227 us: 1.08x faster                                                        |
| tomli_loads                | 1.46 sec                                                    | 1.34 sec: 1.08x faster                                                      |
| tornado_http               | 92.8 ms                                                     | 85.6 ms: 1.08x faster                                                       |
| float                      | 54.4 ms                                                     | 50.8 ms: 1.07x faster                                                       |
| chameleon                  | 5.26 ms                                                     | 4.93 ms: 1.07x faster                                                       |
| pickle_dict                | 18.5 us                                                     | 17.4 us: 1.06x faster                                                       |
| sympy_str                  | 185 ms                                                      | 175 ms: 1.06x faster                                                        |
| sqlglot_normalize          | 190 ms                                                      | 180 ms: 1.05x faster                                                        |
| crypto_pyaes               | 48.9 ms                                                     | 46.5 ms: 1.05x faster                                                       |
| pprint_pformat             | 1.09 sec                                                    | 1.04 sec: 1.05x faster                                                      |
| xml_etree_parse            | 97.6 ms                                                     | 93.8 ms: 1.04x faster                                                       |
| deepcopy_reduce            | 2.06 us                                                     | 1.98 us: 1.04x faster                                                       |
| pprint_safe_repr           | 529 ms                                                      | 512 ms: 1.03x faster                                                        |
| mypy2                      | 459 ms                                                      | 445 ms: 1.03x faster                                                        |
| bench_thread_pool          | 872 us                                                      | 846 us: 1.03x faster                                                        |
| sympy_integrate            | 14.0 ms                                                     | 13.8 ms: 1.02x faster                                                       |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.60 ms: 1.01x slower                                                       |
| fannkuch                   | 253 ms                                                      | 256 ms: 1.01x slower                                                        |
| pidigits                   | 150 ms                                                      | 152 ms: 1.01x slower                                                        |
| richards                   | 31.4 ms                                                     | 31.9 ms: 1.01x slower                                                       |
| sympy_expand               | 299 ms                                                      | 304 ms: 1.02x slower                                                        |
| xml_etree_generate         | 52.5 ms                                                     | 53.6 ms: 1.02x slower                                                       |
| mdp                        | 1.59 sec                                                    | 1.63 sec: 1.02x slower                                                      |
| regex_dna                  | 116 ms                                                      | 119 ms: 1.03x slower                                                        |
| meteor_contest             | 75.2 ms                                                     | 78.0 ms: 1.04x slower                                                       |
| sqlglot_optimize           | 34.5 ms                                                     | 36.0 ms: 1.04x slower                                                       |
| create_gc_cycles           | 713 us                                                      | 745 us: 1.04x slower                                                        |
| pickle_list                | 2.70 us                                                     | 2.82 us: 1.04x slower                                                       |
| scimark_fft                | 179 ms                                                      | 188 ms: 1.05x slower                                                        |
| pyflate                    | 312 ms                                                      | 331 ms: 1.06x slower                                                        |
| regex_effbot               | 1.50 ms                                                     | 1.59 ms: 1.06x slower                                                       |
| 2to3                       | 214 ms                                                      | 228 ms: 1.07x slower                                                        |
| pathlib                    | 70.9 ms                                                     | 75.9 ms: 1.07x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 15.2 ms: 1.07x slower                                                       |
| json_loads                 | 13.0 us                                                     | 14.0 us: 1.08x slower                                                       |
| unpickle_list              | 2.59 us                                                     | 2.79 us: 1.08x slower                                                       |
| go                         | 101 ms                                                      | 111 ms: 1.10x slower                                                        |
| bench_mp_pool              | 63.2 ms                                                     | 69.5 ms: 1.10x slower                                                       |
| coverage                   | 43.4 ms                                                     | 48.1 ms: 1.11x slower                                                       |
| regex_compile              | 91.0 ms                                                     | 101 ms: 1.11x slower                                                        |
| telco                      | 4.06 ms                                                     | 4.53 ms: 1.11x slower                                                       |
| json                       | 2.98 ms                                                     | 3.38 ms: 1.14x slower                                                       |
| pickle                     | 6.64 us                                                     | 7.57 us: 1.14x slower                                                       |
| python_startup             | 19.8 ms                                                     | 23.2 ms: 1.18x slower                                                       |
| unpickle                   | 7.57 us                                                     | 9.04 us: 1.19x slower                                                       |
| scimark_lu                 | 62.8 ms                                                     | 77.6 ms: 1.24x slower                                                       |
| python_startup_no_site     | 16.8 ms                                                     | 20.8 ms: 1.24x slower                                                       |
| scimark_monte_carlo        | 45.3 ms                                                     | 59.6 ms: 1.32x slower                                                       |
| hexiom                     | 4.55 ms                                                     | 6.01 ms: 1.32x slower                                                       |
| scimark_sor                | 78.1 ms                                                     | 104 ms: 1.33x slower                                                        |
| async_generators           | 177 ms                                                      | 251 ms: 1.42x slower                                                        |
| unpack_sequence            | 46.9 ns                                                     | 89.7 ns: 1.91x slower                                                       |
| Geometric mean             | (ref)                                                       | 1.04x faster                                                                |

Benchmark hidden because not significant (5): xml_etree_iterparse, xml_etree_process, docutils, gc_traversal, pycparser
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 97.82% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown