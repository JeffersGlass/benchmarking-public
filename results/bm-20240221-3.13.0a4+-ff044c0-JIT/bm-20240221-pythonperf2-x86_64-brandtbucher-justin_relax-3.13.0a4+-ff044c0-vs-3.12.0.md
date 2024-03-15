
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_relax
- machine: linux-x86_64
- commit hash: ff044c0
- commit date: 2024-02-21
- overall geometric mean: 1.07x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x slower
- Memory change: 1.11x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 310 ms: 1.09x slower                                                       |
| chameleon      | 7.23 ms                                                      | 7.65 ms: 1.06x slower                                                      |
| docutils       | 2.87 sec                                                     | 2.94 sec: 1.03x slower                                                     |
| tornado_http   | 121 ms                                                       | 124 ms: 1.03x slower                                                       |
| Geometric mean | (ref)                                                        | 1.05x slower                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_none            | 452 ms                                                       | 443 ms: 1.02x faster                                                       |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 707 ms: 1.02x slower                                                       |
| async_tree_memoization     | 544 ms                                                       | 555 ms: 1.02x slower                                                       |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 711 ms: 1.02x slower                                                       |
| async_tree_none_tg         | 431 ms                                                       | 440 ms: 1.02x slower                                                       |
| async_tree_io_tg           | 1.05 sec                                                     | 1.09 sec: 1.04x slower                                                     |
| async_tree_memoization_tg  | 540 ms                                                       | 562 ms: 1.04x slower                                                       |
| async_tree_io              | 1.04 sec                                                     | 1.09 sec: 1.05x slower                                                     |
| Geometric mean             | (ref)                                                        | 1.02x slower                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 262 ms: 1.01x faster                                                       |
| float          | 76.6 ms                                                      | 80.2 ms: 1.05x slower                                                      |
| nbody          | 88.0 ms                                                      | 102 ms: 1.16x slower                                                       |
| Geometric mean | (ref)                                                        | 1.06x slower                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.50 ms: 1.02x faster                                                      |
| regex_dna      | 239 ms                                                       | 237 ms: 1.00x faster                                                       |
| regex_compile  | 144 ms                                                       | 152 ms: 1.06x slower                                                       |
| regex_v8       | 23.6 ms                                                      | 25.5 ms: 1.08x slower                                                      |
| Geometric mean | (ref)                                                        | 1.03x slower                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle_list          | 4.43 us                                                      | 4.27 us: 1.04x faster                                                      |
| pickle               | 10.5 us                                                      | 10.3 us: 1.02x faster                                                      |
| pickle_dict          | 32.5 us                                                      | 32.2 us: 1.01x faster                                                      |
| pickle_pure_python   | 318 us                                                       | 315 us: 1.01x faster                                                       |
| unpickle_list        | 4.66 us                                                      | 4.68 us: 1.01x slower                                                      |
| json_loads           | 24.4 us                                                      | 24.7 us: 1.02x slower                                                      |
| xml_etree_process    | 58.4 ms                                                      | 59.4 ms: 1.02x slower                                                      |
| xml_etree_iterparse  | 103 ms                                                       | 105 ms: 1.02x slower                                                       |
| json_dumps           | 10.2 ms                                                      | 10.6 ms: 1.03x slower                                                      |
| xml_etree_parse      | 144 ms                                                       | 151 ms: 1.05x slower                                                       |
| tomli_loads          | 2.16 sec                                                     | 2.37 sec: 1.10x slower                                                     |
| unpickle_pure_python | 210 us                                                       | 240 us: 1.15x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.02x slower                                                               |

