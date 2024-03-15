# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_arena
- machine: windows-amd64
- commit hash: 1a78317
- commit date: 2024-02-29
- overall geometric mean: 1.08x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.07x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 223 ms: 1.05x slower                                                      |
| chameleon      | 5.26 ms                                                     | 4.85 ms: 1.09x faster                                                     |
| docutils       | 1.64 sec                                                    | 1.57 sec: 1.04x faster                                                    |
| html5lib       | 38.9 ms                                                     | 36.3 ms: 1.07x faster                                                     |
| tornado_http   | 92.8 ms                                                     | 85.2 ms: 1.09x faster                                                     |
| Geometric mean | (ref)                                                       | 1.05x faster                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 269 ms: 1.23x faster                                                      |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 452 ms: 1.17x faster                                                      |
| async_tree_memoization     | 399 ms                                                      | 344 ms: 1.16x faster                                                      |
| async_tree_memoization_tg  | 405 ms                                                      | 352 ms: 1.15x faster                                                      |
| async_tree_none_tg         | 309 ms                                                      | 273 ms: 1.13x faster                                                      |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 465 ms: 1.13x faster                                                      |
| async_tree_io              | 808 ms                                                      | 731 ms: 1.10x faster                                                      |
| async_tree_io_tg           | 829 ms                                                      | 759 ms: 1.09x faster                                                      |
| Geometric mean             | (ref)                                                       | 1.14x faster                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 57.6 ms: 1.22x faster                                                     |
| float          | 54.4 ms                                                     | 49.4 ms: 1.10x faster                                                     |
| Geometric mean | (ref)                                                       | 1.10x faster                                                              |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 77.7 ms: 1.17x faster                                                     |
| regex_effbot   | 1.50 ms                                                     | 1.59 ms: 1.06x slower                                                     |
| regex_dna      | 116 ms                                                      | 125 ms: 1.08x slower                                                      |
| regex_v8       | 14.2 ms                                                     | 15.3 ms: 1.08x slower                                                     |
| Geometric mean | (ref)                                                       | 1.01x slower                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.52 ms: 1.47x faster                                                     |
| tomli_loads          | 1.46 sec                                                    | 1.18 sec: 1.23x faster                                                    |
| unpickle_pure_python | 157 us                                                      | 129 us: 1.22x faster                                                      |
| pickle_pure_python   | 208 us                                                      | 175 us: 1.19x faster                                                      |
| pickle_dict          | 18.5 us                                                     | 17.4 us: 1.06x faster                                                     |
| xml_etree_parse      | 97.6 ms                                                     | 93.4 ms: 1.04x faster                                                     |
| xml_etree_iterparse  | 65.6 ms                                                     | 63.0 ms: 1.04x faster                                                     |
| xml_etree_process    | 37.2 ms                                                     | 36.4 ms: 1.02x faster                                                     |
| xml_etree_generate   | 52.5 ms                                                     | 52.9 ms: 1.01x slower                                                     |
| unpickle_list        | 2.59 us                                                     | 2.72 us: 1.05x slower                                                     |
| json_loads           | 13.0 us                                                     | 13.7 us: 1.05x slower                                                     |
| pickle               | 6.64 us                                                     | 7.14 us: 1.08x slower                                                     |
| unpickle             | 7.57 us                                                     | 8.39 us: 1.11x slower                                                     |
| pickle_list          | 2.70 us                                                     | 3.04 us: 1.13x slower                                                     |
| Geometric mean       | (ref)                                                       | 1.05x faster                                                              |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 23.4 ms: 1.18x slower                                                     |
| python_startup_no_site | 16.8 ms                                                     | 21.1 ms: 1.25x slower                                                     |
| Geometric mean         | (ref)                                                       | 1.22x slower                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|-----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| mako            | 7.58 ms                                                     | 5.75 ms: 1.32x faster                                                     |
| genshi_text     | 18.4 ms                                                     | 15.2 ms: 1.21x faster                                                     |
| genshi_xml      | 39.9 ms                                                     | 34.6 ms: 1.15x faster                                                     |
| django_template | 24.4 ms                                                     | 22.7 ms: 1.08x faster                                                     |
| Geometric mean  | (ref)                                                       | 1.19x faster                                                              |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 69.5 us: 4.69x faster                                                     |
| generators                 | 34.0 ms                                                     | 20.6 ms: 1.65x faster                                                     |
| pylint                     | 323 ms                                                      | 210 ms: 1.54x faster                                                      |
| asyncio_tcp                | 726 ms                                                      | 475 ms: 1.53x faster                                                      |
| comprehensions             | 15.6 us                                                     | 10.5 us: 1.48x faster                                                     |
| json_dumps                 | 8.09 ms                                                     | 5.52 ms: 1.47x faster                                                     |
| spectral_norm              | 68.3 ms                                                     | 50.0 ms: 1.37x faster                                                     |
| richards_super             | 38.7 ms                                                     | 29.3 ms: 1.32x faster                                                     |
| mako                       | 7.58 ms                                                     | 5.75 ms: 1.32x faster                                                     |
| deltablue                  | 2.70 ms                                                     | 2.09 ms: 1.29x faster                                                     |
| logging_silent             | 71.8 ns                                                     | 55.9 ns: 1.28x faster                                                     |
| sqlglot_parse              | 953 us                                                      | 766 us: 1.24x faster                                                      |
| unpack_sequence            | 46.9 ns                                                     | 37.7 ns: 1.24x faster                                                     |
| async_tree_none            | 332 ms                                                      | 269 ms: 1.23x faster                                                      |
| richards                   | 31.4 ms                                                     | 25.5 ms: 1.23x faster                                                     |
| tomli_loads                | 1.46 sec                                                    | 1.18 sec: 1.23x faster                                                    |
| chaos                      | 48.4 ms                                                     | 39.4 ms: 1.23x faster                                                     |
| nbody                      | 70.3 ms                                                     | 57.6 ms: 1.22x faster                                                     |
| unpickle_pure_python       | 157 us                                                      | 129 us: 1.22x faster                                                      |
| genshi_text                | 18.4 ms                                                     | 15.2 ms: 1.21x faster                                                     |
| fannkuch                   | 253 ms                                                      | 209 ms: 1.21x faster                                                      |
| raytrace                   | 213 ms                                                      | 177 ms: 1.20x faster                                                      |
| pickle_pure_python         | 208 us                                                      | 175 us: 1.19x faster                                                      |
| logging_simple             | 6.86 us                                                     | 5.81 us: 1.18x faster                                                     |
| sqlglot_transpile          | 1.16 ms                                                     | 988 us: 1.18x faster                                                      |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 452 ms: 1.17x faster                                                      |
| regex_compile              | 91.0 ms                                                     | 77.7 ms: 1.17x faster                                                     |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.22 ms: 1.16x faster                                                     |
| deepcopy_memo              | 26.0 us                                                     | 22.4 us: 1.16x faster                                                     |
| async_tree_memoization     | 399 ms                                                      | 344 ms: 1.16x faster                                                      |
| genshi_xml                 | 39.9 ms                                                     | 34.6 ms: 1.15x faster                                                     |
| crypto_pyaes               | 48.9 ms                                                     | 42.4 ms: 1.15x faster                                                     |
| mdp                        | 1.59 sec                                                    | 1.38 sec: 1.15x faster                                                    |
| async_tree_memoization_tg  | 405 ms                                                      | 352 ms: 1.15x faster                                                      |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.76 sec: 1.15x faster                                                    |
| logging_format             | 7.16 us                                                     | 6.29 us: 1.14x faster                                                     |
| sympy_str                  | 185 ms                                                      | 163 ms: 1.14x faster                                                      |
| sympy_sum                  | 100 ms                                                      | 88.1 ms: 1.14x faster                                                     |
| coroutines                 | 15.0 ms                                                     | 13.2 ms: 1.13x faster                                                     |
| async_tree_none_tg         | 309 ms                                                      | 273 ms: 1.13x faster                                                      |
| hexiom                     | 4.55 ms                                                     | 4.04 ms: 1.13x faster                                                     |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 465 ms: 1.13x faster                                                      |
| sqlite_synth               | 1.77 us                                                     | 1.57 us: 1.12x faster                                                     |
| dulwich_log                | 46.4 ms                                                     | 41.4 ms: 1.12x faster                                                     |
| pprint_safe_repr           | 529 ms                                                      | 473 ms: 1.12x faster                                                      |
| deepcopy                   | 246 us                                                      | 221 us: 1.12x faster                                                      |
| pyflate                    | 312 ms                                                      | 280 ms: 1.11x faster                                                      |
| pprint_pformat             | 1.09 sec                                                    | 976 ms: 1.11x faster                                                      |
| async_tree_io              | 808 ms                                                      | 731 ms: 1.10x faster                                                      |
| nqueens                    | 68.3 ms                                                     | 61.9 ms: 1.10x faster                                                     |
| float                      | 54.4 ms                                                     | 49.4 ms: 1.10x faster                                                     |
| scimark_monte_carlo        | 45.3 ms                                                     | 41.4 ms: 1.09x faster                                                     |
| async_tree_io_tg           | 829 ms                                                      | 759 ms: 1.09x faster                                                      |
| tornado_http               | 92.8 ms                                                     | 85.2 ms: 1.09x faster                                                     |
| chameleon                  | 5.26 ms                                                     | 4.85 ms: 1.09x faster                                                     |
| scimark_fft                | 179 ms                                                      | 166 ms: 1.08x faster                                                      |
| django_template            | 24.4 ms                                                     | 22.7 ms: 1.08x faster                                                     |
| sympy_expand               | 299 ms                                                      | 278 ms: 1.08x faster                                                      |
| go                         | 101 ms                                                      | 93.9 ms: 1.08x faster                                                     |
| sqlglot_normalize          | 190 ms                                                      | 177 ms: 1.07x faster                                                      |
| pycparser                  | 720 ms                                                      | 673 ms: 1.07x faster                                                      |
| html5lib                   | 38.9 ms                                                     | 36.3 ms: 1.07x faster                                                     |
| sympy_integrate            | 14.0 ms                                                     | 13.2 ms: 1.07x faster                                                     |
| pickle_dict                | 18.5 us                                                     | 17.4 us: 1.06x faster                                                     |
| bench_thread_pool          | 872 us                                                      | 825 us: 1.06x faster                                                      |
| mypy2                      | 459 ms                                                      | 436 ms: 1.05x faster                                                      |
| deepcopy_reduce            | 2.06 us                                                     | 1.95 us: 1.05x faster                                                     |
| xml_etree_parse            | 97.6 ms                                                     | 93.4 ms: 1.04x faster                                                     |
| docutils                   | 1.64 sec                                                    | 1.57 sec: 1.04x faster                                                    |
| xml_etree_iterparse        | 65.6 ms                                                     | 63.0 ms: 1.04x faster                                                     |
| meteor_contest             | 75.2 ms                                                     | 73.6 ms: 1.02x faster                                                     |
| xml_etree_process          | 37.2 ms                                                     | 36.4 ms: 1.02x faster                                                     |
| xml_etree_generate         | 52.5 ms                                                     | 52.9 ms: 1.01x slower                                                     |
| aiohttp                    | 883 us                                                      | 894 us: 1.01x slower                                                      |
| 2to3                       | 214 ms                                                      | 223 ms: 1.05x slower                                                      |
| create_gc_cycles           | 713 us                                                      | 748 us: 1.05x slower                                                      |
| unpickle_list              | 2.59 us                                                     | 2.72 us: 1.05x slower                                                     |
| json_loads                 | 13.0 us                                                     | 13.7 us: 1.05x slower                                                     |
| pathlib                    | 70.9 ms                                                     | 74.6 ms: 1.05x slower                                                     |
| coverage                   | 43.4 ms                                                     | 46.0 ms: 1.06x slower                                                     |
| regex_effbot               | 1.50 ms                                                     | 1.59 ms: 1.06x slower                                                     |
| scimark_sor                | 78.1 ms                                                     | 83.1 ms: 1.06x slower                                                     |
| regex_dna                  | 116 ms                                                      | 125 ms: 1.08x slower                                                      |
| pickle                     | 6.64 us                                                     | 7.14 us: 1.08x slower                                                     |
| regex_v8                   | 14.2 ms                                                     | 15.3 ms: 1.08x slower                                                     |
| bench_mp_pool              | 63.2 ms                                                     | 69.2 ms: 1.10x slower                                                     |
| unpickle                   | 7.57 us                                                     | 8.39 us: 1.11x slower                                                     |
| pickle_list                | 2.70 us                                                     | 3.04 us: 1.13x slower                                                     |
| telco                      | 4.06 ms                                                     | 4.70 ms: 1.16x slower                                                     |
| scimark_lu                 | 62.8 ms                                                     | 72.7 ms: 1.16x slower                                                     |
| python_startup             | 19.8 ms                                                     | 23.4 ms: 1.18x slower                                                     |
| python_startup_no_site     | 16.8 ms                                                     | 21.1 ms: 1.25x slower                                                     |
| dask                       | 273 ms                                                      | 363 ms: 1.33x slower                                                      |
| async_generators           | 177 ms                                                      | 237 ms: 1.34x slower                                                      |
| thrift                     | 494 us                                                      | 8.84 ms: 17.90x slower                                                    |
| Geometric mean             | (ref)                                                       | 1.08x faster                                                              |

Benchmark hidden because not significant (4): json, pidigits, sqlglot_optimize, gc_traversal
Ignored benchmarks (3) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.08x
- 95% likely to have a speedup of 1.07x
- 99% likely to have a speedup of 1.07x


# Memory

- memory change: unknown