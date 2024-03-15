
# Results vs. 3.12.0

- fork: python
- ref: b6bd7ffcbc1ffaa68e34
- machine: linux-x86_64
- commit hash: b6bd7ff
- commit date: 2022-12-06
- overall geometric mean: 1.06x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x faster
- Memory change: 0.95x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 246 ms: 1.12x faster                                                  |
| chameleon      | 7.41 ms                                                | 6.45 ms: 1.15x faster                                                 |
| docutils       | 2.77 sec                                               | 2.57 sec: 1.08x faster                                                |
| Geometric mean | (ref)                                                  | 1.11x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 726 ms                                                 | 769 ms: 1.06x slower                                                  |
| async_tree_none         | 472 ms                                                 | 536 ms: 1.14x slower                                                  |
| async_tree_memoization  | 578 ms                                                 | 665 ms: 1.15x slower                                                  |
| async_tree_io           | 1.16 sec                                               | 1.34 sec: 1.16x slower                                                |
| Geometric mean          | (ref)                                                  | 1.13x slower                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| float          | 84.7 ms                                                | 73.2 ms: 1.16x faster                                                 |
| nbody          | 97.0 ms                                                | 94.0 ms: 1.03x faster                                                 |
| pidigits       | 187 ms                                                 | 189 ms: 1.01x slower                                                  |
| Geometric mean | (ref)                                                  | 1.06x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 129 ms: 1.15x faster                                                  |
| regex_v8       | 23.1 ms                                                | 22.3 ms: 1.04x faster                                                 |
| regex_effbot   | 3.61 ms                                                | 3.63 ms: 1.01x slower                                                 |
| regex_dna      | 212 ms                                                 | 217 ms: 1.02x slower                                                  |
| Geometric mean | (ref)                                                  | 1.04x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pickle_list          | 5.08 us                                                | 3.95 us: 1.29x faster                                                 |
| json_loads           | 28.5 us                                                | 23.8 us: 1.20x faster                                                 |
| unpickle             | 15.9 us                                                | 13.3 us: 1.19x faster                                                 |
| xml_etree_generate   | 89.2 ms                                                | 76.9 ms: 1.16x faster                                                 |
| xml_etree_process    | 61.7 ms                                                | 53.7 ms: 1.15x faster                                                 |
| unpickle_pure_python | 230 us                                                 | 200 us: 1.15x faster                                                  |
| pickle_pure_python   | 324 us                                                 | 282 us: 1.15x faster                                                  |
| pickle               | 11.6 us                                                | 10.1 us: 1.14x faster                                                 |
| pickle_dict          | 35.5 us                                                | 31.5 us: 1.13x faster                                                 |
| json_dumps           | 10.4 ms                                                | 9.52 ms: 1.09x faster                                                 |
| xml_etree_parse      | 159 ms                                                 | 148 ms: 1.08x faster                                                  |
| unpickle_list        | 5.29 us                                                | 4.97 us: 1.06x faster                                                 |
| xml_etree_iterparse  | 107 ms                                                 | 104 ms: 1.02x faster                                                  |
| Geometric mean       | (ref)                                                  | 1.14x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup_no_site | 6.94 ms                                                | 6.07 ms: 1.14x faster                                                 |
| python_startup         | 9.55 ms                                                | 8.52 ms: 1.12x faster                                                 |
| Geometric mean         | (ref)                                                  | 1.13x faster                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 11.9 ms                                                | 9.43 ms: 1.26x faster                                                 |
| django_template | 34.6 ms                                                | 33.0 ms: 1.05x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.15x faster                                                          |

