
# Results vs. 3.12.0

- fork: python
- ref: v3.11.0b2
- machine: linux-x86_64
- commit hash: 72f00f4
- commit date: 2022-05-30
- overall geometric mean: 1.04x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 0.95x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 256 ms: 1.07x faster                                       |
| chameleon      | 7.41 ms                                                | 6.62 ms: 1.12x faster                                      |
| docutils       | 2.77 sec                                               | 2.56 sec: 1.08x faster                                     |
| tornado_http   | 103 ms                                                 | 94.9 ms: 1.08x faster                                      |
| Geometric mean | (ref)                                                  | 1.09x faster                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| async_tree_cpu_io_mixed | 726 ms                                                 | 743 ms: 1.02x slower                                       |
| async_tree_memoization  | 578 ms                                                 | 628 ms: 1.09x slower                                       |
| async_tree_none         | 472 ms                                                 | 526 ms: 1.11x slower                                       |
| async_tree_io           | 1.16 sec                                               | 1.31 sec: 1.13x slower                                     |
| Geometric mean          | (ref)                                                  | 1.09x slower                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| float          | 84.7 ms                                                | 74.4 ms: 1.14x faster                                      |
| nbody          | 97.0 ms                                                | 92.0 ms: 1.05x faster                                      |
| pidigits       | 187 ms                                                 | 199 ms: 1.06x slower                                       |
| Geometric mean | (ref)                                                  | 1.04x faster                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.11 ms: 1.16x faster                                      |
| regex_dna      | 212 ms                                                 | 196 ms: 1.08x faster                                       |
| regex_compile  | 148 ms                                                 | 138 ms: 1.08x faster                                       |
| regex_v8       | 23.1 ms                                                | 22.0 ms: 1.05x faster                                      |
| Geometric mean | (ref)                                                  | 1.09x faster                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| pickle_dict          | 35.5 us                                                | 26.4 us: 1.34x faster                                      |
| pickle               | 11.6 us                                                | 9.44 us: 1.23x faster                                      |
| unpickle             | 15.9 us                                                | 13.3 us: 1.19x faster                                      |
| pickle_list          | 5.08 us                                                | 4.30 us: 1.18x faster                                      |
| xml_etree_generate   | 89.2 ms                                                | 76.1 ms: 1.17x faster                                      |
| xml_etree_process    | 61.7 ms                                                | 53.4 ms: 1.16x faster                                      |
| json_loads           | 28.5 us                                                | 25.0 us: 1.14x faster                                      |
| pickle_pure_python   | 324 us                                                 | 305 us: 1.06x faster                                       |
| unpickle_list        | 5.29 us                                                | 5.00 us: 1.06x faster                                      |
| unpickle_pure_python | 230 us                                                 | 227 us: 1.02x faster                                       |
| xml_etree_iterparse  | 107 ms                                                 | 105 ms: 1.01x faster                                       |
| json_dumps           | 10.4 ms                                                | 12.8 ms: 1.23x slower                                      |
| Geometric mean       | (ref)                                                  | 1.10x faster                                               |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| python_startup_no_site | 6.94 ms                                                | 5.99 ms: 1.16x faster                                      |
| python_startup         | 9.55 ms                                                | 8.49 ms: 1.12x faster                                      |
| Geometric mean         | (ref)                                                  | 1.14x faster                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| mako            | 11.9 ms                                                | 9.96 ms: 1.19x faster                                      |
| django_template | 34.6 ms                                                | 32.6 ms: 1.06x faster                                      |
| Geometric mean  | (ref)                                                  | 1.13x faster                                               |

