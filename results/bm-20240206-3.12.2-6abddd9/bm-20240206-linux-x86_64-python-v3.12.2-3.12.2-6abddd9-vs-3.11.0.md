
# Results vs. 3.11.0

- fork: python
- ref: v3.12.2
- machine: linux-x86_64
- commit hash: 6abddd9
- commit date: 2024-02-06
- overall geometric mean: 1.04x faster \*
- HPT reliability: 78.27%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-linux-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 272 ms: 1.03x slower                                   |
| chameleon      | 6.70 ms                                                | 7.26 ms: 1.08x slower                                  |
| docutils       | 2.66 sec                                               | 2.71 sec: 1.02x slower                                 |
| tornado_http   | 98.1 ms                                                | 99.4 ms: 1.01x slower                                  |
| Geometric mean | (ref)                                                  | 1.04x slower                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-linux-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_io              | 1.29 sec                                               | 1.15 sec: 1.12x faster                                 |
| async_tree_none            | 528 ms                                                 | 474 ms: 1.11x faster                                   |
| async_tree_memoization     | 639 ms                                                 | 576 ms: 1.11x faster                                   |
| async_tree_none_tg         | 491 ms                                                 | 446 ms: 1.10x faster                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.18 sec: 1.09x faster                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 573 ms: 1.09x faster                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 727 ms: 1.05x faster                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 727 ms: 1.03x faster                                   |
| Geometric mean             | (ref)                                                  | 1.09x faster                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-linux-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                   |
| nbody          | 96.0 ms                                                | 94.5 ms: 1.02x faster                                  |
| float          | 78.9 ms                                                | 84.1 ms: 1.06x slower                                  |
| Geometric mean | (ref)                                                  | 1.00x slower                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-linux-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_v8       | 22.9 ms                                                | 23.0 ms: 1.00x slower                                  |
| regex_compile  | 141 ms                                                 | 144 ms: 1.02x slower                                   |
| regex_dna      | 205 ms                                                 | 214 ms: 1.05x slower                                   |
| regex_effbot   | 3.51 ms                                                | 3.89 ms: 1.11x slower                                  |
| Geometric mean | (ref)                                                  | 1.04x slower                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-linux-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.28x faster                                  |
| unpickle_pure_python | 242 us                                                 | 228 us: 1.06x faster                                   |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                   |
| json_loads           | 29.2 us                                                | 28.1 us: 1.04x faster                                  |
| pickle_dict          | 34.6 us                                                | 33.4 us: 1.04x faster                                  |
| xml_etree_iterparse  | 108 ms                                                 | 106 ms: 1.02x faster                                   |
| pickle               | 11.0 us                                                | 11.3 us: 1.03x slower                                  |
| unpickle_list        | 5.21 us                                                | 5.36 us: 1.03x slower                                  |
| pickle_list          | 4.59 us                                                | 4.89 us: 1.07x slower                                  |
| xml_etree_process    | 56.9 ms                                                | 61.2 ms: 1.08x slower                                  |
| xml_etree_generate   | 81.1 ms                                                | 88.0 ms: 1.09x slower                                  |
| unpickle             | 13.8 us                                                | 15.3 us: 1.11x slower                                  |
| Geometric mean       | (ref)                                                  | 1.00x faster                                           |

