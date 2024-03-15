
# Results vs. 3.12.0

- fork: python
- ref: 7d4cc5aa854fdea4d01a
- machine: linux-x86_64
- commit hash: 7d4cc5a
- commit date: 2023-04-04
- overall geometric mean: 1.21x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.13x slower
- Memory change: 0.90x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-linux-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 335 ms: 1.22x slower                                                 |
| chameleon      | 7.41 ms                                                | 8.93 ms: 1.21x slower                                                |
| docutils       | 2.77 sec                                               | 3.21 sec: 1.16x slower                                               |
| tornado_http   | 103 ms                                                 | 131 ms: 1.27x slower                                                 |
| Geometric mean | (ref)                                                  | 1.21x slower                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-linux-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 726 ms                                                 | 975 ms: 1.34x slower                                                 |
| async_tree_memoization  | 578 ms                                                 | 873 ms: 1.51x slower                                                 |
| async_tree_none         | 472 ms                                                 | 732 ms: 1.55x slower                                                 |
| async_tree_io           | 1.16 sec                                               | 1.82 sec: 1.57x slower                                               |
| Geometric mean          | (ref)                                                  | 1.49x slower                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-linux-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 188 ms: 1.01x slower                                                 |
| float          | 84.7 ms                                                | 108 ms: 1.27x slower                                                 |
| nbody          | 97.0 ms                                                | 137 ms: 1.42x slower                                                 |
| Geometric mean | (ref)                                                  | 1.22x slower                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-linux-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_dna      | 212 ms                                                 | 213 ms: 1.01x slower                                                 |
| regex_v8       | 23.1 ms                                                | 25.5 ms: 1.10x slower                                                |
| regex_compile  | 148 ms                                                 | 176 ms: 1.19x slower                                                 |
| Geometric mean | (ref)                                                  | 1.07x slower                                                         |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-linux-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| pickle_list          | 5.08 us                                                | 4.38 us: 1.16x faster                                                |
| pickle               | 11.6 us                                                | 10.4 us: 1.12x faster                                                |
| unpickle             | 15.9 us                                                | 14.3 us: 1.11x faster                                                |
| unpickle_list        | 5.29 us                                                | 4.80 us: 1.10x faster                                                |
| pickle_dict          | 35.5 us                                                | 33.7 us: 1.05x faster                                                |
| json_loads           | 28.5 us                                                | 29.0 us: 1.02x slower                                                |
| xml_etree_parse      | 159 ms                                                 | 163 ms: 1.02x slower                                                 |
| xml_etree_iterparse  | 107 ms                                                 | 110 ms: 1.03x slower                                                 |
| xml_etree_generate   | 89.2 ms                                                | 93.1 ms: 1.04x slower                                                |
| xml_etree_process    | 61.7 ms                                                | 74.1 ms: 1.20x slower                                                |
| unpickle_pure_python | 230 us                                                 | 298 us: 1.30x slower                                                 |
| json_dumps           | 10.4 ms                                                | 13.6 ms: 1.31x slower                                                |
| pickle_pure_python   | 324 us                                                 | 452 us: 1.40x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.05x slower                                                         |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-linux-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup_no_site | 6.94 ms                                                | 5.83 ms: 1.19x faster                                                |
| python_startup         | 9.55 ms                                                | 14.2 ms: 1.49x slower                                                |
| Geometric mean         | (ref)                                                  | 1.12x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-linux-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako            | 11.9 ms                                                | 14.7 ms: 1.24x slower                                                |
| django_template | 34.6 ms                                                | 45.8 ms: 1.32x slower                                                |
| Geometric mean  | (ref)                                                  | 1.28x slower                                                         |

