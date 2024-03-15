
# Results vs. 3.12.0

- fork: python
- ref: b905fad83819ec9102ec
- machine: windows-amd64
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.03x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 216 ms: 1.01x faster                                                        |
| chameleon      | 4.98 ms                                                     | 4.93 ms: 1.01x faster                                                       |
| docutils       | 1.66 sec                                                    | 1.59 sec: 1.04x faster                                                      |
| tornado_http   | 89.5 ms                                                     | 86.3 ms: 1.04x faster                                                       |
| Geometric mean | (ref)                                                       | 1.03x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 278 ms: 1.05x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 484 ms: 1.04x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 473 ms: 1.04x faster                                                        |
| async_tree_io_tg           | 771 ms                                                      | 787 ms: 1.02x slower                                                        |
| async_tree_io              | 731 ms                                                      | 763 ms: 1.04x slower                                                        |
| async_tree_memoization     | 339 ms                                                      | 356 ms: 1.05x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.00x faster                                                                |

Benchmark hidden because not significant (2): async_tree_none_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 56.8 ms                                                     | 54.1 ms: 1.05x faster                                                       |
| pidigits       | 152 ms                                                      | 149 ms: 1.02x faster                                                        |
| Geometric mean | (ref)                                                       | 1.02x faster                                                                |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 87.5 ms                                                     | 79.0 ms: 1.11x faster                                                       |
| regex_dna      | 126 ms                                                      | 117 ms: 1.08x faster                                                        |
| regex_effbot   | 1.62 ms                                                     | 1.59 ms: 1.02x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 14.6 ms: 1.03x slower                                                       |
| Geometric mean | (ref)                                                       | 1.04x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark          | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|--------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_pure_python | 195 us                                                      | 184 us: 1.06x faster                                                        |
| pickle             | 7.43 us                                                     | 7.15 us: 1.04x faster                                                       |
| xml_etree_generate | 55.8 ms                                                     | 53.9 ms: 1.04x faster                                                       |
| json_dumps         | 5.70 ms                                                     | 5.61 ms: 1.02x faster                                                       |
| unpickle_list      | 2.75 us                                                     | 2.72 us: 1.01x faster                                                       |
| xml_etree_process  | 37.7 ms                                                     | 37.6 ms: 1.00x faster                                                       |
| pickle_list        | 2.83 us                                                     | 2.87 us: 1.02x slower                                                       |
| pickle_dict        | 18.4 us                                                     | 18.9 us: 1.02x slower                                                       |
| xml_etree_parse    | 93.0 ms                                                     | 95.6 ms: 1.03x slower                                                       |
| unpickle           | 8.18 us                                                     | 8.45 us: 1.03x slower                                                       |
| tomli_loads        | 1.37 sec                                                    | 1.42 sec: 1.04x slower                                                      |
| Geometric mean     | (ref)                                                       | 1.00x faster                                                                |

