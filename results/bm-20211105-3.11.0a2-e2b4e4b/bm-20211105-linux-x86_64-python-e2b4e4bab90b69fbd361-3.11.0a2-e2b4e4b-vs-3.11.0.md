
# Results vs. 3.11.0

- fork: python
- ref: e2b4e4bab90b69fbd361
- machine: linux-x86_64
- commit hash: e2b4e4b
- commit date: 2021-11-05
- overall geometric mean: 1.05x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 274 ms: 1.04x slower                                                  |
| chameleon      | 6.70 ms                                                | 7.46 ms: 1.11x slower                                                 |
| docutils       | 2.66 sec                                               | 2.79 sec: 1.05x slower                                                |
| html5lib       | 64.8 ms                                                | 71.5 ms: 1.10x slower                                                 |
| tornado_http   | 98.1 ms                                                | 111 ms: 1.13x slower                                                  |
| Geometric mean | (ref)                                                  | 1.09x slower                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_none         | 528 ms                                                 | 518 ms: 1.02x faster                                                  |
| async_tree_memoization  | 639 ms                                                 | 676 ms: 1.06x slower                                                  |
| async_tree_cpu_io_mixed | 749 ms                                                 | 818 ms: 1.09x slower                                                  |
| async_tree_io           | 1.29 sec                                               | 1.41 sec: 1.09x slower                                                |
| Geometric mean          | (ref)                                                  | 1.05x slower                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 188 ms: 1.03x faster                                                  |
| float          | 78.9 ms                                                | 83.3 ms: 1.05x slower                                                 |
| nbody          | 96.0 ms                                                | 112 ms: 1.17x slower                                                  |
| Geometric mean | (ref)                                                  | 1.06x slower                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.26 ms: 1.08x faster                                                 |
| regex_compile  | 141 ms                                                 | 145 ms: 1.02x slower                                                  |
| regex_v8       | 22.9 ms                                                | 23.7 ms: 1.04x slower                                                 |
| regex_dna      | 205 ms                                                 | 219 ms: 1.07x slower                                                  |
| Geometric mean | (ref)                                                  | 1.01x slower                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pickle_dict          | 34.6 us                                                | 28.6 us: 1.21x faster                                                 |
| json_loads           | 29.2 us                                                | 25.9 us: 1.13x faster                                                 |
| pickle               | 11.0 us                                                | 10.1 us: 1.09x faster                                                 |
| json_dumps           | 13.3 ms                                                | 12.4 ms: 1.08x faster                                                 |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                                  |
| unpickle_list        | 5.21 us                                                | 5.13 us: 1.02x faster                                                 |
| xml_etree_generate   | 81.1 ms                                                | 81.6 ms: 1.01x slower                                                 |
| pickle_list          | 4.59 us                                                | 4.68 us: 1.02x slower                                                 |
| xml_etree_iterparse  | 108 ms                                                 | 110 ms: 1.02x slower                                                  |
| xml_etree_process    | 56.9 ms                                                | 59.6 ms: 1.05x slower                                                 |
| unpickle_pure_python | 242 us                                                 | 271 us: 1.12x slower                                                  |
| pickle_pure_python   | 320 us                                                 | 364 us: 1.14x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                          |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup_no_site | 6.01 ms                                                | 5.77 ms: 1.04x faster                                                 |
| python_startup         | 8.56 ms                                                | 14.6 ms: 1.70x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.28x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| genshi_xml      | 53.4 ms                                                | 56.1 ms: 1.05x slower                                                 |
| genshi_text     | 22.5 ms                                                | 24.6 ms: 1.09x slower                                                 |
| django_template | 33.5 ms                                                | 37.9 ms: 1.13x slower                                                 |
| mako            | 10.7 ms                                                | 12.1 ms: 1.13x slower                                                 |
| Geometric mean  | (ref)                                                  | 1.10x slower                                                          |

