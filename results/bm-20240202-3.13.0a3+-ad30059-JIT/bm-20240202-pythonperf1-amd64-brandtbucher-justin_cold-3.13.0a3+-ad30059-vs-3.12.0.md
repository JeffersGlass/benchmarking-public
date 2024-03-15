
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_cold
- machine: windows-amd64
- commit hash: ad30059
- commit date: 2024-02-02
- overall geometric mean: 1.01x faster \*
- HPT reliability: 82.40%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 223 ms: 1.02x slower                                                     |
| chameleon      | 4.98 ms                                                     | 4.82 ms: 1.03x faster                                                    |
| docutils       | 1.66 sec                                                    | 1.61 sec: 1.03x faster                                                   |
| tornado_http   | 89.5 ms                                                     | 87.3 ms: 1.03x faster                                                    |
| Geometric mean | (ref)                                                       | 1.02x faster                                                             |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 264 ms: 1.10x faster                                                     |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 468 ms: 1.05x faster                                                     |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 488 ms: 1.03x faster                                                     |
| async_tree_memoization_tg  | 367 ms                                                      | 359 ms: 1.02x faster                                                     |
| async_tree_none_tg         | 285 ms                                                      | 281 ms: 1.01x faster                                                     |
| Geometric mean             | (ref)                                                       | 1.02x faster                                                             |

