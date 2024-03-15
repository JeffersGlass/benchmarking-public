# Results vs. 3.11.0

- fork: brandtbucher
- ref: defer_decref
- machine: linux-x86_64
- commit hash: 5fb754d
- commit date: 2024-03-07
- overall geometric mean: 1.04x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x slower
- Memory change: 1.25x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 301 ms: 1.14x slower                                                 |
| chameleon      | 6.70 ms                                                | 7.48 ms: 1.12x slower                                                |
| docutils       | 2.66 sec                                               | 2.90 sec: 1.09x slower                                               |
| html5lib       | 64.8 ms                                                | 71.7 ms: 1.11x slower                                                |
| tornado_http   | 98.1 ms                                                | 107 ms: 1.09x slower                                                 |
| Geometric mean | (ref)                                                  | 1.11x slower                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|---------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none           | 528 ms                                                 | 459 ms: 1.15x faster                                                 |
| async_tree_memoization    | 639 ms                                                 | 591 ms: 1.08x faster                                                 |
| async_tree_none_tg        | 491 ms                                                 | 469 ms: 1.05x faster                                                 |
| async_tree_io             | 1.29 sec                                               | 1.23 sec: 1.04x faster                                               |
| async_tree_memoization_tg | 626 ms                                                 | 601 ms: 1.04x faster                                                 |
| async_tree_io_tg          | 1.29 sec                                               | 1.25 sec: 1.03x faster                                               |
| Geometric mean            | (ref)                                                  | 1.05x faster                                                         |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 192 ms: 1.01x faster                                                 |
| float          | 78.9 ms                                                | 84.6 ms: 1.07x slower                                                |
| nbody          | 96.0 ms                                                | 107 ms: 1.12x slower                                                 |
| Geometric mean | (ref)                                                  | 1.06x slower                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.68 ms: 1.05x slower                                                |
| regex_dna      | 205 ms                                                 | 224 ms: 1.10x slower                                                 |
| regex_compile  | 141 ms                                                 | 156 ms: 1.11x slower                                                 |
| regex_v8       | 22.9 ms                                                | 25.8 ms: 1.13x slower                                                |
| Geometric mean | (ref)                                                  | 1.09x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.9 ms: 1.22x faster                                                |
| json_loads           | 29.2 us                                                | 27.9 us: 1.05x faster                                                |
| unpickle_list        | 5.21 us                                                | 5.03 us: 1.04x faster                                                |
| xml_etree_parse      | 164 ms                                                 | 160 ms: 1.03x faster                                                 |
| pickle_dict          | 34.6 us                                                | 34.8 us: 1.01x slower                                                |
| tomli_loads          | 2.30 sec                                               | 2.35 sec: 1.02x slower                                               |
| xml_etree_iterparse  | 108 ms                                                 | 113 ms: 1.05x slower                                                 |
| pickle_pure_python   | 320 us                                                 | 336 us: 1.05x slower                                                 |
| pickle               | 11.0 us                                                | 11.7 us: 1.06x slower                                                |
| unpickle_pure_python | 242 us                                                 | 259 us: 1.07x slower                                                 |
| pickle_list          | 4.59 us                                                | 5.00 us: 1.09x slower                                                |
| unpickle             | 13.8 us                                                | 15.3 us: 1.10x slower                                                |
| xml_etree_generate   | 81.1 ms                                                | 90.2 ms: 1.11x slower                                                |
| xml_etree_process    | 56.9 ms                                                | 64.1 ms: 1.13x slower                                                |
| Geometric mean       | (ref)                                                  | 1.03x slower                                                         |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 13.4 ms: 1.56x slower                                                |
| python_startup_no_site | 6.01 ms                                                | 11.9 ms: 1.98x slower                                                |
| Geometric mean         | (ref)                                                  | 1.76x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|-----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| genshi_xml      | 53.4 ms                                                | 58.3 ms: 1.09x slower                                                |
| django_template | 33.5 ms                                                | 38.0 ms: 1.13x slower                                                |
| mako            | 10.7 ms                                                | 12.4 ms: 1.16x slower                                                |
| genshi_text     | 22.5 ms                                                | 26.4 ms: 1.17x slower                                                |
| Geometric mean  | (ref)                                                  | 1.14x slower                                                         |

All benchmarks:
===============

