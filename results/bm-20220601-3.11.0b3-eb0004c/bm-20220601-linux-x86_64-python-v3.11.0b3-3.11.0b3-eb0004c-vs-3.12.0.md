
# Results vs. 3.12.0

- fork: python
- ref: v3.11.0b3
- machine: linux-x86_64
- commit hash: eb0004c
- commit date: 2022-06-01
- overall geometric mean: 1.04x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: 0.95x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220601-linux-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 256 ms: 1.07x faster                                       |
| chameleon      | 7.41 ms                                                | 6.42 ms: 1.15x faster                                      |
| docutils       | 2.77 sec                                               | 2.56 sec: 1.08x faster                                     |
| tornado_http   | 103 ms                                                 | 94.7 ms: 1.08x faster                                      |
| Geometric mean | (ref)                                                  | 1.10x faster                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220601-linux-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| async_tree_cpu_io_mixed | 726 ms                                                 | 735 ms: 1.01x slower                                       |
| async_tree_memoization  | 578 ms                                                 | 636 ms: 1.10x slower                                       |
| async_tree_none         | 472 ms                                                 | 525 ms: 1.11x slower                                       |
| async_tree_io           | 1.16 sec                                               | 1.30 sec: 1.13x slower                                     |
| Geometric mean          | (ref)                                                  | 1.09x slower                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220601-linux-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| float          | 84.7 ms                                                | 73.9 ms: 1.15x faster                                      |
| nbody          | 97.0 ms                                                | 94.9 ms: 1.02x faster                                      |
| pidigits       | 187 ms                                                 | 194 ms: 1.04x slower                                       |
| Geometric mean | (ref)                                                  | 1.04x faster                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220601-linux-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 2.92 ms: 1.24x faster                                      |
| regex_dna      | 212 ms                                                 | 194 ms: 1.09x faster                                       |
| regex_compile  | 148 ms                                                 | 136 ms: 1.09x faster                                       |
| regex_v8       | 23.1 ms                                                | 21.4 ms: 1.08x faster                                      |
| Geometric mean | (ref)                                                  | 1.12x faster                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220601-linux-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| pickle_dict          | 35.5 us                                                | 26.0 us: 1.37x faster                                      |
| pickle               | 11.6 us                                                | 9.37 us: 1.24x faster                                      |
| pickle_list          | 5.08 us                                                | 4.27 us: 1.19x faster                                      |
| unpickle             | 15.9 us                                                | 13.3 us: 1.19x faster                                      |
| xml_etree_generate   | 89.2 ms                                                | 76.7 ms: 1.16x faster                                      |
| xml_etree_process    | 61.7 ms                                                | 53.6 ms: 1.15x faster                                      |
| json_loads           | 28.5 us                                                | 24.9 us: 1.15x faster                                      |
| pickle_pure_python   | 324 us                                                 | 301 us: 1.08x faster                                       |
| unpickle_list        | 5.29 us                                                | 4.96 us: 1.07x faster                                      |
| unpickle_pure_python | 230 us                                                 | 227 us: 1.01x faster                                       |
| xml_etree_iterparse  | 107 ms                                                 | 108 ms: 1.01x slower                                       |
| json_dumps           | 10.4 ms                                                | 12.7 ms: 1.22x slower                                      |
| Geometric mean       | (ref)                                                  | 1.10x faster                                               |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220601-linux-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| python_startup_no_site | 6.94 ms                                                | 6.01 ms: 1.16x faster                                      |
| python_startup         | 9.55 ms                                                | 8.51 ms: 1.12x faster                                      |
| Geometric mean         | (ref)                                                  | 1.14x faster                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220601-linux-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| mako            | 11.9 ms                                                | 9.99 ms: 1.19x faster                                      |
| django_template | 34.6 ms                                                | 33.0 ms: 1.05x faster                                      |
| Geometric mean  | (ref)                                                  | 1.12x faster                                               |

