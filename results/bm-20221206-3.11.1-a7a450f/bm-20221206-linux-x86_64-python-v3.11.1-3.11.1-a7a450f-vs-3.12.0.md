
# Results vs. 3.12.0

- fork: python
- ref: v3.11.1
- machine: linux-x86_64
- commit hash: a7a450f
- commit date: 2022-12-06
- overall geometric mean: 1.03x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: 0.96x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-linux-x86_64-python-v3.11.1-3.11.1-a7a450f |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 258 ms: 1.06x faster                                   |
| chameleon      | 7.41 ms                                                | 6.63 ms: 1.12x faster                                  |
| docutils       | 2.77 sec                                               | 2.57 sec: 1.08x faster                                 |
| tornado_http   | 103 ms                                                 | 99.8 ms: 1.03x faster                                  |
| Geometric mean | (ref)                                                  | 1.07x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-linux-x86_64-python-v3.11.1-3.11.1-a7a450f |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_cpu_io_mixed | 726 ms                                                 | 742 ms: 1.02x slower                                   |
| async_tree_memoization  | 578 ms                                                 | 627 ms: 1.09x slower                                   |
| async_tree_none         | 472 ms                                                 | 523 ms: 1.11x slower                                   |
| async_tree_io           | 1.16 sec                                               | 1.31 sec: 1.13x slower                                 |
| Geometric mean          | (ref)                                                  | 1.09x slower                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-linux-x86_64-python-v3.11.1-3.11.1-a7a450f |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| float          | 84.7 ms                                                | 76.0 ms: 1.11x faster                                  |
| nbody          | 97.0 ms                                                | 95.4 ms: 1.02x faster                                  |
| pidigits       | 187 ms                                                 | 190 ms: 1.01x slower                                   |
| Geometric mean | (ref)                                                  | 1.04x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-linux-x86_64-python-v3.11.1-3.11.1-a7a450f |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.31 ms: 1.09x faster                                  |
| regex_compile  | 148 ms                                                 | 137 ms: 1.08x faster                                   |
| regex_dna      | 212 ms                                                 | 200 ms: 1.06x faster                                   |
| regex_v8       | 23.1 ms                                                | 22.3 ms: 1.04x faster                                  |
| Geometric mean | (ref)                                                  | 1.07x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-linux-x86_64-python-v3.11.1-3.11.1-a7a450f |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_list          | 5.08 us                                                | 4.17 us: 1.22x faster                                  |
| pickle               | 11.6 us                                                | 9.72 us: 1.19x faster                                  |
| json_loads           | 28.5 us                                                | 24.0 us: 1.19x faster                                  |
| unpickle             | 15.9 us                                                | 13.4 us: 1.19x faster                                  |
| xml_etree_generate   | 89.2 ms                                                | 76.6 ms: 1.16x faster                                  |
| xml_etree_process    | 61.7 ms                                                | 53.7 ms: 1.15x faster                                  |
| pickle_dict          | 35.5 us                                                | 31.1 us: 1.14x faster                                  |
| unpickle_list        | 5.29 us                                                | 4.95 us: 1.07x faster                                  |
| pickle_pure_python   | 324 us                                                 | 310 us: 1.05x faster                                   |
| xml_etree_iterparse  | 107 ms                                                 | 103 ms: 1.03x faster                                   |
| xml_etree_parse      | 159 ms                                                 | 158 ms: 1.01x faster                                   |
| unpickle_pure_python | 230 us                                                 | 229 us: 1.01x faster                                   |
| json_dumps           | 10.4 ms                                                | 12.6 ms: 1.21x slower                                  |
| Geometric mean       | (ref)                                                  | 1.09x faster                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-linux-x86_64-python-v3.11.1-3.11.1-a7a450f |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup_no_site | 6.94 ms                                                | 5.98 ms: 1.16x faster                                  |
| python_startup         | 9.55 ms                                                | 8.49 ms: 1.12x faster                                  |
| Geometric mean         | (ref)                                                  | 1.14x faster                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-linux-x86_64-python-v3.11.1-3.11.1-a7a450f |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako            | 11.9 ms                                                | 9.92 ms: 1.20x faster                                  |
| django_template | 34.6 ms                                                | 33.2 ms: 1.04x faster                                  |
| Geometric mean  | (ref)                                                  | 1.12x faster                                           |