Benchmark hidden because not significant (2): xml_etree_generate, unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 15.6 ms: 1.34x slower                                                      |
| python_startup_no_site | 8.64 ms                                                      | 14.1 ms: 1.63x slower                                                      |
| Geometric mean         | (ref)                                                        | 1.48x slower                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 10.7 ms: 1.07x slower                                                      |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| typing_runtime_protocols   | 152 us                                                       | 118 us: 1.29x faster                                                       |
| comprehensions             | 21.9 us                                                      | 19.1 us: 1.15x faster                                                      |
| generators                 | 37.4 ms                                                      | 34.8 ms: 1.08x faster                                                      |
| pickle_list                | 4.43 us                                                      | 4.27 us: 1.04x faster                                                      |
| coroutines                 | 23.0 ms                                                      | 22.4 ms: 1.03x faster                                                      |
| regex_effbot               | 3.57 ms                                                      | 3.50 ms: 1.02x faster                                                      |
| async_tree_none            | 452 ms                                                       | 443 ms: 1.02x faster                                                       |
| pickle                     | 10.5 us                                                      | 10.3 us: 1.02x faster                                                      |
| asyncio_tcp                | 378 ms                                                       | 372 ms: 1.02x faster                                                       |
| pidigits                   | 265 ms                                                       | 262 ms: 1.01x faster                                                       |
| pickle_dict                | 32.5 us                                                      | 32.2 us: 1.01x faster                                                      |
| pickle_pure_python         | 318 us                                                       | 315 us: 1.01x faster                                                       |
| crypto_pyaes               | 80.3 ms                                                      | 79.7 ms: 1.01x faster                                                      |
| sqlite_synth               | 2.77 us                                                      | 2.76 us: 1.01x faster                                                      |
| asyncio_tcp_ssl            | 1.59 sec                                                     | 1.58 sec: 1.01x faster                                                     |
| regex_dna                  | 239 ms                                                       | 237 ms: 1.00x faster                                                       |
| sympy_sum                  | 162 ms                                                       | 161 ms: 1.00x faster                                                       |
| sympy_str                  | 302 ms                                                       | 303 ms: 1.00x slower                                                       |
| logging_simple             | 6.71 us                                                      | 6.75 us: 1.01x slower                                                      |
| unpickle_list              | 4.66 us                                                      | 4.68 us: 1.01x slower                                                      |
| deepcopy_reduce            | 3.37 us                                                      | 3.41 us: 1.01x slower                                                      |
| json_loads                 | 24.4 us                                                      | 24.7 us: 1.02x slower                                                      |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 707 ms: 1.02x slower                                                       |
| xml_etree_process          | 58.4 ms                                                      | 59.4 ms: 1.02x slower                                                      |
| pathlib                    | 18.9 ms                                                      | 19.2 ms: 1.02x slower                                                      |
| async_tree_memoization     | 544 ms                                                       | 555 ms: 1.02x slower                                                       |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 711 ms: 1.02x slower                                                       |
| async_tree_none_tg         | 431 ms                                                       | 440 ms: 1.02x slower                                                       |
| mdp                        | 2.57 sec                                                     | 2.62 sec: 1.02x slower                                                     |
| xml_etree_iterparse        | 103 ms                                                       | 105 ms: 1.02x slower                                                       |
| tornado_http               | 121 ms                                                       | 124 ms: 1.03x slower                                                       |
| docutils                   | 2.87 sec                                                     | 2.94 sec: 1.03x slower                                                     |
| json_dumps                 | 10.2 ms                                                      | 10.6 ms: 1.03x slower                                                      |
| json                       | 5.12 ms                                                      | 5.30 ms: 1.04x slower                                                      |
| async_tree_io_tg           | 1.05 sec                                                     | 1.09 sec: 1.04x slower                                                     |
| meteor_contest             | 128 ms                                                       | 133 ms: 1.04x slower                                                       |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 4.36 ms: 1.04x slower                                                      |
| raytrace                   | 298 ms                                                       | 310 ms: 1.04x slower                                                       |
| sympy_integrate            | 23.9 ms                                                      | 24.9 ms: 1.04x slower                                                      |
| async_tree_memoization_tg  | 540 ms                                                       | 562 ms: 1.04x slower                                                       |
| deepcopy_memo              | 36.8 us                                                      | 38.4 us: 1.04x slower                                                      |
| sqlglot_normalize          | 116 ms                                                       | 121 ms: 1.04x slower                                                       |
| float                      | 76.6 ms                                                      | 80.2 ms: 1.05x slower                                                      |
| bench_thread_pool          | 950 us                                                       | 994 us: 1.05x slower                                                       |
| deepcopy                   | 368 us                                                       | 386 us: 1.05x slower                                                       |
| sqlglot_parse              | 1.38 ms                                                      | 1.44 ms: 1.05x slower                                                      |
| spectral_norm              | 91.6 ms                                                      | 96.2 ms: 1.05x slower                                                      |
| xml_etree_parse            | 144 ms                                                       | 151 ms: 1.05x slower                                                       |
| async_tree_io              | 1.04 sec                                                     | 1.09 sec: 1.05x slower                                                     |
| sqlglot_transpile          | 1.78 ms                                                      | 1.87 ms: 1.05x slower                                                      |
| regex_compile              | 144 ms                                                       | 152 ms: 1.06x slower                                                       |
| chameleon                  | 7.23 ms                                                      | 7.65 ms: 1.06x slower                                                      |
| dulwich_log                | 65.4 ms                                                      | 69.2 ms: 1.06x slower                                                      |
| logging_silent             | 94.4 ns                                                      | 100 ns: 1.06x slower                                                       |
| sympy_expand               | 484 ms                                                       | 516 ms: 1.07x slower                                                       |
| mako                       | 10.0 ms                                                      | 10.7 ms: 1.07x slower                                                      |
| regex_v8                   | 23.6 ms                                                      | 25.5 ms: 1.08x slower                                                      |
| pycparser                  | 1.23 sec                                                     | 1.33 sec: 1.08x slower                                                     |
| chaos                      | 64.0 ms                                                      | 69.3 ms: 1.08x slower                                                      |
| 2to3                       | 285 ms                                                       | 310 ms: 1.09x slower                                                       |
| tomli_loads                | 2.16 sec                                                     | 2.37 sec: 1.10x slower                                                     |
| pprint_safe_repr           | 807 ms                                                       | 888 ms: 1.10x slower                                                       |
| pprint_pformat             | 1.65 sec                                                     | 1.83 sec: 1.10x slower                                                     |
| mypy2                      | 830 ms                                                       | 918 ms: 1.11x slower                                                       |
| sqlglot_optimize           | 57.5 ms                                                      | 64.0 ms: 1.11x slower                                                      |
| scimark_fft                | 301 ms                                                       | 339 ms: 1.13x slower                                                       |
| gc_traversal               | 3.48 ms                                                      | 3.95 ms: 1.14x slower                                                      |
| unpickle_pure_python       | 210 us                                                       | 240 us: 1.15x slower                                                       |
| nbody                      | 88.0 ms                                                      | 102 ms: 1.16x slower                                                       |
| deltablue                  | 3.24 ms                                                      | 3.75 ms: 1.16x slower                                                      |
| nqueens                    | 89.9 ms                                                      | 104 ms: 1.16x slower                                                       |
| richards_super             | 51.3 ms                                                      | 60.5 ms: 1.18x slower                                                      |
| telco                      | 6.96 ms                                                      | 8.23 ms: 1.18x slower                                                      |
| richards                   | 45.7 ms                                                      | 54.4 ms: 1.19x slower                                                      |
| scimark_monte_carlo        | 69.0 ms                                                      | 83.6 ms: 1.21x slower                                                      |
| go                         | 150 ms                                                       | 182 ms: 1.22x slower                                                       |
| fannkuch                   | 350 ms                                                       | 431 ms: 1.23x slower                                                       |
| pyflate                    | 439 ms                                                       | 547 ms: 1.25x slower                                                       |
| coverage                   | 66.7 ms                                                      | 83.7 ms: 1.25x slower                                                      |
| scimark_lu                 | 98.8 ms                                                      | 131 ms: 1.32x slower                                                       |
| hexiom                     | 5.96 ms                                                      | 7.90 ms: 1.33x slower                                                      |
| python_startup             | 11.6 ms                                                      | 15.6 ms: 1.34x slower                                                      |
| scimark_sor                | 109 ms                                                       | 155 ms: 1.42x slower                                                       |
| bench_mp_pool              | 4.76 ms                                                      | 6.83 ms: 1.43x slower                                                      |
| unpack_sequence            | 53.2 ns                                                      | 79.7 ns: 1.50x slower                                                      |
| python_startup_no_site     | 8.64 ms                                                      | 14.1 ms: 1.63x slower                                                      |
| Geometric mean             | (ref)                                                        | 1.07x slower                                                               |

Benchmark hidden because not significant (6): create_gc_cycles, async_generators, logging_format, xml_etree_generate, unpickle, asyncio_websockets
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.03x
- 95% likely to have a slowdown of 1.03x
- 99% likely to have a slowdown of 1.03x


# Memory

- memory change: 1.11x