All benchmarks:
===============

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-linux-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup_no_site  | 6.94 ms                                                | 5.83 ms: 1.19x faster                                                |
| pickle_list             | 5.08 us                                                | 4.38 us: 1.16x faster                                                |
| pickle                  | 11.6 us                                                | 10.4 us: 1.12x faster                                                |
| unpickle                | 15.9 us                                                | 14.3 us: 1.11x faster                                                |
| unpickle_list           | 5.29 us                                                | 4.80 us: 1.10x faster                                                |
| async_generators        | 463 ms                                                 | 421 ms: 1.10x faster                                                 |
| pickle_dict             | 35.5 us                                                | 33.7 us: 1.05x faster                                                |
| telco                   | 7.10 ms                                                | 6.78 ms: 1.05x faster                                                |
| gc_traversal            | 3.79 ms                                                | 3.71 ms: 1.02x faster                                                |
| coverage                | 72.7 ms                                                | 72.1 ms: 1.01x faster                                                |
| regex_dna               | 212 ms                                                 | 213 ms: 1.01x slower                                                 |
| meteor_contest          | 112 ms                                                 | 113 ms: 1.01x slower                                                 |
| pidigits                | 187 ms                                                 | 188 ms: 1.01x slower                                                 |
| json                    | 5.26 ms                                                | 5.32 ms: 1.01x slower                                                |
| json_loads              | 28.5 us                                                | 29.0 us: 1.02x slower                                                |
| xml_etree_parse         | 159 ms                                                 | 163 ms: 1.02x slower                                                 |
| pathlib                 | 19.3 ms                                                | 19.9 ms: 1.03x slower                                                |
| xml_etree_iterparse     | 107 ms                                                 | 110 ms: 1.03x slower                                                 |
| xml_etree_generate      | 89.2 ms                                                | 93.1 ms: 1.04x slower                                                |
| sqlite_synth            | 2.83 us                                                | 3.02 us: 1.07x slower                                                |
| mdp                     | 2.63 sec                                               | 2.85 sec: 1.08x slower                                               |
| scimark_sparse_mat_mult | 5.06 ms                                                | 5.50 ms: 1.09x slower                                                |
| scimark_fft             | 382 ms                                                 | 416 ms: 1.09x slower                                                 |
| bench_thread_pool       | 842 us                                                 | 925 us: 1.10x slower                                                 |
| sympy_str               | 300 ms                                                 | 330 ms: 1.10x slower                                                 |
| regex_v8                | 23.1 ms                                                | 25.5 ms: 1.10x slower                                                |
| dulwich_log             | 68.5 ms                                                | 75.5 ms: 1.10x slower                                                |
| sympy_sum               | 169 ms                                                 | 188 ms: 1.11x slower                                                 |
| gunicorn                | 1.24 ms                                                | 1.39 ms: 1.12x slower                                                |
| aiohttp                 | 1.15 ms                                                | 1.29 ms: 1.12x slower                                                |
| sqlalchemy_imperative   | 18.7 ms                                                | 21.0 ms: 1.12x slower                                                |
| create_gc_cycles        | 1.48 ms                                                | 1.66 ms: 1.13x slower                                                |
| deepcopy_reduce         | 3.35 us                                                | 3.77 us: 1.13x slower                                                |
| fannkuch                | 417 ms                                                 | 471 ms: 1.13x slower                                                 |
| dask                    | 372 ms                                                 | 421 ms: 1.13x slower                                                 |
| sympy_integrate         | 21.4 ms                                                | 24.3 ms: 1.13x slower                                                |
| sympy_expand            | 478 ms                                                 | 545 ms: 1.14x slower                                                 |
| sqlalchemy_declarative  | 147 ms                                                 | 168 ms: 1.14x slower                                                 |
| deepcopy                | 371 us                                                 | 429 us: 1.16x slower                                                 |
| docutils                | 2.77 sec                                               | 3.21 sec: 1.16x slower                                               |
| nqueens                 | 83.3 ms                                                | 97.9 ms: 1.18x slower                                                |
| regex_compile           | 148 ms                                                 | 176 ms: 1.19x slower                                                 |
| sqlglot_optimize        | 54.8 ms                                                | 65.5 ms: 1.20x slower                                                |
| xml_etree_process       | 61.7 ms                                                | 74.1 ms: 1.20x slower                                                |
| chameleon               | 7.41 ms                                                | 8.93 ms: 1.21x slower                                                |
| 2to3                    | 274 ms                                                 | 335 ms: 1.22x slower                                                 |
| deepcopy_memo           | 40.7 us                                                | 49.8 us: 1.22x slower                                                |
| pprint_safe_repr        | 776 ms                                                 | 953 ms: 1.23x slower                                                 |
| sqlglot_normalize       | 110 ms                                                 | 136 ms: 1.23x slower                                                 |
| mako                    | 11.9 ms                                                | 14.7 ms: 1.24x slower                                                |
| spectral_norm           | 115 ms                                                 | 142 ms: 1.24x slower                                                 |
| comprehensions          | 21.8 us                                                | 27.0 us: 1.24x slower                                                |
| unpack_sequence         | 54.0 ns                                                | 67.6 ns: 1.25x slower                                                |
| pprint_pformat          | 1.57 sec                                               | 1.97 sec: 1.26x slower                                               |
| logging_format          | 7.23 us                                                | 9.16 us: 1.27x slower                                                |
| tornado_http            | 103 ms                                                 | 131 ms: 1.27x slower                                                 |
| float                   | 84.7 ms                                                | 108 ms: 1.27x slower                                                 |
| pycparser               | 1.18 sec                                               | 1.52 sec: 1.29x slower                                               |
| unpickle_pure_python    | 230 us                                                 | 298 us: 1.30x slower                                                 |
| logging_simple          | 6.46 us                                                | 8.40 us: 1.30x slower                                                |
| json_dumps              | 10.4 ms                                                | 13.6 ms: 1.31x slower                                                |
| django_template         | 34.6 ms                                                | 45.8 ms: 1.32x slower                                                |
| coroutines              | 23.2 ms                                                | 31.0 ms: 1.34x slower                                                |
| async_tree_cpu_io_mixed | 726 ms                                                 | 975 ms: 1.34x slower                                                 |
| scimark_lu              | 118 ms                                                 | 159 ms: 1.34x slower                                                 |
| pyflate                 | 482 ms                                                 | 660 ms: 1.37x slower                                                 |
| crypto_pyaes            | 81.9 ms                                                | 114 ms: 1.39x slower                                                 |
| pickle_pure_python      | 324 us                                                 | 452 us: 1.40x slower                                                 |
| nbody                   | 97.0 ms                                                | 137 ms: 1.42x slower                                                 |
| sqlglot_transpile       | 1.68 ms                                                | 2.44 ms: 1.45x slower                                                |
| scimark_monte_carlo     | 75.1 ms                                                | 109 ms: 1.45x slower                                                 |
| hexiom                  | 6.41 ms                                                | 9.41 ms: 1.47x slower                                                |
| raytrace                | 312 ms                                                 | 462 ms: 1.48x slower                                                 |
| python_startup          | 9.55 ms                                                | 14.2 ms: 1.49x slower                                                |
| scimark_sor             | 129 ms                                                 | 194 ms: 1.50x slower                                                 |
| sqlglot_parse           | 1.36 ms                                                | 2.04 ms: 1.50x slower                                                |
| async_tree_memoization  | 578 ms                                                 | 873 ms: 1.51x slower                                                 |
| async_tree_none         | 472 ms                                                 | 732 ms: 1.55x slower                                                 |
| chaos                   | 67.0 ms                                                | 105 ms: 1.56x slower                                                 |
| async_tree_io           | 1.16 sec                                               | 1.82 sec: 1.57x slower                                               |
| richards                | 45.8 ms                                                | 73.1 ms: 1.60x slower                                                |
| go                      | 139 ms                                                 | 227 ms: 1.63x slower                                                 |
| logging_silent          | 104 ns                                                 | 175 ns: 1.67x slower                                                 |
| asyncio_tcp             | 491 ms                                                 | 894 ms: 1.82x slower                                                 |
| deltablue               | 3.72 ms                                                | 7.35 ms: 1.98x slower                                                |
| generators              | 31.2 ms                                                | 75.5 ms: 2.42x slower                                                |
| Geometric mean          | (ref)                                                  | 1.21x slower                                                         |

Benchmark hidden because not significant (2): bench_mp_pool, regex_effbot
Ignored benchmarks (10) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (7) of results/bm-20230404-3.10.11-7d4cc5a/bm-20230404-linux-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a.json: djangocms, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.16x
- 95% likely to have a slowdown of 1.15x
- 99% likely to have a slowdown of 1.13x


# Memory

- memory change: 0.90x