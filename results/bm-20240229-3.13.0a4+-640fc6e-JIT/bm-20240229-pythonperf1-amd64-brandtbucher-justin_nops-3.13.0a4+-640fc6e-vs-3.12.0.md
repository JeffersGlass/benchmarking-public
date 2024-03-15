# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_nops
- machine: windows-amd64
- commit hash: 640fc6e
- commit date: 2024-02-29
- overall geometric mean: 1.03x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 226 ms: 1.03x slower                                                     |
| chameleon      | 4.98 ms                                                     | 4.76 ms: 1.05x faster                                                    |
| docutils       | 1.66 sec                                                    | 1.59 sec: 1.05x faster                                                   |
| tornado_http   | 89.5 ms                                                     | 84.8 ms: 1.06x faster                                                    |
| Geometric mean | (ref)                                                       | 1.03x faster                                                             |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 489 ms                                                      | 460 ms: 1.06x faster                                                     |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 474 ms: 1.06x faster                                                     |
| async_tree_none            | 291 ms                                                      | 276 ms: 1.06x faster                                                     |
| async_tree_memoization_tg  | 367 ms                                                      | 355 ms: 1.03x faster                                                     |
| async_tree_none_tg         | 285 ms                                                      | 279 ms: 1.02x faster                                                     |
| async_tree_memoization     | 339 ms                                                      | 349 ms: 1.03x slower                                                     |
| Geometric mean             | (ref)                                                       | 1.03x faster                                                             |

Benchmark hidden because not significant (2): async_tree_io_tg, async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| nbody          | 71.9 ms                                                     | 59.5 ms: 1.21x faster                                                    |
| float          | 56.8 ms                                                     | 49.5 ms: 1.15x faster                                                    |
| pidigits       | 152 ms                                                      | 150 ms: 1.01x faster                                                     |
| Geometric mean | (ref)                                                       | 1.12x faster                                                             |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| regex_compile  | 87.5 ms                                                     | 82.2 ms: 1.06x faster                                                    |
| regex_dna      | 126 ms                                                      | 121 ms: 1.04x faster                                                     |
| regex_effbot   | 1.62 ms                                                     | 1.58 ms: 1.03x faster                                                    |
| regex_v8       | 14.2 ms                                                     | 14.5 ms: 1.02x slower                                                    |
| Geometric mean | (ref)                                                       | 1.03x faster                                                             |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| tomli_loads          | 1.37 sec                                                    | 1.20 sec: 1.14x faster                                                   |
| pickle_pure_python   | 195 us                                                      | 176 us: 1.11x faster                                                     |
| xml_etree_generate   | 55.8 ms                                                     | 53.3 ms: 1.05x faster                                                    |
| xml_etree_process    | 37.7 ms                                                     | 36.3 ms: 1.04x faster                                                    |
| pickle_dict          | 18.4 us                                                     | 17.7 us: 1.04x faster                                                    |
| unpickle_pure_python | 133 us                                                      | 130 us: 1.03x faster                                                     |
| json_dumps           | 5.70 ms                                                     | 5.59 ms: 1.02x faster                                                    |
| xml_etree_iterparse  | 65.2 ms                                                     | 64.1 ms: 1.02x faster                                                    |
| unpickle_list        | 2.75 us                                                     | 2.77 us: 1.01x slower                                                    |
| unpickle             | 8.18 us                                                     | 8.47 us: 1.03x slower                                                    |
| Geometric mean       | (ref)                                                       | 1.03x faster                                                             |