Benchmark hidden because not significant (3): json_loads, xml_etree_iterparse, unpickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 20.5 ms: 1.05x slower                                                       |
| python_startup_no_site | 16.2 ms                                                     | 18.5 ms: 1.14x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.10x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 6.75 ms: 1.05x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| comprehensions             | 14.1 us                                                     | 10.5 us: 1.34x faster                                                       |
| typing_runtime_protocols   | 95.1 us                                                     | 71.4 us: 1.33x faster                                                       |
| mypy2                      | 509 ms                                                      | 421 ms: 1.21x faster                                                        |
| raytrace                   | 192 ms                                                      | 163 ms: 1.18x faster                                                        |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.87 sec: 1.12x faster                                                      |
| regex_compile              | 87.5 ms                                                     | 79.0 ms: 1.11x faster                                                       |
| sqlite_synth               | 1.76 us                                                     | 1.59 us: 1.11x faster                                                       |
| logging_silent             | 60.5 ns                                                     | 54.8 ns: 1.10x faster                                                       |
| sympy_str                  | 175 ms                                                      | 159 ms: 1.10x faster                                                        |
| chaos                      | 43.3 ms                                                     | 39.8 ms: 1.09x faster                                                       |
| coroutines                 | 14.3 ms                                                     | 13.1 ms: 1.09x faster                                                       |
| crypto_pyaes               | 48.5 ms                                                     | 44.8 ms: 1.08x faster                                                       |
| regex_dna                  | 126 ms                                                      | 117 ms: 1.08x faster                                                        |
| spectral_norm              | 66.9 ms                                                     | 62.2 ms: 1.08x faster                                                       |
| sympy_sum                  | 91.5 ms                                                     | 85.1 ms: 1.07x faster                                                       |
| nqueens                    | 62.8 ms                                                     | 58.6 ms: 1.07x faster                                                       |
| scimark_monte_carlo        | 43.7 ms                                                     | 40.8 ms: 1.07x faster                                                       |
| go                         | 91.6 ms                                                     | 85.7 ms: 1.07x faster                                                       |
| sqlglot_normalize          | 187 ms                                                      | 175 ms: 1.07x faster                                                        |
| scimark_lu                 | 58.9 ms                                                     | 55.2 ms: 1.07x faster                                                       |
| pickle_pure_python         | 195 us                                                      | 184 us: 1.06x faster                                                        |
| deepcopy                   | 238 us                                                      | 224 us: 1.06x faster                                                        |
| float                      | 56.8 ms                                                     | 54.1 ms: 1.05x faster                                                       |
| mako                       | 7.09 ms                                                     | 6.75 ms: 1.05x faster                                                       |
| async_tree_none            | 291 ms                                                      | 278 ms: 1.05x faster                                                        |
| deltablue                  | 2.16 ms                                                     | 2.06 ms: 1.05x faster                                                       |
| docutils                   | 1.66 sec                                                    | 1.59 sec: 1.04x faster                                                      |
| async_generators           | 239 ms                                                      | 229 ms: 1.04x faster                                                        |
| dulwich_log                | 44.3 ms                                                     | 42.5 ms: 1.04x faster                                                       |
| pickle                     | 7.43 us                                                     | 7.15 us: 1.04x faster                                                       |
| sqlglot_parse              | 804 us                                                      | 775 us: 1.04x faster                                                        |
| deepcopy_reduce            | 2.09 us                                                     | 2.02 us: 1.04x faster                                                       |
| tornado_http               | 89.5 ms                                                     | 86.3 ms: 1.04x faster                                                       |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 484 ms: 1.04x faster                                                        |
| logging_simple             | 6.28 us                                                     | 6.06 us: 1.04x faster                                                       |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 473 ms: 1.04x faster                                                        |
| xml_etree_generate         | 55.8 ms                                                     | 53.9 ms: 1.04x faster                                                       |
| generators                 | 22.5 ms                                                     | 21.8 ms: 1.03x faster                                                       |
| sympy_expand               | 284 ms                                                      | 275 ms: 1.03x faster                                                        |
| deepcopy_memo              | 23.7 us                                                     | 23.0 us: 1.03x faster                                                       |
| hexiom                     | 4.10 ms                                                     | 3.97 ms: 1.03x faster                                                       |
| pprint_pformat             | 1.05 sec                                                    | 1.02 sec: 1.03x faster                                                      |
| meteor_contest             | 74.6 ms                                                     | 72.8 ms: 1.03x faster                                                       |
| pprint_safe_repr           | 513 ms                                                      | 501 ms: 1.02x faster                                                        |
| pidigits                   | 152 ms                                                      | 149 ms: 1.02x faster                                                        |
| scimark_fft                | 184 ms                                                      | 180 ms: 1.02x faster                                                        |
| sympy_integrate            | 13.0 ms                                                     | 12.7 ms: 1.02x faster                                                       |
| bench_mp_pool              | 69.2 ms                                                     | 67.7 ms: 1.02x faster                                                       |
| regex_effbot               | 1.62 ms                                                     | 1.59 ms: 1.02x faster                                                       |
| sqlglot_optimize           | 34.5 ms                                                     | 33.9 ms: 1.02x faster                                                       |
| sqlglot_transpile          | 1.02 ms                                                     | 1.00 ms: 1.02x faster                                                       |
| richards_super             | 32.1 ms                                                     | 31.6 ms: 1.02x faster                                                       |
| logging_format             | 6.72 us                                                     | 6.61 us: 1.02x faster                                                       |
| json_dumps                 | 5.70 ms                                                     | 5.61 ms: 1.02x faster                                                       |
| 2to3                       | 218 ms                                                      | 216 ms: 1.01x faster                                                        |
| unpickle_list              | 2.75 us                                                     | 2.72 us: 1.01x faster                                                       |
| chameleon                  | 4.98 ms                                                     | 4.93 ms: 1.01x faster                                                       |
| pyflate                    | 295 ms                                                      | 292 ms: 1.01x faster                                                        |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.54 ms: 1.01x faster                                                       |
| xml_etree_process          | 37.7 ms                                                     | 37.6 ms: 1.00x faster                                                       |
| fannkuch                   | 247 ms                                                      | 246 ms: 1.00x faster                                                        |
| gc_traversal               | 1.52 ms                                                     | 1.54 ms: 1.01x slower                                                       |
| pickle_list                | 2.83 us                                                     | 2.87 us: 1.02x slower                                                       |
| async_tree_io_tg           | 771 ms                                                      | 787 ms: 1.02x slower                                                        |
| bench_thread_pool          | 857 us                                                      | 877 us: 1.02x slower                                                        |
| mdp                        | 1.37 sec                                                    | 1.41 sec: 1.02x slower                                                      |
| pickle_dict                | 18.4 us                                                     | 18.9 us: 1.02x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 14.6 ms: 1.03x slower                                                       |
| xml_etree_parse            | 93.0 ms                                                     | 95.6 ms: 1.03x slower                                                       |
| asyncio_tcp                | 487 ms                                                      | 503 ms: 1.03x slower                                                        |
| unpickle                   | 8.18 us                                                     | 8.45 us: 1.03x slower                                                       |
| scimark_sor                | 78.8 ms                                                     | 81.5 ms: 1.04x slower                                                       |
| tomli_loads                | 1.37 sec                                                    | 1.42 sec: 1.04x slower                                                      |
| unpack_sequence            | 37.5 ns                                                     | 39.0 ns: 1.04x slower                                                       |
| async_tree_io              | 731 ms                                                      | 763 ms: 1.04x slower                                                        |
| async_tree_memoization     | 339 ms                                                      | 356 ms: 1.05x slower                                                        |
| python_startup             | 19.5 ms                                                     | 20.5 ms: 1.05x slower                                                       |
| json                       | 3.05 ms                                                     | 3.26 ms: 1.07x slower                                                       |
| telco                      | 4.13 ms                                                     | 4.61 ms: 1.12x slower                                                       |
| python_startup_no_site     | 16.2 ms                                                     | 18.5 ms: 1.14x slower                                                       |
| coverage                   | 40.8 ms                                                     | 48.0 ms: 1.18x slower                                                       |
| Geometric mean             | (ref)                                                       | 1.03x faster                                                                |

Benchmark hidden because not significant (11): dask, async_tree_none_tg, json_loads, pathlib, xml_etree_iterparse, richards, unpickle_pure_python, create_gc_cycles, nbody, async_tree_memoization_tg, pycparser
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: unknown