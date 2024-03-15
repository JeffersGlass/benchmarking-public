
# Results vs. 3.10.4

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: 2e49bd0
- commit date: 2022-04-05
- overall geometric mean: 1.34x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.26x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220405-linux-x86_64-python-main-3.11.0a7-2e49bd0 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| 2to3           | 348 ms                                                 | 264 ms: 1.32x faster                                  |
| chameleon      | 9.68 ms                                                | 6.87 ms: 1.41x faster                                 |
| html5lib       | 88.9 ms                                                | 65.3 ms: 1.36x faster                                 |
| tornado_http   | 136 ms                                                 | 95.4 ms: 1.43x faster                                 |
| Geometric mean | (ref)                                                  | 1.38x faster                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220405-linux-x86_64-python-main-3.11.0a7-2e49bd0 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| nbody          | 154 ms                                                 | 95.2 ms: 1.61x faster                                 |
| float          | 117 ms                                                 | 74.4 ms: 1.57x faster                                 |
| pidigits       | 191 ms                                                 | 197 ms: 1.03x slower                                  |
| Geometric mean | (ref)                                                  | 1.35x faster                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220405-linux-x86_64-python-main-3.11.0a7-2e49bd0 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 137 ms: 1.37x faster                                  |
| regex_effbot   | 3.63 ms                                                | 3.34 ms: 1.09x faster                                 |
| regex_v8       | 27.8 ms                                                | 25.9 ms: 1.07x faster                                 |
| regex_dna      | 227 ms                                                 | 231 ms: 1.02x slower                                  |
| Geometric mean | (ref)                                                  | 1.12x faster                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220405-linux-x86_64-python-main-3.11.0a7-2e49bd0 |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 311 us: 1.56x faster                                  |
| unpickle_pure_python | 331 us                                                 | 231 us: 1.43x faster                                  |
| xml_etree_process    | 79.1 ms                                                | 55.2 ms: 1.43x faster                                 |
| xml_etree_generate   | 99.4 ms                                                | 78.5 ms: 1.27x faster                                 |
| json_dumps           | 14.2 ms                                                | 12.5 ms: 1.13x faster                                 |
| pickle               | 10.7 us                                                | 9.55 us: 1.12x faster                                 |
| xml_etree_iterparse  | 115 ms                                                 | 104 ms: 1.11x faster                                  |
| pickle_list          | 5.08 us                                                | 4.57 us: 1.11x faster                                 |
| json_loads           | 31.2 us                                                | 28.1 us: 1.11x faster                                 |
| xml_etree_parse      | 168 ms                                                 | 157 ms: 1.07x faster                                  |
| pickle_dict          | 29.6 us                                                | 27.6 us: 1.07x faster                                 |
| unpickle_list        | 5.20 us                                                | 4.97 us: 1.05x faster                                 |
| Geometric mean       | (ref)                                                  | 1.18x faster                                          |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220405-linux-x86_64-python-main-3.11.0a7-2e49bd0 |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 8.07 ms: 1.81x faster                                 |
| python_startup_no_site | 5.93 ms                                                | 5.98 ms: 1.01x slower                                 |
| Geometric mean         | (ref)                                                  | 1.34x faster                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220405-linux-x86_64-python-main-3.11.0a7-2e49bd0 |
|-----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| mako            | 16.3 ms                                                | 10.2 ms: 1.60x faster                                 |
| django_template | 48.2 ms                                                | 34.3 ms: 1.41x faster                                 |
| Geometric mean  | (ref)                                                  | 1.50x faster                                          |

