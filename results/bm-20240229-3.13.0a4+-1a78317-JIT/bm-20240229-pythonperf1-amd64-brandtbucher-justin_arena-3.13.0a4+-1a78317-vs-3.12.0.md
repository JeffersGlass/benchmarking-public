# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_arena
- machine: windows-amd64
- commit hash: 1a78317
- commit date: 2024-02-29
- overall geometric mean: 1.04x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 223 ms: 1.02x slower                                                      |
| chameleon      | 4.98 ms                                                     | 4.85 ms: 1.03x faster                                                     |
| docutils       | 1.66 sec                                                    | 1.57 sec: 1.06x faster                                                    |
| tornado_http   | 89.5 ms                                                     | 85.2 ms: 1.05x faster                                                     |
| Geometric mean | (ref)                                                       | 1.03x faster                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 269 ms: 1.08x faster                                                      |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 452 ms: 1.08x faster                                                      |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 465 ms: 1.08x faster                                                      |
| async_tree_none_tg         | 285 ms                                                      | 273 ms: 1.04x faster                                                      |
| async_tree_memoization_tg  | 367 ms                                                      | 352 ms: 1.04x faster                                                      |
| async_tree_io_tg           | 771 ms                                                      | 759 ms: 1.02x faster                                                      |
| async_tree_memoization     | 339 ms                                                      | 344 ms: 1.02x slower                                                      |
| Geometric mean             | (ref)                                                       | 1.04x faster                                                              |

