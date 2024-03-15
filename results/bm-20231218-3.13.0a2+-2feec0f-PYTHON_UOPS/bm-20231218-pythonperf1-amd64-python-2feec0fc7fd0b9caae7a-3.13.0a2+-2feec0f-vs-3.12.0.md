
# Results vs. 3.12.0

- fork: python
- ref: 2feec0fc7fd0b9caae7a
- machine: windows-amd64
- commit hash: 2feec0f
- commit date: 2023-12-18
- overall geometric mean: 1.00x faster
- HPT reliability: 93.85%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf1-amd64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| chameleon      | 4.98 ms                                                     | 4.93 ms: 1.01x faster                                                       |
| docutils       | 1.66 sec                                                    | 1.59 sec: 1.05x faster                                                      |
| tornado_http   | 89.5 ms                                                     | 88.0 ms: 1.02x faster                                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                                |

Benchmark hidden because not significant (1): 2to3

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf1-amd64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 268 ms: 1.09x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 456 ms: 1.07x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 471 ms: 1.07x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 349 ms: 1.05x faster                                                        |
| async_tree_none_tg         | 285 ms                                                      | 274 ms: 1.04x faster                                                        |
| async_tree_io_tg           | 771 ms                                                      | 743 ms: 1.04x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.04x faster                                                                |

