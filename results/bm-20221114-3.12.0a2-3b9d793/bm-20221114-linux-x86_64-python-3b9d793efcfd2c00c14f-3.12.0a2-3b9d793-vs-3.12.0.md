
# Results vs. 3.12.0

- fork: python
- ref: 3b9d793efcfd2c00c14f
- machine: linux-x86_64
- commit hash: 3b9d793
- commit date: 2022-11-14
- overall geometric mean: 1.07x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x faster
- Memory change: 0.95x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-linux-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 245 ms: 1.12x faster                                                  |
| chameleon      | 7.41 ms                                                | 6.30 ms: 1.18x faster                                                 |
| docutils       | 2.77 sec                                               | 2.50 sec: 1.11x faster                                                |
| tornado_http   | 103 ms                                                 | 93.1 ms: 1.10x faster                                                 |
| Geometric mean | (ref)                                                  | 1.13x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-linux-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_none        | 472 ms                                                 | 527 ms: 1.12x slower                                                  |
| async_tree_memoization | 578 ms                                                 | 653 ms: 1.13x slower                                                  |
| async_tree_io          | 1.16 sec                                               | 1.32 sec: 1.14x slower                                                |
| Geometric mean         | (ref)                                                  | 1.10x slower                                                          |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-linux-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| float          | 84.7 ms                                                | 72.0 ms: 1.18x faster                                                 |
| nbody          | 97.0 ms                                                | 93.9 ms: 1.03x faster                                                 |
| pidigits       | 187 ms                                                 | 189 ms: 1.01x slower                                                  |
| Geometric mean | (ref)                                                  | 1.06x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-linux-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 127 ms: 1.17x faster                                                  |
| regex_v8       | 23.1 ms                                                | 21.1 ms: 1.10x faster                                                 |
| regex_effbot   | 3.61 ms                                                | 3.47 ms: 1.04x faster                                                 |
| regex_dna      | 212 ms                                                 | 208 ms: 1.02x faster                                                  |
| Geometric mean | (ref)                                                  | 1.08x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-linux-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pickle_list          | 5.08 us                                                | 4.06 us: 1.25x faster                                                 |
| unpickle             | 15.9 us                                                | 12.9 us: 1.23x faster                                                 |
| json_loads           | 28.5 us                                                | 23.9 us: 1.19x faster                                                 |
| pickle               | 11.6 us                                                | 9.88 us: 1.17x faster                                                 |
| xml_etree_generate   | 89.2 ms                                                | 77.2 ms: 1.15x faster                                                 |
| pickle_dict          | 35.5 us                                                | 30.8 us: 1.15x faster                                                 |
| unpickle_pure_python | 230 us                                                 | 200 us: 1.15x faster                                                  |
| xml_etree_process    | 61.7 ms                                                | 53.9 ms: 1.14x faster                                                 |
| pickle_pure_python   | 324 us                                                 | 283 us: 1.14x faster                                                  |
| json_dumps           | 10.4 ms                                                | 9.66 ms: 1.08x faster                                                 |
| xml_etree_parse      | 159 ms                                                 | 149 ms: 1.07x faster                                                  |
| unpickle_list        | 5.29 us                                                | 4.98 us: 1.06x faster                                                 |
| xml_etree_iterparse  | 107 ms                                                 | 103 ms: 1.04x faster                                                  |
| Geometric mean       | (ref)                                                  | 1.14x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-linux-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup_no_site | 6.94 ms                                                | 6.12 ms: 1.13x faster                                                 |
| python_startup         | 9.55 ms                                                | 8.58 ms: 1.11x faster                                                 |
| Geometric mean         | (ref)                                                  | 1.12x faster                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-linux-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 11.9 ms                                                | 9.39 ms: 1.27x faster                                                 |
| django_template | 34.6 ms                                                | 32.8 ms: 1.05x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.16x faster                                                          |