All benchmarks:
===============

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| pickle_dict             | 35.5 us                                                | 26.4 us: 1.34x faster                                      |
| async_generators        | 463 ms                                                 | 354 ms: 1.31x faster                                       |
| pickle                  | 11.6 us                                                | 9.44 us: 1.23x faster                                      |
| mako                    | 11.9 ms                                                | 9.96 ms: 1.19x faster                                      |
| unpickle                | 15.9 us                                                | 13.3 us: 1.19x faster                                      |
| pickle_list             | 5.08 us                                                | 4.30 us: 1.18x faster                                      |
| spectral_norm           | 115 ms                                                 | 97.3 ms: 1.18x faster                                      |
| xml_etree_generate      | 89.2 ms                                                | 76.1 ms: 1.17x faster                                      |
| pyflate                 | 482 ms                                                 | 413 ms: 1.17x faster                                       |
| unpack_sequence         | 54.0 ns                                                | 46.2 ns: 1.17x faster                                      |
| regex_effbot            | 3.61 ms                                                | 3.11 ms: 1.16x faster                                      |
| scimark_fft             | 382 ms                                                 | 329 ms: 1.16x faster                                       |
| python_startup_no_site  | 6.94 ms                                                | 5.99 ms: 1.16x faster                                      |
| xml_etree_process       | 61.7 ms                                                | 53.4 ms: 1.16x faster                                      |
| logging_format          | 7.23 us                                                | 6.34 us: 1.14x faster                                      |
| json_loads              | 28.5 us                                                | 25.0 us: 1.14x faster                                      |
| scimark_monte_carlo     | 75.1 ms                                                | 66.0 ms: 1.14x faster                                      |
| float                   | 84.7 ms                                                | 74.4 ms: 1.14x faster                                      |
| deepcopy_memo           | 40.7 us                                                | 35.9 us: 1.14x faster                                      |
| logging_simple          | 6.46 us                                                | 5.74 us: 1.13x faster                                      |
| python_startup          | 9.55 ms                                                | 8.49 ms: 1.12x faster                                      |
| scimark_sor             | 129 ms                                                 | 115 ms: 1.12x faster                                       |
| sqlite_synth            | 2.83 us                                                | 2.52 us: 1.12x faster                                      |
| scimark_sparse_mat_mult | 5.06 ms                                                | 4.51 ms: 1.12x faster                                      |
| chameleon               | 7.41 ms                                                | 6.62 ms: 1.12x faster                                      |
| pprint_safe_repr        | 776 ms                                                 | 699 ms: 1.11x faster                                       |
| json                    | 5.26 ms                                                | 4.75 ms: 1.11x faster                                      |
| deepcopy_reduce         | 3.35 us                                                | 3.03 us: 1.10x faster                                      |
| gunicorn                | 1.24 ms                                                | 1.13 ms: 1.10x faster                                      |
| crypto_pyaes            | 81.9 ms                                                | 74.8 ms: 1.09x faster                                      |
| deepcopy                | 371 us                                                 | 340 us: 1.09x faster                                       |
| raytrace                | 312 ms                                                 | 287 ms: 1.09x faster                                       |
| aiohttp                 | 1.15 ms                                                | 1.06 ms: 1.09x faster                                      |
| dulwich_log             | 68.5 ms                                                | 63.1 ms: 1.09x faster                                      |
| telco                   | 7.10 ms                                                | 6.54 ms: 1.08x faster                                      |
| docutils                | 2.77 sec                                               | 2.56 sec: 1.08x faster                                     |
| pprint_pformat          | 1.57 sec                                               | 1.45 sec: 1.08x faster                                     |
| scimark_lu              | 118 ms                                                 | 109 ms: 1.08x faster                                       |
| tornado_http            | 103 ms                                                 | 94.9 ms: 1.08x faster                                      |
| regex_dna               | 212 ms                                                 | 196 ms: 1.08x faster                                       |
| regex_compile           | 148 ms                                                 | 138 ms: 1.08x faster                                       |
| meteor_contest          | 112 ms                                                 | 104 ms: 1.08x faster                                       |
| sqlalchemy_declarative  | 147 ms                                                 | 137 ms: 1.07x faster                                       |
| 2to3                    | 274 ms                                                 | 256 ms: 1.07x faster                                       |
| pathlib                 | 19.3 ms                                                | 18.1 ms: 1.07x faster                                      |
| pickle_pure_python      | 324 us                                                 | 305 us: 1.06x faster                                       |
| django_template         | 34.6 ms                                                | 32.6 ms: 1.06x faster                                      |
| unpickle_list           | 5.29 us                                                | 5.00 us: 1.06x faster                                      |
| nbody                   | 97.0 ms                                                | 92.0 ms: 1.05x faster                                      |
| regex_v8                | 23.1 ms                                                | 22.0 ms: 1.05x faster                                      |
| sympy_sum               | 169 ms                                                 | 161 ms: 1.05x faster                                       |
| sqlalchemy_imperative   | 18.7 ms                                                | 17.9 ms: 1.04x faster                                      |
| sympy_str               | 300 ms                                                 | 288 ms: 1.04x faster                                       |
| bench_thread_pool       | 842 us                                                 | 811 us: 1.04x faster                                       |
| sympy_integrate         | 21.4 ms                                                | 20.7 ms: 1.04x faster                                      |
| fannkuch                | 417 ms                                                 | 403 ms: 1.03x faster                                       |
| pycparser               | 1.18 sec                                               | 1.14 sec: 1.03x faster                                     |
| richards                | 45.8 ms                                                | 44.5 ms: 1.03x faster                                      |
| hexiom                  | 6.41 ms                                                | 6.27 ms: 1.02x faster                                      |
| sqlglot_optimize        | 54.8 ms                                                | 53.9 ms: 1.02x faster                                      |
| logging_silent          | 104 ns                                                 | 103 ns: 1.02x faster                                       |
| unpickle_pure_python    | 230 us                                                 | 227 us: 1.02x faster                                       |
| xml_etree_iterparse     | 107 ms                                                 | 105 ms: 1.01x faster                                       |
| dask                    | 372 ms                                                 | 368 ms: 1.01x faster                                       |
| sympy_expand            | 478 ms                                                 | 475 ms: 1.01x faster                                       |
| go                      | 139 ms                                                 | 139 ms: 1.00x faster                                       |
| chaos                   | 67.0 ms                                                | 67.3 ms: 1.01x slower                                      |
| nqueens                 | 83.3 ms                                                | 84.2 ms: 1.01x slower                                      |
| mdp                     | 2.63 sec                                               | 2.67 sec: 1.02x slower                                     |
| create_gc_cycles        | 1.48 ms                                                | 1.51 ms: 1.02x slower                                      |
| async_tree_cpu_io_mixed | 726 ms                                                 | 743 ms: 1.02x slower                                       |
| deltablue               | 3.72 ms                                                | 3.84 ms: 1.03x slower                                      |
| pidigits                | 187 ms                                                 | 199 ms: 1.06x slower                                       |
| async_tree_memoization  | 578 ms                                                 | 628 ms: 1.09x slower                                       |
| gc_traversal            | 3.79 ms                                                | 4.21 ms: 1.11x slower                                      |
| coroutines              | 23.2 ms                                                | 25.7 ms: 1.11x slower                                      |
| async_tree_none         | 472 ms                                                 | 526 ms: 1.11x slower                                       |
| async_tree_io           | 1.16 sec                                               | 1.31 sec: 1.13x slower                                     |
| comprehensions          | 21.8 us                                                | 26.0 us: 1.19x slower                                      |
| sqlglot_transpile       | 1.68 ms                                                | 2.05 ms: 1.21x slower                                      |
| json_dumps              | 10.4 ms                                                | 12.8 ms: 1.23x slower                                      |
| sqlglot_parse           | 1.36 ms                                                | 1.75 ms: 1.29x slower                                      |
| asyncio_tcp             | 491 ms                                                 | 890 ms: 1.81x slower                                       |
| generators              | 31.2 ms                                                | 74.4 ms: 2.38x slower                                      |
| Geometric mean          | (ref)                                                  | 1.04x faster                                               |

Benchmark hidden because not significant (3): xml_etree_parse, sqlglot_normalize, bench_mp_pool
Ignored benchmarks (11) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, coverage, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (6) of results/bm-20220530-3.11.0b2-72f00f4/bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4.json: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 0.95x