All benchmarks:
===============

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| generators              | 74.9 ms                                                | 57.4 ms: 1.30x faster                                                 |
| pickle_dict             | 34.6 us                                                | 28.6 us: 1.21x faster                                                 |
| json_loads              | 29.2 us                                                | 25.9 us: 1.13x faster                                                 |
| pickle                  | 11.0 us                                                | 10.1 us: 1.09x faster                                                 |
| json_dumps              | 13.3 ms                                                | 12.4 ms: 1.08x faster                                                 |
| regex_effbot            | 3.51 ms                                                | 3.26 ms: 1.08x faster                                                 |
| json                    | 5.24 ms                                                | 4.91 ms: 1.07x faster                                                 |
| telco                   | 6.86 ms                                                | 6.50 ms: 1.06x faster                                                 |
| python_startup_no_site  | 6.01 ms                                                | 5.77 ms: 1.04x faster                                                 |
| gunicorn                | 1.20 ms                                                | 1.15 ms: 1.04x faster                                                 |
| coverage                | 78.8 ms                                                | 75.8 ms: 1.04x faster                                                 |
| xml_etree_parse         | 164 ms                                                 | 158 ms: 1.04x faster                                                  |
| async_generators        | 374 ms                                                 | 361 ms: 1.04x faster                                                  |
| pidigits                | 194 ms                                                 | 188 ms: 1.03x faster                                                  |
| scimark_sparse_mat_mult | 5.03 ms                                                | 4.86 ms: 1.03x faster                                                 |
| logging_simple          | 6.22 us                                                | 6.07 us: 1.02x faster                                                 |
| meteor_contest          | 109 ms                                                 | 106 ms: 1.02x faster                                                  |
| mdp                     | 2.77 sec                                               | 2.71 sec: 1.02x faster                                                |
| spectral_norm           | 108 ms                                                 | 106 ms: 1.02x faster                                                  |
| async_tree_none         | 528 ms                                                 | 518 ms: 1.02x faster                                                  |
| unpickle_list           | 5.21 us                                                | 5.13 us: 1.02x faster                                                 |
| logging_format          | 6.81 us                                                | 6.71 us: 1.02x faster                                                 |
| xml_etree_generate      | 81.1 ms                                                | 81.6 ms: 1.01x slower                                                 |
| sympy_sum               | 169 ms                                                 | 170 ms: 1.01x slower                                                  |
| pprint_pformat          | 1.55 sec                                               | 1.58 sec: 1.02x slower                                                |
| deepcopy_reduce         | 3.22 us                                                | 3.27 us: 1.02x slower                                                 |
| pprint_safe_repr        | 747 ms                                                 | 763 ms: 1.02x slower                                                  |
| pickle_list             | 4.59 us                                                | 4.68 us: 1.02x slower                                                 |
| xml_etree_iterparse     | 108 ms                                                 | 110 ms: 1.02x slower                                                  |
| regex_compile           | 141 ms                                                 | 145 ms: 1.02x slower                                                  |
| sqlalchemy_imperative   | 18.3 ms                                                | 18.8 ms: 1.02x slower                                                 |
| flaskblogging           | 7.28 ms                                                | 7.46 ms: 1.02x slower                                                 |
| scimark_fft             | 345 ms                                                 | 355 ms: 1.03x slower                                                  |
| sympy_str               | 297 ms                                                 | 306 ms: 1.03x slower                                                  |
| pathlib                 | 18.5 ms                                                | 19.1 ms: 1.03x slower                                                 |
| sqlalchemy_declarative  | 140 ms                                                 | 145 ms: 1.03x slower                                                  |
| sympy_integrate         | 21.5 ms                                                | 22.2 ms: 1.04x slower                                                 |
| 2to3                    | 264 ms                                                 | 274 ms: 1.04x slower                                                  |
| regex_v8                | 22.9 ms                                                | 23.7 ms: 1.04x slower                                                 |
| nqueens                 | 87.9 ms                                                | 91.4 ms: 1.04x slower                                                 |
| sympy_expand            | 484 ms                                                 | 505 ms: 1.04x slower                                                  |
| deepcopy                | 365 us                                                 | 382 us: 1.05x slower                                                  |
| xml_etree_process       | 56.9 ms                                                | 59.6 ms: 1.05x slower                                                 |
| thrift                  | 784 us                                                 | 821 us: 1.05x slower                                                  |
| genshi_xml              | 53.4 ms                                                | 56.1 ms: 1.05x slower                                                 |
| docutils                | 2.66 sec                                               | 2.79 sec: 1.05x slower                                                |
| logging_silent          | 111 ns                                                 | 117 ns: 1.05x slower                                                  |
| fannkuch                | 405 ms                                                 | 427 ms: 1.05x slower                                                  |
| float                   | 78.9 ms                                                | 83.3 ms: 1.05x slower                                                 |
| sqlglot_optimize        | 55.3 ms                                                | 58.4 ms: 1.06x slower                                                 |
| dulwich_log             | 64.6 ms                                                | 68.3 ms: 1.06x slower                                                 |
| raytrace                | 309 ms                                                 | 326 ms: 1.06x slower                                                  |
| async_tree_memoization  | 639 ms                                                 | 676 ms: 1.06x slower                                                  |
| sqlglot_normalize       | 113 ms                                                 | 119 ms: 1.06x slower                                                  |
| pycparser               | 1.19 sec                                               | 1.26 sec: 1.06x slower                                                |
| coroutines              | 27.0 ms                                                | 28.8 ms: 1.06x slower                                                 |
| regex_dna               | 205 ms                                                 | 219 ms: 1.07x slower                                                  |
| bench_thread_pool       | 834 us                                                 | 892 us: 1.07x slower                                                  |
| chaos                   | 71.9 ms                                                | 77.1 ms: 1.07x slower                                                 |
| sqlite_synth            | 2.57 us                                                | 2.76 us: 1.07x slower                                                 |
| hexiom                  | 6.89 ms                                                | 7.42 ms: 1.08x slower                                                 |
| async_tree_cpu_io_mixed | 749 ms                                                 | 818 ms: 1.09x slower                                                  |
| genshi_text             | 22.5 ms                                                | 24.6 ms: 1.09x slower                                                 |
| async_tree_io           | 1.29 sec                                               | 1.41 sec: 1.09x slower                                                |
| html5lib                | 64.8 ms                                                | 71.5 ms: 1.10x slower                                                 |
| scimark_monte_carlo     | 70.7 ms                                                | 78.4 ms: 1.11x slower                                                 |
| chameleon               | 6.70 ms                                                | 7.46 ms: 1.11x slower                                                 |
| richards                | 49.8 ms                                                | 55.7 ms: 1.12x slower                                                 |
| unpickle_pure_python    | 242 us                                                 | 271 us: 1.12x slower                                                  |
| go                      | 149 ms                                                 | 167 ms: 1.13x slower                                                  |
| tornado_http            | 98.1 ms                                                | 111 ms: 1.13x slower                                                  |
| django_template         | 33.5 ms                                                | 37.9 ms: 1.13x slower                                                 |
| mako                    | 10.7 ms                                                | 12.1 ms: 1.13x slower                                                 |
| pickle_pure_python      | 320 us                                                 | 364 us: 1.14x slower                                                  |
| nbody                   | 96.0 ms                                                | 112 ms: 1.17x slower                                                  |
| scimark_lu              | 116 ms                                                 | 136 ms: 1.17x slower                                                  |
| crypto_pyaes            | 76.7 ms                                                | 90.2 ms: 1.18x slower                                                 |
| deltablue               | 3.92 ms                                                | 4.86 ms: 1.24x slower                                                 |
| pyflate                 | 434 ms                                                 | 541 ms: 1.25x slower                                                  |
| scimark_sor             | 121 ms                                                 | 156 ms: 1.28x slower                                                  |
| sqlglot_transpile       | 1.75 ms                                                | 2.37 ms: 1.35x slower                                                 |
| sqlglot_parse           | 1.43 ms                                                | 2.06 ms: 1.44x slower                                                 |
| python_startup          | 8.56 ms                                                | 14.6 ms: 1.70x slower                                                 |
| Geometric mean          | (ref)                                                  | 1.05x slower                                                          |

Benchmark hidden because not significant (5): pylint, unpickle, bench_mp_pool, unpack_sequence, deepcopy_memo
Ignored benchmarks (17) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, comprehensions, create_gc_cycles, dask, djangocms, gc_traversal, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.03x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 1.00x