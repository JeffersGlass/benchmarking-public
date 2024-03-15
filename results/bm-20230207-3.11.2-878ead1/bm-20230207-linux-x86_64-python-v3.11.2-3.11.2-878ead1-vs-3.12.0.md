
# Results vs. 3.12.0

- fork: python
- ref: v3.11.2
- machine: linux-x86_64
- commit hash: 878ead1
- commit date: 2023-02-07
- overall geometric mean: 1.04x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 0.96x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-linux-x86_64-python-v3.11.2-3.11.2-878ead1 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 257 ms: 1.07x faster                                   |
| chameleon      | 7.41 ms                                                | 6.49 ms: 1.14x faster                                  |
| docutils       | 2.77 sec                                               | 2.55 sec: 1.09x faster                                 |
| tornado_http   | 103 ms                                                 | 96.1 ms: 1.07x faster                                  |
| Geometric mean | (ref)                                                  | 1.09x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-linux-x86_64-python-v3.11.2-3.11.2-878ead1 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_cpu_io_mixed | 726 ms                                                 | 740 ms: 1.02x slower                                   |
| async_tree_memoization  | 578 ms                                                 | 628 ms: 1.09x slower                                   |
| async_tree_none         | 472 ms                                                 | 524 ms: 1.11x slower                                   |
| async_tree_io           | 1.16 sec                                               | 1.30 sec: 1.12x slower                                 |
| Geometric mean          | (ref)                                                  | 1.08x slower                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-linux-x86_64-python-v3.11.2-3.11.2-878ead1 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| float          | 84.7 ms                                                | 76.6 ms: 1.11x faster                                  |
| nbody          | 97.0 ms                                                | 93.0 ms: 1.04x faster                                  |
| pidigits       | 187 ms                                                 | 190 ms: 1.01x slower                                   |
| Geometric mean | (ref)                                                  | 1.04x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-linux-x86_64-python-v3.11.2-3.11.2-878ead1 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_dna      | 212 ms                                                 | 192 ms: 1.10x faster                                   |
| regex_v8       | 23.1 ms                                                | 21.3 ms: 1.08x faster                                  |
| regex_compile  | 148 ms                                                 | 138 ms: 1.08x faster                                   |
| regex_effbot   | 3.61 ms                                                | 3.39 ms: 1.07x faster                                  |
| Geometric mean | (ref)                                                  | 1.08x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-linux-x86_64-python-v3.11.2-3.11.2-878ead1 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_list          | 5.08 us                                                | 4.16 us: 1.22x faster                                  |
| unpickle             | 15.9 us                                                | 13.2 us: 1.20x faster                                  |
| xml_etree_generate   | 89.2 ms                                                | 76.5 ms: 1.16x faster                                  |
| pickle               | 11.6 us                                                | 10.00 us: 1.16x faster                                 |
| xml_etree_process    | 61.7 ms                                                | 53.8 ms: 1.15x faster                                  |
| pickle_dict          | 35.5 us                                                | 31.4 us: 1.13x faster                                  |
| json_loads           | 28.5 us                                                | 26.2 us: 1.09x faster                                  |
| unpickle_list        | 5.29 us                                                | 4.94 us: 1.07x faster                                  |
| pickle_pure_python   | 324 us                                                 | 305 us: 1.06x faster                                   |
| xml_etree_iterparse  | 107 ms                                                 | 104 ms: 1.03x faster                                   |
| unpickle_pure_python | 230 us                                                 | 228 us: 1.01x faster                                   |
| json_dumps           | 10.4 ms                                                | 12.5 ms: 1.20x slower                                  |
| Geometric mean       | (ref)                                                  | 1.08x faster                                           |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-linux-x86_64-python-v3.11.2-3.11.2-878ead1 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup_no_site | 6.94 ms                                                | 5.97 ms: 1.16x faster                                  |
| python_startup         | 9.55 ms                                                | 8.47 ms: 1.13x faster                                  |
| Geometric mean         | (ref)                                                  | 1.14x faster                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-linux-x86_64-python-v3.11.2-3.11.2-878ead1 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako            | 11.9 ms                                                | 9.83 ms: 1.21x faster                                  |
| django_template | 34.6 ms                                                | 32.7 ms: 1.06x faster                                  |
| Geometric mean  | (ref)                                                  | 1.13x faster                                           |

