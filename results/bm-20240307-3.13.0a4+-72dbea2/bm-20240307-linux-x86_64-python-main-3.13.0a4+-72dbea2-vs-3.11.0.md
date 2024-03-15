# Results vs. 3.11.0

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: 72dbea2
- commit date: 2024-03-07
- overall geometric mean: 1.07x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240307-linux-x86_64-python-main-3.13.0a4+-72dbea2 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 262 ms: 1.01x faster                                   |
| chameleon      | 6.70 ms                                                | 6.92 ms: 1.03x slower                                  |
| docutils       | 2.66 sec                                               | 2.63 sec: 1.01x faster                                 |
| html5lib       | 64.8 ms                                                | 66.1 ms: 1.02x slower                                  |
| tornado_http   | 98.1 ms                                                | 95.1 ms: 1.03x faster                                  |
| Geometric mean | (ref)                                                  | 1.00x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240307-linux-x86_64-python-main-3.13.0a4+-72dbea2 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 430 ms: 1.23x faster                                   |
| async_tree_memoization     | 639 ms                                                 | 554 ms: 1.15x faster                                   |
| async_tree_memoization_tg  | 626 ms                                                 | 562 ms: 1.11x faster                                   |
| async_tree_none_tg         | 491 ms                                                 | 443 ms: 1.11x faster                                   |
| async_tree_io              | 1.29 sec                                               | 1.17 sec: 1.10x faster                                 |
| async_tree_io_tg           | 1.29 sec                                               | 1.18 sec: 1.09x faster                                 |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 703 ms: 1.07x faster                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 718 ms: 1.06x faster                                   |
| Geometric mean             | (ref)                                                  | 1.11x faster                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240307-linux-x86_64-python-main-3.13.0a4+-72dbea2 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 92.0 ms: 1.04x faster                                  |
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                   |
| float          | 78.9 ms                                                | 80.4 ms: 1.02x slower                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240307-linux-x86_64-python-main-3.13.0a4+-72dbea2 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 131 ms: 1.08x faster                                   |
| regex_effbot   | 3.51 ms                                                | 3.54 ms: 1.01x slower                                  |
| regex_dna      | 205 ms                                                 | 217 ms: 1.06x slower                                   |
| regex_v8       | 22.9 ms                                                | 25.2 ms: 1.10x slower                                  |
| Geometric mean | (ref)                                                  | 1.02x slower                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240307-linux-x86_64-python-main-3.13.0a4+-72dbea2 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.29x faster                                  |
| unpickle_pure_python | 242 us                                                 | 214 us: 1.13x faster                                   |
| pickle_pure_python   | 320 us                                                 | 296 us: 1.08x faster                                   |
| tomli_loads          | 2.30 sec                                               | 2.16 sec: 1.07x faster                                 |
| xml_etree_parse      | 164 ms                                                 | 156 ms: 1.05x faster                                   |
| json_loads           | 29.2 us                                                | 28.0 us: 1.04x faster                                  |
| unpickle_list        | 5.21 us                                                | 5.02 us: 1.04x faster                                  |
| xml_etree_iterparse  | 108 ms                                                 | 104 ms: 1.04x faster                                   |
| xml_etree_process    | 56.9 ms                                                | 57.8 ms: 1.02x slower                                  |
| pickle_dict          | 34.6 us                                                | 35.9 us: 1.04x slower                                  |
| xml_etree_generate   | 81.1 ms                                                | 84.4 ms: 1.04x slower                                  |
| pickle               | 11.0 us                                                | 11.5 us: 1.05x slower                                  |
| unpickle             | 13.8 us                                                | 14.6 us: 1.05x slower                                  |
| pickle_list          | 4.59 us                                                | 5.10 us: 1.11x slower                                  |
| Geometric mean       | (ref)                                                  | 1.03x faster                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240307-linux-x86_64-python-main-3.13.0a4+-72dbea2 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                  |
| python_startup_no_site | 6.01 ms                                                | 8.72 ms: 1.45x slower                                  |
| Geometric mean         | (ref)                                                  | 1.31x slower                                           |

Benchmarks with tag 'template':
===============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240307-linux-x86_64-python-main-3.13.0a4+-72dbea2 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| genshi_xml     | 53.4 ms                                                | 50.7 ms: 1.05x faster                                  |
| genshi_text    | 22.5 ms                                                | 23.0 ms: 1.02x slower                                  |
| mako           | 10.7 ms                                                | 11.1 ms: 1.04x slower                                  |
| Geometric mean | (ref)                                                  | 1.00x slower                                           |

