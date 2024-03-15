
# Results vs. 3.12.0

- fork: python
- ref: v3.10.10
- machine: linux-x86_64
- commit hash: aad5f6a
- commit date: 2023-02-07
- overall geometric mean: 1.20x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.13x slower
- Memory change: 0.90x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 335 ms: 1.22x slower                                     |
| chameleon      | 7.41 ms                                                | 9.13 ms: 1.23x slower                                    |
| docutils       | 2.77 sec                                               | 3.22 sec: 1.16x slower                                   |
| tornado_http   | 103 ms                                                 | 130 ms: 1.27x slower                                     |
| Geometric mean | (ref)                                                  | 1.22x slower                                             |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------:|
| async_tree_cpu_io_mixed | 726 ms                                                 | 997 ms: 1.37x slower                                     |
| async_tree_memoization  | 578 ms                                                 | 856 ms: 1.48x slower                                     |
| async_tree_none         | 472 ms                                                 | 721 ms: 1.53x slower                                     |
| async_tree_io           | 1.16 sec                                               | 1.78 sec: 1.54x slower                                   |
| Geometric mean          | (ref)                                                  | 1.48x slower                                             |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 189 ms: 1.01x slower                                     |
| float          | 84.7 ms                                                | 109 ms: 1.29x slower                                     |
| nbody          | 97.0 ms                                                | 137 ms: 1.41x slower                                     |
| Geometric mean | (ref)                                                  | 1.22x slower                                             |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------:|
| regex_dna      | 212 ms                                                 | 216 ms: 1.02x slower                                     |
| regex_v8       | 23.1 ms                                                | 24.1 ms: 1.04x slower                                    |
| regex_compile  | 148 ms                                                 | 177 ms: 1.19x slower                                     |
| Geometric mean | (ref)                                                  | 1.06x slower                                             |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------:|
| pickle_list          | 5.08 us                                                | 4.17 us: 1.22x faster                                    |
| pickle_dict          | 35.5 us                                                | 30.5 us: 1.16x faster                                    |
| pickle               | 11.6 us                                                | 10.2 us: 1.14x faster                                    |
| unpickle_list        | 5.29 us                                                | 4.94 us: 1.07x faster                                    |
| unpickle             | 15.9 us                                                | 14.8 us: 1.07x faster                                    |
| xml_etree_parse      | 159 ms                                                 | 161 ms: 1.01x slower                                     |
| json_loads           | 28.5 us                                                | 29.2 us: 1.03x slower                                    |
| xml_etree_iterparse  | 107 ms                                                 | 110 ms: 1.03x slower                                     |
| xml_etree_generate   | 89.2 ms                                                | 93.0 ms: 1.04x slower                                    |
| xml_etree_process    | 61.7 ms                                                | 74.4 ms: 1.21x slower                                    |
| unpickle_pure_python | 230 us                                                 | 297 us: 1.29x slower                                     |
| json_dumps           | 10.4 ms                                                | 13.6 ms: 1.31x slower                                    |
| pickle_pure_python   | 324 us                                                 | 449 us: 1.38x slower                                     |
| Geometric mean       | (ref)                                                  | 1.04x slower                                             |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------:|
| python_startup_no_site | 6.94 ms                                                | 5.79 ms: 1.20x faster                                    |
| python_startup         | 9.55 ms                                                | 9.33 ms: 1.02x faster                                    |
| Geometric mean         | (ref)                                                  | 1.11x faster                                             |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a |
|-----------------|:------------------------------------------------------:|:--------------------------------------------------------:|
| mako            | 11.9 ms                                                | 14.6 ms: 1.23x slower                                    |
| django_template | 34.6 ms                                                | 46.6 ms: 1.35x slower                                    |
| Geometric mean  | (ref)                                                  | 1.29x slower                                             |

