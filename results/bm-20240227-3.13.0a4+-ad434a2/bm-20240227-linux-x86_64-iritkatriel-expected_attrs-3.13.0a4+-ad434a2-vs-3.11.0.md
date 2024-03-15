
# Results vs. 3.11.0

- fork: iritkatriel
- ref: expected_attrs
- machine: linux-x86_64
- commit hash: ad434a2
- commit date: 2024-02-27
- overall geometric mean: 1.08x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 262 ms: 1.01x faster                                                  |
| chameleon      | 6.70 ms                                                | 6.64 ms: 1.01x faster                                                 |
| docutils       | 2.66 sec                                               | 2.57 sec: 1.03x faster                                                |
| tornado_http   | 98.1 ms                                                | 94.6 ms: 1.04x faster                                                 |
| Geometric mean | (ref)                                                  | 1.02x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 431 ms: 1.22x faster                                                  |
| async_tree_memoization     | 639 ms                                                 | 555 ms: 1.15x faster                                                  |
| async_tree_none_tg         | 491 ms                                                 | 441 ms: 1.11x faster                                                  |
| async_tree_memoization_tg  | 626 ms                                                 | 567 ms: 1.11x faster                                                  |
| async_tree_io              | 1.29 sec                                               | 1.17 sec: 1.10x faster                                                |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                                |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 702 ms: 1.07x faster                                                  |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 718 ms: 1.06x faster                                                  |
| Geometric mean             | (ref)                                                  | 1.11x faster                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 88.2 ms: 1.09x faster                                                 |
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                                  |
| float          | 78.9 ms                                                | 80.6 ms: 1.02x slower                                                 |
| Geometric mean | (ref)                                                  | 1.03x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 131 ms: 1.08x faster                                                  |
| regex_effbot   | 3.51 ms                                                | 3.81 ms: 1.09x slower                                                 |
| regex_dna      | 205 ms                                                 | 224 ms: 1.09x slower                                                  |
| regex_v8       | 22.9 ms                                                | 26.3 ms: 1.15x slower                                                 |
| Geometric mean | (ref)                                                  | 1.06x slower                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                 |
| unpickle_pure_python | 242 us                                                 | 210 us: 1.15x faster                                                  |
| pickle_pure_python   | 320 us                                                 | 292 us: 1.10x faster                                                  |
| tomli_loads          | 2.30 sec                                               | 2.14 sec: 1.08x faster                                                |
| unpickle_list        | 5.21 us                                                | 4.90 us: 1.06x faster                                                 |
| json_loads           | 29.2 us                                                | 27.5 us: 1.06x faster                                                 |
| xml_etree_parse      | 164 ms                                                 | 156 ms: 1.05x faster                                                  |
| xml_etree_iterparse  | 108 ms                                                 | 103 ms: 1.05x faster                                                  |
| pickle_dict          | 34.6 us                                                | 33.6 us: 1.03x faster                                                 |
| xml_etree_process    | 56.9 ms                                                | 57.6 ms: 1.01x slower                                                 |
| pickle               | 11.0 us                                                | 11.4 us: 1.03x slower                                                 |
| xml_etree_generate   | 81.1 ms                                                | 84.0 ms: 1.04x slower                                                 |
| pickle_list          | 4.59 us                                                | 4.82 us: 1.05x slower                                                 |
| unpickle             | 13.8 us                                                | 15.0 us: 1.09x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.04x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                 |
| python_startup_no_site | 6.01 ms                                                | 8.76 ms: 1.46x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.31x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|-----------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 10.9 ms: 1.02x slower                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 109 us: 4.76x faster                                                  |
| generators                 | 74.9 ms                                                | 28.7 ms: 2.61x faster                                                 |
| asyncio_tcp                | 875 ms                                                 | 482 ms: 1.82x faster                                                  |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.78 sec: 1.75x faster                                                |
| comprehensions             | 23.6 us                                                | 16.3 us: 1.45x faster                                                 |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                 |
| deltablue                  | 3.92 ms                                                | 3.14 ms: 1.25x faster                                                 |
| coroutines                 | 27.0 ms                                                | 21.9 ms: 1.24x faster                                                 |
| chaos                      | 71.9 ms                                                | 58.5 ms: 1.23x faster                                                 |
| async_tree_none            | 528 ms                                                 | 431 ms: 1.22x faster                                                  |
| raytrace                   | 309 ms                                                 | 257 ms: 1.20x faster                                                  |
| hexiom                     | 6.89 ms                                                | 5.89 ms: 1.17x faster                                                 |
| richards_super             | 61.9 ms                                                | 53.2 ms: 1.16x faster                                                 |
| sympy_sum                  | 169 ms                                                 | 146 ms: 1.16x faster                                                  |
| sqlglot_parse              | 1.43 ms                                                | 1.24 ms: 1.15x faster                                                 |
| unpickle_pure_python       | 242 us                                                 | 210 us: 1.15x faster                                                  |
| async_tree_memoization     | 639 ms                                                 | 555 ms: 1.15x faster                                                  |
| logging_silent             | 111 ns                                                 | 98.1 ns: 1.13x faster                                                 |
| sqlglot_transpile          | 1.75 ms                                                | 1.55 ms: 1.13x faster                                                 |
| sympy_str                  | 297 ms                                                 | 264 ms: 1.12x faster                                                  |
| async_tree_none_tg         | 491 ms                                                 | 441 ms: 1.11x faster                                                  |
| crypto_pyaes               | 76.7 ms                                                | 69.0 ms: 1.11x faster                                                 |
| sympy_integrate            | 21.5 ms                                                | 19.3 ms: 1.11x faster                                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 567 ms: 1.11x faster                                                  |
| go                         | 149 ms                                                 | 135 ms: 1.10x faster                                                  |
| mdp                        | 2.77 sec                                               | 2.53 sec: 1.10x faster                                                |
| async_tree_io              | 1.29 sec                                               | 1.17 sec: 1.10x faster                                                |
| pickle_pure_python         | 320 us                                                 | 292 us: 1.10x faster                                                  |
| nqueens                    | 87.9 ms                                                | 80.3 ms: 1.09x faster                                                 |
| nbody                      | 96.0 ms                                                | 88.2 ms: 1.09x faster                                                 |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                                |
| regex_compile              | 141 ms                                                 | 131 ms: 1.08x faster                                                  |
| sympy_expand               | 484 ms                                                 | 448 ms: 1.08x faster                                                  |
| logging_simple             | 6.22 us                                                | 5.76 us: 1.08x faster                                                 |
| fannkuch                   | 405 ms                                                 | 376 ms: 1.08x faster                                                  |
| deepcopy_memo              | 40.2 us                                                | 37.3 us: 1.08x faster                                                 |
| tomli_loads                | 2.30 sec                                               | 2.14 sec: 1.08x faster                                                |
| logging_format             | 6.81 us                                                | 6.35 us: 1.07x faster                                                 |
| sqlglot_normalize          | 113 ms                                                 | 105 ms: 1.07x faster                                                  |
| deepcopy                   | 365 us                                                 | 341 us: 1.07x faster                                                  |
| scimark_monte_carlo        | 70.7 ms                                                | 66.2 ms: 1.07x faster                                                 |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 702 ms: 1.07x faster                                                  |
| deepcopy_reduce            | 3.22 us                                                | 3.01 us: 1.07x faster                                                 |
| unpickle_list              | 5.21 us                                                | 4.90 us: 1.06x faster                                                 |
| pprint_pformat             | 1.55 sec                                               | 1.46 sec: 1.06x faster                                                |
| json_loads                 | 29.2 us                                                | 27.5 us: 1.06x faster                                                 |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 718 ms: 1.06x faster                                                  |
| richards                   | 49.8 ms                                                | 47.2 ms: 1.06x faster                                                 |
| sqlglot_optimize           | 55.3 ms                                                | 52.7 ms: 1.05x faster                                                 |
| xml_etree_parse            | 164 ms                                                 | 156 ms: 1.05x faster                                                  |
| pprint_safe_repr           | 747 ms                                                 | 713 ms: 1.05x faster                                                  |
| xml_etree_iterparse        | 108 ms                                                 | 103 ms: 1.05x faster                                                  |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.82 ms: 1.04x faster                                                 |
| scimark_lu                 | 116 ms                                                 | 112 ms: 1.04x faster                                                  |
| gc_traversal               | 4.01 ms                                                | 3.84 ms: 1.04x faster                                                 |
| scimark_sor                | 121 ms                                                 | 116 ms: 1.04x faster                                                  |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                                  |
| tornado_http               | 98.1 ms                                                | 94.6 ms: 1.04x faster                                                 |
| pathlib                    | 18.5 ms                                                | 17.9 ms: 1.04x faster                                                 |
| docutils                   | 2.66 sec                                               | 2.57 sec: 1.03x faster                                                |
| spectral_norm              | 108 ms                                                 | 105 ms: 1.03x faster                                                  |
| json                       | 5.24 ms                                                | 5.08 ms: 1.03x faster                                                 |
| pickle_dict                | 34.6 us                                                | 33.6 us: 1.03x faster                                                 |
| bench_thread_pool          | 834 us                                                 | 813 us: 1.03x faster                                                  |
| meteor_contest             | 109 ms                                                 | 106 ms: 1.03x faster                                                  |
| pycparser                  | 1.19 sec                                               | 1.16 sec: 1.02x faster                                                |
| unpack_sequence            | 43.5 ns                                                | 42.9 ns: 1.01x faster                                                 |
| 2to3                       | 264 ms                                                 | 262 ms: 1.01x faster                                                  |
| chameleon                  | 6.70 ms                                                | 6.64 ms: 1.01x faster                                                 |
| dulwich_log                | 64.6 ms                                                | 65.1 ms: 1.01x slower                                                 |
| xml_etree_process          | 56.9 ms                                                | 57.6 ms: 1.01x slower                                                 |
| pyflate                    | 434 ms                                                 | 439 ms: 1.01x slower                                                  |
| float                      | 78.9 ms                                                | 80.6 ms: 1.02x slower                                                 |
| mako                       | 10.7 ms                                                | 10.9 ms: 1.02x slower                                                 |
| scimark_fft                | 345 ms                                                 | 357 ms: 1.03x slower                                                  |
| pickle                     | 11.0 us                                                | 11.4 us: 1.03x slower                                                 |
| xml_etree_generate         | 81.1 ms                                                | 84.0 ms: 1.04x slower                                                 |
| create_gc_cycles           | 1.43 ms                                                | 1.49 ms: 1.04x slower                                                 |
| pickle_list                | 4.59 us                                                | 4.82 us: 1.05x slower                                                 |
| unpickle                   | 13.8 us                                                | 15.0 us: 1.09x slower                                                 |
| regex_effbot               | 3.51 ms                                                | 3.81 ms: 1.09x slower                                                 |
| regex_dna                  | 205 ms                                                 | 224 ms: 1.09x slower                                                  |
| sqlite_synth               | 2.57 us                                                | 2.84 us: 1.11x slower                                                 |
| regex_v8                   | 22.9 ms                                                | 26.3 ms: 1.15x slower                                                 |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                 |
| async_generators           | 374 ms                                                 | 448 ms: 1.20x slower                                                  |
| telco                      | 6.86 ms                                                | 8.25 ms: 1.20x slower                                                 |
| coverage                   | 78.8 ms                                                | 95.2 ms: 1.21x slower                                                 |
| mypy2                      | 686 ms                                                 | 837 ms: 1.22x slower                                                  |
| python_startup_no_site     | 6.01 ms                                                | 8.76 ms: 1.46x slower                                                 |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                          |

Benchmark hidden because not significant (2): bench_mp_pool, asyncio_websockets
Ignored benchmarks (13) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.04x
- 95% likely to have a speedup of 1.04x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: 0.98x