All benchmarks:
===============

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-linux-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_generators        | 463 ms                                                 | 355 ms: 1.30x faster                                                  |
| mako                    | 11.9 ms                                                | 9.39 ms: 1.27x faster                                                 |
| scimark_sparse_mat_mult | 5.06 ms                                                | 4.00 ms: 1.27x faster                                                 |
| pickle_list             | 5.08 us                                                | 4.06 us: 1.25x faster                                                 |
| scimark_fft             | 382 ms                                                 | 309 ms: 1.24x faster                                                  |
| scimark_sor             | 129 ms                                                 | 105 ms: 1.23x faster                                                  |
| unpickle                | 15.9 us                                                | 12.9 us: 1.23x faster                                                 |
| spectral_norm           | 115 ms                                                 | 94.9 ms: 1.21x faster                                                 |
| deepcopy_memo           | 40.7 us                                                | 33.6 us: 1.21x faster                                                 |
| pyflate                 | 482 ms                                                 | 402 ms: 1.20x faster                                                  |
| json_loads              | 28.5 us                                                | 23.9 us: 1.19x faster                                                 |
| unpack_sequence         | 54.0 ns                                                | 45.7 ns: 1.18x faster                                                 |
| chameleon               | 7.41 ms                                                | 6.30 ms: 1.18x faster                                                 |
| float                   | 84.7 ms                                                | 72.0 ms: 1.18x faster                                                 |
| pickle                  | 11.6 us                                                | 9.88 us: 1.17x faster                                                 |
| regex_compile           | 148 ms                                                 | 127 ms: 1.17x faster                                                  |
| deepcopy_reduce         | 3.35 us                                                | 2.89 us: 1.16x faster                                                 |
| xml_etree_generate      | 89.2 ms                                                | 77.2 ms: 1.15x faster                                                 |
| pickle_dict             | 35.5 us                                                | 30.8 us: 1.15x faster                                                 |
| deltablue               | 3.72 ms                                                | 3.22 ms: 1.15x faster                                                 |
| unpickle_pure_python    | 230 us                                                 | 200 us: 1.15x faster                                                  |
| gunicorn                | 1.24 ms                                                | 1.08 ms: 1.15x faster                                                 |
| aiohttp                 | 1.15 ms                                                | 999 us: 1.15x faster                                                  |
| logging_format          | 7.23 us                                                | 6.30 us: 1.15x faster                                                 |
| xml_etree_process       | 61.7 ms                                                | 53.9 ms: 1.14x faster                                                 |
| pickle_pure_python      | 324 us                                                 | 283 us: 1.14x faster                                                  |
| python_startup_no_site  | 6.94 ms                                                | 6.12 ms: 1.13x faster                                                 |
| logging_simple          | 6.46 us                                                | 5.70 us: 1.13x faster                                                 |
| deepcopy                | 371 us                                                 | 328 us: 1.13x faster                                                  |
| pprint_safe_repr        | 776 ms                                                 | 685 ms: 1.13x faster                                                  |
| fannkuch                | 417 ms                                                 | 369 ms: 1.13x faster                                                  |
| json                    | 5.26 ms                                                | 4.65 ms: 1.13x faster                                                 |
| raytrace                | 312 ms                                                 | 277 ms: 1.13x faster                                                  |
| pprint_pformat          | 1.57 sec                                               | 1.39 sec: 1.13x faster                                                |
| logging_silent          | 104 ns                                                 | 93.4 ns: 1.12x faster                                                 |
| 2to3                    | 274 ms                                                 | 245 ms: 1.12x faster                                                  |
| telco                   | 7.10 ms                                                | 6.38 ms: 1.11x faster                                                 |
| python_startup          | 9.55 ms                                                | 8.58 ms: 1.11x faster                                                 |
| dulwich_log             | 68.5 ms                                                | 61.8 ms: 1.11x faster                                                 |
| docutils                | 2.77 sec                                               | 2.50 sec: 1.11x faster                                                |
| scimark_monte_carlo     | 75.1 ms                                                | 68.0 ms: 1.10x faster                                                 |
| tornado_http            | 103 ms                                                 | 93.1 ms: 1.10x faster                                                 |
| meteor_contest          | 112 ms                                                 | 102 ms: 1.10x faster                                                  |
| regex_v8                | 23.1 ms                                                | 21.1 ms: 1.10x faster                                                 |
| crypto_pyaes            | 81.9 ms                                                | 74.6 ms: 1.10x faster                                                 |
| pycparser               | 1.18 sec                                               | 1.08 sec: 1.10x faster                                                |
| richards                | 45.8 ms                                                | 41.8 ms: 1.10x faster                                                 |
| scimark_lu              | 118 ms                                                 | 108 ms: 1.09x faster                                                  |
| pathlib                 | 19.3 ms                                                | 17.7 ms: 1.09x faster                                                 |
| sqlite_synth            | 2.83 us                                                | 2.60 us: 1.09x faster                                                 |
| bench_thread_pool       | 842 us                                                 | 780 us: 1.08x faster                                                  |
| json_dumps              | 10.4 ms                                                | 9.66 ms: 1.08x faster                                                 |
| sqlglot_optimize        | 54.8 ms                                                | 51.0 ms: 1.07x faster                                                 |
| xml_etree_parse         | 159 ms                                                 | 149 ms: 1.07x faster                                                  |
| sympy_str               | 300 ms                                                 | 282 ms: 1.06x faster                                                  |
| hexiom                  | 6.41 ms                                                | 6.04 ms: 1.06x faster                                                 |
| unpickle_list           | 5.29 us                                                | 4.98 us: 1.06x faster                                                 |
| mdp                     | 2.63 sec                                               | 2.48 sec: 1.06x faster                                                |
| django_template         | 34.6 ms                                                | 32.8 ms: 1.05x faster                                                 |
| sympy_integrate         | 21.4 ms                                                | 20.4 ms: 1.05x faster                                                 |
| sympy_expand            | 478 ms                                                 | 456 ms: 1.05x faster                                                  |
| sqlglot_normalize       | 110 ms                                                 | 105 ms: 1.05x faster                                                  |
| sqlglot_transpile       | 1.68 ms                                                | 1.62 ms: 1.04x faster                                                 |
| regex_effbot            | 3.61 ms                                                | 3.47 ms: 1.04x faster                                                 |
| go                      | 139 ms                                                 | 135 ms: 1.04x faster                                                  |
| xml_etree_iterparse     | 107 ms                                                 | 103 ms: 1.04x faster                                                  |
| nbody                   | 97.0 ms                                                | 93.9 ms: 1.03x faster                                                 |
| dask                    | 372 ms                                                 | 360 ms: 1.03x faster                                                  |
| nqueens                 | 83.3 ms                                                | 81.1 ms: 1.03x faster                                                 |
| sympy_sum               | 169 ms                                                 | 165 ms: 1.03x faster                                                  |
| sqlglot_parse           | 1.36 ms                                                | 1.33 ms: 1.02x faster                                                 |
| regex_dna               | 212 ms                                                 | 208 ms: 1.02x faster                                                  |
| chaos                   | 67.0 ms                                                | 65.8 ms: 1.02x faster                                                 |
| create_gc_cycles        | 1.48 ms                                                | 1.46 ms: 1.01x faster                                                 |
| gc_traversal            | 3.79 ms                                                | 3.77 ms: 1.01x faster                                                 |
| pidigits                | 187 ms                                                 | 189 ms: 1.01x slower                                                  |
| coroutines              | 23.2 ms                                                | 24.7 ms: 1.07x slower                                                 |
| comprehensions          | 21.8 us                                                | 23.4 us: 1.08x slower                                                 |
| async_tree_none         | 472 ms                                                 | 527 ms: 1.12x slower                                                  |
| async_tree_memoization  | 578 ms                                                 | 653 ms: 1.13x slower                                                  |
| async_tree_io           | 1.16 sec                                               | 1.32 sec: 1.14x slower                                                |
| coverage                | 72.7 ms                                                | 101 ms: 1.38x slower                                                  |
| asyncio_tcp             | 491 ms                                                 | 884 ms: 1.80x slower                                                  |
| generators              | 31.2 ms                                                | 77.4 ms: 2.48x slower                                                 |
| Geometric mean          | (ref)                                                  | 1.07x faster                                                          |

Benchmark hidden because not significant (2): bench_mp_pool, async_tree_cpu_io_mixed
Ignored benchmarks (12) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
Ignored benchmarks (5) of results/bm-20221114-3.12.0a2-3b9d793/bm-20221114-linux-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793.json: djangocms, genshi_text, genshi_xml, html5lib, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.06x
- 95% likely to have a speedup of 1.05x
- 99% likely to have a speedup of 1.05x


# Memory

- memory change: 0.95x