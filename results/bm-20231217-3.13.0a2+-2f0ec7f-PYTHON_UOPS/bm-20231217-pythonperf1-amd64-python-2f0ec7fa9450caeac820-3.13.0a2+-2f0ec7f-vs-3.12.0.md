
# Results vs. 3.12.0

- fork: python
- ref: 2f0ec7fa9450caeac820
- machine: windows-amd64
- commit hash: 2f0ec7f
- commit date: 2023-12-17
- overall geometric mean: 1.00x slower
- HPT reliability: 86.90%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| chameleon      | 4.98 ms                                                     | 5.01 ms: 1.01x slower                                                       |
| docutils       | 1.66 sec                                                    | 1.57 sec: 1.06x faster                                                      |
| tornado_http   | 89.5 ms                                                     | 87.5 ms: 1.02x faster                                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                                |

Benchmark hidden because not significant (1): 2to3

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 269 ms: 1.08x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 455 ms: 1.08x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 471 ms: 1.07x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 352 ms: 1.04x faster                                                        |
| async_tree_none_tg         | 285 ms                                                      | 274 ms: 1.04x faster                                                        |
| async_tree_io_tg           | 771 ms                                                      | 754 ms: 1.02x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.04x faster                                                                |

Benchmark hidden because not significant (2): async_tree_io, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 152 ms                                                      | 150 ms: 1.01x faster                                                        |
| float          | 56.8 ms                                                     | 58.1 ms: 1.02x slower                                                       |
| nbody          | 71.9 ms                                                     | 82.6 ms: 1.15x slower                                                       |
| Geometric mean | (ref)                                                       | 1.05x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 117 ms: 1.08x faster                                                        |
| regex_effbot   | 1.62 ms                                                     | 1.56 ms: 1.03x faster                                                       |
| regex_compile  | 87.5 ms                                                     | 84.8 ms: 1.03x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 14.7 ms: 1.03x slower                                                       |
| Geometric mean | (ref)                                                       | 1.03x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 180 us: 1.09x faster                                                        |
| unpickle_list        | 2.75 us                                                     | 2.56 us: 1.08x faster                                                       |
| json_loads           | 13.9 us                                                     | 13.3 us: 1.04x faster                                                       |
| json_dumps           | 5.70 ms                                                     | 5.58 ms: 1.02x faster                                                       |
| pickle               | 7.43 us                                                     | 7.30 us: 1.02x faster                                                       |
| xml_etree_generate   | 55.8 ms                                                     | 54.9 ms: 1.02x faster                                                       |
| xml_etree_process    | 37.7 ms                                                     | 37.3 ms: 1.01x faster                                                       |
| pickle_dict          | 18.4 us                                                     | 18.6 us: 1.01x slower                                                       |
| xml_etree_parse      | 93.0 ms                                                     | 94.0 ms: 1.01x slower                                                       |
| unpickle_pure_python | 133 us                                                      | 135 us: 1.01x slower                                                        |
| xml_etree_iterparse  | 65.2 ms                                                     | 66.5 ms: 1.02x slower                                                       |
| tomli_loads          | 1.37 sec                                                    | 1.48 sec: 1.08x slower                                                      |
| pickle_list          | 2.83 us                                                     | 3.36 us: 1.19x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.00x slower                                                                |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 20.4 ms: 1.05x slower                                                       |
| python_startup_no_site | 16.2 ms                                                     | 18.2 ms: 1.12x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.09x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 7.67 ms: 1.08x slower                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.65 sec: 1.27x faster                                                      |
| typing_runtime_protocols   | 95.1 us                                                     | 75.4 us: 1.26x faster                                                       |
| mypy2                      | 509 ms                                                      | 420 ms: 1.21x faster                                                        |
| sqlite_synth               | 1.76 us                                                     | 1.57 us: 1.12x faster                                                       |
| coroutines                 | 14.3 ms                                                     | 12.9 ms: 1.11x faster                                                       |
| raytrace                   | 192 ms                                                      | 175 ms: 1.10x faster                                                        |
| logging_silent             | 60.5 ns                                                     | 55.3 ns: 1.09x faster                                                       |
| pickle_pure_python         | 195 us                                                      | 180 us: 1.09x faster                                                        |
| regex_dna                  | 126 ms                                                      | 117 ms: 1.08x faster                                                        |
| async_tree_none            | 291 ms                                                      | 269 ms: 1.08x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 455 ms: 1.08x faster                                                        |
| unpickle_list              | 2.75 us                                                     | 2.56 us: 1.08x faster                                                       |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 471 ms: 1.07x faster                                                        |
| comprehensions             | 14.1 us                                                     | 13.3 us: 1.06x faster                                                       |
| docutils                   | 1.66 sec                                                    | 1.57 sec: 1.06x faster                                                      |
| scimark_lu                 | 58.9 ms                                                     | 55.9 ms: 1.05x faster                                                       |
| deepcopy_reduce            | 2.09 us                                                     | 1.99 us: 1.05x faster                                                       |
| sympy_sum                  | 91.5 ms                                                     | 87.0 ms: 1.05x faster                                                       |
| asyncio_tcp                | 487 ms                                                      | 464 ms: 1.05x faster                                                        |
| sympy_str                  | 175 ms                                                      | 167 ms: 1.05x faster                                                        |
| deepcopy                   | 238 us                                                      | 227 us: 1.05x faster                                                        |
| json_loads                 | 13.9 us                                                     | 13.3 us: 1.04x faster                                                       |
| async_generators           | 239 ms                                                      | 229 ms: 1.04x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 352 ms: 1.04x faster                                                        |
| async_tree_none_tg         | 285 ms                                                      | 274 ms: 1.04x faster                                                        |
| sqlglot_parse              | 804 us                                                      | 773 us: 1.04x faster                                                        |
| bench_mp_pool              | 69.2 ms                                                     | 66.7 ms: 1.04x faster                                                       |
| deepcopy_memo              | 23.7 us                                                     | 22.9 us: 1.04x faster                                                       |
| richards_super             | 32.1 ms                                                     | 31.0 ms: 1.04x faster                                                       |
| regex_effbot               | 1.62 ms                                                     | 1.56 ms: 1.03x faster                                                       |
| create_gc_cycles           | 752 us                                                      | 728 us: 1.03x faster                                                        |
| dulwich_log                | 44.3 ms                                                     | 42.9 ms: 1.03x faster                                                       |
| regex_compile              | 87.5 ms                                                     | 84.8 ms: 1.03x faster                                                       |
| dask                       | 263 ms                                                      | 255 ms: 1.03x faster                                                        |
| sympy_expand               | 284 ms                                                      | 277 ms: 1.03x faster                                                        |
| tornado_http               | 89.5 ms                                                     | 87.5 ms: 1.02x faster                                                       |
| async_tree_io_tg           | 771 ms                                                      | 754 ms: 1.02x faster                                                        |
| generators                 | 22.5 ms                                                     | 22.0 ms: 1.02x faster                                                       |
| json_dumps                 | 5.70 ms                                                     | 5.58 ms: 1.02x faster                                                       |
| pickle                     | 7.43 us                                                     | 7.30 us: 1.02x faster                                                       |
| richards                   | 28.4 ms                                                     | 27.9 ms: 1.02x faster                                                       |
| pathlib                    | 80.5 ms                                                     | 79.1 ms: 1.02x faster                                                       |
| sqlglot_transpile          | 1.02 ms                                                     | 1.00 ms: 1.02x faster                                                       |
| xml_etree_generate         | 55.8 ms                                                     | 54.9 ms: 1.02x faster                                                       |
| pidigits                   | 152 ms                                                      | 150 ms: 1.01x faster                                                        |
| xml_etree_process          | 37.7 ms                                                     | 37.3 ms: 1.01x faster                                                       |
| sqlglot_normalize          | 187 ms                                                      | 185 ms: 1.01x faster                                                        |
| pycparser                  | 699 ms                                                      | 693 ms: 1.01x faster                                                        |
| gc_traversal               | 1.52 ms                                                     | 1.51 ms: 1.01x faster                                                       |
| logging_simple             | 6.28 us                                                     | 6.24 us: 1.01x faster                                                       |
| logging_format             | 6.72 us                                                     | 6.68 us: 1.00x faster                                                       |
| chameleon                  | 4.98 ms                                                     | 5.01 ms: 1.01x slower                                                       |
| pickle_dict                | 18.4 us                                                     | 18.6 us: 1.01x slower                                                       |
| crypto_pyaes               | 48.5 ms                                                     | 48.9 ms: 1.01x slower                                                       |
| xml_etree_parse            | 93.0 ms                                                     | 94.0 ms: 1.01x slower                                                       |
| unpickle_pure_python       | 133 us                                                      | 135 us: 1.01x slower                                                        |
| sympy_integrate            | 13.0 ms                                                     | 13.2 ms: 1.02x slower                                                       |
| go                         | 91.6 ms                                                     | 93.0 ms: 1.02x slower                                                       |
| xml_etree_iterparse        | 65.2 ms                                                     | 66.5 ms: 1.02x slower                                                       |
| meteor_contest             | 74.6 ms                                                     | 76.3 ms: 1.02x slower                                                       |
| float                      | 56.8 ms                                                     | 58.1 ms: 1.02x slower                                                       |
| sqlglot_optimize           | 34.5 ms                                                     | 35.4 ms: 1.02x slower                                                       |
| scimark_sor                | 78.8 ms                                                     | 81.1 ms: 1.03x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 14.7 ms: 1.03x slower                                                       |
| pprint_safe_repr           | 513 ms                                                      | 531 ms: 1.03x slower                                                        |
| pprint_pformat             | 1.05 sec                                                    | 1.09 sec: 1.04x slower                                                      |
| chaos                      | 43.3 ms                                                     | 45.2 ms: 1.04x slower                                                       |
| nqueens                    | 62.8 ms                                                     | 65.9 ms: 1.05x slower                                                       |
| python_startup             | 19.5 ms                                                     | 20.4 ms: 1.05x slower                                                       |
| unpack_sequence            | 37.5 ns                                                     | 40.3 ns: 1.07x slower                                                       |
| tomli_loads                | 1.37 sec                                                    | 1.48 sec: 1.08x slower                                                      |
| mako                       | 7.09 ms                                                     | 7.67 ms: 1.08x slower                                                       |
| fannkuch                   | 247 ms                                                      | 268 ms: 1.09x slower                                                        |
| coverage                   | 40.8 ms                                                     | 44.7 ms: 1.10x slower                                                       |
| pyflate                    | 295 ms                                                      | 323 ms: 1.10x slower                                                        |
| mdp                        | 1.37 sec                                                    | 1.53 sec: 1.12x slower                                                      |
| python_startup_no_site     | 16.2 ms                                                     | 18.2 ms: 1.12x slower                                                       |
| scimark_monte_carlo        | 43.7 ms                                                     | 49.5 ms: 1.13x slower                                                       |
| scimark_fft                | 184 ms                                                      | 210 ms: 1.14x slower                                                        |
| telco                      | 4.13 ms                                                     | 4.72 ms: 1.14x slower                                                       |
| nbody                      | 71.9 ms                                                     | 82.6 ms: 1.15x slower                                                       |
| pickle_list                | 2.83 us                                                     | 3.36 us: 1.19x slower                                                       |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 3.12 ms: 1.22x slower                                                       |
| hexiom                     | 4.10 ms                                                     | 5.07 ms: 1.24x slower                                                       |
| spectral_norm              | 66.9 ms                                                     | 85.0 ms: 1.27x slower                                                       |
| deltablue                  | 2.16 ms                                                     | 2.77 ms: 1.28x slower                                                       |
| Geometric mean             | (ref)                                                       | 1.00x slower                                                                |

Benchmark hidden because not significant (6): json, 2to3, bench_thread_pool, async_tree_io, async_tree_memoization, unpickle
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 86.90% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown