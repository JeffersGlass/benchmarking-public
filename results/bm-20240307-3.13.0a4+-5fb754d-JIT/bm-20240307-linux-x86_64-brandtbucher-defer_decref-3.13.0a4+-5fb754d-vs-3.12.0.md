# Results vs. 3.12.0

- fork: brandtbucher
- ref: defer_decref
- machine: linux-x86_64
- commit hash: 5fb754d
- commit date: 2024-03-07
- overall geometric mean: 1.07x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x slower
- Memory change: 1.17x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 301 ms: 1.10x slower                                                 |
| chameleon      | 7.41 ms                                                | 7.48 ms: 1.01x slower                                                |
| docutils       | 2.77 sec                                               | 2.90 sec: 1.05x slower                                               |
| tornado_http   | 103 ms                                                 | 107 ms: 1.04x slower                                                 |
| Geometric mean | (ref)                                                  | 1.05x slower                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 459 ms: 1.03x faster                                                 |
| async_tree_memoization     | 578 ms                                                 | 591 ms: 1.02x slower                                                 |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 744 ms: 1.03x slower                                                 |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 755 ms: 1.04x slower                                                 |
| async_tree_none_tg         | 450 ms                                                 | 469 ms: 1.04x slower                                                 |
| async_tree_memoization_tg  | 575 ms                                                 | 601 ms: 1.05x slower                                                 |
| async_tree_io_tg           | 1.18 sec                                               | 1.25 sec: 1.06x slower                                               |
| async_tree_io              | 1.16 sec                                               | 1.23 sec: 1.07x slower                                               |
| Geometric mean             | (ref)                                                  | 1.03x slower                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 192 ms: 1.03x slower                                                 |
| nbody          | 97.0 ms                                                | 107 ms: 1.11x slower                                                 |
| Geometric mean | (ref)                                                  | 1.04x slower                                                         |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.68 ms: 1.02x slower                                                |
| regex_compile  | 148 ms                                                 | 156 ms: 1.05x slower                                                 |
| regex_dna      | 212 ms                                                 | 224 ms: 1.06x slower                                                 |
| regex_v8       | 23.1 ms                                                | 25.8 ms: 1.11x slower                                                |
| Geometric mean | (ref)                                                  | 1.06x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| unpickle_list        | 5.29 us                                                | 5.03 us: 1.05x faster                                                |
| unpickle             | 15.9 us                                                | 15.3 us: 1.04x faster                                                |
| pickle_dict          | 35.5 us                                                | 34.8 us: 1.02x faster                                                |
| json_loads           | 28.5 us                                                | 27.9 us: 1.02x faster                                                |
| pickle_list          | 5.08 us                                                | 5.00 us: 1.02x faster                                                |
| pickle               | 11.6 us                                                | 11.7 us: 1.01x slower                                                |
| tomli_loads          | 2.33 sec                                               | 2.35 sec: 1.01x slower                                               |
| xml_etree_generate   | 89.2 ms                                                | 90.2 ms: 1.01x slower                                                |
| pickle_pure_python   | 324 us                                                 | 336 us: 1.04x slower                                                 |
| xml_etree_process    | 61.7 ms                                                | 64.1 ms: 1.04x slower                                                |
| json_dumps           | 10.4 ms                                                | 10.9 ms: 1.05x slower                                                |
| xml_etree_iterparse  | 107 ms                                                 | 113 ms: 1.06x slower                                                 |
| unpickle_pure_python | 230 us                                                 | 259 us: 1.13x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                         |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 13.4 ms: 1.40x slower                                                |
| python_startup_no_site | 6.94 ms                                                | 11.9 ms: 1.71x slower                                                |
| Geometric mean         | (ref)                                                  | 1.55x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|-----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako            | 11.9 ms                                                | 12.4 ms: 1.04x slower                                                |
| django_template | 34.6 ms                                                | 38.0 ms: 1.10x slower                                                |
| Geometric mean  | (ref)                                                  | 1.07x slower                                                         |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 119 us: 1.32x faster                                                 |
| comprehensions             | 21.8 us                                                | 19.3 us: 1.13x faster                                                |
| unpickle_list              | 5.29 us                                                | 5.03 us: 1.05x faster                                                |
| logging_format             | 7.23 us                                                | 6.97 us: 1.04x faster                                                |
| unpickle                   | 15.9 us                                                | 15.3 us: 1.04x faster                                                |
| async_tree_none            | 472 ms                                                 | 459 ms: 1.03x faster                                                 |
| gc_traversal               | 3.79 ms                                                | 3.70 ms: 1.03x faster                                                |
| pickle_dict                | 35.5 us                                                | 34.8 us: 1.02x faster                                                |
| json_loads                 | 28.5 us                                                | 27.9 us: 1.02x faster                                                |
| logging_simple             | 6.46 us                                                | 6.34 us: 1.02x faster                                                |
| generators                 | 31.2 ms                                                | 30.7 ms: 1.02x faster                                                |
| pickle_list                | 5.08 us                                                | 5.00 us: 1.02x faster                                                |
| scimark_fft                | 382 ms                                                 | 376 ms: 1.02x faster                                                 |
| deepcopy_reduce            | 3.35 us                                                | 3.32 us: 1.01x faster                                                |
| pickle                     | 11.6 us                                                | 11.7 us: 1.01x slower                                                |
| chameleon                  | 7.41 ms                                                | 7.48 ms: 1.01x slower                                                |
| tomli_loads                | 2.33 sec                                               | 2.35 sec: 1.01x slower                                               |
| asyncio_websockets         | 551 ms                                                 | 557 ms: 1.01x slower                                                 |
| xml_etree_generate         | 89.2 ms                                                | 90.2 ms: 1.01x slower                                                |
| deepcopy                   | 371 us                                                 | 378 us: 1.02x slower                                                 |
| regex_effbot               | 3.61 ms                                                | 3.68 ms: 1.02x slower                                                |
| async_tree_memoization     | 578 ms                                                 | 591 ms: 1.02x slower                                                 |
| sympy_str                  | 300 ms                                                 | 307 ms: 1.02x slower                                                 |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 744 ms: 1.03x slower                                                 |
| pidigits                   | 187 ms                                                 | 192 ms: 1.03x slower                                                 |
| sympy_sum                  | 169 ms                                                 | 173 ms: 1.03x slower                                                 |
| create_gc_cycles           | 1.48 ms                                                | 1.52 ms: 1.03x slower                                                |
| logging_silent             | 104 ns                                                 | 107 ns: 1.03x slower                                                 |
| scimark_monte_carlo        | 75.1 ms                                                | 77.5 ms: 1.03x slower                                                |
| deepcopy_memo              | 40.7 us                                                | 42.1 us: 1.03x slower                                                |
| crypto_pyaes               | 81.9 ms                                                | 84.6 ms: 1.03x slower                                                |
| raytrace                   | 312 ms                                                 | 323 ms: 1.03x slower                                                 |
| pickle_pure_python         | 324 us                                                 | 336 us: 1.04x slower                                                 |
| xml_etree_process          | 61.7 ms                                                | 64.1 ms: 1.04x slower                                                |
| sqlglot_normalize          | 110 ms                                                 | 115 ms: 1.04x slower                                                 |
| mako                       | 11.9 ms                                                | 12.4 ms: 1.04x slower                                                |
| sqlite_synth               | 2.83 us                                                | 2.95 us: 1.04x slower                                                |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 755 ms: 1.04x slower                                                 |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.86 sec: 1.04x slower                                               |
| tornado_http               | 103 ms                                                 | 107 ms: 1.04x slower                                                 |
| async_tree_none_tg         | 450 ms                                                 | 469 ms: 1.04x slower                                                 |
| asyncio_tcp                | 491 ms                                                 | 513 ms: 1.05x slower                                                 |
| async_tree_memoization_tg  | 575 ms                                                 | 601 ms: 1.05x slower                                                 |
| docutils                   | 2.77 sec                                               | 2.90 sec: 1.05x slower                                               |
| deltablue                  | 3.72 ms                                                | 3.90 ms: 1.05x slower                                                |
| json_dumps                 | 10.4 ms                                                | 10.9 ms: 1.05x slower                                                |
| regex_compile              | 148 ms                                                 | 156 ms: 1.05x slower                                                 |
| dulwich_log                | 68.5 ms                                                | 72.3 ms: 1.05x slower                                                |
| regex_dna                  | 212 ms                                                 | 224 ms: 1.06x slower                                                 |
| xml_etree_iterparse        | 107 ms                                                 | 113 ms: 1.06x slower                                                 |
| pprint_safe_repr           | 776 ms                                                 | 821 ms: 1.06x slower                                                 |
| async_tree_io_tg           | 1.18 sec                                               | 1.25 sec: 1.06x slower                                               |
| meteor_contest             | 112 ms                                                 | 119 ms: 1.06x slower                                                 |
| pprint_pformat             | 1.57 sec                                               | 1.67 sec: 1.06x slower                                               |
| sqlglot_parse              | 1.36 ms                                                | 1.45 ms: 1.06x slower                                                |
| chaos                      | 67.0 ms                                                | 71.3 ms: 1.07x slower                                                |
| async_tree_io              | 1.16 sec                                               | 1.23 sec: 1.07x slower                                               |
| sympy_expand               | 478 ms                                                 | 512 ms: 1.07x slower                                                 |
| async_generators           | 463 ms                                                 | 496 ms: 1.07x slower                                                 |
| sqlglot_transpile          | 1.68 ms                                                | 1.81 ms: 1.07x slower                                                |
| sympy_integrate            | 21.4 ms                                                | 23.0 ms: 1.07x slower                                                |
| spectral_norm              | 115 ms                                                 | 124 ms: 1.08x slower                                                 |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 5.49 ms: 1.09x slower                                                |
| sqlglot_optimize           | 54.8 ms                                                | 60.0 ms: 1.09x slower                                                |
| 2to3                       | 274 ms                                                 | 301 ms: 1.10x slower                                                 |
| django_template            | 34.6 ms                                                | 38.0 ms: 1.10x slower                                                |
| mdp                        | 2.63 sec                                               | 2.90 sec: 1.10x slower                                               |
| nbody                      | 97.0 ms                                                | 107 ms: 1.11x slower                                                 |
| regex_v8                   | 23.1 ms                                                | 25.8 ms: 1.11x slower                                                |
| pycparser                  | 1.18 sec                                               | 1.32 sec: 1.12x slower                                               |
| richards_super             | 51.5 ms                                                | 57.7 ms: 1.12x slower                                                |
| coroutines                 | 23.2 ms                                                | 26.0 ms: 1.12x slower                                                |
| aiohttp                    | 1.15 ms                                                | 1.29 ms: 1.12x slower                                                |
| gunicorn                   | 1.24 ms                                                | 1.39 ms: 1.12x slower                                                |
| unpickle_pure_python       | 230 us                                                 | 259 us: 1.13x slower                                                 |
| richards                   | 45.8 ms                                                | 51.8 ms: 1.13x slower                                                |
| mypy2                      | 830 ms                                                 | 944 ms: 1.14x slower                                                 |
| pyflate                    | 482 ms                                                 | 548 ms: 1.14x slower                                                 |
| bench_mp_pool              | 24.0 ms                                                | 28.1 ms: 1.17x slower                                                |
| scimark_sor                | 129 ms                                                 | 154 ms: 1.20x slower                                                 |
| scimark_lu                 | 118 ms                                                 | 142 ms: 1.20x slower                                                 |
| nqueens                    | 83.3 ms                                                | 101 ms: 1.21x slower                                                 |
| fannkuch                   | 417 ms                                                 | 508 ms: 1.22x slower                                                 |
| hexiom                     | 6.41 ms                                                | 7.90 ms: 1.23x slower                                                |
| go                         | 139 ms                                                 | 175 ms: 1.25x slower                                                 |
| telco                      | 7.10 ms                                                | 8.91 ms: 1.25x slower                                                |
| coverage                   | 72.7 ms                                                | 101 ms: 1.38x slower                                                 |
| python_startup             | 9.55 ms                                                | 13.4 ms: 1.40x slower                                                |
| python_startup_no_site     | 6.94 ms                                                | 11.9 ms: 1.71x slower                                                |
| bench_thread_pool          | 842 us                                                 | 1.58 ms: 1.87x slower                                                |
| Geometric mean             | (ref)                                                  | 1.07x slower                                                         |

Benchmark hidden because not significant (4): pathlib, float, xml_etree_parse, json
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: dask, sqlalchemy_declarative, sqlalchemy_imperative, unpack_sequence
Ignored benchmarks (6) of results/bm-20240307-3.13.0a4+-5fb754d-JIT/bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d.json: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.04x
- 95% likely to have a slowdown of 1.04x
- 99% likely to have a slowdown of 1.04x


# Memory

- memory change: 1.17x