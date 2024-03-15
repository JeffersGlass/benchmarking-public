
# Results vs. 3.12.0

- fork: python
- ref: 3d5d3f7af6498effbc60
- machine: linux-x86_64
- commit hash: 3d5d3f7
- commit date: 2023-01-10
- overall geometric mean: 1.07x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x faster
- Memory change: 0.94x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 253 ms: 1.09x faster                                                  |
| chameleon      | 7.41 ms                                                | 6.46 ms: 1.15x faster                                                 |
| docutils       | 2.77 sec                                               | 2.48 sec: 1.12x faster                                                |
| Geometric mean | (ref)                                                  | 1.12x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 726 ms                                                 | 747 ms: 1.03x slower                                                  |
| async_tree_memoization  | 578 ms                                                 | 616 ms: 1.07x slower                                                  |
| async_tree_none         | 472 ms                                                 | 521 ms: 1.10x slower                                                  |
| async_tree_io           | 1.16 sec                                               | 1.30 sec: 1.12x slower                                                |
| Geometric mean          | (ref)                                                  | 1.08x slower                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| float          | 84.7 ms                                                | 72.2 ms: 1.17x faster                                                 |
| nbody          | 97.0 ms                                                | 93.1 ms: 1.04x faster                                                 |
| pidigits       | 187 ms                                                 | 192 ms: 1.03x slower                                                  |
| Geometric mean | (ref)                                                  | 1.06x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 132 ms: 1.13x faster                                                  |
| regex_v8       | 23.1 ms                                                | 21.1 ms: 1.10x faster                                                 |
| regex_effbot   | 3.61 ms                                                | 3.49 ms: 1.03x faster                                                 |
| regex_dna      | 212 ms                                                 | 209 ms: 1.02x faster                                                  |
| Geometric mean | (ref)                                                  | 1.07x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pickle_list          | 5.08 us                                                | 4.02 us: 1.27x faster                                                 |
| unpickle             | 15.9 us                                                | 13.0 us: 1.22x faster                                                 |
| pickle_dict          | 35.5 us                                                | 30.0 us: 1.19x faster                                                 |
| json_loads           | 28.5 us                                                | 24.3 us: 1.17x faster                                                 |
| pickle               | 11.6 us                                                | 10.0 us: 1.16x faster                                                 |
| unpickle_pure_python | 230 us                                                 | 200 us: 1.15x faster                                                  |
| xml_etree_generate   | 89.2 ms                                                | 77.5 ms: 1.15x faster                                                 |
| xml_etree_process    | 61.7 ms                                                | 53.9 ms: 1.15x faster                                                 |
| pickle_pure_python   | 324 us                                                 | 285 us: 1.14x faster                                                  |
| json_dumps           | 10.4 ms                                                | 9.54 ms: 1.09x faster                                                 |
| xml_etree_parse      | 159 ms                                                 | 149 ms: 1.07x faster                                                  |
| unpickle_list        | 5.29 us                                                | 4.96 us: 1.07x faster                                                 |
| Geometric mean       | (ref)                                                  | 1.14x faster                                                          |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup_no_site | 6.94 ms                                                | 6.09 ms: 1.14x faster                                                 |
| python_startup         | 9.55 ms                                                | 8.54 ms: 1.12x faster                                                 |
| Geometric mean         | (ref)                                                  | 1.13x faster                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 11.9 ms                                                | 9.74 ms: 1.22x faster                                                 |
| django_template | 34.6 ms                                                | 32.6 ms: 1.06x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.14x faster                                                          |

