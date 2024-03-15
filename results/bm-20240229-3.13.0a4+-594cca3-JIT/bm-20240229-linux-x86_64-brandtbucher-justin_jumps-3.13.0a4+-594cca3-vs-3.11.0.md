# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_jumps
- machine: linux-x86_64
- commit hash: 594cca3
- commit date: 2024-02-29
- overall geometric mean: 1.04x faster \*
- HPT reliability: 99.40%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.24x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 276 ms: 1.04x slower                                                 |
| docutils       | 2.66 sec                                               | 2.70 sec: 1.02x slower                                               |
| tornado_http   | 98.1 ms                                                | 96.6 ms: 1.01x faster                                                |
| Geometric mean | (ref)                                                  | 1.01x slower                                                         |

Benchmark hidden because not significant (1): chameleon

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 434 ms: 1.22x faster                                                 |
| async_tree_memoization     | 639 ms                                                 | 560 ms: 1.14x faster                                                 |
| async_tree_none_tg         | 491 ms                                                 | 445 ms: 1.10x faster                                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 573 ms: 1.09x faster                                                 |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                               |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                               |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 702 ms: 1.07x faster                                                 |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 716 ms: 1.06x faster                                                 |
| Geometric mean             | (ref)                                                  | 1.11x faster                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                                 |
| nbody          | 96.0 ms                                                | 92.9 ms: 1.03x faster                                                |
| float          | 78.9 ms                                                | 78.2 ms: 1.01x faster                                                |
| Geometric mean | (ref)                                                  | 1.03x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 143 ms: 1.01x slower                                                 |
| regex_effbot   | 3.51 ms                                                | 3.56 ms: 1.02x slower                                                |
| regex_v8       | 22.9 ms                                                | 24.3 ms: 1.06x slower                                                |
| regex_dna      | 205 ms                                                 | 224 ms: 1.10x slower                                                 |
| Geometric mean | (ref)                                                  | 1.05x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.3 ms: 1.30x faster                                                |
| tomli_loads          | 2.30 sec                                               | 2.03 sec: 1.13x faster                                               |
| pickle_pure_python   | 320 us                                                 | 299 us: 1.07x faster                                                 |
| json_loads           | 29.2 us                                                | 27.4 us: 1.06x faster                                                |
| xml_etree_parse      | 164 ms                                                 | 156 ms: 1.05x faster                                                 |
| pickle_dict          | 34.6 us                                                | 33.3 us: 1.04x faster                                                |
| unpickle_list        | 5.21 us                                                | 5.05 us: 1.03x faster                                                |
| unpickle_pure_python | 242 us                                                 | 236 us: 1.03x faster                                                 |
| xml_etree_iterparse  | 108 ms                                                 | 106 ms: 1.02x faster                                                 |
| xml_etree_process    | 56.9 ms                                                | 58.2 ms: 1.02x slower                                                |
| pickle               | 11.0 us                                                | 11.3 us: 1.03x slower                                                |
| unpickle             | 13.8 us                                                | 14.6 us: 1.06x slower                                                |
| xml_etree_generate   | 81.1 ms                                                | 85.9 ms: 1.06x slower                                                |
| pickle_list          | 4.59 us                                                | 5.01 us: 1.09x slower                                                |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                         |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 12.2 ms: 1.43x slower                                                |
| python_startup_no_site | 6.01 ms                                                | 10.9 ms: 1.81x slower                                                |
| Geometric mean         | (ref)                                                  | 1.61x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 10.8 ms: 1.01x slower                                                |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 111 us: 4.69x faster                                                 |
| generators                 | 74.9 ms                                                | 29.3 ms: 2.55x faster                                                |
| asyncio_tcp                | 875 ms                                                 | 488 ms: 1.80x faster                                                 |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.73x faster                                               |
| comprehensions             | 23.6 us                                                | 17.0 us: 1.38x faster                                                |
| json_dumps                 | 13.3 ms                                                | 10.3 ms: 1.30x faster                                                |
| async_tree_none            | 528 ms                                                 | 434 ms: 1.22x faster                                                 |
| richards_super             | 61.9 ms                                                | 52.2 ms: 1.19x faster                                                |
| coroutines                 | 27.0 ms                                                | 22.9 ms: 1.18x faster                                                |
| deltablue                  | 3.92 ms                                                | 3.40 ms: 1.16x faster                                                |
| chaos                      | 71.9 ms                                                | 62.4 ms: 1.15x faster                                                |
| async_tree_memoization     | 639 ms                                                 | 560 ms: 1.14x faster                                                 |
| tomli_loads                | 2.30 sec                                               | 2.03 sec: 1.13x faster                                               |
| sqlglot_parse              | 1.43 ms                                                | 1.29 ms: 1.11x faster                                                |
| logging_silent             | 111 ns                                                 | 100.0 ns: 1.11x faster                                               |
| logging_simple             | 6.22 us                                                | 5.61 us: 1.11x faster                                                |
| logging_format             | 6.81 us                                                | 6.17 us: 1.10x faster                                                |
| async_tree_none_tg         | 491 ms                                                 | 445 ms: 1.10x faster                                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 573 ms: 1.09x faster                                                 |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                               |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                               |
| sqlglot_transpile          | 1.75 ms                                                | 1.63 ms: 1.08x faster                                                |
| raytrace                   | 309 ms                                                 | 288 ms: 1.07x faster                                                 |
| sympy_sum                  | 169 ms                                                 | 158 ms: 1.07x faster                                                 |
| pickle_pure_python         | 320 us                                                 | 299 us: 1.07x faster                                                 |
| gc_traversal               | 4.01 ms                                                | 3.75 ms: 1.07x faster                                                |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 702 ms: 1.07x faster                                                 |
| richards                   | 49.8 ms                                                | 46.7 ms: 1.07x faster                                                |
| mdp                        | 2.77 sec                                               | 2.61 sec: 1.06x faster                                               |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 716 ms: 1.06x faster                                                 |
| json_loads                 | 29.2 us                                                | 27.4 us: 1.06x faster                                                |
| sympy_str                  | 297 ms                                                 | 281 ms: 1.06x faster                                                 |
| crypto_pyaes               | 76.7 ms                                                | 72.5 ms: 1.06x faster                                                |
| deepcopy_reduce            | 3.22 us                                                | 3.05 us: 1.05x faster                                                |
| sqlglot_normalize          | 113 ms                                                 | 107 ms: 1.05x faster                                                 |
| xml_etree_parse            | 164 ms                                                 | 156 ms: 1.05x faster                                                 |
| json                       | 5.24 ms                                                | 5.00 ms: 1.05x faster                                                |
| deepcopy                   | 365 us                                                 | 350 us: 1.04x faster                                                 |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                                 |
| pickle_dict                | 34.6 us                                                | 33.3 us: 1.04x faster                                                |
| unpickle_list              | 5.21 us                                                | 5.05 us: 1.03x faster                                                |
| nbody                      | 96.0 ms                                                | 92.9 ms: 1.03x faster                                                |
| deepcopy_memo              | 40.2 us                                                | 38.9 us: 1.03x faster                                                |
| sympy_integrate            | 21.5 ms                                                | 20.9 ms: 1.03x faster                                                |
| scimark_fft                | 345 ms                                                 | 337 ms: 1.03x faster                                                 |
| unpickle_pure_python       | 242 us                                                 | 236 us: 1.03x faster                                                 |
| fannkuch                   | 405 ms                                                 | 396 ms: 1.02x faster                                                 |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.93 ms: 1.02x faster                                                |
| pycparser                  | 1.19 sec                                               | 1.16 sec: 1.02x faster                                               |
| xml_etree_iterparse        | 108 ms                                                 | 106 ms: 1.02x faster                                                 |
| tornado_http               | 98.1 ms                                                | 96.6 ms: 1.01x faster                                                |
| sympy_expand               | 484 ms                                                 | 478 ms: 1.01x faster                                                 |
| meteor_contest             | 109 ms                                                 | 108 ms: 1.01x faster                                                 |
| float                      | 78.9 ms                                                | 78.2 ms: 1.01x faster                                                |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                                 |
| regex_compile              | 141 ms                                                 | 143 ms: 1.01x slower                                                 |
| sqlglot_optimize           | 55.3 ms                                                | 56.0 ms: 1.01x slower                                                |
| mako                       | 10.7 ms                                                | 10.8 ms: 1.01x slower                                                |
| bench_thread_pool          | 834 us                                                 | 846 us: 1.01x slower                                                 |
| docutils                   | 2.66 sec                                               | 2.70 sec: 1.02x slower                                               |
| regex_effbot               | 3.51 ms                                                | 3.56 ms: 1.02x slower                                                |
| hexiom                     | 6.89 ms                                                | 7.02 ms: 1.02x slower                                                |
| xml_etree_process          | 56.9 ms                                                | 58.2 ms: 1.02x slower                                                |
| pickle                     | 11.0 us                                                | 11.3 us: 1.03x slower                                                |
| nqueens                    | 87.9 ms                                                | 90.7 ms: 1.03x slower                                                |
| scimark_sor                | 121 ms                                                 | 126 ms: 1.04x slower                                                 |
| create_gc_cycles           | 1.43 ms                                                | 1.49 ms: 1.04x slower                                                |
| spectral_norm              | 108 ms                                                 | 113 ms: 1.04x slower                                                 |
| 2to3                       | 264 ms                                                 | 276 ms: 1.04x slower                                                 |
| unpickle                   | 13.8 us                                                | 14.6 us: 1.06x slower                                                |
| go                         | 149 ms                                                 | 157 ms: 1.06x slower                                                 |
| xml_etree_generate         | 81.1 ms                                                | 85.9 ms: 1.06x slower                                                |
| regex_v8                   | 22.9 ms                                                | 24.3 ms: 1.06x slower                                                |
| dulwich_log                | 64.6 ms                                                | 68.7 ms: 1.06x slower                                                |
| sqlite_synth               | 2.57 us                                                | 2.81 us: 1.09x slower                                                |
| pickle_list                | 4.59 us                                                | 5.01 us: 1.09x slower                                                |
| regex_dna                  | 205 ms                                                 | 224 ms: 1.10x slower                                                 |
| pyflate                    | 434 ms                                                 | 484 ms: 1.12x slower                                                 |
| scimark_lu                 | 116 ms                                                 | 131 ms: 1.13x slower                                                 |
| bench_mp_pool              | 24.0 ms                                                | 27.8 ms: 1.16x slower                                                |
| coverage                   | 78.8 ms                                                | 95.6 ms: 1.21x slower                                                |
| telco                      | 6.86 ms                                                | 8.37 ms: 1.22x slower                                                |
| async_generators           | 374 ms                                                 | 457 ms: 1.22x slower                                                 |
| mypy2                      | 686 ms                                                 | 884 ms: 1.29x slower                                                 |
| python_startup             | 8.56 ms                                                | 12.2 ms: 1.43x slower                                                |
| python_startup_no_site     | 6.01 ms                                                | 10.9 ms: 1.81x slower                                                |
| unpack_sequence            | 43.5 ns                                                | 84.9 ns: 1.95x slower                                                |
| Geometric mean             | (ref)                                                  | 1.04x faster                                                         |

Benchmark hidden because not significant (5): pprint_safe_repr, pprint_pformat, chameleon, pathlib, scimark_monte_carlo
Ignored benchmarks (13) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.40% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.24x