# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_jumps
- machine: linux-x86_64
- commit hash: 594cca3
- commit date: 2024-02-29
- overall geometric mean: 1.05x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 1.11x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 307 ms: 1.08x slower                                                       |
| chameleon      | 7.23 ms                                                      | 7.48 ms: 1.04x slower                                                      |
| docutils       | 2.87 sec                                                     | 2.92 sec: 1.02x slower                                                     |
| tornado_http   | 121 ms                                                       | 124 ms: 1.02x slower                                                       |
| Geometric mean | (ref)                                                        | 1.04x slower                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_none            | 452 ms                                                       | 443 ms: 1.02x faster                                                       |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 711 ms: 1.02x slower                                                       |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 711 ms: 1.02x slower                                                       |
| async_tree_memoization     | 544 ms                                                       | 560 ms: 1.03x slower                                                       |
| async_tree_none_tg         | 431 ms                                                       | 446 ms: 1.03x slower                                                       |
| async_tree_io_tg           | 1.05 sec                                                     | 1.10 sec: 1.04x slower                                                     |
| async_tree_memoization_tg  | 540 ms                                                       | 567 ms: 1.05x slower                                                       |
| async_tree_io              | 1.04 sec                                                     | 1.10 sec: 1.05x slower                                                     |
| Geometric mean             | (ref)                                                        | 1.03x slower                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 262 ms: 1.01x faster                                                       |
| float          | 76.6 ms                                                      | 78.4 ms: 1.02x slower                                                      |
| nbody          | 88.0 ms                                                      | 101 ms: 1.14x slower                                                       |
| Geometric mean | (ref)                                                        | 1.05x slower                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_dna      | 239 ms                                                       | 237 ms: 1.01x faster                                                       |
| regex_effbot   | 3.57 ms                                                      | 3.63 ms: 1.02x slower                                                      |
| regex_compile  | 144 ms                                                       | 148 ms: 1.03x slower                                                       |
| regex_v8       | 23.6 ms                                                      | 25.3 ms: 1.07x slower                                                      |
| Geometric mean | (ref)                                                        | 1.03x slower                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle_dict          | 32.5 us                                                      | 30.5 us: 1.07x faster                                                      |
| pickle_list          | 4.43 us                                                      | 4.28 us: 1.03x faster                                                      |
| pickle               | 10.5 us                                                      | 10.3 us: 1.02x faster                                                      |
| xml_etree_generate   | 86.1 ms                                                      | 84.4 ms: 1.02x faster                                                      |
| xml_etree_process    | 58.4 ms                                                      | 58.0 ms: 1.01x faster                                                      |
| tomli_loads          | 2.16 sec                                                     | 2.14 sec: 1.01x faster                                                     |
| unpickle_list        | 4.66 us                                                      | 4.72 us: 1.01x slower                                                      |
| xml_etree_parse      | 144 ms                                                       | 146 ms: 1.02x slower                                                       |
| json_dumps           | 10.2 ms                                                      | 10.5 ms: 1.02x slower                                                      |
| json_loads           | 24.4 us                                                      | 25.5 us: 1.05x slower                                                      |
| unpickle             | 14.8 us                                                      | 15.5 us: 1.05x slower                                                      |
| unpickle_pure_python | 210 us                                                       | 233 us: 1.11x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.01x slower                                                               |