Benchmark hidden because not significant (2): tomli_loads, pickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-linux-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 9.45 ms: 1.10x slower                                  |
| python_startup_no_site | 6.01 ms                                                | 6.80 ms: 1.13x slower                                  |
| Geometric mean         | (ref)                                                  | 1.12x slower                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-linux-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| django_template | 33.5 ms                                                | 34.8 ms: 1.04x slower                                  |
| mako            | 10.7 ms                                                | 11.7 ms: 1.10x slower                                  |
| Geometric mean  | (ref)                                                  | 1.07x slower                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-linux-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 123 us: 4.24x faster                                   |
| generators                 | 74.9 ms                                                | 32.3 ms: 2.32x faster                                  |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.73x faster                                 |
| asyncio_tcp                | 875 ms                                                 | 509 ms: 1.72x faster                                   |
| json_dumps                 | 13.3 ms                                                | 10.4 ms: 1.28x faster                                  |
| richards_super             | 61.9 ms                                                | 50.4 ms: 1.23x faster                                  |
| coroutines                 | 27.0 ms                                                | 23.5 ms: 1.15x faster                                  |
| gc_traversal               | 4.01 ms                                                | 3.54 ms: 1.13x faster                                  |
| comprehensions             | 23.6 us                                                | 21.0 us: 1.12x faster                                  |
| async_tree_io              | 1.29 sec                                               | 1.15 sec: 1.12x faster                                 |
| async_tree_none            | 528 ms                                                 | 474 ms: 1.11x faster                                   |
| async_tree_memoization     | 639 ms                                                 | 576 ms: 1.11x faster                                   |
| richards                   | 49.8 ms                                                | 45.2 ms: 1.10x faster                                  |
| async_tree_none_tg         | 491 ms                                                 | 446 ms: 1.10x faster                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.18 sec: 1.09x faster                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 573 ms: 1.09x faster                                   |
| chaos                      | 71.9 ms                                                | 66.3 ms: 1.08x faster                                  |
| deltablue                  | 3.92 ms                                                | 3.64 ms: 1.08x faster                                  |
| coverage                   | 78.8 ms                                                | 73.3 ms: 1.07x faster                                  |
| hexiom                     | 6.89 ms                                                | 6.44 ms: 1.07x faster                                  |
| unpickle_pure_python       | 242 us                                                 | 228 us: 1.06x faster                                   |
| logging_silent             | 111 ns                                                 | 105 ns: 1.06x faster                                   |
| nqueens                    | 87.9 ms                                                | 83.7 ms: 1.05x faster                                  |
| sqlglot_parse              | 1.43 ms                                                | 1.37 ms: 1.05x faster                                  |
| go                         | 149 ms                                                 | 142 ms: 1.05x faster                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 727 ms: 1.05x faster                                   |
| xml_etree_parse            | 164 ms                                                 | 158 ms: 1.04x faster                                   |
| json_loads                 | 29.2 us                                                | 28.1 us: 1.04x faster                                  |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                   |
| sqlglot_transpile          | 1.75 ms                                                | 1.69 ms: 1.04x faster                                  |
| pickle_dict                | 34.6 us                                                | 33.4 us: 1.04x faster                                  |
| sympy_sum                  | 169 ms                                                 | 163 ms: 1.03x faster                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 727 ms: 1.03x faster                                   |
| sympy_integrate            | 21.5 ms                                                | 20.8 ms: 1.03x faster                                  |
| xml_etree_iterparse        | 108 ms                                                 | 106 ms: 1.02x faster                                   |
| sympy_expand               | 484 ms                                                 | 477 ms: 1.02x faster                                   |
| nbody                      | 96.0 ms                                                | 94.5 ms: 1.02x faster                                  |
| sympy_str                  | 297 ms                                                 | 294 ms: 1.01x faster                                   |
| deepcopy_memo              | 40.2 us                                                | 39.7 us: 1.01x faster                                  |
| sqlglot_normalize          | 113 ms                                                 | 112 ms: 1.01x faster                                   |
| mdp                        | 2.77 sec                                               | 2.76 sec: 1.01x faster                                 |
| sqlglot_optimize           | 55.3 ms                                                | 55.0 ms: 1.01x faster                                  |
| deepcopy                   | 365 us                                                 | 364 us: 1.00x faster                                   |
| raytrace                   | 309 ms                                                 | 308 ms: 1.00x faster                                   |
| regex_v8                   | 22.9 ms                                                | 23.0 ms: 1.00x slower                                  |
| bench_thread_pool          | 834 us                                                 | 839 us: 1.01x slower                                   |
| deepcopy_reduce            | 3.22 us                                                | 3.24 us: 1.01x slower                                  |
| mypy2                      | 686 ms                                                 | 692 ms: 1.01x slower                                   |
| tornado_http               | 98.1 ms                                                | 99.4 ms: 1.01x slower                                  |
| pathlib                    | 18.5 ms                                                | 18.8 ms: 1.02x slower                                  |
| docutils                   | 2.66 sec                                               | 2.71 sec: 1.02x slower                                 |
| aiohttp                    | 1.12 ms                                                | 1.14 ms: 1.02x slower                                  |
| create_gc_cycles           | 1.43 ms                                                | 1.46 ms: 1.02x slower                                  |
| regex_compile              | 141 ms                                                 | 144 ms: 1.02x slower                                   |
| pprint_safe_repr           | 747 ms                                                 | 765 ms: 1.02x slower                                   |
| pickle                     | 11.0 us                                                | 11.3 us: 1.03x slower                                  |
| logging_simple             | 6.22 us                                                | 6.38 us: 1.03x slower                                  |
| meteor_contest             | 109 ms                                                 | 112 ms: 1.03x slower                                   |
| unpickle_list              | 5.21 us                                                | 5.36 us: 1.03x slower                                  |
| 2to3                       | 264 ms                                                 | 272 ms: 1.03x slower                                   |
| pycparser                  | 1.19 sec                                               | 1.22 sec: 1.03x slower                                 |
| gunicorn                   | 1.20 ms                                                | 1.24 ms: 1.03x slower                                  |
| scimark_lu                 | 116 ms                                                 | 120 ms: 1.03x slower                                   |
| fannkuch                   | 405 ms                                                 | 420 ms: 1.04x slower                                   |
| sqlalchemy_declarative     | 140 ms                                                 | 146 ms: 1.04x slower                                   |
| django_template            | 33.5 ms                                                | 34.8 ms: 1.04x slower                                  |
| telco                      | 6.86 ms                                                | 7.13 ms: 1.04x slower                                  |
| scimark_monte_carlo        | 70.7 ms                                                | 73.9 ms: 1.04x slower                                  |
| regex_dna                  | 205 ms                                                 | 214 ms: 1.05x slower                                   |
| logging_format             | 6.81 us                                                | 7.12 us: 1.05x slower                                  |
| dulwich_log                | 64.6 ms                                                | 67.9 ms: 1.05x slower                                  |
| crypto_pyaes               | 76.7 ms                                                | 80.9 ms: 1.05x slower                                  |
| spectral_norm              | 108 ms                                                 | 114 ms: 1.06x slower                                   |
| scimark_sor                | 121 ms                                                 | 129 ms: 1.06x slower                                   |
| float                      | 78.9 ms                                                | 84.1 ms: 1.06x slower                                  |
| pickle_list                | 4.59 us                                                | 4.89 us: 1.07x slower                                  |
| xml_etree_process          | 56.9 ms                                                | 61.2 ms: 1.08x slower                                  |
| chameleon                  | 6.70 ms                                                | 7.26 ms: 1.08x slower                                  |
| xml_etree_generate         | 81.1 ms                                                | 88.0 ms: 1.09x slower                                  |
| unpack_sequence            | 43.5 ns                                                | 47.6 ns: 1.10x slower                                  |
| mako                       | 10.7 ms                                                | 11.7 ms: 1.10x slower                                  |
| pyflate                    | 434 ms                                                 | 477 ms: 1.10x slower                                   |
| python_startup             | 8.56 ms                                                | 9.45 ms: 1.10x slower                                  |
| unpickle                   | 13.8 us                                                | 15.3 us: 1.11x slower                                  |
| scimark_fft                | 345 ms                                                 | 383 ms: 1.11x slower                                   |
| regex_effbot               | 3.51 ms                                                | 3.89 ms: 1.11x slower                                  |
| sqlite_synth               | 2.57 us                                                | 2.86 us: 1.11x slower                                  |
| python_startup_no_site     | 6.01 ms                                                | 6.80 ms: 1.13x slower                                  |
| async_generators           | 374 ms                                                 | 453 ms: 1.21x slower                                   |
| Geometric mean             | (ref)                                                  | 1.04x faster                                           |

Benchmark hidden because not significant (9): tomli_loads, json, pickle_pure_python, bench_mp_pool, pprint_pformat, asyncio_websockets, sqlalchemy_imperative, dask, scimark_sparse_mat_mult
Ignored benchmarks (7) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: djangocms, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 78.27% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.02x