All benchmarks:
===============

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220601-linux-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| pickle_dict             | 35.5 us                                                | 26.0 us: 1.37x faster                                      |
| async_generators        | 463 ms                                                 | 356 ms: 1.30x faster                                       |
| pickle                  | 11.6 us                                                | 9.37 us: 1.24x faster                                      |
| regex_effbot            | 3.61 ms                                                | 2.92 ms: 1.24x faster                                      |
| pickle_list             | 5.08 us                                                | 4.27 us: 1.19x faster                                      |
| mako                    | 11.9 ms                                                | 9.99 ms: 1.19x faster                                      |
| unpickle                | 15.9 us                                                | 13.3 us: 1.19x faster                                      |
| pyflate                 | 482 ms                                                 | 409 ms: 1.18x faster                                       |
| spectral_norm           | 115 ms                                                 | 97.5 ms: 1.18x faster                                      |
| scimark_fft             | 382 ms                                                 | 328 ms: 1.16x faster                                       |
| xml_etree_generate      | 89.2 ms                                                | 76.7 ms: 1.16x faster                                      |
| python_startup_no_site  | 6.94 ms                                                | 6.01 ms: 1.16x faster                                      |
| chameleon               | 7.41 ms                                                | 6.42 ms: 1.15x faster                                      |
| xml_etree_process       | 61.7 ms                                                | 53.6 ms: 1.15x faster                                      |
| float                   | 84.7 ms                                                | 73.9 ms: 1.15x faster                                      |
| json_loads              | 28.5 us                                                | 24.9 us: 1.15x faster                                      |
| logging_format          | 7.23 us                                                | 6.35 us: 1.14x faster                                      |
| scimark_sor             | 129 ms                                                 | 114 ms: 1.13x faster                                       |
| scimark_monte_carlo     | 75.1 ms                                                | 66.6 ms: 1.13x faster                                      |
| unpack_sequence         | 54.0 ns                                                | 48.0 ns: 1.13x faster                                      |
| python_startup          | 9.55 ms                                                | 8.51 ms: 1.12x faster                                      |
| deepcopy_reduce         | 3.35 us                                                | 2.98 us: 1.12x faster                                      |
| sqlite_synth            | 2.83 us                                                | 2.53 us: 1.12x faster                                      |
| pprint_safe_repr        | 776 ms                                                 | 694 ms: 1.12x faster                                       |
| crypto_pyaes            | 81.9 ms                                                | 73.6 ms: 1.11x faster                                      |
| logging_simple          | 6.46 us                                                | 5.82 us: 1.11x faster                                      |
| json                    | 5.26 ms                                                | 4.74 ms: 1.11x faster                                      |
| scimark_sparse_mat_mult | 5.06 ms                                                | 4.57 ms: 1.11x faster                                      |
| gunicorn                | 1.24 ms                                                | 1.12 ms: 1.11x faster                                      |
| deepcopy_memo           | 40.7 us                                                | 36.9 us: 1.10x faster                                      |
| scimark_lu              | 118 ms                                                 | 107 ms: 1.10x faster                                       |
| regex_dna               | 212 ms                                                 | 194 ms: 1.09x faster                                       |
| deepcopy                | 371 us                                                 | 340 us: 1.09x faster                                       |
| regex_compile           | 148 ms                                                 | 136 ms: 1.09x faster                                       |
| dulwich_log             | 68.5 ms                                                | 63.0 ms: 1.09x faster                                      |
| aiohttp                 | 1.15 ms                                                | 1.06 ms: 1.08x faster                                      |
| pprint_pformat          | 1.57 sec                                               | 1.45 sec: 1.08x faster                                     |
| tornado_http            | 103 ms                                                 | 94.7 ms: 1.08x faster                                      |
| docutils                | 2.77 sec                                               | 2.56 sec: 1.08x faster                                     |
| regex_v8                | 23.1 ms                                                | 21.4 ms: 1.08x faster                                      |
| telco                   | 7.10 ms                                                | 6.59 ms: 1.08x faster                                      |
| pickle_pure_python      | 324 us                                                 | 301 us: 1.08x faster                                       |
| meteor_contest          | 112 ms                                                 | 105 ms: 1.07x faster                                       |
| sqlalchemy_declarative  | 147 ms                                                 | 137 ms: 1.07x faster                                       |
| 2to3                    | 274 ms                                                 | 256 ms: 1.07x faster                                       |
| raytrace                | 312 ms                                                 | 292 ms: 1.07x faster                                       |
| pathlib                 | 19.3 ms                                                | 18.1 ms: 1.07x faster                                      |
| unpickle_list           | 5.29 us                                                | 4.96 us: 1.07x faster                                      |
| fannkuch                | 417 ms                                                 | 393 ms: 1.06x faster                                       |
| sympy_str               | 300 ms                                                 | 285 ms: 1.05x faster                                       |
| django_template         | 34.6 ms                                                | 33.0 ms: 1.05x faster                                      |
| sqlalchemy_imperative   | 18.7 ms                                                | 17.8 ms: 1.05x faster                                      |
| sympy_sum               | 169 ms                                                 | 162 ms: 1.04x faster                                       |
| sympy_integrate         | 21.4 ms                                                | 20.7 ms: 1.03x faster                                      |
| logging_silent          | 104 ns                                                 | 101 ns: 1.03x faster                                       |
| bench_thread_pool       | 842 us                                                 | 816 us: 1.03x faster                                       |
| nbody                   | 97.0 ms                                                | 94.9 ms: 1.02x faster                                      |
| sympy_expand            | 478 ms                                                 | 469 ms: 1.02x faster                                       |
| deltablue               | 3.72 ms                                                | 3.65 ms: 1.02x faster                                      |
| sqlglot_optimize        | 54.8 ms                                                | 54.0 ms: 1.01x faster                                      |
| unpickle_pure_python    | 230 us                                                 | 227 us: 1.01x faster                                       |
| richards                | 45.8 ms                                                | 45.3 ms: 1.01x faster                                      |
| dask                    | 372 ms                                                 | 368 ms: 1.01x faster                                       |
| sqlglot_normalize       | 110 ms                                                 | 109 ms: 1.01x faster                                       |
| hexiom                  | 6.41 ms                                                | 6.36 ms: 1.01x faster                                      |
| gc_traversal            | 3.79 ms                                                | 3.79 ms: 1.00x faster                                      |
| nqueens                 | 83.3 ms                                                | 83.8 ms: 1.01x slower                                      |
| xml_etree_iterparse     | 107 ms                                                 | 108 ms: 1.01x slower                                       |
| async_tree_cpu_io_mixed | 726 ms                                                 | 735 ms: 1.01x slower                                       |
| chaos                   | 67.0 ms                                                | 68.2 ms: 1.02x slower                                      |
| create_gc_cycles        | 1.48 ms                                                | 1.51 ms: 1.02x slower                                      |
| mdp                     | 2.63 sec                                               | 2.69 sec: 1.02x slower                                     |
| pidigits                | 187 ms                                                 | 194 ms: 1.04x slower                                       |
| async_tree_memoization  | 578 ms                                                 | 636 ms: 1.10x slower                                       |
| async_tree_none         | 472 ms                                                 | 525 ms: 1.11x slower                                       |
| coroutines              | 23.2 ms                                                | 26.0 ms: 1.12x slower                                      |
| async_tree_io           | 1.16 sec                                               | 1.30 sec: 1.13x slower                                     |
| comprehensions          | 21.8 us                                                | 25.9 us: 1.19x slower                                      |
| sqlglot_transpile       | 1.68 ms                                                | 2.04 ms: 1.21x slower                                      |
| json_dumps              | 10.4 ms                                                | 12.7 ms: 1.22x slower                                      |
| sqlglot_parse           | 1.36 ms                                                | 1.75 ms: 1.29x slower                                      |
| asyncio_tcp             | 491 ms                                                 | 888 ms: 1.81x slower                                       |
| generators              | 31.2 ms                                                | 73.8 ms: 2.36x slower                                      |
| Geometric mean          | (ref)                                                  | 1.04x faster                                               |

Benchmark hidden because not significant (4): xml_etree_parse, pycparser, go, bench_mp_pool
Ignored benchmarks (11) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, coverage, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (7) of results/bm-20220601-3.11.0b3-eb0004c/bm-20220601-linux-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c.json: djangocms, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 0.95x