All benchmarks:
===============

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-linux-x86_64-python-v3.11.2-3.11.2-878ead1 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_generators        | 463 ms                                                 | 357 ms: 1.30x faster                                   |
| pickle_list             | 5.08 us                                                | 4.16 us: 1.22x faster                                  |
| mako                    | 11.9 ms                                                | 9.83 ms: 1.21x faster                                  |
| unpickle                | 15.9 us                                                | 13.2 us: 1.20x faster                                  |
| spectral_norm           | 115 ms                                                 | 98.4 ms: 1.17x faster                                  |
| scimark_fft             | 382 ms                                                 | 327 ms: 1.17x faster                                   |
| xml_etree_generate      | 89.2 ms                                                | 76.5 ms: 1.16x faster                                  |
| python_startup_no_site  | 6.94 ms                                                | 5.97 ms: 1.16x faster                                  |
| pickle                  | 11.6 us                                                | 10.00 us: 1.16x faster                                 |
| pyflate                 | 482 ms                                                 | 417 ms: 1.16x faster                                   |
| sqlite_synth            | 2.83 us                                                | 2.46 us: 1.15x faster                                  |
| xml_etree_process       | 61.7 ms                                                | 53.8 ms: 1.15x faster                                  |
| chameleon               | 7.41 ms                                                | 6.49 ms: 1.14x faster                                  |
| pickle_dict             | 35.5 us                                                | 31.4 us: 1.13x faster                                  |
| python_startup          | 9.55 ms                                                | 8.47 ms: 1.13x faster                                  |
| scimark_sor             | 129 ms                                                 | 115 ms: 1.13x faster                                   |
| logging_format          | 7.23 us                                                | 6.49 us: 1.11x faster                                  |
| pprint_safe_repr        | 776 ms                                                 | 697 ms: 1.11x faster                                   |
| crypto_pyaes            | 81.9 ms                                                | 73.8 ms: 1.11x faster                                  |
| scimark_monte_carlo     | 75.1 ms                                                | 67.7 ms: 1.11x faster                                  |
| deepcopy_memo           | 40.7 us                                                | 36.8 us: 1.11x faster                                  |
| unpack_sequence         | 54.0 ns                                                | 48.8 ns: 1.11x faster                                  |
| float                   | 84.7 ms                                                | 76.6 ms: 1.11x faster                                  |
| scimark_lu              | 118 ms                                                 | 107 ms: 1.10x faster                                   |
| regex_dna               | 212 ms                                                 | 192 ms: 1.10x faster                                   |
| deepcopy_reduce         | 3.35 us                                                | 3.04 us: 1.10x faster                                  |
| gunicorn                | 1.24 ms                                                | 1.13 ms: 1.10x faster                                  |
| aiohttp                 | 1.15 ms                                                | 1.05 ms: 1.10x faster                                  |
| scimark_sparse_mat_mult | 5.06 ms                                                | 4.63 ms: 1.09x faster                                  |
| json_loads              | 28.5 us                                                | 26.2 us: 1.09x faster                                  |
| docutils                | 2.77 sec                                               | 2.55 sec: 1.09x faster                                 |
| pathlib                 | 19.3 ms                                                | 17.8 ms: 1.09x faster                                  |
| regex_v8                | 23.1 ms                                                | 21.3 ms: 1.08x faster                                  |
| pprint_pformat          | 1.57 sec                                               | 1.45 sec: 1.08x faster                                 |
| logging_simple          | 6.46 us                                                | 5.97 us: 1.08x faster                                  |
| telco                   | 7.10 ms                                                | 6.59 ms: 1.08x faster                                  |
| dulwich_log             | 68.5 ms                                                | 63.7 ms: 1.08x faster                                  |
| regex_compile           | 148 ms                                                 | 138 ms: 1.08x faster                                   |
| meteor_contest          | 112 ms                                                 | 105 ms: 1.07x faster                                   |
| raytrace                | 312 ms                                                 | 291 ms: 1.07x faster                                   |
| unpickle_list           | 5.29 us                                                | 4.94 us: 1.07x faster                                  |
| json                    | 5.26 ms                                                | 4.92 ms: 1.07x faster                                  |
| tornado_http            | 103 ms                                                 | 96.1 ms: 1.07x faster                                  |
| deepcopy                | 371 us                                                 | 348 us: 1.07x faster                                   |
| 2to3                    | 274 ms                                                 | 257 ms: 1.07x faster                                   |
| regex_effbot            | 3.61 ms                                                | 3.39 ms: 1.07x faster                                  |
| fannkuch                | 417 ms                                                 | 392 ms: 1.06x faster                                   |
| pycparser               | 1.18 sec                                               | 1.11 sec: 1.06x faster                                 |
| pickle_pure_python      | 324 us                                                 | 305 us: 1.06x faster                                   |
| django_template         | 34.6 ms                                                | 32.7 ms: 1.06x faster                                  |
| logging_silent          | 104 ns                                                 | 99.8 ns: 1.05x faster                                  |
| nbody                   | 97.0 ms                                                | 93.0 ms: 1.04x faster                                  |
| sympy_str               | 300 ms                                                 | 288 ms: 1.04x faster                                   |
| sqlalchemy_declarative  | 147 ms                                                 | 141 ms: 1.04x faster                                   |
| bench_thread_pool       | 842 us                                                 | 812 us: 1.04x faster                                   |
| sqlglot_optimize        | 54.8 ms                                                | 53.3 ms: 1.03x faster                                  |
| sqlalchemy_imperative   | 18.7 ms                                                | 18.2 ms: 1.03x faster                                  |
| xml_etree_iterparse     | 107 ms                                                 | 104 ms: 1.03x faster                                   |
| sympy_integrate         | 21.4 ms                                                | 20.8 ms: 1.03x faster                                  |
| sympy_expand            | 478 ms                                                 | 468 ms: 1.02x faster                                   |
| sympy_sum               | 169 ms                                                 | 166 ms: 1.02x faster                                   |
| dask                    | 372 ms                                                 | 365 ms: 1.02x faster                                   |
| sqlglot_normalize       | 110 ms                                                 | 109 ms: 1.02x faster                                   |
| deltablue               | 3.72 ms                                                | 3.68 ms: 1.01x faster                                  |
| sqlglot_transpile       | 1.68 ms                                                | 1.67 ms: 1.01x faster                                  |
| unpickle_pure_python    | 230 us                                                 | 228 us: 1.01x faster                                   |
| hexiom                  | 6.41 ms                                                | 6.36 ms: 1.01x faster                                  |
| create_gc_cycles        | 1.48 ms                                                | 1.49 ms: 1.01x slower                                  |
| sqlglot_parse           | 1.36 ms                                                | 1.38 ms: 1.01x slower                                  |
| pidigits                | 187 ms                                                 | 190 ms: 1.01x slower                                   |
| go                      | 139 ms                                                 | 141 ms: 1.01x slower                                   |
| chaos                   | 67.0 ms                                                | 68.2 ms: 1.02x slower                                  |
| async_tree_cpu_io_mixed | 726 ms                                                 | 740 ms: 1.02x slower                                   |
| mdp                     | 2.63 sec                                               | 2.77 sec: 1.05x slower                                 |
| async_tree_memoization  | 578 ms                                                 | 628 ms: 1.09x slower                                   |
| gc_traversal            | 3.79 ms                                                | 4.15 ms: 1.09x slower                                  |
| coroutines              | 23.2 ms                                                | 25.6 ms: 1.11x slower                                  |
| async_tree_none         | 472 ms                                                 | 524 ms: 1.11x slower                                   |
| async_tree_io           | 1.16 sec                                               | 1.30 sec: 1.12x slower                                 |
| json_dumps              | 10.4 ms                                                | 12.5 ms: 1.20x slower                                  |
| coverage                | 72.7 ms                                                | 103 ms: 1.42x slower                                   |
| asyncio_tcp             | 491 ms                                                 | 884 ms: 1.80x slower                                   |
| generators              | 31.2 ms                                                | 74.1 ms: 2.37x slower                                  |
| Geometric mean          | (ref)                                                  | 1.04x faster                                           |

Benchmark hidden because not significant (4): richards, nqueens, xml_etree_parse, bench_mp_pool
Ignored benchmarks (11) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, comprehensions, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (7) of results/bm-20230207-3.11.2-878ead1/bm-20230207-linux-x86_64-python-v3.11.2-3.11.2-878ead1.json: djangocms, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 0.96x