Benchmark hidden because not significant (2): pickle_pure_python, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 15.5 ms: 1.34x slower                                                      |
| python_startup_no_site | 8.64 ms                                                      | 14.1 ms: 1.63x slower                                                      |
| Geometric mean         | (ref)                                                        | 1.48x slower                                                               |

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| typing_runtime_protocols   | 152 us                                                       | 123 us: 1.23x faster                                                       |
| comprehensions             | 21.9 us                                                      | 18.7 us: 1.17x faster                                                      |
| generators                 | 37.4 ms                                                      | 33.4 ms: 1.12x faster                                                      |
| pickle_dict                | 32.5 us                                                      | 30.5 us: 1.07x faster                                                      |
| crypto_pyaes               | 80.3 ms                                                      | 77.0 ms: 1.04x faster                                                      |
| pickle_list                | 4.43 us                                                      | 4.28 us: 1.03x faster                                                      |
| coroutines                 | 23.0 ms                                                      | 22.3 ms: 1.03x faster                                                      |
| sqlite_synth               | 2.77 us                                                      | 2.70 us: 1.03x faster                                                      |
| logging_format             | 7.48 us                                                      | 7.28 us: 1.03x faster                                                      |
| pickle                     | 10.5 us                                                      | 10.3 us: 1.02x faster                                                      |
| xml_etree_generate         | 86.1 ms                                                      | 84.4 ms: 1.02x faster                                                      |
| async_tree_none            | 452 ms                                                       | 443 ms: 1.02x faster                                                       |
| sympy_sum                  | 162 ms                                                       | 159 ms: 1.02x faster                                                       |
| create_gc_cycles           | 1.59 ms                                                      | 1.56 ms: 1.02x faster                                                      |
| logging_simple             | 6.71 us                                                      | 6.60 us: 1.02x faster                                                      |
| async_generators           | 390 ms                                                       | 385 ms: 1.01x faster                                                       |
| pidigits                   | 265 ms                                                       | 262 ms: 1.01x faster                                                       |
| regex_dna                  | 239 ms                                                       | 237 ms: 1.01x faster                                                       |
| xml_etree_process          | 58.4 ms                                                      | 58.0 ms: 1.01x faster                                                      |
| tomli_loads                | 2.16 sec                                                     | 2.14 sec: 1.01x faster                                                     |
| asyncio_tcp                | 378 ms                                                       | 376 ms: 1.01x faster                                                       |
| deepcopy_reduce            | 3.37 us                                                      | 3.35 us: 1.00x faster                                                      |
| asyncio_tcp_ssl            | 1.59 sec                                                     | 1.58 sec: 1.00x faster                                                     |
| raytrace                   | 298 ms                                                       | 300 ms: 1.01x slower                                                       |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 4.25 ms: 1.01x slower                                                      |
| unpickle_list              | 4.66 us                                                      | 4.72 us: 1.01x slower                                                      |
| spectral_norm              | 91.6 ms                                                      | 92.9 ms: 1.01x slower                                                      |
| pathlib                    | 18.9 ms                                                      | 19.2 ms: 1.02x slower                                                      |
| xml_etree_parse            | 144 ms                                                       | 146 ms: 1.02x slower                                                       |
| regex_effbot               | 3.57 ms                                                      | 3.63 ms: 1.02x slower                                                      |
| sqlglot_normalize          | 116 ms                                                       | 118 ms: 1.02x slower                                                       |
| docutils                   | 2.87 sec                                                     | 2.92 sec: 1.02x slower                                                     |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 711 ms: 1.02x slower                                                       |
| mdp                        | 2.57 sec                                                     | 2.62 sec: 1.02x slower                                                     |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 711 ms: 1.02x slower                                                       |
| meteor_contest             | 128 ms                                                       | 131 ms: 1.02x slower                                                       |
| float                      | 76.6 ms                                                      | 78.4 ms: 1.02x slower                                                      |
| sympy_integrate            | 23.9 ms                                                      | 24.5 ms: 1.02x slower                                                      |
| tornado_http               | 121 ms                                                       | 124 ms: 1.02x slower                                                       |
| json_dumps                 | 10.2 ms                                                      | 10.5 ms: 1.02x slower                                                      |
| regex_compile              | 144 ms                                                       | 148 ms: 1.03x slower                                                       |
| async_tree_memoization     | 544 ms                                                       | 560 ms: 1.03x slower                                                       |
| json                       | 5.12 ms                                                      | 5.28 ms: 1.03x slower                                                      |
| async_tree_none_tg         | 431 ms                                                       | 446 ms: 1.03x slower                                                       |
| chameleon                  | 7.23 ms                                                      | 7.48 ms: 1.04x slower                                                      |
| bench_thread_pool          | 950 us                                                       | 986 us: 1.04x slower                                                       |
| sqlglot_parse              | 1.38 ms                                                      | 1.43 ms: 1.04x slower                                                      |
| async_tree_io_tg           | 1.05 sec                                                     | 1.10 sec: 1.04x slower                                                     |
| pprint_safe_repr           | 807 ms                                                       | 843 ms: 1.04x slower                                                       |
| json_loads                 | 24.4 us                                                      | 25.5 us: 1.05x slower                                                      |
| sqlglot_transpile          | 1.78 ms                                                      | 1.86 ms: 1.05x slower                                                      |
| unpickle                   | 14.8 us                                                      | 15.5 us: 1.05x slower                                                      |
| logging_silent             | 94.4 ns                                                      | 99.0 ns: 1.05x slower                                                      |
| async_tree_memoization_tg  | 540 ms                                                       | 567 ms: 1.05x slower                                                       |
| chaos                      | 64.0 ms                                                      | 67.2 ms: 1.05x slower                                                      |
| async_tree_io              | 1.04 sec                                                     | 1.10 sec: 1.05x slower                                                     |
| deepcopy                   | 368 us                                                       | 389 us: 1.06x slower                                                       |
| dulwich_log                | 65.4 ms                                                      | 69.1 ms: 1.06x slower                                                      |
| pprint_pformat             | 1.65 sec                                                     | 1.76 sec: 1.06x slower                                                     |
| sympy_expand               | 484 ms                                                       | 517 ms: 1.07x slower                                                       |
| regex_v8                   | 23.6 ms                                                      | 25.3 ms: 1.07x slower                                                      |
| scimark_fft                | 301 ms                                                       | 322 ms: 1.07x slower                                                       |
| deepcopy_memo              | 36.8 us                                                      | 39.6 us: 1.08x slower                                                      |
| 2to3                       | 285 ms                                                       | 307 ms: 1.08x slower                                                       |
| pycparser                  | 1.23 sec                                                     | 1.33 sec: 1.08x slower                                                     |
| sqlglot_optimize           | 57.5 ms                                                      | 62.8 ms: 1.09x slower                                                      |
| nqueens                    | 89.9 ms                                                      | 99.1 ms: 1.10x slower                                                      |
| mypy2                      | 830 ms                                                       | 915 ms: 1.10x slower                                                       |
| unpickle_pure_python       | 210 us                                                       | 233 us: 1.11x slower                                                       |
| richards                   | 45.7 ms                                                      | 51.2 ms: 1.12x slower                                                      |
| fannkuch                   | 350 ms                                                       | 394 ms: 1.13x slower                                                       |
| scimark_monte_carlo        | 69.0 ms                                                      | 77.7 ms: 1.13x slower                                                      |
| richards_super             | 51.3 ms                                                      | 58.3 ms: 1.14x slower                                                      |
| nbody                      | 88.0 ms                                                      | 101 ms: 1.14x slower                                                       |
| unpack_sequence            | 53.2 ns                                                      | 61.5 ns: 1.16x slower                                                      |
| telco                      | 6.96 ms                                                      | 8.06 ms: 1.16x slower                                                      |
| go                         | 150 ms                                                       | 176 ms: 1.17x slower                                                       |
| coverage                   | 66.7 ms                                                      | 78.8 ms: 1.18x slower                                                      |
| deltablue                  | 3.24 ms                                                      | 3.83 ms: 1.18x slower                                                      |
| pyflate                    | 439 ms                                                       | 529 ms: 1.21x slower                                                       |
| hexiom                     | 5.96 ms                                                      | 7.34 ms: 1.23x slower                                                      |
| scimark_lu                 | 98.8 ms                                                      | 124 ms: 1.25x slower                                                       |
| python_startup             | 11.6 ms                                                      | 15.5 ms: 1.34x slower                                                      |
| scimark_sor                | 109 ms                                                       | 155 ms: 1.42x slower                                                       |
| bench_mp_pool              | 4.76 ms                                                      | 6.86 ms: 1.44x slower                                                      |
| python_startup_no_site     | 8.64 ms                                                      | 14.1 ms: 1.63x slower                                                      |
| Geometric mean             | (ref)                                                        | 1.05x slower                                                               |

Benchmark hidden because not significant (6): gc_traversal, pickle_pure_python, mako, xml_etree_iterparse, sympy_str, asyncio_websockets
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 1.11x