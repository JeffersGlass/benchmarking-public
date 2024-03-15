# Results vs. base

- fork: brandtbucher
- ref: defer_decref
- machine: linux-x86_64
- commit hash: 5fb754d
- commit date: 2024-03-07
- overall geometric mean: 1.07x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x slower
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240306-linux-x86_64-python-c62144a02cfae412a9de-3.13.0a4+-c62144a | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 280 ms                                                                 | 301 ms: 1.07x slower                                                 |
| chameleon      | 7.04 ms                                                                | 7.48 ms: 1.06x slower                                                |
| docutils       | 2.76 sec                                                               | 2.90 sec: 1.05x slower                                               |
| html5lib       | 67.6 ms                                                                | 71.7 ms: 1.06x slower                                                |
| tornado_http   | 98.6 ms                                                                | 107 ms: 1.09x slower                                                 |
| Geometric mean | (ref)                                                                  | 1.07x slower                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240306-linux-x86_64-python-c62144a02cfae412a9de-3.13.0a4+-c62144a | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_io_tg           | 1.24 sec                                                               | 1.25 sec: 1.01x slower                                               |
| async_tree_memoization_tg  | 593 ms                                                                 | 601 ms: 1.01x slower                                                 |
| async_tree_io              | 1.22 sec                                                               | 1.23 sec: 1.01x slower                                               |
| async_tree_cpu_io_mixed_tg | 741 ms                                                                 | 755 ms: 1.02x slower                                                 |
| async_tree_none_tg         | 459 ms                                                                 | 469 ms: 1.02x slower                                                 |
| async_tree_cpu_io_mixed    | 725 ms                                                                 | 744 ms: 1.03x slower                                                 |
| async_tree_memoization     | 575 ms                                                                 | 591 ms: 1.03x slower                                                 |
| async_tree_none            | 446 ms                                                                 | 459 ms: 1.03x slower                                                 |
| Geometric mean             | (ref)                                                                  | 1.02x slower                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240306-linux-x86_64-python-c62144a02cfae412a9de-3.13.0a4+-c62144a | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| pidigits       | 189 ms                                                                 | 192 ms: 1.01x slower                                                 |
| float          | 79.8 ms                                                                | 84.6 ms: 1.06x slower                                                |
| nbody          | 94.1 ms                                                                | 107 ms: 1.14x slower                                                 |
| Geometric mean | (ref)                                                                  | 1.07x slower                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240306-linux-x86_64-python-c62144a02cfae412a9de-3.13.0a4+-c62144a | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_effbot   | 3.75 ms                                                                | 3.68 ms: 1.02x faster                                                |
| regex_dna      | 221 ms                                                                 | 224 ms: 1.02x slower                                                 |
| regex_v8       | 25.3 ms                                                                | 25.8 ms: 1.02x slower                                                |
| regex_compile  | 141 ms                                                                 | 156 ms: 1.11x slower                                                 |
| Geometric mean | (ref)                                                                  | 1.03x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240306-linux-x86_64-python-c62144a02cfae412a9de-3.13.0a4+-c62144a | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| unpickle_list        | 4.99 us                                                                | 5.03 us: 1.01x slower                                                |
| pickle_list          | 4.93 us                                                                | 5.00 us: 1.01x slower                                                |
| pickle               | 11.5 us                                                                | 11.7 us: 1.01x slower                                                |
| pickle_dict          | 34.2 us                                                                | 34.8 us: 1.02x slower                                                |
| xml_etree_generate   | 88.4 ms                                                                | 90.2 ms: 1.02x slower                                                |
| json_dumps           | 10.7 ms                                                                | 10.9 ms: 1.02x slower                                                |
| xml_etree_iterparse  | 108 ms                                                                 | 113 ms: 1.05x slower                                                 |
| xml_etree_process    | 59.9 ms                                                                | 64.1 ms: 1.07x slower                                                |
| pickle_pure_python   | 306 us                                                                 | 336 us: 1.10x slower                                                 |
| unpickle_pure_python | 233 us                                                                 | 259 us: 1.11x slower                                                 |
| tomli_loads          | 2.02 sec                                                               | 2.35 sec: 1.17x slower                                               |
| Geometric mean       | (ref)                                                                  | 1.04x slower                                                         |