Benchmark hidden because not significant (4): pickle, json_loads, pickle_list, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 24.1 ms: 1.24x slower                                                    |
| python_startup_no_site | 16.2 ms                                                     | 21.9 ms: 1.35x slower                                                    |
| Geometric mean         | (ref)                                                       | 1.29x slower                                                             |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|-----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| mako            | 7.09 ms                                                     | 5.78 ms: 1.23x faster                                                    |
| django_template | 22.9 ms                                                     | 21.6 ms: 1.06x faster                                                    |
| Geometric mean  | (ref)                                                       | 1.14x faster                                                             |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 69.2 us: 1.38x faster                                                    |
| comprehensions             | 14.1 us                                                     | 10.4 us: 1.35x faster                                                    |
| spectral_norm              | 66.9 ms                                                     | 51.9 ms: 1.29x faster                                                    |
| mako                       | 7.09 ms                                                     | 5.78 ms: 1.23x faster                                                    |
| nbody                      | 71.9 ms                                                     | 59.5 ms: 1.21x faster                                                    |
| mypy2                      | 509 ms                                                      | 435 ms: 1.17x faster                                                     |
| float                      | 56.8 ms                                                     | 49.5 ms: 1.15x faster                                                    |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.84 sec: 1.14x faster                                                   |
| tomli_loads                | 1.37 sec                                                    | 1.20 sec: 1.14x faster                                                   |
| crypto_pyaes               | 48.5 ms                                                     | 42.8 ms: 1.13x faster                                                    |
| sqlite_synth               | 1.76 us                                                     | 1.56 us: 1.13x faster                                                    |
| fannkuch                   | 247 ms                                                      | 221 ms: 1.12x faster                                                     |
| pickle_pure_python         | 195 us                                                      | 176 us: 1.11x faster                                                     |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.31 ms: 1.11x faster                                                    |
| logging_silent             | 60.5 ns                                                     | 55.2 ns: 1.10x faster                                                    |
| chaos                      | 43.3 ms                                                     | 39.9 ms: 1.09x faster                                                    |
| deepcopy_reduce            | 2.09 us                                                     | 1.93 us: 1.08x faster                                                    |
| generators                 | 22.5 ms                                                     | 20.8 ms: 1.08x faster                                                    |
| raytrace                   | 192 ms                                                      | 178 ms: 1.08x faster                                                     |
| sympy_str                  | 175 ms                                                      | 163 ms: 1.08x faster                                                     |
| dulwich_log                | 44.3 ms                                                     | 41.2 ms: 1.07x faster                                                    |
| deepcopy                   | 238 us                                                      | 222 us: 1.07x faster                                                     |
| logging_simple             | 6.28 us                                                     | 5.86 us: 1.07x faster                                                    |
| coroutines                 | 14.3 ms                                                     | 13.3 ms: 1.07x faster                                                    |
| pathlib                    | 80.5 ms                                                     | 75.3 ms: 1.07x faster                                                    |
| logging_format             | 6.72 us                                                     | 6.29 us: 1.07x faster                                                    |
| sqlglot_normalize          | 187 ms                                                      | 175 ms: 1.07x faster                                                     |
| regex_compile              | 87.5 ms                                                     | 82.2 ms: 1.06x faster                                                    |
| scimark_fft                | 184 ms                                                      | 173 ms: 1.06x faster                                                     |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 460 ms: 1.06x faster                                                     |
| deepcopy_memo              | 23.7 us                                                     | 22.3 us: 1.06x faster                                                    |
| sympy_sum                  | 91.5 ms                                                     | 86.2 ms: 1.06x faster                                                    |
| django_template            | 22.9 ms                                                     | 21.6 ms: 1.06x faster                                                    |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 474 ms: 1.06x faster                                                     |
| pprint_pformat             | 1.05 sec                                                    | 988 ms: 1.06x faster                                                     |
| async_tree_none            | 291 ms                                                      | 276 ms: 1.06x faster                                                     |
| deltablue                  | 2.16 ms                                                     | 2.04 ms: 1.06x faster                                                    |
| tornado_http               | 89.5 ms                                                     | 84.8 ms: 1.06x faster                                                    |
| asyncio_tcp                | 487 ms                                                      | 465 ms: 1.05x faster                                                     |
| sqlglot_parse              | 804 us                                                      | 767 us: 1.05x faster                                                     |
| xml_etree_generate         | 55.8 ms                                                     | 53.3 ms: 1.05x faster                                                    |
| docutils                   | 1.66 sec                                                    | 1.59 sec: 1.05x faster                                                   |
| chameleon                  | 4.98 ms                                                     | 4.76 ms: 1.05x faster                                                    |
| pprint_safe_repr           | 513 ms                                                      | 491 ms: 1.05x faster                                                     |
| regex_dna                  | 126 ms                                                      | 121 ms: 1.04x faster                                                     |
| xml_etree_process          | 37.7 ms                                                     | 36.3 ms: 1.04x faster                                                    |
| pickle_dict                | 18.4 us                                                     | 17.7 us: 1.04x faster                                                    |
| pyflate                    | 295 ms                                                      | 284 ms: 1.04x faster                                                     |
| sqlglot_transpile          | 1.02 ms                                                     | 988 us: 1.03x faster                                                     |
| async_tree_memoization_tg  | 367 ms                                                      | 355 ms: 1.03x faster                                                     |
| unpickle_pure_python       | 133 us                                                      | 130 us: 1.03x faster                                                     |
| regex_effbot               | 1.62 ms                                                     | 1.58 ms: 1.03x faster                                                    |
| richards_super             | 32.1 ms                                                     | 31.3 ms: 1.02x faster                                                    |
| meteor_contest             | 74.6 ms                                                     | 72.9 ms: 1.02x faster                                                    |
| sympy_expand               | 284 ms                                                      | 278 ms: 1.02x faster                                                     |
| async_tree_none_tg         | 285 ms                                                      | 279 ms: 1.02x faster                                                     |
| bench_thread_pool          | 857 us                                                      | 838 us: 1.02x faster                                                     |
| json_dumps                 | 5.70 ms                                                     | 5.59 ms: 1.02x faster                                                    |
| xml_etree_iterparse        | 65.2 ms                                                     | 64.1 ms: 1.02x faster                                                    |
| gc_traversal               | 1.52 ms                                                     | 1.50 ms: 1.02x faster                                                    |
| scimark_monte_carlo        | 43.7 ms                                                     | 43.0 ms: 1.02x faster                                                    |
| richards                   | 28.4 ms                                                     | 28.0 ms: 1.02x faster                                                    |
| pidigits                   | 152 ms                                                      | 150 ms: 1.01x faster                                                     |
| unpickle_list              | 2.75 us                                                     | 2.77 us: 1.01x slower                                                    |
| sympy_integrate            | 13.0 ms                                                     | 13.1 ms: 1.01x slower                                                    |
| bench_mp_pool              | 69.2 ms                                                     | 70.3 ms: 1.02x slower                                                    |
| regex_v8                   | 14.2 ms                                                     | 14.5 ms: 1.02x slower                                                    |
| aiohttp                    | 884 us                                                      | 904 us: 1.02x slower                                                     |
| async_tree_memoization     | 339 ms                                                      | 349 ms: 1.03x slower                                                     |
| 2to3                       | 218 ms                                                      | 226 ms: 1.03x slower                                                     |
| unpickle                   | 8.18 us                                                     | 8.47 us: 1.03x slower                                                    |
| scimark_sor                | 78.8 ms                                                     | 81.7 ms: 1.04x slower                                                    |
| go                         | 91.6 ms                                                     | 95.4 ms: 1.04x slower                                                    |
| json                       | 3.05 ms                                                     | 3.18 ms: 1.04x slower                                                    |
| hexiom                     | 4.10 ms                                                     | 4.43 ms: 1.08x slower                                                    |
| mdp                        | 1.37 sec                                                    | 1.54 sec: 1.12x slower                                                   |
| telco                      | 4.13 ms                                                     | 4.74 ms: 1.15x slower                                                    |
| coverage                   | 40.8 ms                                                     | 47.6 ms: 1.17x slower                                                    |
| unpack_sequence            | 37.5 ns                                                     | 43.8 ns: 1.17x slower                                                    |
| scimark_lu                 | 58.9 ms                                                     | 72.8 ms: 1.24x slower                                                    |
| python_startup             | 19.5 ms                                                     | 24.1 ms: 1.24x slower                                                    |
| python_startup_no_site     | 16.2 ms                                                     | 21.9 ms: 1.35x slower                                                    |
| dask                       | 263 ms                                                      | 362 ms: 1.38x slower                                                     |
| Geometric mean             | (ref)                                                       | 1.03x faster                                                             |

Benchmark hidden because not significant (11): async_tree_io_tg, create_gc_cycles, pickle, sqlglot_optimize, nqueens, json_loads, pycparser, async_generators, pickle_list, xml_etree_parse, async_tree_io
Ignored benchmarks (2) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (5) of results/bm-20240229-3.13.0a4+-640fc6e-JIT/bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e.json: genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: unknown