Benchmark hidden because not significant (1): django_template

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240307-linux-x86_64-python-main-3.13.0a4+-72dbea2 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 110 us: 4.72x faster                                   |
| generators                 | 74.9 ms                                                | 29.9 ms: 2.50x faster                                  |
| asyncio_tcp                | 875 ms                                                 | 484 ms: 1.81x faster                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.78 sec: 1.75x faster                                 |
| pylint                     | 476 ms                                                 | 306 ms: 1.56x faster                                   |
| comprehensions             | 23.6 us                                                | 15.8 us: 1.50x faster                                  |
| json_dumps                 | 13.3 ms                                                | 10.4 ms: 1.29x faster                                  |
| deltablue                  | 3.92 ms                                                | 3.15 ms: 1.24x faster                                  |
| coroutines                 | 27.0 ms                                                | 21.9 ms: 1.23x faster                                  |
| async_tree_none            | 528 ms                                                 | 430 ms: 1.23x faster                                   |
| richards_super             | 61.9 ms                                                | 50.7 ms: 1.22x faster                                  |
| chaos                      | 71.9 ms                                                | 59.6 ms: 1.21x faster                                  |
| raytrace                   | 309 ms                                                 | 262 ms: 1.18x faster                                   |
| async_tree_memoization     | 639 ms                                                 | 554 ms: 1.15x faster                                   |
| sqlglot_parse              | 1.43 ms                                                | 1.24 ms: 1.15x faster                                  |
| sympy_sum                  | 169 ms                                                 | 147 ms: 1.15x faster                                   |
| hexiom                     | 6.89 ms                                                | 6.04 ms: 1.14x faster                                  |
| unpickle_pure_python       | 242 us                                                 | 214 us: 1.13x faster                                   |
| sqlglot_transpile          | 1.75 ms                                                | 1.56 ms: 1.12x faster                                  |
| sympy_str                  | 297 ms                                                 | 265 ms: 1.12x faster                                   |
| richards                   | 49.8 ms                                                | 44.5 ms: 1.12x faster                                  |
| logging_simple             | 6.22 us                                                | 5.58 us: 1.11x faster                                  |
| async_tree_memoization_tg  | 626 ms                                                 | 562 ms: 1.11x faster                                   |
| mdp                        | 2.77 sec                                               | 2.49 sec: 1.11x faster                                 |
| logging_silent             | 111 ns                                                 | 100 ns: 1.11x faster                                   |
| async_tree_none_tg         | 491 ms                                                 | 443 ms: 1.11x faster                                   |
| logging_format             | 6.81 us                                                | 6.15 us: 1.11x faster                                  |
| async_tree_io              | 1.29 sec                                               | 1.17 sec: 1.10x faster                                 |
| sympy_integrate            | 21.5 ms                                                | 19.5 ms: 1.10x faster                                  |
| nqueens                    | 87.9 ms                                                | 80.1 ms: 1.10x faster                                  |
| async_tree_io_tg           | 1.29 sec                                               | 1.18 sec: 1.09x faster                                 |
| go                         | 149 ms                                                 | 136 ms: 1.09x faster                                   |
| gc_traversal               | 4.01 ms                                                | 3.67 ms: 1.09x faster                                  |
| sqlglot_normalize          | 113 ms                                                 | 104 ms: 1.08x faster                                   |
| pickle_pure_python         | 320 us                                                 | 296 us: 1.08x faster                                   |
| sympy_expand               | 484 ms                                                 | 450 ms: 1.08x faster                                   |
| regex_compile              | 141 ms                                                 | 131 ms: 1.08x faster                                   |
| scimark_monte_carlo        | 70.7 ms                                                | 65.9 ms: 1.07x faster                                  |
| crypto_pyaes               | 76.7 ms                                                | 71.7 ms: 1.07x faster                                  |
| tomli_loads                | 2.30 sec                                               | 2.16 sec: 1.07x faster                                 |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 703 ms: 1.07x faster                                   |
| deepcopy                   | 365 us                                                 | 344 us: 1.06x faster                                   |
| deepcopy_reduce            | 3.22 us                                                | 3.03 us: 1.06x faster                                  |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 718 ms: 1.06x faster                                   |
| genshi_xml                 | 53.4 ms                                                | 50.7 ms: 1.05x faster                                  |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.78 ms: 1.05x faster                                  |
| deepcopy_memo              | 40.2 us                                                | 38.2 us: 1.05x faster                                  |
| xml_etree_parse            | 164 ms                                                 | 156 ms: 1.05x faster                                   |
| scimark_sor                | 121 ms                                                 | 116 ms: 1.05x faster                                   |
| sqlglot_optimize           | 55.3 ms                                                | 52.9 ms: 1.05x faster                                  |
| pprint_pformat             | 1.55 sec                                               | 1.49 sec: 1.04x faster                                 |
| nbody                      | 96.0 ms                                                | 92.0 ms: 1.04x faster                                  |
| djangocms                  | 33.5 us                                                | 32.2 us: 1.04x faster                                  |
| json_loads                 | 29.2 us                                                | 28.0 us: 1.04x faster                                  |
| unpickle_list              | 5.21 us                                                | 5.02 us: 1.04x faster                                  |
| xml_etree_iterparse        | 108 ms                                                 | 104 ms: 1.04x faster                                   |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                   |
| scimark_lu                 | 116 ms                                                 | 112 ms: 1.04x faster                                   |
| meteor_contest             | 109 ms                                                 | 105 ms: 1.04x faster                                   |
| fannkuch                   | 405 ms                                                 | 391 ms: 1.04x faster                                   |
| tornado_http               | 98.1 ms                                                | 95.1 ms: 1.03x faster                                  |
| pprint_safe_repr           | 747 ms                                                 | 725 ms: 1.03x faster                                   |
| json                       | 5.24 ms                                                | 5.13 ms: 1.02x faster                                  |
| thrift                     | 784 us                                                 | 771 us: 1.02x faster                                   |
| pathlib                    | 18.5 ms                                                | 18.2 ms: 1.02x faster                                  |
| bench_thread_pool          | 834 us                                                 | 823 us: 1.01x faster                                   |
| docutils                   | 2.66 sec                                               | 2.63 sec: 1.01x faster                                 |
| 2to3                       | 264 ms                                                 | 262 ms: 1.01x faster                                   |
| regex_effbot               | 3.51 ms                                                | 3.54 ms: 1.01x slower                                  |
| dulwich_log                | 64.6 ms                                                | 65.4 ms: 1.01x slower                                  |
| spectral_norm              | 108 ms                                                 | 110 ms: 1.02x slower                                   |
| xml_etree_process          | 56.9 ms                                                | 57.8 ms: 1.02x slower                                  |
| float                      | 78.9 ms                                                | 80.4 ms: 1.02x slower                                  |
| html5lib                   | 64.8 ms                                                | 66.1 ms: 1.02x slower                                  |
| aiohttp                    | 1.12 ms                                                | 1.14 ms: 1.02x slower                                  |
| genshi_text                | 22.5 ms                                                | 23.0 ms: 1.02x slower                                  |
| unpack_sequence            | 43.5 ns                                                | 44.7 ns: 1.03x slower                                  |
| chameleon                  | 6.70 ms                                                | 6.92 ms: 1.03x slower                                  |
| create_gc_cycles           | 1.43 ms                                                | 1.49 ms: 1.04x slower                                  |
| pickle_dict                | 34.6 us                                                | 35.9 us: 1.04x slower                                  |
| gunicorn                   | 1.20 ms                                                | 1.25 ms: 1.04x slower                                  |
| xml_etree_generate         | 81.1 ms                                                | 84.4 ms: 1.04x slower                                  |
| mako                       | 10.7 ms                                                | 11.1 ms: 1.04x slower                                  |
| pickle                     | 11.0 us                                                | 11.5 us: 1.05x slower                                  |
| pyflate                    | 434 ms                                                 | 455 ms: 1.05x slower                                   |
| scimark_fft                | 345 ms                                                 | 364 ms: 1.05x slower                                   |
| unpickle                   | 13.8 us                                                | 14.6 us: 1.05x slower                                  |
| regex_dna                  | 205 ms                                                 | 217 ms: 1.06x slower                                   |
| regex_v8                   | 22.9 ms                                                | 25.2 ms: 1.10x slower                                  |
| pickle_list                | 4.59 us                                                | 5.10 us: 1.11x slower                                  |
| sqlite_synth               | 2.57 us                                                | 2.87 us: 1.12x slower                                  |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                  |
| async_generators           | 374 ms                                                 | 443 ms: 1.19x slower                                   |
| telco                      | 6.86 ms                                                | 8.28 ms: 1.21x slower                                  |
| coverage                   | 78.8 ms                                                | 95.7 ms: 1.22x slower                                  |
| mypy2                      | 686 ms                                                 | 841 ms: 1.23x slower                                   |
| dask                       | 365 ms                                                 | 519 ms: 1.42x slower                                   |
| python_startup_no_site     | 6.01 ms                                                | 8.72 ms: 1.45x slower                                  |
| Geometric mean             | (ref)                                                  | 1.07x faster                                           |

Benchmark hidden because not significant (4): bench_mp_pool, asyncio_websockets, pycparser, django_template
Ignored benchmarks (3) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 0.99x