All benchmarks:
===============

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_generators        | 463 ms                                                 | 354 ms: 1.31x faster                                                  |
| unpack_sequence         | 54.0 ns                                                | 41.4 ns: 1.30x faster                                                 |
| pickle_list             | 5.08 us                                                | 4.02 us: 1.27x faster                                                 |
| scimark_sparse_mat_mult | 5.06 ms                                                | 4.13 ms: 1.22x faster                                                 |
| unpickle                | 15.9 us                                                | 13.0 us: 1.22x faster                                                 |
| mako                    | 11.9 ms                                                | 9.74 ms: 1.22x faster                                                 |
| scimark_fft             | 382 ms                                                 | 314 ms: 1.22x faster                                                  |
| pyflate                 | 482 ms                                                 | 397 ms: 1.22x faster                                                  |
| spectral_norm           | 115 ms                                                 | 95.0 ms: 1.21x faster                                                 |
| scimark_sor             | 129 ms                                                 | 108 ms: 1.19x faster                                                  |
| pickle_dict             | 35.5 us                                                | 30.0 us: 1.19x faster                                                 |
| deepcopy_memo           | 40.7 us                                                | 34.7 us: 1.17x faster                                                 |
| float                   | 84.7 ms                                                | 72.2 ms: 1.17x faster                                                 |
| json_loads              | 28.5 us                                                | 24.3 us: 1.17x faster                                                 |
| pickle                  | 11.6 us                                                | 10.0 us: 1.16x faster                                                 |
| fannkuch                | 417 ms                                                 | 362 ms: 1.15x faster                                                  |
| unpickle_pure_python    | 230 us                                                 | 200 us: 1.15x faster                                                  |
| xml_etree_generate      | 89.2 ms                                                | 77.5 ms: 1.15x faster                                                 |
| chameleon               | 7.41 ms                                                | 6.46 ms: 1.15x faster                                                 |
| xml_etree_process       | 61.7 ms                                                | 53.9 ms: 1.15x faster                                                 |
| scimark_monte_carlo     | 75.1 ms                                                | 65.7 ms: 1.14x faster                                                 |
| deltablue               | 3.72 ms                                                | 3.25 ms: 1.14x faster                                                 |
| pprint_safe_repr        | 776 ms                                                 | 680 ms: 1.14x faster                                                  |
| python_startup_no_site  | 6.94 ms                                                | 6.09 ms: 1.14x faster                                                 |
| logging_format          | 7.23 us                                                | 6.35 us: 1.14x faster                                                 |
| pickle_pure_python      | 324 us                                                 | 285 us: 1.14x faster                                                  |
| pprint_pformat          | 1.57 sec                                               | 1.38 sec: 1.13x faster                                                |
| telco                   | 7.10 ms                                                | 6.26 ms: 1.13x faster                                                 |
| regex_compile           | 148 ms                                                 | 132 ms: 1.13x faster                                                  |
| logging_simple          | 6.46 us                                                | 5.77 us: 1.12x faster                                                 |
| deepcopy_reduce         | 3.35 us                                                | 2.99 us: 1.12x faster                                                 |
| python_startup          | 9.55 ms                                                | 8.54 ms: 1.12x faster                                                 |
| logging_silent          | 104 ns                                                 | 93.5 ns: 1.12x faster                                                 |
| docutils                | 2.77 sec                                               | 2.48 sec: 1.12x faster                                                |
| json                    | 5.26 ms                                                | 4.74 ms: 1.11x faster                                                 |
| dulwich_log             | 68.5 ms                                                | 62.1 ms: 1.10x faster                                                 |
| sqlite_synth            | 2.83 us                                                | 2.57 us: 1.10x faster                                                 |
| raytrace                | 312 ms                                                 | 284 ms: 1.10x faster                                                  |
| scimark_lu              | 118 ms                                                 | 107 ms: 1.10x faster                                                  |
| regex_v8                | 23.1 ms                                                | 21.1 ms: 1.10x faster                                                 |
| deepcopy                | 371 us                                                 | 339 us: 1.09x faster                                                  |
| pycparser               | 1.18 sec                                               | 1.08 sec: 1.09x faster                                                |
| json_dumps              | 10.4 ms                                                | 9.54 ms: 1.09x faster                                                 |
| 2to3                    | 274 ms                                                 | 253 ms: 1.09x faster                                                  |
| richards                | 45.8 ms                                                | 42.3 ms: 1.08x faster                                                 |
| crypto_pyaes            | 81.9 ms                                                | 75.7 ms: 1.08x faster                                                 |
| sqlglot_optimize        | 54.8 ms                                                | 50.7 ms: 1.08x faster                                                 |
| meteor_contest          | 112 ms                                                 | 104 ms: 1.08x faster                                                  |
| bench_thread_pool       | 842 us                                                 | 782 us: 1.08x faster                                                  |
| hexiom                  | 6.41 ms                                                | 5.98 ms: 1.07x faster                                                 |
| pathlib                 | 19.3 ms                                                | 18.0 ms: 1.07x faster                                                 |
| xml_etree_parse         | 159 ms                                                 | 149 ms: 1.07x faster                                                  |
| nqueens                 | 83.3 ms                                                | 78.0 ms: 1.07x faster                                                 |
| unpickle_list           | 5.29 us                                                | 4.96 us: 1.07x faster                                                 |
| gc_traversal            | 3.79 ms                                                | 3.57 ms: 1.06x faster                                                 |
| django_template         | 34.6 ms                                                | 32.6 ms: 1.06x faster                                                 |
| sympy_str               | 300 ms                                                 | 282 ms: 1.06x faster                                                  |
| sqlglot_normalize       | 110 ms                                                 | 104 ms: 1.06x faster                                                  |
| sympy_integrate         | 21.4 ms                                                | 20.3 ms: 1.05x faster                                                 |
| sympy_expand            | 478 ms                                                 | 455 ms: 1.05x faster                                                  |
| dask                    | 372 ms                                                 | 355 ms: 1.05x faster                                                  |
| nbody                   | 97.0 ms                                                | 93.1 ms: 1.04x faster                                                 |
| sympy_sum               | 169 ms                                                 | 163 ms: 1.04x faster                                                  |
| regex_effbot            | 3.61 ms                                                | 3.49 ms: 1.03x faster                                                 |
| go                      | 139 ms                                                 | 135 ms: 1.03x faster                                                  |
| create_gc_cycles        | 1.48 ms                                                | 1.45 ms: 1.02x faster                                                 |
| regex_dna               | 212 ms                                                 | 209 ms: 1.02x faster                                                  |
| mdp                     | 2.63 sec                                               | 2.66 sec: 1.01x slower                                                |
| chaos                   | 67.0 ms                                                | 67.7 ms: 1.01x slower                                                 |
| asyncio_tcp             | 491 ms                                                 | 504 ms: 1.03x slower                                                  |
| pidigits                | 187 ms                                                 | 192 ms: 1.03x slower                                                  |
| async_tree_cpu_io_mixed | 726 ms                                                 | 747 ms: 1.03x slower                                                  |
| sqlglot_parse           | 1.36 ms                                                | 1.41 ms: 1.03x slower                                                 |
| async_tree_memoization  | 578 ms                                                 | 616 ms: 1.07x slower                                                  |
| comprehensions          | 21.8 us                                                | 23.7 us: 1.09x slower                                                 |
| coroutines              | 23.2 ms                                                | 25.4 ms: 1.10x slower                                                 |
| async_tree_none         | 472 ms                                                 | 521 ms: 1.10x slower                                                  |
| async_tree_io           | 1.16 sec                                               | 1.30 sec: 1.12x slower                                                |
| coverage                | 72.7 ms                                                | 99.0 ms: 1.36x slower                                                 |
| generators              | 31.2 ms                                                | 79.1 ms: 2.53x slower                                                 |
| Geometric mean          | (ref)                                                  | 1.07x faster                                                          |

Benchmark hidden because not significant (3): xml_etree_iterparse, bench_mp_pool, sqlglot_transpile
Ignored benchmarks (15) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, gunicorn, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
Ignored benchmarks (5) of results/bm-20230110-3.12.0a4-3d5d3f7/bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7.json: djangocms, genshi_text, genshi_xml, html5lib, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.06x
- 95% likely to have a speedup of 1.06x
- 99% likely to have a speedup of 1.05x


# Memory

- memory change: 0.94x