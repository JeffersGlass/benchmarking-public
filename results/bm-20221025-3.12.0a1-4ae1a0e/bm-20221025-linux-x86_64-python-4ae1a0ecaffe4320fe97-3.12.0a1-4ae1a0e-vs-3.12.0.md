
# Results vs. 3.12.0

- fork: python
- ref: 4ae1a0ecaffe4320fe97
- machine: linux-x86_64
- commit hash: 4ae1a0e
- commit date: 2022-10-25
- overall geometric mean: 1.07x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x faster
- Memory change: 0.95x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 249 ms: 1.10x faster                                                  |
| chameleon      | 7.41 ms                                                | 6.51 ms: 1.14x faster                                                 |
| docutils       | 2.77 sec                                               | 2.52 sec: 1.10x faster                                                |
| tornado_http   | 103 ms                                                 | 93.7 ms: 1.10x faster                                                 |
| Geometric mean | (ref)                                                  | 1.11x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_none        | 472 ms                                                 | 529 ms: 1.12x slower                                                  |
| async_tree_memoization | 578 ms                                                 | 656 ms: 1.13x slower                                                  |
| async_tree_io          | 1.16 sec                                               | 1.33 sec: 1.15x slower                                                |
| Geometric mean         | (ref)                                                  | 1.10x slower                                                          |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| float          | 84.7 ms                                                | 71.4 ms: 1.19x faster                                                 |
| pidigits       | 187 ms                                                 | 198 ms: 1.06x slower                                                  |
| Geometric mean | (ref)                                                  | 1.04x faster                                                          |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 127 ms: 1.17x faster                                                  |
| regex_v8       | 23.1 ms                                                | 21.4 ms: 1.08x faster                                                 |
| regex_effbot   | 3.61 ms                                                | 3.37 ms: 1.07x faster                                                 |
| regex_dna      | 212 ms                                                 | 201 ms: 1.05x faster                                                  |
| Geometric mean | (ref)                                                  | 1.09x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| json_loads           | 28.5 us                                                | 23.5 us: 1.21x faster                                                 |
| pickle_list          | 5.08 us                                                | 4.19 us: 1.21x faster                                                 |
| unpickle             | 15.9 us                                                | 13.2 us: 1.20x faster                                                 |
| xml_etree_generate   | 89.2 ms                                                | 76.0 ms: 1.17x faster                                                 |
| xml_etree_process    | 61.7 ms                                                | 53.4 ms: 1.16x faster                                                 |
| pickle               | 11.6 us                                                | 10.1 us: 1.14x faster                                                 |
| pickle_dict          | 35.5 us                                                | 31.1 us: 1.14x faster                                                 |
| unpickle_pure_python | 230 us                                                 | 202 us: 1.14x faster                                                  |
| pickle_pure_python   | 324 us                                                 | 285 us: 1.14x faster                                                  |
| json_dumps           | 10.4 ms                                                | 9.36 ms: 1.11x faster                                                 |
| xml_etree_parse      | 159 ms                                                 | 145 ms: 1.10x faster                                                  |
| unpickle_list        | 5.29 us                                                | 4.91 us: 1.08x faster                                                 |
| xml_etree_iterparse  | 107 ms                                                 | 101 ms: 1.06x faster                                                  |
| Geometric mean       | (ref)                                                  | 1.14x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup_no_site | 6.94 ms                                                | 5.93 ms: 1.17x faster                                                 |
| python_startup         | 9.55 ms                                                | 8.42 ms: 1.14x faster                                                 |
| Geometric mean         | (ref)                                                  | 1.15x faster                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 11.9 ms                                                | 9.64 ms: 1.23x faster                                                 |
| django_template | 34.6 ms                                                | 33.0 ms: 1.05x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.14x faster                                                          |