Benchmark hidden because not significant (2): async_tree_io, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf1-amd64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 152 ms                                                      | 151 ms: 1.01x faster                                                        |
| nbody          | 71.9 ms                                                     | 82.3 ms: 1.14x slower                                                       |
| Geometric mean | (ref)                                                       | 1.04x slower                                                                |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf1-amd64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 121 ms: 1.05x faster                                                        |
| regex_compile  | 87.5 ms                                                     | 84.4 ms: 1.04x faster                                                       |
| regex_effbot   | 1.62 ms                                                     | 1.57 ms: 1.03x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 15.1 ms: 1.06x slower                                                       |
| Geometric mean | (ref)                                                       | 1.01x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf1-amd64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 181 us: 1.08x faster                                                        |
| json_loads           | 13.9 us                                                     | 13.3 us: 1.04x faster                                                       |
| pickle               | 7.43 us                                                     | 7.19 us: 1.03x faster                                                       |
| xml_etree_generate   | 55.8 ms                                                     | 54.8 ms: 1.02x faster                                                       |
| xml_etree_process    | 37.7 ms                                                     | 37.1 ms: 1.02x faster                                                       |
| json_dumps           | 5.70 ms                                                     | 5.62 ms: 1.01x faster                                                       |
| unpickle_list        | 2.75 us                                                     | 2.72 us: 1.01x faster                                                       |
| xml_etree_parse      | 93.0 ms                                                     | 94.2 ms: 1.01x slower                                                       |
| pickle_dict          | 18.4 us                                                     | 18.7 us: 1.02x slower                                                       |
| unpickle_pure_python | 133 us                                                      | 135 us: 1.02x slower                                                        |
| unpickle             | 8.18 us                                                     | 8.37 us: 1.02x slower                                                       |
| xml_etree_iterparse  | 65.2 ms                                                     | 67.0 ms: 1.03x slower                                                       |
| tomli_loads          | 1.37 sec                                                    | 1.47 sec: 1.07x slower                                                      |
| pickle_list          | 2.83 us                                                     | 3.39 us: 1.20x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.01x slower                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf1-amd64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 20.3 ms: 1.04x slower                                                       |
| python_startup_no_site | 16.2 ms                                                     | 18.1 ms: 1.11x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.08x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf1-amd64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 6.96 ms: 1.02x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf1-amd64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 74.3 us: 1.28x faster                                                       |
| mypy2                      | 509 ms                                                      | 420 ms: 1.21x faster                                                        |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.74 sec: 1.21x faster                                                      |
| sqlite_synth               | 1.76 us                                                     | 1.56 us: 1.13x faster                                                       |
| coroutines                 | 14.3 ms                                                     | 12.8 ms: 1.12x faster                                                       |
| raytrace                   | 192 ms                                                      | 173 ms: 1.11x faster                                                        |
| logging_silent             | 60.5 ns                                                     | 54.8 ns: 1.10x faster                                                       |
| comprehensions             | 14.1 us                                                     | 12.8 us: 1.10x faster                                                       |
| async_tree_none            | 291 ms                                                      | 268 ms: 1.09x faster                                                        |
| pickle_pure_python         | 195 us                                                      | 181 us: 1.08x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 456 ms: 1.07x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 471 ms: 1.07x faster                                                        |
| sympy_sum                  | 91.5 ms                                                     | 86.1 ms: 1.06x faster                                                       |
| deepcopy_reduce            | 2.09 us                                                     | 1.97 us: 1.06x faster                                                       |
| deepcopy                   | 238 us                                                      | 226 us: 1.05x faster                                                        |
| sympy_str                  | 175 ms                                                      | 167 ms: 1.05x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 349 ms: 1.05x faster                                                        |
| deepcopy_memo              | 23.7 us                                                     | 22.6 us: 1.05x faster                                                       |
| docutils                   | 1.66 sec                                                    | 1.59 sec: 1.05x faster                                                      |
| regex_dna                  | 126 ms                                                      | 121 ms: 1.05x faster                                                        |
| richards_super             | 32.1 ms                                                     | 30.7 ms: 1.04x faster                                                       |
| json_loads                 | 13.9 us                                                     | 13.3 us: 1.04x faster                                                       |
| scimark_lu                 | 58.9 ms                                                     | 56.5 ms: 1.04x faster                                                       |
| async_generators           | 239 ms                                                      | 230 ms: 1.04x faster                                                        |
| async_tree_none_tg         | 285 ms                                                      | 274 ms: 1.04x faster                                                        |
| async_tree_io_tg           | 771 ms                                                      | 743 ms: 1.04x faster                                                        |
| sqlglot_parse              | 804 us                                                      | 775 us: 1.04x faster                                                        |
| regex_compile              | 87.5 ms                                                     | 84.4 ms: 1.04x faster                                                       |
| pickle                     | 7.43 us                                                     | 7.19 us: 1.03x faster                                                       |
| richards                   | 28.4 ms                                                     | 27.6 ms: 1.03x faster                                                       |
| regex_effbot               | 1.62 ms                                                     | 1.57 ms: 1.03x faster                                                       |
| gc_traversal               | 1.52 ms                                                     | 1.48 ms: 1.03x faster                                                       |
| sympy_expand               | 284 ms                                                      | 276 ms: 1.03x faster                                                        |
| dask                       | 263 ms                                                      | 256 ms: 1.03x faster                                                        |
| sqlglot_transpile          | 1.02 ms                                                     | 997 us: 1.03x faster                                                        |
| bench_mp_pool              | 69.2 ms                                                     | 67.5 ms: 1.03x faster                                                       |
| sqlglot_normalize          | 187 ms                                                      | 183 ms: 1.02x faster                                                        |
| dulwich_log                | 44.3 ms                                                     | 43.3 ms: 1.02x faster                                                       |
| pycparser                  | 699 ms                                                      | 684 ms: 1.02x faster                                                        |
| scimark_sor                | 78.8 ms                                                     | 77.1 ms: 1.02x faster                                                       |
| logging_format             | 6.72 us                                                     | 6.58 us: 1.02x faster                                                       |
| xml_etree_generate         | 55.8 ms                                                     | 54.8 ms: 1.02x faster                                                       |
| logging_simple             | 6.28 us                                                     | 6.16 us: 1.02x faster                                                       |
| mako                       | 7.09 ms                                                     | 6.96 ms: 1.02x faster                                                       |
| create_gc_cycles           | 752 us                                                      | 739 us: 1.02x faster                                                        |
| tornado_http               | 89.5 ms                                                     | 88.0 ms: 1.02x faster                                                       |
| xml_etree_process          | 37.7 ms                                                     | 37.1 ms: 1.02x faster                                                       |
| generators                 | 22.5 ms                                                     | 22.2 ms: 1.02x faster                                                       |
| crypto_pyaes               | 48.5 ms                                                     | 47.8 ms: 1.01x faster                                                       |
| json_dumps                 | 5.70 ms                                                     | 5.62 ms: 1.01x faster                                                       |
| chameleon                  | 4.98 ms                                                     | 4.93 ms: 1.01x faster                                                       |
| pidigits                   | 152 ms                                                      | 151 ms: 1.01x faster                                                        |
| unpickle_list              | 2.75 us                                                     | 2.72 us: 1.01x faster                                                       |
| go                         | 91.6 ms                                                     | 91.2 ms: 1.00x faster                                                       |
| sqlglot_optimize           | 34.5 ms                                                     | 34.9 ms: 1.01x slower                                                       |
| meteor_contest             | 74.6 ms                                                     | 75.6 ms: 1.01x slower                                                       |
| xml_etree_parse            | 93.0 ms                                                     | 94.2 ms: 1.01x slower                                                       |
| pprint_safe_repr           | 513 ms                                                      | 520 ms: 1.01x slower                                                        |
| sympy_integrate            | 13.0 ms                                                     | 13.1 ms: 1.01x slower                                                       |
| pickle_dict                | 18.4 us                                                     | 18.7 us: 1.02x slower                                                       |
| unpickle_pure_python       | 133 us                                                      | 135 us: 1.02x slower                                                        |
| nqueens                    | 62.8 ms                                                     | 63.9 ms: 1.02x slower                                                       |
| pathlib                    | 80.5 ms                                                     | 81.9 ms: 1.02x slower                                                       |
| pprint_pformat             | 1.05 sec                                                    | 1.07 sec: 1.02x slower                                                      |
| unpickle                   | 8.18 us                                                     | 8.37 us: 1.02x slower                                                       |
| xml_etree_iterparse        | 65.2 ms                                                     | 67.0 ms: 1.03x slower                                                       |
| chaos                      | 43.3 ms                                                     | 44.6 ms: 1.03x slower                                                       |
| python_startup             | 19.5 ms                                                     | 20.3 ms: 1.04x slower                                                       |
| unpack_sequence            | 37.5 ns                                                     | 39.2 ns: 1.05x slower                                                       |
| mdp                        | 1.37 sec                                                    | 1.44 sec: 1.05x slower                                                      |
| regex_v8                   | 14.2 ms                                                     | 15.1 ms: 1.06x slower                                                       |
| tomli_loads                | 1.37 sec                                                    | 1.47 sec: 1.07x slower                                                      |
| pyflate                    | 295 ms                                                      | 321 ms: 1.09x slower                                                        |
| coverage                   | 40.8 ms                                                     | 44.9 ms: 1.10x slower                                                       |
| python_startup_no_site     | 16.2 ms                                                     | 18.1 ms: 1.11x slower                                                       |
| scimark_fft                | 184 ms                                                      | 209 ms: 1.13x slower                                                        |
| scimark_monte_carlo        | 43.7 ms                                                     | 49.5 ms: 1.13x slower                                                       |
| nbody                      | 71.9 ms                                                     | 82.3 ms: 1.14x slower                                                       |
| telco                      | 4.13 ms                                                     | 4.75 ms: 1.15x slower                                                       |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.98 ms: 1.16x slower                                                       |
| fannkuch                   | 247 ms                                                      | 291 ms: 1.18x slower                                                        |
| pickle_list                | 2.83 us                                                     | 3.39 us: 1.20x slower                                                       |
| hexiom                     | 4.10 ms                                                     | 4.99 ms: 1.22x slower                                                       |
| deltablue                  | 2.16 ms                                                     | 2.67 ms: 1.23x slower                                                       |
| spectral_norm              | 66.9 ms                                                     | 82.6 ms: 1.23x slower                                                       |
| Geometric mean             | (ref)                                                       | 1.00x faster                                                                |

Benchmark hidden because not significant (7): asyncio_tcp, json, 2to3, async_tree_io, async_tree_memoization, float, bench_thread_pool
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 93.85% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown