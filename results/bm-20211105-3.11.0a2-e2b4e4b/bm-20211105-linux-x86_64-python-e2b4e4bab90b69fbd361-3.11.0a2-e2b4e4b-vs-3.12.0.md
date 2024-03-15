
# Results vs. 3.12.0

- fork: python
- ref: e2b4e4bab90b69fbd361
- machine: linux-x86_64
- commit hash: e2b4e4b
- commit date: 2021-11-05
- overall geometric mean: 1.04x slower \*
- HPT reliability: 99.97%
- HPT 99th percentile: 1.01x slower
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 274 ms: 1.00x faster                                                  |
| chameleon      | 7.41 ms                                                | 7.46 ms: 1.01x slower                                                 |
| docutils       | 2.77 sec                                               | 2.79 sec: 1.01x slower                                                |
| tornado_http   | 103 ms                                                 | 111 ms: 1.08x slower                                                  |
| Geometric mean | (ref)                                                  | 1.02x slower                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_none         | 472 ms                                                 | 518 ms: 1.10x slower                                                  |
| async_tree_cpu_io_mixed | 726 ms                                                 | 818 ms: 1.13x slower                                                  |
| async_tree_memoization  | 578 ms                                                 | 676 ms: 1.17x slower                                                  |
| async_tree_io           | 1.16 sec                                               | 1.41 sec: 1.22x slower                                                |
| Geometric mean          | (ref)                                                  | 1.15x slower                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| float          | 84.7 ms                                                | 83.3 ms: 1.02x faster                                                 |
| pidigits       | 187 ms                                                 | 188 ms: 1.00x slower                                                  |
| nbody          | 97.0 ms                                                | 112 ms: 1.15x slower                                                  |
| Geometric mean | (ref)                                                  | 1.04x slower                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.26 ms: 1.11x faster                                                 |
| regex_compile  | 148 ms                                                 | 145 ms: 1.03x faster                                                  |
| regex_v8       | 23.1 ms                                                | 23.7 ms: 1.03x slower                                                 |
| regex_dna      | 212 ms                                                 | 219 ms: 1.03x slower                                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pickle_dict          | 35.5 us                                                | 28.6 us: 1.24x faster                                                 |
| unpickle             | 15.9 us                                                | 13.7 us: 1.16x faster                                                 |
| pickle               | 11.6 us                                                | 10.1 us: 1.15x faster                                                 |
| json_loads           | 28.5 us                                                | 25.9 us: 1.10x faster                                                 |
| xml_etree_generate   | 89.2 ms                                                | 81.6 ms: 1.09x faster                                                 |
| pickle_list          | 5.08 us                                                | 4.68 us: 1.09x faster                                                 |
| xml_etree_process    | 61.7 ms                                                | 59.6 ms: 1.04x faster                                                 |
| unpickle_list        | 5.29 us                                                | 5.13 us: 1.03x faster                                                 |
| xml_etree_iterparse  | 107 ms                                                 | 110 ms: 1.03x slower                                                  |
| pickle_pure_python   | 324 us                                                 | 364 us: 1.12x slower                                                  |
| unpickle_pure_python | 230 us                                                 | 271 us: 1.18x slower                                                  |
| json_dumps           | 10.4 ms                                                | 12.4 ms: 1.19x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                          |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup_no_site | 6.94 ms                                                | 5.77 ms: 1.20x faster                                                 |
| python_startup         | 9.55 ms                                                | 14.6 ms: 1.52x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.13x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 11.9 ms                                                | 12.1 ms: 1.02x slower                                                 |
| django_template | 34.6 ms                                                | 37.9 ms: 1.10x slower                                                 |
| Geometric mean  | (ref)                                                  | 1.06x slower                                                          |

All benchmarks:
===============

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_generators        | 463 ms                                                 | 361 ms: 1.28x faster                                                  |
| pickle_dict             | 35.5 us                                                | 28.6 us: 1.24x faster                                                 |
| unpack_sequence         | 54.0 ns                                                | 43.6 ns: 1.24x faster                                                 |
| python_startup_no_site  | 6.94 ms                                                | 5.77 ms: 1.20x faster                                                 |
| unpickle                | 15.9 us                                                | 13.7 us: 1.16x faster                                                 |
| pickle                  | 11.6 us                                                | 10.1 us: 1.15x faster                                                 |
| regex_effbot            | 3.61 ms                                                | 3.26 ms: 1.11x faster                                                 |
| json_loads              | 28.5 us                                                | 25.9 us: 1.10x faster                                                 |
| xml_etree_generate      | 89.2 ms                                                | 81.6 ms: 1.09x faster                                                 |
| telco                   | 7.10 ms                                                | 6.50 ms: 1.09x faster                                                 |
| spectral_norm           | 115 ms                                                 | 106 ms: 1.09x faster                                                  |
| pickle_list             | 5.08 us                                                | 4.68 us: 1.09x faster                                                 |
| logging_format          | 7.23 us                                                | 6.71 us: 1.08x faster                                                 |
| gunicorn                | 1.24 ms                                                | 1.15 ms: 1.08x faster                                                 |
| scimark_fft             | 382 ms                                                 | 355 ms: 1.08x faster                                                  |
| json                    | 5.26 ms                                                | 4.91 ms: 1.07x faster                                                 |
| logging_simple          | 6.46 us                                                | 6.07 us: 1.06x faster                                                 |
| meteor_contest          | 112 ms                                                 | 106 ms: 1.06x faster                                                  |
| scimark_sparse_mat_mult | 5.06 ms                                                | 4.86 ms: 1.04x faster                                                 |
| xml_etree_process       | 61.7 ms                                                | 59.6 ms: 1.04x faster                                                 |
| unpickle_list           | 5.29 us                                                | 5.13 us: 1.03x faster                                                 |
| sqlite_synth            | 2.83 us                                                | 2.76 us: 1.03x faster                                                 |
| regex_compile           | 148 ms                                                 | 145 ms: 1.03x faster                                                  |
| deepcopy_reduce         | 3.35 us                                                | 3.27 us: 1.02x faster                                                 |
| float                   | 84.7 ms                                                | 83.3 ms: 1.02x faster                                                 |
| pprint_safe_repr        | 776 ms                                                 | 763 ms: 1.02x faster                                                  |
| pathlib                 | 19.3 ms                                                | 19.1 ms: 1.01x faster                                                 |
| sqlalchemy_declarative  | 147 ms                                                 | 145 ms: 1.01x faster                                                  |
| dulwich_log             | 68.5 ms                                                | 68.3 ms: 1.00x faster                                                 |
| 2to3                    | 274 ms                                                 | 274 ms: 1.00x faster                                                  |
| pidigits                | 187 ms                                                 | 188 ms: 1.00x slower                                                  |
| chameleon               | 7.41 ms                                                | 7.46 ms: 1.01x slower                                                 |
| sympy_sum               | 169 ms                                                 | 170 ms: 1.01x slower                                                  |
| pprint_pformat          | 1.57 sec                                               | 1.58 sec: 1.01x slower                                                |
| docutils                | 2.77 sec                                               | 2.79 sec: 1.01x slower                                                |
| mako                    | 11.9 ms                                                | 12.1 ms: 1.02x slower                                                 |
| sympy_str               | 300 ms                                                 | 306 ms: 1.02x slower                                                  |
| fannkuch                | 417 ms                                                 | 427 ms: 1.02x slower                                                  |
| regex_v8                | 23.1 ms                                                | 23.7 ms: 1.03x slower                                                 |
| deepcopy                | 371 us                                                 | 382 us: 1.03x slower                                                  |
| mdp                     | 2.63 sec                                               | 2.71 sec: 1.03x slower                                                |
| regex_dna               | 212 ms                                                 | 219 ms: 1.03x slower                                                  |
| xml_etree_iterparse     | 107 ms                                                 | 110 ms: 1.03x slower                                                  |
| sympy_integrate         | 21.4 ms                                                | 22.2 ms: 1.04x slower                                                 |
| coverage                | 72.7 ms                                                | 75.8 ms: 1.04x slower                                                 |
| scimark_monte_carlo     | 75.1 ms                                                | 78.4 ms: 1.04x slower                                                 |
| raytrace                | 312 ms                                                 | 326 ms: 1.04x slower                                                  |
| sympy_expand            | 478 ms                                                 | 505 ms: 1.06x slower                                                  |
| bench_thread_pool       | 842 us                                                 | 892 us: 1.06x slower                                                  |
| sqlglot_optimize        | 54.8 ms                                                | 58.4 ms: 1.06x slower                                                 |
| pycparser               | 1.18 sec                                               | 1.26 sec: 1.07x slower                                                |
| tornado_http            | 103 ms                                                 | 111 ms: 1.08x slower                                                  |
| sqlglot_normalize       | 110 ms                                                 | 119 ms: 1.08x slower                                                  |
| django_template         | 34.6 ms                                                | 37.9 ms: 1.10x slower                                                 |
| nqueens                 | 83.3 ms                                                | 91.4 ms: 1.10x slower                                                 |
| async_tree_none         | 472 ms                                                 | 518 ms: 1.10x slower                                                  |
| crypto_pyaes            | 81.9 ms                                                | 90.2 ms: 1.10x slower                                                 |
| logging_silent          | 104 ns                                                 | 117 ns: 1.12x slower                                                  |
| pyflate                 | 482 ms                                                 | 541 ms: 1.12x slower                                                  |
| pickle_pure_python      | 324 us                                                 | 364 us: 1.12x slower                                                  |
| async_tree_cpu_io_mixed | 726 ms                                                 | 818 ms: 1.13x slower                                                  |
| chaos                   | 67.0 ms                                                | 77.1 ms: 1.15x slower                                                 |
| nbody                   | 97.0 ms                                                | 112 ms: 1.15x slower                                                  |
| scimark_lu              | 118 ms                                                 | 136 ms: 1.16x slower                                                  |
| hexiom                  | 6.41 ms                                                | 7.42 ms: 1.16x slower                                                 |
| async_tree_memoization  | 578 ms                                                 | 676 ms: 1.17x slower                                                  |
| unpickle_pure_python    | 230 us                                                 | 271 us: 1.18x slower                                                  |
| json_dumps              | 10.4 ms                                                | 12.4 ms: 1.19x slower                                                 |
| go                      | 139 ms                                                 | 167 ms: 1.20x slower                                                  |
| scimark_sor             | 129 ms                                                 | 156 ms: 1.21x slower                                                  |
| richards                | 45.8 ms                                                | 55.7 ms: 1.22x slower                                                 |
| async_tree_io           | 1.16 sec                                               | 1.41 sec: 1.22x slower                                                |
| coroutines              | 23.2 ms                                                | 28.8 ms: 1.24x slower                                                 |
| deltablue               | 3.72 ms                                                | 4.86 ms: 1.31x slower                                                 |
| sqlglot_transpile       | 1.68 ms                                                | 2.37 ms: 1.41x slower                                                 |
| sqlglot_parse           | 1.36 ms                                                | 2.06 ms: 1.51x slower                                                 |
| python_startup          | 9.55 ms                                                | 14.6 ms: 1.52x slower                                                 |
| generators              | 31.2 ms                                                | 57.4 ms: 1.84x slower                                                 |
| Geometric mean          | (ref)                                                  | 1.04x slower                                                          |

Benchmark hidden because not significant (4): xml_etree_parse, deepcopy_memo, bench_mp_pool, sqlalchemy_imperative
Ignored benchmarks (16) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, comprehensions, create_gc_cycles, dask, gc_traversal, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (6) of results/bm-20211105-3.11.0a2-e2b4e4b/bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 99.97% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 0.93x