All benchmarks:
===============

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_generators        | 463 ms                                                 | 349 ms: 1.33x faster                                                  |
| mako                    | 11.9 ms                                                | 9.64 ms: 1.23x faster                                                 |
| scimark_fft             | 382 ms                                                 | 312 ms: 1.22x faster                                                  |
| scimark_sparse_mat_mult | 5.06 ms                                                | 4.13 ms: 1.22x faster                                                 |
| unpack_sequence         | 54.0 ns                                                | 44.1 ns: 1.22x faster                                                 |
| scimark_sor             | 129 ms                                                 | 106 ms: 1.22x faster                                                  |
| json_loads              | 28.5 us                                                | 23.5 us: 1.21x faster                                                 |
| pickle_list             | 5.08 us                                                | 4.19 us: 1.21x faster                                                 |
| spectral_norm           | 115 ms                                                 | 95.2 ms: 1.21x faster                                                 |
| unpickle                | 15.9 us                                                | 13.2 us: 1.20x faster                                                 |
| float                   | 84.7 ms                                                | 71.4 ms: 1.19x faster                                                 |
| pyflate                 | 482 ms                                                 | 407 ms: 1.19x faster                                                  |
| deepcopy_memo           | 40.7 us                                                | 34.4 us: 1.18x faster                                                 |
| xml_etree_generate      | 89.2 ms                                                | 76.0 ms: 1.17x faster                                                 |
| python_startup_no_site  | 6.94 ms                                                | 5.93 ms: 1.17x faster                                                 |
| pprint_safe_repr        | 776 ms                                                 | 665 ms: 1.17x faster                                                  |
| regex_compile           | 148 ms                                                 | 127 ms: 1.17x faster                                                  |
| gunicorn                | 1.24 ms                                                | 1.07 ms: 1.16x faster                                                 |
| xml_etree_process       | 61.7 ms                                                | 53.4 ms: 1.16x faster                                                 |
| json                    | 5.26 ms                                                | 4.55 ms: 1.16x faster                                                 |
| deepcopy_reduce         | 3.35 us                                                | 2.91 us: 1.15x faster                                                 |
| aiohttp                 | 1.15 ms                                                | 1.00 ms: 1.15x faster                                                 |
| pickle                  | 11.6 us                                                | 10.1 us: 1.14x faster                                                 |
| pickle_dict             | 35.5 us                                                | 31.1 us: 1.14x faster                                                 |
| logging_silent          | 104 ns                                                 | 91.6 ns: 1.14x faster                                                 |
| pprint_pformat          | 1.57 sec                                               | 1.38 sec: 1.14x faster                                                |
| unpickle_pure_python    | 230 us                                                 | 202 us: 1.14x faster                                                  |
| chameleon               | 7.41 ms                                                | 6.51 ms: 1.14x faster                                                 |
| pickle_pure_python      | 324 us                                                 | 285 us: 1.14x faster                                                  |
| python_startup          | 9.55 ms                                                | 8.42 ms: 1.14x faster                                                 |
| logging_format          | 7.23 us                                                | 6.38 us: 1.13x faster                                                 |
| scimark_monte_carlo     | 75.1 ms                                                | 66.6 ms: 1.13x faster                                                 |
| fannkuch                | 417 ms                                                 | 370 ms: 1.13x faster                                                  |
| deltablue               | 3.72 ms                                                | 3.30 ms: 1.13x faster                                                 |
| deepcopy                | 371 us                                                 | 333 us: 1.12x faster                                                  |
| logging_simple          | 6.46 us                                                | 5.80 us: 1.11x faster                                                 |
| json_dumps              | 10.4 ms                                                | 9.36 ms: 1.11x faster                                                 |
| raytrace                | 312 ms                                                 | 282 ms: 1.11x faster                                                  |
| 2to3                    | 274 ms                                                 | 249 ms: 1.10x faster                                                  |
| docutils                | 2.77 sec                                               | 2.52 sec: 1.10x faster                                                |
| dulwich_log             | 68.5 ms                                                | 62.4 ms: 1.10x faster                                                 |
| xml_etree_parse         | 159 ms                                                 | 145 ms: 1.10x faster                                                  |
| tornado_http            | 103 ms                                                 | 93.7 ms: 1.10x faster                                                 |
| crypto_pyaes            | 81.9 ms                                                | 74.8 ms: 1.09x faster                                                 |
| scimark_lu              | 118 ms                                                 | 108 ms: 1.09x faster                                                  |
| telco                   | 7.10 ms                                                | 6.55 ms: 1.08x faster                                                 |
| regex_v8                | 23.1 ms                                                | 21.4 ms: 1.08x faster                                                 |
| richards                | 45.8 ms                                                | 42.4 ms: 1.08x faster                                                 |
| meteor_contest          | 112 ms                                                 | 104 ms: 1.08x faster                                                  |
| sqlite_synth            | 2.83 us                                                | 2.62 us: 1.08x faster                                                 |
| pathlib                 | 19.3 ms                                                | 17.9 ms: 1.08x faster                                                 |
| bench_thread_pool       | 842 us                                                 | 780 us: 1.08x faster                                                  |
| unpickle_list           | 5.29 us                                                | 4.91 us: 1.08x faster                                                 |
| regex_effbot            | 3.61 ms                                                | 3.37 ms: 1.07x faster                                                 |
| sqlglot_optimize        | 54.8 ms                                                | 51.2 ms: 1.07x faster                                                 |
| gc_traversal            | 3.79 ms                                                | 3.55 ms: 1.07x faster                                                 |
| xml_etree_iterparse     | 107 ms                                                 | 101 ms: 1.06x faster                                                  |
| mdp                     | 2.63 sec                                               | 2.48 sec: 1.06x faster                                                |
| sympy_str               | 300 ms                                                 | 283 ms: 1.06x faster                                                  |
| sqlglot_normalize       | 110 ms                                                 | 104 ms: 1.06x faster                                                  |
| pycparser               | 1.18 sec                                               | 1.12 sec: 1.06x faster                                                |
| regex_dna               | 212 ms                                                 | 201 ms: 1.05x faster                                                  |
| sympy_expand            | 478 ms                                                 | 455 ms: 1.05x faster                                                  |
| hexiom                  | 6.41 ms                                                | 6.11 ms: 1.05x faster                                                 |
| django_template         | 34.6 ms                                                | 33.0 ms: 1.05x faster                                                 |
| sympy_integrate         | 21.4 ms                                                | 20.4 ms: 1.05x faster                                                 |
| dask                    | 372 ms                                                 | 360 ms: 1.03x faster                                                  |
| nqueens                 | 83.3 ms                                                | 80.7 ms: 1.03x faster                                                 |
| sqlglot_transpile       | 1.68 ms                                                | 1.63 ms: 1.03x faster                                                 |
| go                      | 139 ms                                                 | 135 ms: 1.03x faster                                                  |
| sympy_sum               | 169 ms                                                 | 164 ms: 1.03x faster                                                  |
| comprehensions          | 21.8 us                                                | 21.3 us: 1.02x faster                                                 |
| sqlglot_parse           | 1.36 ms                                                | 1.34 ms: 1.02x faster                                                 |
| create_gc_cycles        | 1.48 ms                                                | 1.46 ms: 1.01x faster                                                 |
| pidigits                | 187 ms                                                 | 198 ms: 1.06x slower                                                  |
| coroutines              | 23.2 ms                                                | 24.7 ms: 1.06x slower                                                 |
| async_tree_none         | 472 ms                                                 | 529 ms: 1.12x slower                                                  |
| async_tree_memoization  | 578 ms                                                 | 656 ms: 1.13x slower                                                  |
| async_tree_io           | 1.16 sec                                               | 1.33 sec: 1.15x slower                                                |
| coverage                | 72.7 ms                                                | 102 ms: 1.40x slower                                                  |
| asyncio_tcp             | 491 ms                                                 | 890 ms: 1.81x slower                                                  |
| generators              | 31.2 ms                                                | 74.1 ms: 2.37x slower                                                 |
| Geometric mean          | (ref)                                                  | 1.07x faster                                                          |

Benchmark hidden because not significant (4): nbody, bench_mp_pool, chaos, async_tree_cpu_io_mixed
Ignored benchmarks (12) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
Ignored benchmarks (6) of results/bm-20221025-3.12.0a1-4ae1a0e/bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e.json: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.06x
- 95% likely to have a speedup of 1.05x
- 99% likely to have a speedup of 1.05x


# Memory

- memory change: 0.95x