All benchmarks:
===============

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-linux-x86_64-python-v3.11.1-3.11.1-a7a450f |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_generators        | 463 ms                                                 | 358 ms: 1.29x faster                                   |
| pickle_list             | 5.08 us                                                | 4.17 us: 1.22x faster                                  |
| unpack_sequence         | 54.0 ns                                                | 44.6 ns: 1.21x faster                                  |
| mako                    | 11.9 ms                                                | 9.92 ms: 1.20x faster                                  |
| pickle                  | 11.6 us                                                | 9.72 us: 1.19x faster                                  |
| json_loads              | 28.5 us                                                | 24.0 us: 1.19x faster                                  |
| unpickle                | 15.9 us                                                | 13.4 us: 1.19x faster                                  |
| scimark_fft             | 382 ms                                                 | 327 ms: 1.17x faster                                   |
| xml_etree_generate      | 89.2 ms                                                | 76.6 ms: 1.16x faster                                  |
| pyflate                 | 482 ms                                                 | 415 ms: 1.16x faster                                   |
| python_startup_no_site  | 6.94 ms                                                | 5.98 ms: 1.16x faster                                  |
| xml_etree_process       | 61.7 ms                                                | 53.7 ms: 1.15x faster                                  |
| sqlite_synth            | 2.83 us                                                | 2.47 us: 1.15x faster                                  |
| pickle_dict             | 35.5 us                                                | 31.1 us: 1.14x faster                                  |
| json                    | 5.26 ms                                                | 4.63 ms: 1.14x faster                                  |
| spectral_norm           | 115 ms                                                 | 101 ms: 1.13x faster                                   |
| crypto_pyaes            | 81.9 ms                                                | 72.6 ms: 1.13x faster                                  |
| python_startup          | 9.55 ms                                                | 8.49 ms: 1.12x faster                                  |
| chameleon               | 7.41 ms                                                | 6.63 ms: 1.12x faster                                  |
| float                   | 84.7 ms                                                | 76.0 ms: 1.11x faster                                  |
| scimark_sor             | 129 ms                                                 | 116 ms: 1.11x faster                                   |
| pprint_safe_repr        | 776 ms                                                 | 700 ms: 1.11x faster                                   |
| logging_format          | 7.23 us                                                | 6.54 us: 1.11x faster                                  |
| gunicorn                | 1.24 ms                                                | 1.13 ms: 1.10x faster                                  |
| scimark_sparse_mat_mult | 5.06 ms                                                | 4.59 ms: 1.10x faster                                  |
| scimark_lu              | 118 ms                                                 | 107 ms: 1.10x faster                                   |
| scimark_monte_carlo     | 75.1 ms                                                | 68.4 ms: 1.10x faster                                  |
| aiohttp                 | 1.15 ms                                                | 1.05 ms: 1.10x faster                                  |
| deepcopy_memo           | 40.7 us                                                | 37.2 us: 1.10x faster                                  |
| regex_effbot            | 3.61 ms                                                | 3.31 ms: 1.09x faster                                  |
| pprint_pformat          | 1.57 sec                                               | 1.44 sec: 1.09x faster                                 |
| fannkuch                | 417 ms                                                 | 384 ms: 1.09x faster                                   |
| logging_simple          | 6.46 us                                                | 5.95 us: 1.09x faster                                  |
| regex_compile           | 148 ms                                                 | 137 ms: 1.08x faster                                   |
| deepcopy_reduce         | 3.35 us                                                | 3.09 us: 1.08x faster                                  |
| dulwich_log             | 68.5 ms                                                | 63.5 ms: 1.08x faster                                  |
| docutils                | 2.77 sec                                               | 2.57 sec: 1.08x faster                                 |
| pathlib                 | 19.3 ms                                                | 18.1 ms: 1.07x faster                                  |
| unpickle_list           | 5.29 us                                                | 4.95 us: 1.07x faster                                  |
| telco                   | 7.10 ms                                                | 6.66 ms: 1.07x faster                                  |
| deepcopy                | 371 us                                                 | 349 us: 1.06x faster                                   |
| raytrace                | 312 ms                                                 | 294 ms: 1.06x faster                                   |
| 2to3                    | 274 ms                                                 | 258 ms: 1.06x faster                                   |
| meteor_contest          | 112 ms                                                 | 106 ms: 1.06x faster                                   |
| regex_dna               | 212 ms                                                 | 200 ms: 1.06x faster                                   |
| pickle_pure_python      | 324 us                                                 | 310 us: 1.05x faster                                   |
| django_template         | 34.6 ms                                                | 33.2 ms: 1.04x faster                                  |
| sqlalchemy_declarative  | 147 ms                                                 | 141 ms: 1.04x faster                                   |
| sqlalchemy_imperative   | 18.7 ms                                                | 18.0 ms: 1.04x faster                                  |
| regex_v8                | 23.1 ms                                                | 22.3 ms: 1.04x faster                                  |
| sympy_str               | 300 ms                                                 | 289 ms: 1.04x faster                                   |
| bench_thread_pool       | 842 us                                                 | 813 us: 1.04x faster                                   |
| xml_etree_iterparse     | 107 ms                                                 | 103 ms: 1.03x faster                                   |
| sqlglot_optimize        | 54.8 ms                                                | 53.3 ms: 1.03x faster                                  |
| tornado_http            | 103 ms                                                 | 99.8 ms: 1.03x faster                                  |
| logging_silent          | 104 ns                                                 | 102 ns: 1.02x faster                                   |
| sympy_integrate         | 21.4 ms                                                | 21.0 ms: 1.02x faster                                  |
| sympy_sum               | 169 ms                                                 | 166 ms: 1.02x faster                                   |
| dask                    | 372 ms                                                 | 365 ms: 1.02x faster                                   |
| sqlglot_normalize       | 110 ms                                                 | 108 ms: 1.02x faster                                   |
| nbody                   | 97.0 ms                                                | 95.4 ms: 1.02x faster                                  |
| deltablue               | 3.72 ms                                                | 3.67 ms: 1.01x faster                                  |
| pycparser               | 1.18 sec                                               | 1.16 sec: 1.01x faster                                 |
| sympy_expand            | 478 ms                                                 | 472 ms: 1.01x faster                                   |
| xml_etree_parse         | 159 ms                                                 | 158 ms: 1.01x faster                                   |
| unpickle_pure_python    | 230 us                                                 | 229 us: 1.01x faster                                   |
| create_gc_cycles        | 1.48 ms                                                | 1.48 ms: 1.00x slower                                  |
| hexiom                  | 6.41 ms                                                | 6.46 ms: 1.01x slower                                  |
| sqlglot_parse           | 1.36 ms                                                | 1.38 ms: 1.01x slower                                  |
| pidigits                | 187 ms                                                 | 190 ms: 1.01x slower                                   |
| nqueens                 | 83.3 ms                                                | 85.0 ms: 1.02x slower                                  |
| async_tree_cpu_io_mixed | 726 ms                                                 | 742 ms: 1.02x slower                                   |
| richards                | 45.8 ms                                                | 46.9 ms: 1.02x slower                                  |
| chaos                   | 67.0 ms                                                | 69.6 ms: 1.04x slower                                  |
| async_tree_memoization  | 578 ms                                                 | 627 ms: 1.09x slower                                   |
| coroutines              | 23.2 ms                                                | 25.3 ms: 1.09x slower                                  |
| async_tree_none         | 472 ms                                                 | 523 ms: 1.11x slower                                   |
| gc_traversal            | 3.79 ms                                                | 4.26 ms: 1.12x slower                                  |
| async_tree_io           | 1.16 sec                                               | 1.31 sec: 1.13x slower                                 |
| json_dumps              | 10.4 ms                                                | 12.6 ms: 1.21x slower                                  |
| coverage                | 72.7 ms                                                | 104 ms: 1.43x slower                                   |
| asyncio_tcp             | 491 ms                                                 | 889 ms: 1.81x slower                                   |
| generators              | 31.2 ms                                                | 73.3 ms: 2.35x slower                                  |
| Geometric mean          | (ref)                                                  | 1.03x faster                                           |

Benchmark hidden because not significant (4): sqlglot_transpile, bench_mp_pool, go, mdp
Ignored benchmarks (11) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, comprehensions, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (7) of results/bm-20221206-3.11.1-a7a450f/bm-20221206-linux-x86_64-python-v3.11.1-3.11.1-a7a450f.json: djangocms, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 0.96x