All benchmarks:
===============

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------:|
| pickle_list             | 5.08 us                                                | 4.17 us: 1.22x faster                                    |
| python_startup_no_site  | 6.94 ms                                                | 5.79 ms: 1.20x faster                                    |
| pickle_dict             | 35.5 us                                                | 30.5 us: 1.16x faster                                    |
| pickle                  | 11.6 us                                                | 10.2 us: 1.14x faster                                    |
| async_generators        | 463 ms                                                 | 426 ms: 1.09x faster                                     |
| gc_traversal            | 3.79 ms                                                | 3.54 ms: 1.07x faster                                    |
| unpickle_list           | 5.29 us                                                | 4.94 us: 1.07x faster                                    |
| unpickle                | 15.9 us                                                | 14.8 us: 1.07x faster                                    |
| telco                   | 7.10 ms                                                | 6.71 ms: 1.06x faster                                    |
| python_startup          | 9.55 ms                                                | 9.33 ms: 1.02x faster                                    |
| coverage                | 72.7 ms                                                | 71.5 ms: 1.02x faster                                    |
| meteor_contest          | 112 ms                                                 | 113 ms: 1.00x slower                                     |
| pidigits                | 187 ms                                                 | 189 ms: 1.01x slower                                     |
| xml_etree_parse         | 159 ms                                                 | 161 ms: 1.01x slower                                     |
| regex_dna               | 212 ms                                                 | 216 ms: 1.02x slower                                     |
| pathlib                 | 19.3 ms                                                | 19.7 ms: 1.02x slower                                    |
| json_loads              | 28.5 us                                                | 29.2 us: 1.03x slower                                    |
| json                    | 5.26 ms                                                | 5.40 ms: 1.03x slower                                    |
| xml_etree_iterparse     | 107 ms                                                 | 110 ms: 1.03x slower                                     |
| xml_etree_generate      | 89.2 ms                                                | 93.0 ms: 1.04x slower                                    |
| regex_v8                | 23.1 ms                                                | 24.1 ms: 1.04x slower                                    |
| sqlite_synth            | 2.83 us                                                | 2.97 us: 1.05x slower                                    |
| scimark_sparse_mat_mult | 5.06 ms                                                | 5.39 ms: 1.07x slower                                    |
| scimark_fft             | 382 ms                                                 | 408 ms: 1.07x slower                                     |
| mdp                     | 2.63 sec                                               | 2.82 sec: 1.07x slower                                   |
| bench_thread_pool       | 842 us                                                 | 919 us: 1.09x slower                                     |
| sympy_str               | 300 ms                                                 | 329 ms: 1.10x slower                                     |
| dulwich_log             | 68.5 ms                                                | 75.4 ms: 1.10x slower                                    |
| create_gc_cycles        | 1.48 ms                                                | 1.63 ms: 1.11x slower                                    |
| sympy_sum               | 169 ms                                                 | 189 ms: 1.12x slower                                     |
| fannkuch                | 417 ms                                                 | 467 ms: 1.12x slower                                     |
| sqlalchemy_imperative   | 18.7 ms                                                | 20.9 ms: 1.12x slower                                    |
| gunicorn                | 1.24 ms                                                | 1.39 ms: 1.12x slower                                    |
| aiohttp                 | 1.15 ms                                                | 1.29 ms: 1.12x slower                                    |
| sympy_integrate         | 21.4 ms                                                | 24.4 ms: 1.14x slower                                    |
| deepcopy_reduce         | 3.35 us                                                | 3.81 us: 1.14x slower                                    |
| sqlalchemy_declarative  | 147 ms                                                 | 167 ms: 1.14x slower                                     |
| sympy_expand            | 478 ms                                                 | 546 ms: 1.14x slower                                     |
| deepcopy                | 371 us                                                 | 428 us: 1.15x slower                                     |
| docutils                | 2.77 sec                                               | 3.22 sec: 1.16x slower                                   |
| dask                    | 372 ms                                                 | 434 ms: 1.17x slower                                     |
| unpack_sequence         | 54.0 ns                                                | 64.0 ns: 1.19x slower                                    |
| regex_compile           | 148 ms                                                 | 177 ms: 1.19x slower                                     |
| sqlglot_optimize        | 54.8 ms                                                | 65.4 ms: 1.19x slower                                    |
| nqueens                 | 83.3 ms                                                | 100 ms: 1.20x slower                                     |
| xml_etree_process       | 61.7 ms                                                | 74.4 ms: 1.21x slower                                    |
| 2to3                    | 274 ms                                                 | 335 ms: 1.22x slower                                     |
| deepcopy_memo           | 40.7 us                                                | 49.9 us: 1.23x slower                                    |
| mako                    | 11.9 ms                                                | 14.6 ms: 1.23x slower                                    |
| sqlglot_normalize       | 110 ms                                                 | 136 ms: 1.23x slower                                     |
| chameleon               | 7.41 ms                                                | 9.13 ms: 1.23x slower                                    |
| spectral_norm           | 115 ms                                                 | 143 ms: 1.25x slower                                     |
| pprint_safe_repr        | 776 ms                                                 | 975 ms: 1.26x slower                                     |
| tornado_http            | 103 ms                                                 | 130 ms: 1.27x slower                                     |
| logging_format          | 7.23 us                                                | 9.20 us: 1.27x slower                                    |
| float                   | 84.7 ms                                                | 109 ms: 1.29x slower                                     |
| pprint_pformat          | 1.57 sec                                               | 2.02 sec: 1.29x slower                                   |
| unpickle_pure_python    | 230 us                                                 | 297 us: 1.29x slower                                     |
| logging_simple          | 6.46 us                                                | 8.41 us: 1.30x slower                                    |
| pycparser               | 1.18 sec                                               | 1.54 sec: 1.30x slower                                   |
| json_dumps              | 10.4 ms                                                | 13.6 ms: 1.31x slower                                    |
| coroutines              | 23.2 ms                                                | 30.6 ms: 1.32x slower                                    |
| django_template         | 34.6 ms                                                | 46.6 ms: 1.35x slower                                    |
| scimark_lu              | 118 ms                                                 | 160 ms: 1.36x slower                                     |
| pyflate                 | 482 ms                                                 | 659 ms: 1.37x slower                                     |
| async_tree_cpu_io_mixed | 726 ms                                                 | 997 ms: 1.37x slower                                     |
| pickle_pure_python      | 324 us                                                 | 449 us: 1.38x slower                                     |
| scimark_monte_carlo     | 75.1 ms                                                | 105 ms: 1.40x slower                                     |
| crypto_pyaes            | 81.9 ms                                                | 115 ms: 1.40x slower                                     |
| nbody                   | 97.0 ms                                                | 137 ms: 1.41x slower                                     |
| sqlglot_transpile       | 1.68 ms                                                | 2.41 ms: 1.43x slower                                    |
| hexiom                  | 6.41 ms                                                | 9.42 ms: 1.47x slower                                    |
| async_tree_memoization  | 578 ms                                                 | 856 ms: 1.48x slower                                     |
| raytrace                | 312 ms                                                 | 463 ms: 1.48x slower                                     |
| sqlglot_parse           | 1.36 ms                                                | 2.03 ms: 1.49x slower                                    |
| scimark_sor             | 129 ms                                                 | 193 ms: 1.49x slower                                     |
| async_tree_none         | 472 ms                                                 | 721 ms: 1.53x slower                                     |
| async_tree_io           | 1.16 sec                                               | 1.78 sec: 1.54x slower                                   |
| richards                | 45.8 ms                                                | 72.6 ms: 1.58x slower                                    |
| chaos                   | 67.0 ms                                                | 106 ms: 1.59x slower                                     |
| go                      | 139 ms                                                 | 226 ms: 1.62x slower                                     |
| logging_silent          | 104 ns                                                 | 174 ns: 1.67x slower                                     |
| asyncio_tcp             | 491 ms                                                 | 915 ms: 1.86x slower                                     |
| deltablue               | 3.72 ms                                                | 7.41 ms: 2.00x slower                                    |
| generators              | 31.2 ms                                                | 76.1 ms: 2.44x slower                                    |
| Geometric mean          | (ref)                                                  | 1.20x slower                                             |

Benchmark hidden because not significant (2): bench_mp_pool, regex_effbot
Ignored benchmarks (11) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, comprehensions, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (7) of results/bm-20230207-3.10.10-aad5f6a/bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a.json: djangocms, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.16x
- 95% likely to have a slowdown of 1.16x
- 99% likely to have a slowdown of 1.13x


# Memory

- memory change: 0.90x