All benchmarks:
===============

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220405-linux-x86_64-python-main-3.11.0a7-2e49bd0 |
|-------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| deltablue               | 7.91 ms                                                | 3.70 ms: 2.14x faster                                 |
| logging_silent          | 190 ns                                                 | 104 ns: 1.83x faster                                  |
| python_startup          | 14.6 ms                                                | 8.07 ms: 1.81x faster                                 |
| scimark_sor             | 220 ms                                                 | 123 ms: 1.79x faster                                  |
| go                      | 240 ms                                                 | 143 ms: 1.68x faster                                  |
| scimark_monte_carlo     | 118 ms                                                 | 70.8 ms: 1.67x faster                                 |
| richards                | 79.3 ms                                                | 47.5 ms: 1.67x faster                                 |
| raytrace                | 507 ms                                                 | 306 ms: 1.66x faster                                  |
| chaos                   | 115 ms                                                 | 70.2 ms: 1.64x faster                                 |
| pyflate                 | 716 ms                                                 | 438 ms: 1.63x faster                                  |
| spectral_norm           | 170 ms                                                 | 105 ms: 1.63x faster                                  |
| scimark_lu              | 176 ms                                                 | 108 ms: 1.63x faster                                  |
| nbody                   | 154 ms                                                 | 95.2 ms: 1.61x faster                                 |
| mako                    | 16.3 ms                                                | 10.2 ms: 1.60x faster                                 |
| float                   | 117 ms                                                 | 74.4 ms: 1.57x faster                                 |
| pickle_pure_python      | 484 us                                                 | 311 us: 1.56x faster                                  |
| crypto_pyaes            | 128 ms                                                 | 82.7 ms: 1.54x faster                                 |
| hexiom                  | 10.4 ms                                                | 6.84 ms: 1.52x faster                                 |
| unpickle_pure_python    | 331 us                                                 | 231 us: 1.43x faster                                  |
| xml_etree_process       | 79.1 ms                                                | 55.2 ms: 1.43x faster                                 |
| logging_format          | 9.09 us                                                | 6.35 us: 1.43x faster                                 |
| logging_simple          | 8.30 us                                                | 5.80 us: 1.43x faster                                 |
| tornado_http            | 136 ms                                                 | 95.4 ms: 1.43x faster                                 |
| chameleon               | 9.68 ms                                                | 6.87 ms: 1.41x faster                                 |
| django_template         | 48.2 ms                                                | 34.3 ms: 1.41x faster                                 |
| thrift                  | 1.07 ms                                                | 762 us: 1.41x faster                                  |
| scimark_fft             | 466 ms                                                 | 335 ms: 1.39x faster                                  |
| regex_compile           | 188 ms                                                 | 137 ms: 1.37x faster                                  |
| html5lib                | 88.9 ms                                                | 65.3 ms: 1.36x faster                                 |
| unpack_sequence         | 60.0 ns                                                | 44.9 ns: 1.34x faster                                 |
| scimark_sparse_mat_mult | 6.47 ms                                                | 4.85 ms: 1.33x faster                                 |
| fannkuch                | 532 ms                                                 | 401 ms: 1.33x faster                                  |
| dulwich_log             | 84.3 ms                                                | 63.8 ms: 1.32x faster                                 |
| 2to3                    | 348 ms                                                 | 264 ms: 1.32x faster                                  |
| pycparser               | 1.58 sec                                               | 1.24 sec: 1.27x faster                                |
| xml_etree_generate      | 99.4 ms                                                | 78.5 ms: 1.27x faster                                 |
| sympy_integrate         | 25.8 ms                                                | 20.5 ms: 1.26x faster                                 |
| nqueens                 | 106 ms                                                 | 85.2 ms: 1.24x faster                                 |
| sympy_sum               | 196 ms                                                 | 160 ms: 1.23x faster                                  |
| sqlite_synth            | 3.02 us                                                | 2.51 us: 1.21x faster                                 |
| sympy_str               | 346 ms                                                 | 287 ms: 1.20x faster                                  |
| sympy_expand            | 566 ms                                                 | 476 ms: 1.19x faster                                  |
| json_dumps              | 14.2 ms                                                | 12.5 ms: 1.13x faster                                 |
| json                    | 5.69 ms                                                | 5.07 ms: 1.12x faster                                 |
| meteor_contest          | 120 ms                                                 | 107 ms: 1.12x faster                                  |
| pickle                  | 10.7 us                                                | 9.55 us: 1.12x faster                                 |
| xml_etree_iterparse     | 115 ms                                                 | 104 ms: 1.11x faster                                  |
| pickle_list             | 5.08 us                                                | 4.57 us: 1.11x faster                                 |
| json_loads              | 31.2 us                                                | 28.1 us: 1.11x faster                                 |
| pathlib                 | 20.5 ms                                                | 18.5 ms: 1.11x faster                                 |
| telco                   | 7.27 ms                                                | 6.59 ms: 1.10x faster                                 |
| regex_effbot            | 3.63 ms                                                | 3.34 ms: 1.09x faster                                 |
| regex_v8                | 27.8 ms                                                | 25.9 ms: 1.07x faster                                 |
| xml_etree_parse         | 168 ms                                                 | 157 ms: 1.07x faster                                  |
| pickle_dict             | 29.6 us                                                | 27.6 us: 1.07x faster                                 |
| unpickle_list           | 5.20 us                                                | 4.97 us: 1.05x faster                                 |
| python_startup_no_site  | 5.93 ms                                                | 5.98 ms: 1.01x slower                                 |
| regex_dna               | 227 ms                                                 | 231 ms: 1.02x slower                                  |
| pidigits                | 191 ms                                                 | 197 ms: 1.03x slower                                  |
| Geometric mean          | (ref)                                                  | 1.34x faster                                          |

Benchmark hidden because not significant (1): unpickle
Ignored benchmarks (41) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, async_generators, async_tree_cpu_io_mixed, async_tree_io, async_tree_memoization, async_tree_none, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, bench_mp_pool, bench_thread_pool, comprehensions, coroutines, coverage, create_gc_cycles, dask, deepcopy, deepcopy_memo, deepcopy_reduce, djangocms, docutils, flaskblogging, gc_traversal, generators, genshi_text, genshi_xml, gunicorn, mdp, mypy2, pprint_pformat, pprint_safe_repr, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, sqlglot_normalize, sqlglot_optimize, sqlglot_parse, sqlglot_transpile, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.30x
- 95% likely to have a speedup of 1.27x
- 99% likely to have a speedup of 1.26x


# Memory

- memory change: 1.06x