Benchmark hidden because not significant (1): async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| nbody          | 71.9 ms                                                     | 57.6 ms: 1.25x faster                                                     |
| float          | 56.8 ms                                                     | 49.4 ms: 1.15x faster                                                     |
| pidigits       | 152 ms                                                      | 150 ms: 1.01x faster                                                      |
| Geometric mean | (ref)                                                       | 1.13x faster                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_compile  | 87.5 ms                                                     | 77.7 ms: 1.13x faster                                                     |
| regex_effbot   | 1.62 ms                                                     | 1.59 ms: 1.02x faster                                                     |
| regex_dna      | 126 ms                                                      | 125 ms: 1.01x faster                                                      |
| regex_v8       | 14.2 ms                                                     | 15.3 ms: 1.08x slower                                                     |
| Geometric mean | (ref)                                                       | 1.02x faster                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| tomli_loads          | 1.37 sec                                                    | 1.18 sec: 1.15x faster                                                    |
| pickle_pure_python   | 195 us                                                      | 175 us: 1.11x faster                                                      |
| pickle_dict          | 18.4 us                                                     | 17.4 us: 1.06x faster                                                     |
| xml_etree_generate   | 55.8 ms                                                     | 52.9 ms: 1.05x faster                                                     |
| pickle               | 7.43 us                                                     | 7.14 us: 1.04x faster                                                     |
| xml_etree_process    | 37.7 ms                                                     | 36.4 ms: 1.04x faster                                                     |
| unpickle_pure_python | 133 us                                                      | 129 us: 1.03x faster                                                      |
| xml_etree_iterparse  | 65.2 ms                                                     | 63.0 ms: 1.03x faster                                                     |
| json_dumps           | 5.70 ms                                                     | 5.52 ms: 1.03x faster                                                     |
| json_loads           | 13.9 us                                                     | 13.7 us: 1.02x faster                                                     |
| unpickle_list        | 2.75 us                                                     | 2.72 us: 1.01x faster                                                     |
| unpickle             | 8.18 us                                                     | 8.39 us: 1.03x slower                                                     |
| pickle_list          | 2.83 us                                                     | 3.04 us: 1.08x slower                                                     |
| Geometric mean       | (ref)                                                       | 1.03x faster                                                              |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 23.4 ms: 1.20x slower                                                     |
| python_startup_no_site | 16.2 ms                                                     | 21.1 ms: 1.30x slower                                                     |
| Geometric mean         | (ref)                                                       | 1.25x slower                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|-----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| mako            | 7.09 ms                                                     | 5.75 ms: 1.23x faster                                                     |
| django_template | 22.9 ms                                                     | 22.7 ms: 1.01x faster                                                     |
| Geometric mean  | (ref)                                                       | 1.12x faster                                                              |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 69.5 us: 1.37x faster                                                     |
| comprehensions             | 14.1 us                                                     | 10.5 us: 1.34x faster                                                     |
| spectral_norm              | 66.9 ms                                                     | 50.0 ms: 1.34x faster                                                     |
| nbody                      | 71.9 ms                                                     | 57.6 ms: 1.25x faster                                                     |
| mako                       | 7.09 ms                                                     | 5.75 ms: 1.23x faster                                                     |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.76 sec: 1.19x faster                                                    |
| fannkuch                   | 247 ms                                                      | 209 ms: 1.18x faster                                                      |
| mypy2                      | 509 ms                                                      | 436 ms: 1.17x faster                                                      |
| tomli_loads                | 1.37 sec                                                    | 1.18 sec: 1.15x faster                                                    |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.22 ms: 1.15x faster                                                     |
| float                      | 56.8 ms                                                     | 49.4 ms: 1.15x faster                                                     |
| crypto_pyaes               | 48.5 ms                                                     | 42.4 ms: 1.14x faster                                                     |
| regex_compile              | 87.5 ms                                                     | 77.7 ms: 1.13x faster                                                     |
| sqlite_synth               | 1.76 us                                                     | 1.57 us: 1.12x faster                                                     |
| pickle_pure_python         | 195 us                                                      | 175 us: 1.11x faster                                                      |
| richards                   | 28.4 ms                                                     | 25.5 ms: 1.11x faster                                                     |
| scimark_fft                | 184 ms                                                      | 166 ms: 1.11x faster                                                      |
| chaos                      | 43.3 ms                                                     | 39.4 ms: 1.10x faster                                                     |
| richards_super             | 32.1 ms                                                     | 29.3 ms: 1.09x faster                                                     |
| generators                 | 22.5 ms                                                     | 20.6 ms: 1.09x faster                                                     |
| pprint_safe_repr           | 513 ms                                                      | 473 ms: 1.09x faster                                                      |
| raytrace                   | 192 ms                                                      | 177 ms: 1.09x faster                                                      |
| async_tree_none            | 291 ms                                                      | 269 ms: 1.08x faster                                                      |
| logging_silent             | 60.5 ns                                                     | 55.9 ns: 1.08x faster                                                     |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 452 ms: 1.08x faster                                                      |
| coroutines                 | 14.3 ms                                                     | 13.2 ms: 1.08x faster                                                     |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 465 ms: 1.08x faster                                                      |
| logging_simple             | 6.28 us                                                     | 5.81 us: 1.08x faster                                                     |
| deepcopy                   | 238 us                                                      | 221 us: 1.08x faster                                                      |
| pathlib                    | 80.5 ms                                                     | 74.6 ms: 1.08x faster                                                     |
| sympy_str                  | 175 ms                                                      | 163 ms: 1.08x faster                                                      |
| deepcopy_reduce            | 2.09 us                                                     | 1.95 us: 1.07x faster                                                     |
| pprint_pformat             | 1.05 sec                                                    | 976 ms: 1.07x faster                                                      |
| dulwich_log                | 44.3 ms                                                     | 41.4 ms: 1.07x faster                                                     |
| logging_format             | 6.72 us                                                     | 6.29 us: 1.07x faster                                                     |
| json                       | 3.05 ms                                                     | 2.88 ms: 1.06x faster                                                     |
| deepcopy_memo              | 23.7 us                                                     | 22.4 us: 1.06x faster                                                     |
| docutils                   | 1.66 sec                                                    | 1.57 sec: 1.06x faster                                                    |
| scimark_monte_carlo        | 43.7 ms                                                     | 41.4 ms: 1.06x faster                                                     |
| pickle_dict                | 18.4 us                                                     | 17.4 us: 1.06x faster                                                     |
| xml_etree_generate         | 55.8 ms                                                     | 52.9 ms: 1.05x faster                                                     |
| sqlglot_normalize          | 187 ms                                                      | 177 ms: 1.05x faster                                                      |
| pyflate                    | 295 ms                                                      | 280 ms: 1.05x faster                                                      |
| tornado_http               | 89.5 ms                                                     | 85.2 ms: 1.05x faster                                                     |
| sqlglot_parse              | 804 us                                                      | 766 us: 1.05x faster                                                      |
| async_tree_none_tg         | 285 ms                                                      | 273 ms: 1.04x faster                                                      |
| async_tree_memoization_tg  | 367 ms                                                      | 352 ms: 1.04x faster                                                      |
| pickle                     | 7.43 us                                                     | 7.14 us: 1.04x faster                                                     |
| sympy_sum                  | 91.5 ms                                                     | 88.1 ms: 1.04x faster                                                     |
| pycparser                  | 699 ms                                                      | 673 ms: 1.04x faster                                                      |
| bench_thread_pool          | 857 us                                                      | 825 us: 1.04x faster                                                      |
| xml_etree_process          | 37.7 ms                                                     | 36.4 ms: 1.04x faster                                                     |
| unpickle_pure_python       | 133 us                                                      | 129 us: 1.03x faster                                                      |
| sqlglot_transpile          | 1.02 ms                                                     | 988 us: 1.03x faster                                                      |
| deltablue                  | 2.16 ms                                                     | 2.09 ms: 1.03x faster                                                     |
| xml_etree_iterparse        | 65.2 ms                                                     | 63.0 ms: 1.03x faster                                                     |
| json_dumps                 | 5.70 ms                                                     | 5.52 ms: 1.03x faster                                                     |
| chameleon                  | 4.98 ms                                                     | 4.85 ms: 1.03x faster                                                     |
| asyncio_tcp                | 487 ms                                                      | 475 ms: 1.03x faster                                                      |
| sympy_expand               | 284 ms                                                      | 278 ms: 1.02x faster                                                      |
| json_loads                 | 13.9 us                                                     | 13.7 us: 1.02x faster                                                     |
| regex_effbot               | 1.62 ms                                                     | 1.59 ms: 1.02x faster                                                     |
| gc_traversal               | 1.52 ms                                                     | 1.50 ms: 1.02x faster                                                     |
| async_tree_io_tg           | 771 ms                                                      | 759 ms: 1.02x faster                                                      |
| nqueens                    | 62.8 ms                                                     | 61.9 ms: 1.01x faster                                                     |
| pidigits                   | 152 ms                                                      | 150 ms: 1.01x faster                                                      |
| hexiom                     | 4.10 ms                                                     | 4.04 ms: 1.01x faster                                                     |
| meteor_contest             | 74.6 ms                                                     | 73.6 ms: 1.01x faster                                                     |
| regex_dna                  | 126 ms                                                      | 125 ms: 1.01x faster                                                      |
| async_generators           | 239 ms                                                      | 237 ms: 1.01x faster                                                      |
| django_template            | 22.9 ms                                                     | 22.7 ms: 1.01x faster                                                     |
| unpickle_list              | 2.75 us                                                     | 2.72 us: 1.01x faster                                                     |
| unpack_sequence            | 37.5 ns                                                     | 37.7 ns: 1.01x slower                                                     |
| mdp                        | 1.37 sec                                                    | 1.38 sec: 1.01x slower                                                    |
| aiohttp                    | 884 us                                                      | 894 us: 1.01x slower                                                      |
| async_tree_memoization     | 339 ms                                                      | 344 ms: 1.02x slower                                                      |
| sympy_integrate            | 13.0 ms                                                     | 13.2 ms: 1.02x slower                                                     |
| 2to3                       | 218 ms                                                      | 223 ms: 1.02x slower                                                      |
| unpickle                   | 8.18 us                                                     | 8.39 us: 1.03x slower                                                     |
| go                         | 91.6 ms                                                     | 93.9 ms: 1.03x slower                                                     |
| scimark_sor                | 78.8 ms                                                     | 83.1 ms: 1.06x slower                                                     |
| pickle_list                | 2.83 us                                                     | 3.04 us: 1.08x slower                                                     |
| regex_v8                   | 14.2 ms                                                     | 15.3 ms: 1.08x slower                                                     |
| coverage                   | 40.8 ms                                                     | 46.0 ms: 1.13x slower                                                     |
| telco                      | 4.13 ms                                                     | 4.70 ms: 1.14x slower                                                     |
| python_startup             | 19.5 ms                                                     | 23.4 ms: 1.20x slower                                                     |
| scimark_lu                 | 58.9 ms                                                     | 72.7 ms: 1.23x slower                                                     |
| python_startup_no_site     | 16.2 ms                                                     | 21.1 ms: 1.30x slower                                                     |
| dask                       | 263 ms                                                      | 363 ms: 1.38x slower                                                      |
| Geometric mean             | (ref)                                                       | 1.04x faster                                                              |

Benchmark hidden because not significant (5): create_gc_cycles, async_tree_io, bench_mp_pool, sqlglot_optimize, xml_etree_parse
Ignored benchmarks (2) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (5) of results/bm-20240229-3.13.0a4+-1a78317-JIT/bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317.json: genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: unknown