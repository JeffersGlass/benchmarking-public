
# Results vs. 3.12.0

- fork: python
- ref: v3.11.7
- machine: linux-x86_64
- commit hash: fa7a6f2
- commit date: 2023-12-04
- overall geometric mean: 1.01x slower
- HPT reliability: 92.51%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.95x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 261 ms: 1.05x faster                                   |
| chameleon      | 7.41 ms                                                | 7.03 ms: 1.05x faster                                  |
| docutils       | 2.77 sec                                               | 2.59 sec: 1.07x faster                                 |
| tornado_http   | 103 ms                                                 | 96.6 ms: 1.06x faster                                  |
| Geometric mean | (ref)                                                  | 1.06x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 748 ms: 1.03x slower                                   |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 750 ms: 1.03x slower                                   |
| async_tree_none_tg         | 450 ms                                                 | 479 ms: 1.06x slower                                   |
| async_tree_memoization_tg  | 575 ms                                                 | 614 ms: 1.07x slower                                   |
| async_tree_io_tg           | 1.18 sec                                               | 1.29 sec: 1.09x slower                                 |
| async_tree_memoization     | 578 ms                                                 | 650 ms: 1.12x slower                                   |
| async_tree_none            | 472 ms                                                 | 533 ms: 1.13x slower                                   |
| async_tree_io              | 1.16 sec                                               | 1.31 sec: 1.13x slower                                 |
| Geometric mean             | (ref)                                                  | 1.08x slower                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| float          | 84.7 ms                                                | 79.1 ms: 1.07x faster                                  |
| nbody          | 97.0 ms                                                | 93.5 ms: 1.04x faster                                  |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x faster                                   |
| Geometric mean | (ref)                                                  | 1.04x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 137 ms: 1.08x faster                                   |
| regex_effbot   | 3.61 ms                                                | 3.43 ms: 1.05x faster                                  |
| regex_dna      | 212 ms                                                 | 209 ms: 1.01x faster                                   |
| regex_v8       | 23.1 ms                                                | 22.9 ms: 1.01x faster                                  |
| Geometric mean | (ref)                                                  | 1.04x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| unpickle             | 15.9 us                                                | 14.1 us: 1.12x faster                                  |
| json_loads           | 28.5 us                                                | 25.8 us: 1.11x faster                                  |
| xml_etree_generate   | 89.2 ms                                                | 81.0 ms: 1.10x faster                                  |
| xml_etree_process    | 61.7 ms                                                | 56.6 ms: 1.09x faster                                  |
| pickle_list          | 5.08 us                                                | 4.69 us: 1.08x faster                                  |
| pickle               | 11.6 us                                                | 11.0 us: 1.05x faster                                  |
| pickle_pure_python   | 324 us                                                 | 317 us: 1.02x faster                                   |
| unpickle_list        | 5.29 us                                                | 5.23 us: 1.01x faster                                  |
| tomli_loads          | 2.33 sec                                               | 2.31 sec: 1.01x faster                                 |
| xml_etree_iterparse  | 107 ms                                                 | 108 ms: 1.01x slower                                   |
| pickle_dict          | 35.5 us                                                | 36.1 us: 1.02x slower                                  |
| xml_etree_parse      | 159 ms                                                 | 163 ms: 1.02x slower                                   |
| unpickle_pure_python | 230 us                                                 | 239 us: 1.04x slower                                   |
| json_dumps           | 10.4 ms                                                | 13.2 ms: 1.27x slower                                  |
| Geometric mean       | (ref)                                                  | 1.02x faster                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup_no_site | 6.94 ms                                                | 6.04 ms: 1.15x faster                                  |
| python_startup         | 9.55 ms                                                | 8.59 ms: 1.11x faster                                  |
| Geometric mean         | (ref)                                                  | 1.13x faster                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako            | 11.9 ms                                                | 11.1 ms: 1.07x faster                                  |
| django_template | 34.6 ms                                                | 34.0 ms: 1.02x faster                                  |
| Geometric mean  | (ref)                                                  | 1.04x faster                                           |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_generators           | 463 ms                                                 | 362 ms: 1.28x faster                                   |
| mypy2                      | 830 ms                                                 | 679 ms: 1.22x faster                                   |
| python_startup_no_site     | 6.94 ms                                                | 6.04 ms: 1.15x faster                                  |
| pyflate                    | 482 ms                                                 | 424 ms: 1.14x faster                                   |
| unpack_sequence            | 54.0 ns                                                | 47.9 ns: 1.13x faster                                  |
| unpickle                   | 15.9 us                                                | 14.1 us: 1.12x faster                                  |
| python_startup             | 9.55 ms                                                | 8.59 ms: 1.11x faster                                  |
| scimark_fft                | 382 ms                                                 | 345 ms: 1.11x faster                                   |
| json_loads                 | 28.5 us                                                | 25.8 us: 1.11x faster                                  |
| xml_etree_generate         | 89.2 ms                                                | 81.0 ms: 1.10x faster                                  |
| sqlite_synth               | 2.83 us                                                | 2.58 us: 1.10x faster                                  |
| xml_etree_process          | 61.7 ms                                                | 56.6 ms: 1.09x faster                                  |
| pickle_list                | 5.08 us                                                | 4.69 us: 1.08x faster                                  |
| regex_compile              | 148 ms                                                 | 137 ms: 1.08x faster                                   |
| deepcopy_reduce            | 3.35 us                                                | 3.10 us: 1.08x faster                                  |
| mako                       | 11.9 ms                                                | 11.1 ms: 1.07x faster                                  |
| crypto_pyaes               | 81.9 ms                                                | 76.3 ms: 1.07x faster                                  |
| float                      | 84.7 ms                                                | 79.1 ms: 1.07x faster                                  |
| logging_format             | 7.23 us                                                | 6.76 us: 1.07x faster                                  |
| docutils                   | 2.77 sec                                               | 2.59 sec: 1.07x faster                                 |
| spectral_norm              | 115 ms                                                 | 108 ms: 1.07x faster                                   |
| json                       | 5.26 ms                                                | 4.94 ms: 1.07x faster                                  |
| sqlalchemy_declarative     | 147 ms                                                 | 138 ms: 1.06x faster                                   |
| dulwich_log                | 68.5 ms                                                | 64.5 ms: 1.06x faster                                  |
| tornado_http               | 103 ms                                                 | 96.6 ms: 1.06x faster                                  |
| gunicorn                   | 1.24 ms                                                | 1.17 ms: 1.06x faster                                  |
| pprint_safe_repr           | 776 ms                                                 | 735 ms: 1.05x faster                                   |
| chameleon                  | 7.41 ms                                                | 7.03 ms: 1.05x faster                                  |
| pickle                     | 11.6 us                                                | 11.0 us: 1.05x faster                                  |
| regex_effbot               | 3.61 ms                                                | 3.43 ms: 1.05x faster                                  |
| pathlib                    | 19.3 ms                                                | 18.4 ms: 1.05x faster                                  |
| 2to3                       | 274 ms                                                 | 261 ms: 1.05x faster                                   |
| deepcopy                   | 371 us                                                 | 355 us: 1.05x faster                                   |
| scimark_sor                | 129 ms                                                 | 123 ms: 1.05x faster                                   |
| aiohttp                    | 1.15 ms                                                | 1.10 ms: 1.05x faster                                  |
| logging_simple             | 6.46 us                                                | 6.18 us: 1.05x faster                                  |
| telco                      | 7.10 ms                                                | 6.79 ms: 1.04x faster                                  |
| sqlalchemy_imperative      | 18.7 ms                                                | 17.9 ms: 1.04x faster                                  |
| fannkuch                   | 417 ms                                                 | 400 ms: 1.04x faster                                   |
| nbody                      | 97.0 ms                                                | 93.5 ms: 1.04x faster                                  |
| pycparser                  | 1.18 sec                                               | 1.14 sec: 1.04x faster                                 |
| meteor_contest             | 112 ms                                                 | 109 ms: 1.03x faster                                   |
| pprint_pformat             | 1.57 sec                                               | 1.52 sec: 1.03x faster                                 |
| scimark_monte_carlo        | 75.1 ms                                                | 72.8 ms: 1.03x faster                                  |
| sympy_integrate            | 21.4 ms                                                | 20.8 ms: 1.03x faster                                  |
| dask                       | 372 ms                                                 | 362 ms: 1.03x faster                                   |
| deepcopy_memo              | 40.7 us                                                | 39.8 us: 1.02x faster                                  |
| sympy_sum                  | 169 ms                                                 | 165 ms: 1.02x faster                                   |
| scimark_lu                 | 118 ms                                                 | 116 ms: 1.02x faster                                   |
| raytrace                   | 312 ms                                                 | 306 ms: 1.02x faster                                   |
| pickle_pure_python         | 324 us                                                 | 317 us: 1.02x faster                                   |
| django_template            | 34.6 ms                                                | 34.0 ms: 1.02x faster                                  |
| sympy_str                  | 300 ms                                                 | 295 ms: 1.02x faster                                   |
| create_gc_cycles           | 1.48 ms                                                | 1.45 ms: 1.02x faster                                  |
| gc_traversal               | 3.79 ms                                                | 3.74 ms: 1.01x faster                                  |
| bench_thread_pool          | 842 us                                                 | 831 us: 1.01x faster                                   |
| regex_dna                  | 212 ms                                                 | 209 ms: 1.01x faster                                   |
| regex_v8                   | 23.1 ms                                                | 22.9 ms: 1.01x faster                                  |
| unpickle_list              | 5.29 us                                                | 5.23 us: 1.01x faster                                  |
| tomli_loads                | 2.33 sec                                               | 2.31 sec: 1.01x faster                                 |
| pidigits                   | 187 ms                                                 | 187 ms: 1.00x faster                                   |
| sqlglot_optimize           | 54.8 ms                                                | 55.0 ms: 1.00x slower                                  |
| xml_etree_iterparse        | 107 ms                                                 | 108 ms: 1.01x slower                                   |
| logging_silent             | 104 ns                                                 | 106 ns: 1.02x slower                                   |
| pickle_dict                | 35.5 us                                                | 36.1 us: 1.02x slower                                  |
| sqlglot_normalize          | 110 ms                                                 | 112 ms: 1.02x slower                                   |
| deltablue                  | 3.72 ms                                                | 3.79 ms: 1.02x slower                                  |
| sqlglot_transpile          | 1.68 ms                                                | 1.72 ms: 1.02x slower                                  |
| xml_etree_parse            | 159 ms                                                 | 163 ms: 1.02x slower                                   |
| nqueens                    | 83.3 ms                                                | 85.2 ms: 1.02x slower                                  |
| go                         | 139 ms                                                 | 143 ms: 1.03x slower                                   |
| mdp                        | 2.63 sec                                               | 2.71 sec: 1.03x slower                                 |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 748 ms: 1.03x slower                                   |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 750 ms: 1.03x slower                                   |
| sympy_expand               | 478 ms                                                 | 495 ms: 1.04x slower                                   |
| richards                   | 45.8 ms                                                | 47.6 ms: 1.04x slower                                  |
| sqlglot_parse              | 1.36 ms                                                | 1.42 ms: 1.04x slower                                  |
| unpickle_pure_python       | 230 us                                                 | 239 us: 1.04x slower                                   |
| hexiom                     | 6.41 ms                                                | 6.77 ms: 1.06x slower                                  |
| chaos                      | 67.0 ms                                                | 70.8 ms: 1.06x slower                                  |
| comprehensions             | 21.8 us                                                | 23.1 us: 1.06x slower                                  |
| async_tree_none_tg         | 450 ms                                                 | 479 ms: 1.06x slower                                   |
| async_tree_memoization_tg  | 575 ms                                                 | 614 ms: 1.07x slower                                   |
| async_tree_io_tg           | 1.18 sec                                               | 1.29 sec: 1.09x slower                                 |
| coverage                   | 72.7 ms                                                | 79.5 ms: 1.09x slower                                  |
| async_tree_memoization     | 578 ms                                                 | 650 ms: 1.12x slower                                   |
| async_tree_none            | 472 ms                                                 | 533 ms: 1.13x slower                                   |
| async_tree_io              | 1.16 sec                                               | 1.31 sec: 1.13x slower                                 |
| coroutines                 | 23.2 ms                                                | 26.4 ms: 1.14x slower                                  |
| richards_super             | 51.5 ms                                                | 59.5 ms: 1.16x slower                                  |
| json_dumps                 | 10.4 ms                                                | 13.2 ms: 1.27x slower                                  |
| asyncio_tcp_ssl            | 1.79 sec                                               | 3.10 sec: 1.74x slower                                 |
| asyncio_tcp                | 491 ms                                                 | 880 ms: 1.79x slower                                   |
| generators                 | 31.2 ms                                                | 75.5 ms: 2.42x slower                                  |
| typing_runtime_protocols   | 158 us                                                 | 512 us: 3.25x slower                                   |
| Geometric mean             | (ref)                                                  | 1.01x slower                                           |

Benchmark hidden because not significant (3): asyncio_websockets, bench_mp_pool, scimark_sparse_mat_mult
Ignored benchmarks (7) of results/bm-20231204-3.11.7-fa7a6f2/bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2.json: djangocms, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 92.51% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.95x