Benchmark hidden because not significant (3): async_tree_io_tg, async_tree_io, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| nbody          | 71.9 ms                                                     | 61.9 ms: 1.16x faster                                                    |
| float          | 56.8 ms                                                     | 50.8 ms: 1.12x faster                                                    |
| Geometric mean | (ref)                                                       | 1.09x faster                                                             |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| regex_compile  | 87.5 ms                                                     | 81.6 ms: 1.07x faster                                                    |
| regex_dna      | 126 ms                                                      | 118 ms: 1.07x faster                                                     |
| regex_effbot   | 1.62 ms                                                     | 1.57 ms: 1.03x faster                                                    |
| regex_v8       | 14.2 ms                                                     | 17.2 ms: 1.21x slower                                                    |
| Geometric mean | (ref)                                                       | 1.01x slower                                                             |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 175 us: 1.12x faster                                                     |
| unpickle_pure_python | 133 us                                                      | 126 us: 1.06x faster                                                     |
| tomli_loads          | 1.37 sec                                                    | 1.32 sec: 1.03x faster                                                   |
| json_dumps           | 5.70 ms                                                     | 5.54 ms: 1.03x faster                                                    |
| pickle_dict          | 18.4 us                                                     | 18.0 us: 1.02x faster                                                    |
| pickle_list          | 2.83 us                                                     | 2.78 us: 1.02x faster                                                    |
| pickle               | 7.43 us                                                     | 7.30 us: 1.02x faster                                                    |
| xml_etree_generate   | 55.8 ms                                                     | 56.3 ms: 1.01x slower                                                    |
| json_loads           | 13.9 us                                                     | 14.1 us: 1.01x slower                                                    |
| xml_etree_process    | 37.7 ms                                                     | 38.2 ms: 1.01x slower                                                    |
| xml_etree_iterparse  | 65.2 ms                                                     | 66.6 ms: 1.02x slower                                                    |
| xml_etree_parse      | 93.0 ms                                                     | 95.2 ms: 1.02x slower                                                    |
| unpickle             | 8.18 us                                                     | 8.82 us: 1.08x slower                                                    |
| Geometric mean       | (ref)                                                       | 1.01x faster                                                             |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 21.3 ms: 1.09x slower                                                    |
| python_startup_no_site | 16.2 ms                                                     | 19.2 ms: 1.18x slower                                                    |
| Geometric mean         | (ref)                                                       | 1.13x slower                                                             |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|-----------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 6.68 ms: 1.06x faster                                                    |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 72.1 us: 1.32x faster                                                    |
| comprehensions             | 14.1 us                                                     | 11.9 us: 1.19x faster                                                    |
| nbody                      | 71.9 ms                                                     | 61.9 ms: 1.16x faster                                                    |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.81 sec: 1.16x faster                                                   |
| mypy2                      | 509 ms                                                      | 441 ms: 1.15x faster                                                     |
| logging_silent             | 60.5 ns                                                     | 53.2 ns: 1.14x faster                                                    |
| sqlite_synth               | 1.76 us                                                     | 1.57 us: 1.12x faster                                                    |
| float                      | 56.8 ms                                                     | 50.8 ms: 1.12x faster                                                    |
| pickle_pure_python         | 195 us                                                      | 175 us: 1.12x faster                                                     |
| raytrace                   | 192 ms                                                      | 173 ms: 1.11x faster                                                     |
| richards_super             | 32.1 ms                                                     | 29.0 ms: 1.11x faster                                                    |
| richards                   | 28.4 ms                                                     | 25.7 ms: 1.11x faster                                                    |
| async_tree_none            | 291 ms                                                      | 264 ms: 1.10x faster                                                     |
| coroutines                 | 14.3 ms                                                     | 13.0 ms: 1.10x faster                                                    |
| deepcopy_memo              | 23.7 us                                                     | 21.6 us: 1.10x faster                                                    |
| deepcopy_reduce            | 2.09 us                                                     | 1.93 us: 1.09x faster                                                    |
| generators                 | 22.5 ms                                                     | 20.8 ms: 1.08x faster                                                    |
| deepcopy                   | 238 us                                                      | 221 us: 1.08x faster                                                     |
| regex_compile              | 87.5 ms                                                     | 81.6 ms: 1.07x faster                                                    |
| regex_dna                  | 126 ms                                                      | 118 ms: 1.07x faster                                                     |
| sqlglot_parse              | 804 us                                                      | 752 us: 1.07x faster                                                     |
| mako                       | 7.09 ms                                                     | 6.68 ms: 1.06x faster                                                    |
| unpickle_pure_python       | 133 us                                                      | 126 us: 1.06x faster                                                     |
| scimark_sor                | 78.8 ms                                                     | 74.4 ms: 1.06x faster                                                    |
| nqueens                    | 62.8 ms                                                     | 59.7 ms: 1.05x faster                                                    |
| scimark_lu                 | 58.9 ms                                                     | 56.0 ms: 1.05x faster                                                    |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 468 ms: 1.05x faster                                                     |
| dulwich_log                | 44.3 ms                                                     | 42.5 ms: 1.04x faster                                                    |
| logging_simple             | 6.28 us                                                     | 6.03 us: 1.04x faster                                                    |
| sympy_str                  | 175 ms                                                      | 169 ms: 1.04x faster                                                     |
| sqlglot_normalize          | 187 ms                                                      | 181 ms: 1.03x faster                                                     |
| chameleon                  | 4.98 ms                                                     | 4.82 ms: 1.03x faster                                                    |
| tomli_loads                | 1.37 sec                                                    | 1.32 sec: 1.03x faster                                                   |
| docutils                   | 1.66 sec                                                    | 1.61 sec: 1.03x faster                                                   |
| crypto_pyaes               | 48.5 ms                                                     | 47.0 ms: 1.03x faster                                                    |
| sqlglot_transpile          | 1.02 ms                                                     | 990 us: 1.03x faster                                                     |
| json                       | 3.05 ms                                                     | 2.96 ms: 1.03x faster                                                    |
| pprint_pformat             | 1.05 sec                                                    | 1.01 sec: 1.03x faster                                                   |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 488 ms: 1.03x faster                                                     |
| json_dumps                 | 5.70 ms                                                     | 5.54 ms: 1.03x faster                                                    |
| pprint_safe_repr           | 513 ms                                                      | 499 ms: 1.03x faster                                                     |
| regex_effbot               | 1.62 ms                                                     | 1.57 ms: 1.03x faster                                                    |
| tornado_http               | 89.5 ms                                                     | 87.3 ms: 1.03x faster                                                    |
| pickle_dict                | 18.4 us                                                     | 18.0 us: 1.02x faster                                                    |
| async_tree_memoization_tg  | 367 ms                                                      | 359 ms: 1.02x faster                                                     |
| create_gc_cycles           | 752 us                                                      | 736 us: 1.02x faster                                                     |
| logging_format             | 6.72 us                                                     | 6.58 us: 1.02x faster                                                    |
| pickle_list                | 2.83 us                                                     | 2.78 us: 1.02x faster                                                    |
| pickle                     | 7.43 us                                                     | 7.30 us: 1.02x faster                                                    |
| async_tree_none_tg         | 285 ms                                                      | 281 ms: 1.01x faster                                                     |
| deltablue                  | 2.16 ms                                                     | 2.14 ms: 1.01x faster                                                    |
| sympy_sum                  | 91.5 ms                                                     | 90.9 ms: 1.01x faster                                                    |
| xml_etree_generate         | 55.8 ms                                                     | 56.3 ms: 1.01x slower                                                    |
| sqlglot_optimize           | 34.5 ms                                                     | 34.8 ms: 1.01x slower                                                    |
| spectral_norm              | 66.9 ms                                                     | 67.7 ms: 1.01x slower                                                    |
| bench_mp_pool              | 69.2 ms                                                     | 70.0 ms: 1.01x slower                                                    |
| json_loads                 | 13.9 us                                                     | 14.1 us: 1.01x slower                                                    |
| chaos                      | 43.3 ms                                                     | 43.9 ms: 1.01x slower                                                    |
| xml_etree_process          | 37.7 ms                                                     | 38.2 ms: 1.01x slower                                                    |
| gc_traversal               | 1.52 ms                                                     | 1.55 ms: 1.02x slower                                                    |
| pathlib                    | 80.5 ms                                                     | 82.0 ms: 1.02x slower                                                    |
| sympy_expand               | 284 ms                                                      | 290 ms: 1.02x slower                                                     |
| xml_etree_iterparse        | 65.2 ms                                                     | 66.6 ms: 1.02x slower                                                    |
| xml_etree_parse            | 93.0 ms                                                     | 95.2 ms: 1.02x slower                                                    |
| 2to3                       | 218 ms                                                      | 223 ms: 1.02x slower                                                     |
| async_generators           | 239 ms                                                      | 248 ms: 1.04x slower                                                     |
| meteor_contest             | 74.6 ms                                                     | 77.5 ms: 1.04x slower                                                    |
| sympy_integrate            | 13.0 ms                                                     | 13.5 ms: 1.04x slower                                                    |
| pyflate                    | 295 ms                                                      | 313 ms: 1.06x slower                                                     |
| scimark_fft                | 184 ms                                                      | 197 ms: 1.07x slower                                                     |
| unpickle                   | 8.18 us                                                     | 8.82 us: 1.08x slower                                                    |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.79 ms: 1.09x slower                                                    |
| python_startup             | 19.5 ms                                                     | 21.3 ms: 1.09x slower                                                    |
| go                         | 91.6 ms                                                     | 100 ms: 1.10x slower                                                     |
| telco                      | 4.13 ms                                                     | 4.57 ms: 1.11x slower                                                    |
| coverage                   | 40.8 ms                                                     | 47.3 ms: 1.16x slower                                                    |
| unpack_sequence            | 37.5 ns                                                     | 43.9 ns: 1.17x slower                                                    |
| python_startup_no_site     | 16.2 ms                                                     | 19.2 ms: 1.18x slower                                                    |
| regex_v8                   | 14.2 ms                                                     | 17.2 ms: 1.21x slower                                                    |
| mdp                        | 1.37 sec                                                    | 1.68 sec: 1.22x slower                                                   |
| scimark_monte_carlo        | 43.7 ms                                                     | 56.6 ms: 1.30x slower                                                    |
| hexiom                     | 4.10 ms                                                     | 5.52 ms: 1.35x slower                                                    |
| Geometric mean             | (ref)                                                       | 1.01x faster                                                             |

Benchmark hidden because not significant (10): bench_thread_pool, fannkuch, pidigits, pycparser, dask, unpickle_list, async_tree_io_tg, async_tree_io, async_tree_memoization, asyncio_tcp
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 82.40% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown