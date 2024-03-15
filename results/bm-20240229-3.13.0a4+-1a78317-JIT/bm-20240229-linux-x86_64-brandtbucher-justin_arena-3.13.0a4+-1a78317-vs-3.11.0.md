# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_arena
- machine: linux-x86_64
- commit hash: 1a78317
- commit date: 2024-02-29
- overall geometric mean: 1.04x faster \*
- HPT reliability: 98.43%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.24x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 276 ms: 1.05x slower                                                 |
| chameleon      | 6.70 ms                                                | 6.86 ms: 1.02x slower                                                |
| docutils       | 2.66 sec                                               | 2.70 sec: 1.01x slower                                               |
| html5lib       | 64.8 ms                                                | 67.3 ms: 1.04x slower                                                |
| tornado_http   | 98.1 ms                                                | 96.9 ms: 1.01x faster                                                |
| Geometric mean | (ref)                                                  | 1.02x slower                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 435 ms: 1.21x faster                                                 |
| async_tree_memoization     | 639 ms                                                 | 561 ms: 1.14x faster                                                 |
| async_tree_none_tg         | 491 ms                                                 | 446 ms: 1.10x faster                                                 |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                               |
| async_tree_memoization_tg  | 626 ms                                                 | 576 ms: 1.09x faster                                                 |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                               |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 707 ms: 1.06x faster                                                 |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 726 ms: 1.05x faster                                                 |
| Geometric mean             | (ref)                                                  | 1.10x faster                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 92.0 ms: 1.04x faster                                                |
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                                 |
| float          | 78.9 ms                                                | 77.9 ms: 1.01x faster                                                |
| Geometric mean | (ref)                                                  | 1.03x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 142 ms: 1.00x slower                                                 |
| regex_v8       | 22.9 ms                                                | 24.2 ms: 1.06x slower                                                |
| regex_effbot   | 3.51 ms                                                | 3.74 ms: 1.07x slower                                                |
| regex_dna      | 205 ms                                                 | 224 ms: 1.09x slower                                                 |
| Geometric mean | (ref)                                                  | 1.06x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                |
| tomli_loads          | 2.30 sec                                               | 2.01 sec: 1.15x faster                                               |
| pickle_pure_python   | 320 us                                                 | 297 us: 1.08x faster                                                 |
| unpickle_list        | 5.21 us                                                | 4.90 us: 1.06x faster                                                |
| json_loads           | 29.2 us                                                | 27.5 us: 1.06x faster                                                |
| xml_etree_parse      | 164 ms                                                 | 156 ms: 1.05x faster                                                 |
| unpickle_pure_python | 242 us                                                 | 236 us: 1.02x faster                                                 |
| xml_etree_iterparse  | 108 ms                                                 | 106 ms: 1.02x faster                                                 |
| pickle_dict          | 34.6 us                                                | 34.7 us: 1.00x slower                                                |
| xml_etree_process    | 56.9 ms                                                | 58.2 ms: 1.02x slower                                                |
| pickle               | 11.0 us                                                | 11.3 us: 1.03x slower                                                |
| xml_etree_generate   | 81.1 ms                                                | 84.9 ms: 1.05x slower                                                |
| pickle_list          | 4.59 us                                                | 4.90 us: 1.07x slower                                                |
| unpickle             | 13.8 us                                                | 15.4 us: 1.12x slower                                                |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                         |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 12.1 ms: 1.42x slower                                                |
| python_startup_no_site | 6.01 ms                                                | 10.7 ms: 1.78x slower                                                |
| Geometric mean         | (ref)                                                  | 1.59x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|-----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| genshi_xml      | 53.4 ms                                                | 54.4 ms: 1.02x slower                                                |
| django_template | 33.5 ms                                                | 34.3 ms: 1.02x slower                                                |
| mako            | 10.7 ms                                                | 10.9 ms: 1.02x slower                                                |
| genshi_text     | 22.5 ms                                                | 24.0 ms: 1.07x slower                                                |
| Geometric mean  | (ref)                                                  | 1.03x slower                                                         |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 110 us: 4.73x faster                                                 |
| generators                 | 74.9 ms                                                | 29.3 ms: 2.55x faster                                                |
| asyncio_tcp                | 875 ms                                                 | 489 ms: 1.79x faster                                                 |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.73x faster                                               |
| pylint                     | 476 ms                                                 | 318 ms: 1.50x faster                                                 |
| comprehensions             | 23.6 us                                                | 17.1 us: 1.38x faster                                                |
| json_dumps                 | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                |
| async_tree_none            | 528 ms                                                 | 435 ms: 1.21x faster                                                 |
| coroutines                 | 27.0 ms                                                | 22.8 ms: 1.19x faster                                                |
| richards_super             | 61.9 ms                                                | 52.2 ms: 1.19x faster                                                |
| deltablue                  | 3.92 ms                                                | 3.39 ms: 1.16x faster                                                |
| tomli_loads                | 2.30 sec                                               | 2.01 sec: 1.15x faster                                               |
| chaos                      | 71.9 ms                                                | 62.9 ms: 1.14x faster                                                |
| gc_traversal               | 4.01 ms                                                | 3.51 ms: 1.14x faster                                                |
| async_tree_memoization     | 639 ms                                                 | 561 ms: 1.14x faster                                                 |
| logging_silent             | 111 ns                                                 | 97.9 ns: 1.13x faster                                                |
| sqlglot_parse              | 1.43 ms                                                | 1.28 ms: 1.12x faster                                                |
| logging_simple             | 6.22 us                                                | 5.65 us: 1.10x faster                                                |
| async_tree_none_tg         | 491 ms                                                 | 446 ms: 1.10x faster                                                 |
| logging_format             | 6.81 us                                                | 6.24 us: 1.09x faster                                                |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                               |
| async_tree_memoization_tg  | 626 ms                                                 | 576 ms: 1.09x faster                                                 |
| richards                   | 49.8 ms                                                | 45.8 ms: 1.09x faster                                                |
| sympy_sum                  | 169 ms                                                 | 156 ms: 1.08x faster                                                 |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                               |
| pickle_pure_python         | 320 us                                                 | 297 us: 1.08x faster                                                 |
| sqlglot_transpile          | 1.75 ms                                                | 1.63 ms: 1.08x faster                                                |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.68 ms: 1.07x faster                                                |
| raytrace                   | 309 ms                                                 | 288 ms: 1.07x faster                                                 |
| deepcopy_reduce            | 3.22 us                                                | 3.02 us: 1.07x faster                                                |
| unpickle_list              | 5.21 us                                                | 4.90 us: 1.06x faster                                                |
| sympy_str                  | 297 ms                                                 | 280 ms: 1.06x faster                                                 |
| json_loads                 | 29.2 us                                                | 27.5 us: 1.06x faster                                                |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 707 ms: 1.06x faster                                                 |
| sqlglot_normalize          | 113 ms                                                 | 106 ms: 1.06x faster                                                 |
| xml_etree_parse            | 164 ms                                                 | 156 ms: 1.05x faster                                                 |
| deepcopy                   | 365 us                                                 | 347 us: 1.05x faster                                                 |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 726 ms: 1.05x faster                                                 |
| mdp                        | 2.77 sec                                               | 2.65 sec: 1.05x faster                                               |
| nbody                      | 96.0 ms                                                | 92.0 ms: 1.04x faster                                                |
| crypto_pyaes               | 76.7 ms                                                | 73.7 ms: 1.04x faster                                                |
| deepcopy_memo              | 40.2 us                                                | 38.6 us: 1.04x faster                                                |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                                 |
| scimark_fft                | 345 ms                                                 | 333 ms: 1.04x faster                                                 |
| json                       | 5.24 ms                                                | 5.07 ms: 1.03x faster                                                |
| sympy_integrate            | 21.5 ms                                                | 20.8 ms: 1.03x faster                                                |
| fannkuch                   | 405 ms                                                 | 393 ms: 1.03x faster                                                 |
| unpickle_pure_python       | 242 us                                                 | 236 us: 1.02x faster                                                 |
| meteor_contest             | 109 ms                                                 | 107 ms: 1.02x faster                                                 |
| pycparser                  | 1.19 sec                                               | 1.16 sec: 1.02x faster                                               |
| xml_etree_iterparse        | 108 ms                                                 | 106 ms: 1.02x faster                                                 |
| sympy_expand               | 484 ms                                                 | 475 ms: 1.02x faster                                                 |
| float                      | 78.9 ms                                                | 77.9 ms: 1.01x faster                                                |
| tornado_http               | 98.1 ms                                                | 96.9 ms: 1.01x faster                                                |
| pathlib                    | 18.5 ms                                                | 18.4 ms: 1.01x faster                                                |
| regex_compile              | 141 ms                                                 | 142 ms: 1.00x slower                                                 |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                                 |
| pickle_dict                | 34.6 us                                                | 34.7 us: 1.00x slower                                                |
| sqlglot_optimize           | 55.3 ms                                                | 55.7 ms: 1.01x slower                                                |
| bench_thread_pool          | 834 us                                                 | 844 us: 1.01x slower                                                 |
| hexiom                     | 6.89 ms                                                | 6.98 ms: 1.01x slower                                                |
| docutils                   | 2.66 sec                                               | 2.70 sec: 1.01x slower                                               |
| nqueens                    | 87.9 ms                                                | 89.0 ms: 1.01x slower                                                |
| thrift                     | 784 us                                                 | 797 us: 1.02x slower                                                 |
| genshi_xml                 | 53.4 ms                                                | 54.4 ms: 1.02x slower                                                |
| django_template            | 33.5 ms                                                | 34.3 ms: 1.02x slower                                                |
| xml_etree_process          | 56.9 ms                                                | 58.2 ms: 1.02x slower                                                |
| chameleon                  | 6.70 ms                                                | 6.86 ms: 1.02x slower                                                |
| mako                       | 10.7 ms                                                | 10.9 ms: 1.02x slower                                                |
| pickle                     | 11.0 us                                                | 11.3 us: 1.03x slower                                                |
| spectral_norm              | 108 ms                                                 | 112 ms: 1.03x slower                                                 |
| html5lib                   | 64.8 ms                                                | 67.3 ms: 1.04x slower                                                |
| create_gc_cycles           | 1.43 ms                                                | 1.50 ms: 1.04x slower                                                |
| go                         | 149 ms                                                 | 155 ms: 1.05x slower                                                 |
| 2to3                       | 264 ms                                                 | 276 ms: 1.05x slower                                                 |
| xml_etree_generate         | 81.1 ms                                                | 84.9 ms: 1.05x slower                                                |
| aiohttp                    | 1.12 ms                                                | 1.17 ms: 1.05x slower                                                |
| regex_v8                   | 22.9 ms                                                | 24.2 ms: 1.06x slower                                                |
| gunicorn                   | 1.20 ms                                                | 1.27 ms: 1.06x slower                                                |
| dulwich_log                | 64.6 ms                                                | 68.6 ms: 1.06x slower                                                |
| scimark_sor                | 121 ms                                                 | 129 ms: 1.06x slower                                                 |
| regex_effbot               | 3.51 ms                                                | 3.74 ms: 1.07x slower                                                |
| genshi_text                | 22.5 ms                                                | 24.0 ms: 1.07x slower                                                |
| pickle_list                | 4.59 us                                                | 4.90 us: 1.07x slower                                                |
| pyflate                    | 434 ms                                                 | 471 ms: 1.09x slower                                                 |
| regex_dna                  | 205 ms                                                 | 224 ms: 1.09x slower                                                 |
| sqlite_synth               | 2.57 us                                                | 2.83 us: 1.10x slower                                                |
| scimark_lu                 | 116 ms                                                 | 129 ms: 1.11x slower                                                 |
| unpickle                   | 13.8 us                                                | 15.4 us: 1.12x slower                                                |
| bench_mp_pool              | 24.0 ms                                                | 28.1 ms: 1.17x slower                                                |
| telco                      | 6.86 ms                                                | 8.26 ms: 1.20x slower                                                |
| coverage                   | 78.8 ms                                                | 95.9 ms: 1.22x slower                                                |
| async_generators           | 374 ms                                                 | 462 ms: 1.24x slower                                                 |
| mypy2                      | 686 ms                                                 | 881 ms: 1.29x slower                                                 |
| python_startup             | 8.56 ms                                                | 12.1 ms: 1.42x slower                                                |
| dask                       | 365 ms                                                 | 530 ms: 1.45x slower                                                 |
| python_startup_no_site     | 6.01 ms                                                | 10.7 ms: 1.78x slower                                                |
| unpack_sequence            | 43.5 ns                                                | 92.1 ns: 2.12x slower                                                |
| Geometric mean             | (ref)                                                  | 1.04x faster                                                         |

Benchmark hidden because not significant (4): djangocms, pprint_safe_repr, scimark_monte_carlo, pprint_pformat
Ignored benchmarks (3) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 98.43% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.24x