| Benchmark                 | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|---------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols  | 520 us                                                 | 119 us: 4.35x faster                                                 |
| generators                | 74.9 ms                                                | 30.7 ms: 2.44x faster                                                |
| asyncio_tcp               | 875 ms                                                 | 513 ms: 1.71x faster                                                 |
| asyncio_tcp_ssl           | 3.11 sec                                               | 1.86 sec: 1.67x faster                                               |
| pylint                    | 476 ms                                                 | 348 ms: 1.37x faster                                                 |
| comprehensions            | 23.6 us                                                | 19.3 us: 1.22x faster                                                |
| json_dumps                | 13.3 ms                                                | 10.9 ms: 1.22x faster                                                |
| async_tree_none           | 528 ms                                                 | 459 ms: 1.15x faster                                                 |
| gc_traversal              | 4.01 ms                                                | 3.70 ms: 1.08x faster                                                |
| async_tree_memoization    | 639 ms                                                 | 591 ms: 1.08x faster                                                 |
| richards_super            | 61.9 ms                                                | 57.7 ms: 1.07x faster                                                |
| async_tree_none_tg        | 491 ms                                                 | 469 ms: 1.05x faster                                                 |
| json_loads                | 29.2 us                                                | 27.9 us: 1.05x faster                                                |
| async_tree_io             | 1.29 sec                                               | 1.23 sec: 1.04x faster                                               |
| async_tree_memoization_tg | 626 ms                                                 | 601 ms: 1.04x faster                                                 |
| coroutines                | 27.0 ms                                                | 26.0 ms: 1.04x faster                                                |
| unpickle_list             | 5.21 us                                                | 5.03 us: 1.04x faster                                                |
| logging_silent            | 111 ns                                                 | 107 ns: 1.03x faster                                                 |
| async_tree_io_tg          | 1.29 sec                                               | 1.25 sec: 1.03x faster                                               |
| xml_etree_parse           | 164 ms                                                 | 160 ms: 1.03x faster                                                 |
| djangocms                 | 33.5 us                                                | 32.7 us: 1.02x faster                                                |
| pidigits                  | 194 ms                                                 | 192 ms: 1.01x faster                                                 |
| chaos                     | 71.9 ms                                                | 71.3 ms: 1.01x faster                                                |
| pickle_dict               | 34.6 us                                                | 34.8 us: 1.01x slower                                                |
| sqlglot_parse             | 1.43 ms                                                | 1.45 ms: 1.01x slower                                                |
| json                      | 5.24 ms                                                | 5.30 ms: 1.01x slower                                                |
| asyncio_websockets        | 550 ms                                                 | 557 ms: 1.01x slower                                                 |
| sqlglot_normalize         | 113 ms                                                 | 115 ms: 1.02x slower                                                 |
| logging_simple            | 6.22 us                                                | 6.34 us: 1.02x slower                                                |
| tomli_loads               | 2.30 sec                                               | 2.35 sec: 1.02x slower                                               |
| logging_format            | 6.81 us                                                | 6.97 us: 1.02x slower                                                |
| sympy_sum                 | 169 ms                                                 | 173 ms: 1.03x slower                                                 |
| deepcopy_reduce           | 3.22 us                                                | 3.32 us: 1.03x slower                                                |
| sympy_str                 | 297 ms                                                 | 307 ms: 1.03x slower                                                 |
| sqlglot_transpile         | 1.75 ms                                                | 1.81 ms: 1.03x slower                                                |
| deepcopy                  | 365 us                                                 | 378 us: 1.03x slower                                                 |
| richards                  | 49.8 ms                                                | 51.8 ms: 1.04x slower                                                |
| pathlib                   | 18.5 ms                                                | 19.3 ms: 1.04x slower                                                |
| mdp                       | 2.77 sec                                               | 2.90 sec: 1.05x slower                                               |
| xml_etree_iterparse       | 108 ms                                                 | 113 ms: 1.05x slower                                                 |
| raytrace                  | 309 ms                                                 | 323 ms: 1.05x slower                                                 |
| deepcopy_memo             | 40.2 us                                                | 42.1 us: 1.05x slower                                                |
| regex_effbot              | 3.51 ms                                                | 3.68 ms: 1.05x slower                                                |
| pickle_pure_python        | 320 us                                                 | 336 us: 1.05x slower                                                 |
| sympy_expand              | 484 ms                                                 | 512 ms: 1.06x slower                                                 |
| create_gc_cycles          | 1.43 ms                                                | 1.52 ms: 1.06x slower                                                |
| thrift                    | 784 us                                                 | 831 us: 1.06x slower                                                 |
| pickle                    | 11.0 us                                                | 11.7 us: 1.06x slower                                                |
| sympy_integrate           | 21.5 ms                                                | 23.0 ms: 1.07x slower                                                |
| float                     | 78.9 ms                                                | 84.6 ms: 1.07x slower                                                |
| unpickle_pure_python      | 242 us                                                 | 259 us: 1.07x slower                                                 |
| pprint_pformat            | 1.55 sec                                               | 1.67 sec: 1.07x slower                                               |
| sqlglot_optimize          | 55.3 ms                                                | 60.0 ms: 1.08x slower                                                |
| scimark_fft               | 345 ms                                                 | 376 ms: 1.09x slower                                                 |
| pickle_list               | 4.59 us                                                | 5.00 us: 1.09x slower                                                |
| docutils                  | 2.66 sec                                               | 2.90 sec: 1.09x slower                                               |
| genshi_xml                | 53.4 ms                                                | 58.3 ms: 1.09x slower                                                |
| scimark_sparse_mat_mult   | 5.03 ms                                                | 5.49 ms: 1.09x slower                                                |
| tornado_http              | 98.1 ms                                                | 107 ms: 1.09x slower                                                 |
| meteor_contest            | 109 ms                                                 | 119 ms: 1.09x slower                                                 |
| scimark_monte_carlo       | 70.7 ms                                                | 77.5 ms: 1.10x slower                                                |
| regex_dna                 | 205 ms                                                 | 224 ms: 1.10x slower                                                 |
| pprint_safe_repr          | 747 ms                                                 | 821 ms: 1.10x slower                                                 |
| crypto_pyaes              | 76.7 ms                                                | 84.6 ms: 1.10x slower                                                |
| unpickle                  | 13.8 us                                                | 15.3 us: 1.10x slower                                                |
| html5lib                  | 64.8 ms                                                | 71.7 ms: 1.11x slower                                                |
| regex_compile             | 141 ms                                                 | 156 ms: 1.11x slower                                                 |
| pycparser                 | 1.19 sec                                               | 1.32 sec: 1.11x slower                                               |
| xml_etree_generate        | 81.1 ms                                                | 90.2 ms: 1.11x slower                                                |
| chameleon                 | 6.70 ms                                                | 7.48 ms: 1.12x slower                                                |
| dulwich_log               | 64.6 ms                                                | 72.3 ms: 1.12x slower                                                |
| nbody                     | 96.0 ms                                                | 107 ms: 1.12x slower                                                 |
| regex_v8                  | 22.9 ms                                                | 25.8 ms: 1.13x slower                                                |
| xml_etree_process         | 56.9 ms                                                | 64.1 ms: 1.13x slower                                                |
| django_template           | 33.5 ms                                                | 38.0 ms: 1.13x slower                                                |
| 2to3                      | 264 ms                                                 | 301 ms: 1.14x slower                                                 |
| hexiom                    | 6.89 ms                                                | 7.90 ms: 1.15x slower                                                |
| sqlite_synth              | 2.57 us                                                | 2.95 us: 1.15x slower                                                |
| nqueens                   | 87.9 ms                                                | 101 ms: 1.15x slower                                                 |
| spectral_norm             | 108 ms                                                 | 124 ms: 1.15x slower                                                 |
| aiohttp                   | 1.12 ms                                                | 1.29 ms: 1.16x slower                                                |
| mako                      | 10.7 ms                                                | 12.4 ms: 1.16x slower                                                |
| gunicorn                  | 1.20 ms                                                | 1.39 ms: 1.16x slower                                                |
| genshi_text               | 22.5 ms                                                | 26.4 ms: 1.17x slower                                                |
| bench_mp_pool             | 24.0 ms                                                | 28.1 ms: 1.17x slower                                                |
| go                        | 149 ms                                                 | 175 ms: 1.17x slower                                                 |
| scimark_lu                | 116 ms                                                 | 142 ms: 1.22x slower                                                 |
| fannkuch                  | 405 ms                                                 | 508 ms: 1.25x slower                                                 |
| pyflate                   | 434 ms                                                 | 548 ms: 1.26x slower                                                 |
| scimark_sor               | 121 ms                                                 | 154 ms: 1.27x slower                                                 |
| coverage                  | 78.8 ms                                                | 101 ms: 1.28x slower                                                 |
| telco                     | 6.86 ms                                                | 8.91 ms: 1.30x slower                                                |
| async_generators          | 374 ms                                                 | 496 ms: 1.33x slower                                                 |
| mypy2                     | 686 ms                                                 | 944 ms: 1.38x slower                                                 |
| python_startup            | 8.56 ms                                                | 13.4 ms: 1.56x slower                                                |
| bench_thread_pool         | 834 us                                                 | 1.58 ms: 1.89x slower                                                |
| python_startup_no_site    | 6.01 ms                                                | 11.9 ms: 1.98x slower                                                |
| Geometric mean            | (ref)                                                  | 1.04x slower                                                         |

Benchmark hidden because not significant (3): async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed, deltablue
Ignored benchmarks (5) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: dask, flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative, unpack_sequence


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.04x
- 95% likely to have a slowdown of 1.04x
- 99% likely to have a slowdown of 1.03x


# Memory

- memory change: 1.25x