All benchmarks:
===============

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_generators        | 463 ms                                                 | 354 ms: 1.31x faster                                                  |
| pickle_list             | 5.08 us                                                | 3.95 us: 1.29x faster                                                 |
| mako                    | 11.9 ms                                                | 9.43 ms: 1.26x faster                                                 |
| unpack_sequence         | 54.0 ns                                                | 43.1 ns: 1.25x faster                                                 |
| scimark_sor             | 129 ms                                                 | 105 ms: 1.23x faster                                                  |
| scimark_fft             | 382 ms                                                 | 314 ms: 1.22x faster                                                  |
| scimark_sparse_mat_mult | 5.06 ms                                                | 4.20 ms: 1.20x faster                                                 |
| spectral_norm           | 115 ms                                                 | 96.0 ms: 1.20x faster                                                 |
| json_loads              | 28.5 us                                                | 23.8 us: 1.20x faster                                                 |
| pyflate                 | 482 ms                                                 | 405 ms: 1.19x faster                                                  |
| deepcopy_memo           | 40.7 us                                                | 34.2 us: 1.19x faster                                                 |
| unpickle                | 15.9 us                                                | 13.3 us: 1.19x faster                                                 |
| xml_etree_generate      | 89.2 ms                                                | 76.9 ms: 1.16x faster                                                 |
| float                   | 84.7 ms                                                | 73.2 ms: 1.16x faster                                                 |
| deltablue               | 3.72 ms                                                | 3.22 ms: 1.15x faster                                                 |
| regex_compile           | 148 ms                                                 | 129 ms: 1.15x faster                                                  |
| xml_etree_process       | 61.7 ms                                                | 53.7 ms: 1.15x faster                                                 |
| chameleon               | 7.41 ms                                                | 6.45 ms: 1.15x faster                                                 |
| logging_silent          | 104 ns                                                 | 90.9 ns: 1.15x faster                                                 |
| scimark_monte_carlo     | 75.1 ms                                                | 65.4 ms: 1.15x faster                                                 |
| unpickle_pure_python    | 230 us                                                 | 200 us: 1.15x faster                                                  |
| pickle_pure_python      | 324 us                                                 | 282 us: 1.15x faster                                                  |
| pickle                  | 11.6 us                                                | 10.1 us: 1.14x faster                                                 |
| python_startup_no_site  | 6.94 ms                                                | 6.07 ms: 1.14x faster                                                 |
| pprint_safe_repr        | 776 ms                                                 | 686 ms: 1.13x faster                                                  |
| logging_format          | 7.23 us                                                | 6.41 us: 1.13x faster                                                 |
| deepcopy_reduce         | 3.35 us                                                | 2.97 us: 1.13x faster                                                 |
| pickle_dict             | 35.5 us                                                | 31.5 us: 1.13x faster                                                 |
| json                    | 5.26 ms                                                | 4.67 ms: 1.13x faster                                                 |
| python_startup          | 9.55 ms                                                | 8.52 ms: 1.12x faster                                                 |
| deepcopy                | 371 us                                                 | 332 us: 1.12x faster                                                  |
| 2to3                    | 274 ms                                                 | 246 ms: 1.12x faster                                                  |
| raytrace                | 312 ms                                                 | 281 ms: 1.11x faster                                                  |
| scimark_lu              | 118 ms                                                 | 106 ms: 1.11x faster                                                  |
| pprint_pformat          | 1.57 sec                                               | 1.41 sec: 1.11x faster                                                |
| fannkuch                | 417 ms                                                 | 379 ms: 1.10x faster                                                  |
| telco                   | 7.10 ms                                                | 6.46 ms: 1.10x faster                                                 |
| logging_simple          | 6.46 us                                                | 5.88 us: 1.10x faster                                                 |
| sqlite_synth            | 2.83 us                                                | 2.58 us: 1.10x faster                                                 |
| dulwich_log             | 68.5 ms                                                | 62.5 ms: 1.10x faster                                                 |
| richards                | 45.8 ms                                                | 42.0 ms: 1.09x faster                                                 |
| json_dumps              | 10.4 ms                                                | 9.52 ms: 1.09x faster                                                 |
| crypto_pyaes            | 81.9 ms                                                | 75.3 ms: 1.09x faster                                                 |
| sqlglot_optimize        | 54.8 ms                                                | 50.6 ms: 1.08x faster                                                 |
| bench_thread_pool       | 842 us                                                 | 778 us: 1.08x faster                                                  |
| meteor_contest          | 112 ms                                                 | 104 ms: 1.08x faster                                                  |
| pycparser               | 1.18 sec                                               | 1.09 sec: 1.08x faster                                                |
| docutils                | 2.77 sec                                               | 2.57 sec: 1.08x faster                                                |
| xml_etree_parse         | 159 ms                                                 | 148 ms: 1.08x faster                                                  |
| unpickle_list           | 5.29 us                                                | 4.97 us: 1.06x faster                                                 |
| pathlib                 | 19.3 ms                                                | 18.3 ms: 1.06x faster                                                 |
| sympy_str               | 300 ms                                                 | 283 ms: 1.06x faster                                                  |
| hexiom                  | 6.41 ms                                                | 6.08 ms: 1.05x faster                                                 |
| mdp                     | 2.63 sec                                               | 2.50 sec: 1.05x faster                                                |
| sqlglot_normalize       | 110 ms                                                 | 105 ms: 1.05x faster                                                  |
| django_template         | 34.6 ms                                                | 33.0 ms: 1.05x faster                                                 |
| sympy_integrate         | 21.4 ms                                                | 20.4 ms: 1.05x faster                                                 |
| sympy_expand            | 478 ms                                                 | 458 ms: 1.04x faster                                                  |
| nqueens                 | 83.3 ms                                                | 80.1 ms: 1.04x faster                                                 |
| regex_v8                | 23.1 ms                                                | 22.3 ms: 1.04x faster                                                 |
| dask                    | 372 ms                                                 | 360 ms: 1.03x faster                                                  |
| nbody                   | 97.0 ms                                                | 94.0 ms: 1.03x faster                                                 |
| sqlglot_transpile       | 1.68 ms                                                | 1.63 ms: 1.03x faster                                                 |
| sympy_sum               | 169 ms                                                 | 164 ms: 1.03x faster                                                  |
| go                      | 139 ms                                                 | 136 ms: 1.03x faster                                                  |
| create_gc_cycles        | 1.48 ms                                                | 1.44 ms: 1.03x faster                                                 |
| xml_etree_iterparse     | 107 ms                                                 | 104 ms: 1.02x faster                                                  |
| sqlglot_parse           | 1.36 ms                                                | 1.34 ms: 1.01x faster                                                 |
| regex_effbot            | 3.61 ms                                                | 3.63 ms: 1.01x slower                                                 |
| gc_traversal            | 3.79 ms                                                | 3.81 ms: 1.01x slower                                                 |
| pidigits                | 187 ms                                                 | 189 ms: 1.01x slower                                                  |
| regex_dna               | 212 ms                                                 | 217 ms: 1.02x slower                                                  |
| async_tree_cpu_io_mixed | 726 ms                                                 | 769 ms: 1.06x slower                                                  |
| coroutines              | 23.2 ms                                                | 25.0 ms: 1.08x slower                                                 |
| comprehensions          | 21.8 us                                                | 23.5 us: 1.08x slower                                                 |
| async_tree_none         | 472 ms                                                 | 536 ms: 1.14x slower                                                  |
| async_tree_memoization  | 578 ms                                                 | 665 ms: 1.15x slower                                                  |
| async_tree_io           | 1.16 sec                                               | 1.34 sec: 1.16x slower                                                |
| coverage                | 72.7 ms                                                | 102 ms: 1.41x slower                                                  |
| asyncio_tcp             | 491 ms                                                 | 890 ms: 1.81x slower                                                  |
| generators              | 31.2 ms                                                | 79.1 ms: 2.53x slower                                                 |
| Geometric mean          | (ref)                                                  | 1.06x faster                                                          |

Benchmark hidden because not significant (2): chaos, bench_mp_pool
Ignored benchmarks (15) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, gunicorn, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
Ignored benchmarks (5) of results/bm-20221206-3.12.0a3-b6bd7ff/bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff.json: djangocms, genshi_text, genshi_xml, html5lib, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.05x
- 95% likely to have a speedup of 1.05x
- 99% likely to have a speedup of 1.04x


# Memory

- memory change: 0.95x