Benchmark hidden because not significant (3): json_loads, unpickle, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240306-linux-x86_64-python-c62144a02cfae412a9de-3.13.0a4+-c62144a | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 12.6 ms                                                                | 13.4 ms: 1.06x slower                                                |
| python_startup_no_site | 11.2 ms                                                                | 11.9 ms: 1.06x slower                                                |
| Geometric mean         | (ref)                                                                  | 1.06x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20240306-linux-x86_64-python-c62144a02cfae412a9de-3.13.0a4+-c62144a | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|-----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| genshi_xml      | 54.1 ms                                                                | 58.3 ms: 1.08x slower                                                |
| mako            | 11.4 ms                                                                | 12.4 ms: 1.08x slower                                                |
| django_template | 34.6 ms                                                                | 38.0 ms: 1.10x slower                                                |
| genshi_text     | 23.9 ms                                                                | 26.4 ms: 1.10x slower                                                |
| Geometric mean  | (ref)                                                                  | 1.09x slower                                                         |

All benchmarks:
===============

| Benchmark                  | bm-20240306-linux-x86_64-python-c62144a02cfae412a9de-3.13.0a4+-c62144a | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| gc_traversal               | 3.90 ms                                                                | 3.70 ms: 1.06x faster                                                |
| regex_effbot               | 3.75 ms                                                                | 3.68 ms: 1.02x faster                                                |
| asyncio_websockets         | 563 ms                                                                 | 557 ms: 1.01x faster                                                 |
| create_gc_cycles           | 1.53 ms                                                                | 1.52 ms: 1.01x faster                                                |
| asyncio_tcp_ssl            | 1.86 sec                                                               | 1.86 sec: 1.00x slower                                               |
| unpickle_list              | 4.99 us                                                                | 5.03 us: 1.01x slower                                                |
| async_tree_io_tg           | 1.24 sec                                                               | 1.25 sec: 1.01x slower                                               |
| pickle_list                | 4.93 us                                                                | 5.00 us: 1.01x slower                                                |
| asyncio_tcp                | 506 ms                                                                 | 513 ms: 1.01x slower                                                 |
| pickle                     | 11.5 us                                                                | 11.7 us: 1.01x slower                                                |
| pidigits                   | 189 ms                                                                 | 192 ms: 1.01x slower                                                 |
| async_tree_memoization_tg  | 593 ms                                                                 | 601 ms: 1.01x slower                                                 |
| async_tree_io              | 1.22 sec                                                               | 1.23 sec: 1.01x slower                                               |
| regex_dna                  | 221 ms                                                                 | 224 ms: 1.02x slower                                                 |
| sqlite_synth               | 2.90 us                                                                | 2.95 us: 1.02x slower                                                |
| pickle_dict                | 34.2 us                                                                | 34.8 us: 1.02x slower                                                |
| regex_v8                   | 25.3 ms                                                                | 25.8 ms: 1.02x slower                                                |
| async_tree_cpu_io_mixed_tg | 741 ms                                                                 | 755 ms: 1.02x slower                                                 |
| xml_etree_generate         | 88.4 ms                                                                | 90.2 ms: 1.02x slower                                                |
| async_tree_none_tg         | 459 ms                                                                 | 469 ms: 1.02x slower                                                 |
| json_dumps                 | 10.7 ms                                                                | 10.9 ms: 1.02x slower                                                |
| async_tree_cpu_io_mixed    | 725 ms                                                                 | 744 ms: 1.03x slower                                                 |
| pathlib                    | 18.8 ms                                                                | 19.3 ms: 1.03x slower                                                |
| async_tree_memoization     | 575 ms                                                                 | 591 ms: 1.03x slower                                                 |
| async_tree_none            | 446 ms                                                                 | 459 ms: 1.03x slower                                                 |
| coverage                   | 97.7 ms                                                                | 101 ms: 1.03x slower                                                 |
| thrift                     | 806 us                                                                 | 831 us: 1.03x slower                                                 |
| generators                 | 29.7 ms                                                                | 30.7 ms: 1.03x slower                                                |
| mdp                        | 2.78 sec                                                               | 2.90 sec: 1.04x slower                                               |
| xml_etree_iterparse        | 108 ms                                                                 | 113 ms: 1.05x slower                                                 |
| docutils                   | 2.76 sec                                                               | 2.90 sec: 1.05x slower                                               |
| scimark_monte_carlo        | 73.8 ms                                                                | 77.5 ms: 1.05x slower                                                |
| dulwich_log                | 68.8 ms                                                                | 72.3 ms: 1.05x slower                                                |
| telco                      | 8.45 ms                                                                | 8.91 ms: 1.05x slower                                                |
| sqlglot_normalize          | 108 ms                                                                 | 115 ms: 1.06x slower                                                 |
| float                      | 79.8 ms                                                                | 84.6 ms: 1.06x slower                                                |
| html5lib                   | 67.6 ms                                                                | 71.7 ms: 1.06x slower                                                |
| chameleon                  | 7.04 ms                                                                | 7.48 ms: 1.06x slower                                                |
| python_startup             | 12.6 ms                                                                | 13.4 ms: 1.06x slower                                                |
| python_startup_no_site     | 11.2 ms                                                                | 11.9 ms: 1.06x slower                                                |
| async_generators           | 466 ms                                                                 | 496 ms: 1.06x slower                                                 |
| sympy_expand               | 480 ms                                                                 | 512 ms: 1.07x slower                                                 |
| logging_silent             | 101 ns                                                                 | 107 ns: 1.07x slower                                                 |
| pylint                     | 326 ms                                                                 | 348 ms: 1.07x slower                                                 |
| deepcopy                   | 353 us                                                                 | 378 us: 1.07x slower                                                 |
| richards_super             | 53.9 ms                                                                | 57.7 ms: 1.07x slower                                                |
| xml_etree_process          | 59.9 ms                                                                | 64.1 ms: 1.07x slower                                                |
| typing_runtime_protocols   | 111 us                                                                 | 119 us: 1.07x slower                                                 |
| 2to3                       | 280 ms                                                                 | 301 ms: 1.07x slower                                                 |
| aiohttp                    | 1.20 ms                                                                | 1.29 ms: 1.08x slower                                                |
| sympy_str                  | 285 ms                                                                 | 307 ms: 1.08x slower                                                 |
| gunicorn                   | 1.29 ms                                                                | 1.39 ms: 1.08x slower                                                |
| bench_mp_pool              | 26.1 ms                                                                | 28.1 ms: 1.08x slower                                                |
| genshi_xml                 | 54.1 ms                                                                | 58.3 ms: 1.08x slower                                                |
| meteor_contest             | 110 ms                                                                 | 119 ms: 1.08x slower                                                 |
| logging_format             | 6.46 us                                                                | 6.97 us: 1.08x slower                                                |
| raytrace                   | 299 ms                                                                 | 323 ms: 1.08x slower                                                 |
| deepcopy_memo              | 39.0 us                                                                | 42.1 us: 1.08x slower                                                |
| pprint_safe_repr           | 760 ms                                                                 | 821 ms: 1.08x slower                                                 |
| mako                       | 11.4 ms                                                                | 12.4 ms: 1.08x slower                                                |
| deepcopy_reduce            | 3.06 us                                                                | 3.32 us: 1.08x slower                                                |
| sqlglot_optimize           | 55.4 ms                                                                | 60.0 ms: 1.08x slower                                                |
| pprint_pformat             | 1.54 sec                                                               | 1.67 sec: 1.09x slower                                               |
| tornado_http               | 98.6 ms                                                                | 107 ms: 1.09x slower                                                 |
| sympy_sum                  | 160 ms                                                                 | 173 ms: 1.09x slower                                                 |
| logging_simple             | 5.83 us                                                                | 6.34 us: 1.09x slower                                                |
| scimark_lu                 | 130 ms                                                                 | 142 ms: 1.09x slower                                                 |
| go                         | 160 ms                                                                 | 175 ms: 1.09x slower                                                 |
| sympy_integrate            | 21.1 ms                                                                | 23.0 ms: 1.09x slower                                                |
| spectral_norm              | 114 ms                                                                 | 124 ms: 1.09x slower                                                 |
| richards                   | 47.3 ms                                                                | 51.8 ms: 1.09x slower                                                |
| sqlglot_transpile          | 1.65 ms                                                                | 1.81 ms: 1.10x slower                                                |
| django_template            | 34.6 ms                                                                | 38.0 ms: 1.10x slower                                                |
| pickle_pure_python         | 306 us                                                                 | 336 us: 1.10x slower                                                 |
| scimark_fft                | 341 ms                                                                 | 376 ms: 1.10x slower                                                 |
| genshi_text                | 23.9 ms                                                                | 26.4 ms: 1.10x slower                                                |
| deltablue                  | 3.53 ms                                                                | 3.90 ms: 1.11x slower                                                |
| regex_compile              | 141 ms                                                                 | 156 ms: 1.11x slower                                                 |
| pycparser                  | 1.19 sec                                                               | 1.32 sec: 1.11x slower                                               |
| unpickle_pure_python       | 233 us                                                                 | 259 us: 1.11x slower                                                 |
| sqlglot_parse              | 1.30 ms                                                                | 1.45 ms: 1.11x slower                                                |
| comprehensions             | 17.3 us                                                                | 19.3 us: 1.12x slower                                                |
| chaos                      | 63.8 ms                                                                | 71.3 ms: 1.12x slower                                                |
| nqueens                    | 90.2 ms                                                                | 101 ms: 1.12x slower                                                 |
| hexiom                     | 7.04 ms                                                                | 7.90 ms: 1.12x slower                                                |
| pyflate                    | 487 ms                                                                 | 548 ms: 1.13x slower                                                 |
| scimark_sor                | 136 ms                                                                 | 154 ms: 1.14x slower                                                 |
| nbody                      | 94.1 ms                                                                | 107 ms: 1.14x slower                                                 |
| coroutines                 | 22.7 ms                                                                | 26.0 ms: 1.14x slower                                                |
| scimark_sparse_mat_mult    | 4.79 ms                                                                | 5.49 ms: 1.15x slower                                                |
| crypto_pyaes               | 73.5 ms                                                                | 84.6 ms: 1.15x slower                                                |
| tomli_loads                | 2.02 sec                                                               | 2.35 sec: 1.17x slower                                               |
| fannkuch                   | 396 ms                                                                 | 508 ms: 1.28x slower                                                 |
| bench_thread_pool          | 859 us                                                                 | 1.58 ms: 1.84x slower                                                |
| Geometric mean             | (ref)                                                                  | 1.07x slower                                                         |

Benchmark hidden because not significant (6): json, json_loads, unpickle, xml_etree_parse, djangocms, mypy2
Ignored benchmarks (1) of results/bm-20240306-3.13.0a4+-c62144a-JIT/bm-20240306-linux-x86_64-python-c62144a02cfae412a9de-3.13.0a4+-c62144a.json: unpack_sequence


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.06x
- 95% likely to have a slowdown of 1.05x
- 99% likely to have a slowdown of 1.04x


# Memory

- memory change: 1.01x