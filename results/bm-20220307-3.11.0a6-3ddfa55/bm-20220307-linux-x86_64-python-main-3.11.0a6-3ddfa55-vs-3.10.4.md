
# Results vs. 3.10.4

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: 3ddfa55
- commit date: 2022-03-07
- overall geometric mean: 1.29x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.24x faster
- Memory change: 1.09x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220307-linux-x86_64-python-main-3.11.0a6-3ddfa55 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| 2to3           | 348 ms                                                 | 268 ms: 1.30x faster                                  |
| chameleon      | 9.68 ms                                                | 6.93 ms: 1.40x faster                                 |
| html5lib       | 88.9 ms                                                | 68.6 ms: 1.30x faster                                 |
| tornado_http   | 136 ms                                                 | 99.2 ms: 1.37x faster                                 |
| Geometric mean | (ref)                                                  | 1.34x faster                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220307-linux-x86_64-python-main-3.11.0a6-3ddfa55 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| nbody          | 154 ms                                                 | 97.7 ms: 1.57x faster                                 |
| float          | 117 ms                                                 | 78.7 ms: 1.49x faster                                 |
| pidigits       | 191 ms                                                 | 208 ms: 1.09x slower                                  |
| Geometric mean | (ref)                                                  | 1.29x faster                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220307-linux-x86_64-python-main-3.11.0a6-3ddfa55 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 140 ms: 1.35x faster                                  |
| regex_v8       | 27.8 ms                                                | 23.0 ms: 1.21x faster                                 |
| regex_effbot   | 3.63 ms                                                | 3.49 ms: 1.04x faster                                 |
| regex_dna      | 227 ms                                                 | 221 ms: 1.03x faster                                  |
| Geometric mean | (ref)                                                  | 1.15x faster                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220307-linux-x86_64-python-main-3.11.0a6-3ddfa55 |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 335 us: 1.44x faster                                  |
| xml_etree_process    | 79.1 ms                                                | 56.0 ms: 1.41x faster                                 |
| unpickle_pure_python | 331 us                                                 | 246 us: 1.34x faster                                  |
| xml_etree_generate   | 99.4 ms                                                | 79.6 ms: 1.25x faster                                 |
| pickle_list          | 5.08 us                                                | 4.51 us: 1.13x faster                                 |
| json_dumps           | 14.2 ms                                                | 12.6 ms: 1.12x faster                                 |
| json_loads           | 31.2 us                                                | 28.1 us: 1.11x faster                                 |
| pickle               | 10.7 us                                                | 9.69 us: 1.10x faster                                 |
| xml_etree_iterparse  | 115 ms                                                 | 105 ms: 1.10x faster                                  |
| xml_etree_parse      | 168 ms                                                 | 156 ms: 1.07x faster                                  |
| unpickle_list        | 5.20 us                                                | 4.92 us: 1.06x faster                                 |
| pickle_dict          | 29.6 us                                                | 28.1 us: 1.05x faster                                 |
| Geometric mean       | (ref)                                                  | 1.16x faster                                          |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220307-linux-x86_64-python-main-3.11.0a6-3ddfa55 |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 8.20 ms: 1.78x faster                                 |
| python_startup_no_site | 5.93 ms                                                | 6.07 ms: 1.02x slower                                 |
| Geometric mean         | (ref)                                                  | 1.32x faster                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220307-linux-x86_64-python-main-3.11.0a6-3ddfa55 |
|-----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| mako            | 16.3 ms                                                | 10.6 ms: 1.54x faster                                 |
| django_template | 48.2 ms                                                | 36.0 ms: 1.34x faster                                 |
| Geometric mean  | (ref)                                                  | 1.43x faster                                          |

All benchmarks:
===============

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220307-linux-x86_64-python-main-3.11.0a6-3ddfa55 |
|-------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| deltablue               | 7.91 ms                                                | 4.16 ms: 1.90x faster                                 |
| python_startup          | 14.6 ms                                                | 8.20 ms: 1.78x faster                                 |
| scimark_sor             | 220 ms                                                 | 123 ms: 1.78x faster                                  |
| logging_silent          | 190 ns                                                 | 113 ns: 1.68x faster                                  |
| richards                | 79.3 ms                                                | 48.5 ms: 1.63x faster                                 |
| go                      | 240 ms                                                 | 148 ms: 1.63x faster                                  |
| scimark_monte_carlo     | 118 ms                                                 | 72.9 ms: 1.62x faster                                 |
| raytrace                | 507 ms                                                 | 318 ms: 1.59x faster                                  |
| spectral_norm           | 170 ms                                                 | 107 ms: 1.58x faster                                  |
| pyflate                 | 716 ms                                                 | 453 ms: 1.58x faster                                  |
| nbody                   | 154 ms                                                 | 97.7 ms: 1.57x faster                                 |
| chaos                   | 115 ms                                                 | 73.5 ms: 1.57x faster                                 |
| mako                    | 16.3 ms                                                | 10.6 ms: 1.54x faster                                 |
| scimark_lu              | 176 ms                                                 | 115 ms: 1.53x faster                                  |
| crypto_pyaes            | 128 ms                                                 | 84.6 ms: 1.51x faster                                 |
| logging_simple          | 8.30 us                                                | 5.52 us: 1.50x faster                                 |
| logging_format          | 9.09 us                                                | 6.08 us: 1.49x faster                                 |
| float                   | 117 ms                                                 | 78.7 ms: 1.49x faster                                 |
| hexiom                  | 10.4 ms                                                | 7.04 ms: 1.48x faster                                 |
| pickle_pure_python      | 484 us                                                 | 335 us: 1.44x faster                                  |
| xml_etree_process       | 79.1 ms                                                | 56.0 ms: 1.41x faster                                 |
| chameleon               | 9.68 ms                                                | 6.93 ms: 1.40x faster                                 |
| scimark_fft             | 466 ms                                                 | 336 ms: 1.38x faster                                  |
| tornado_http            | 136 ms                                                 | 99.2 ms: 1.37x faster                                 |
| thrift                  | 1.07 ms                                                | 789 us: 1.36x faster                                  |
| regex_compile           | 188 ms                                                 | 140 ms: 1.35x faster                                  |
| unpickle_pure_python    | 331 us                                                 | 246 us: 1.34x faster                                  |
| scimark_sparse_mat_mult | 6.47 ms                                                | 4.82 ms: 1.34x faster                                 |
| django_template         | 48.2 ms                                                | 36.0 ms: 1.34x faster                                 |
| fannkuch                | 532 ms                                                 | 398 ms: 1.33x faster                                  |
| 2to3                    | 348 ms                                                 | 268 ms: 1.30x faster                                  |
| pycparser               | 1.58 sec                                               | 1.21 sec: 1.30x faster                                |
| html5lib                | 88.9 ms                                                | 68.6 ms: 1.30x faster                                 |
| dulwich_log             | 84.3 ms                                                | 66.5 ms: 1.27x faster                                 |
| xml_etree_generate      | 99.4 ms                                                | 79.6 ms: 1.25x faster                                 |
| sympy_integrate         | 25.8 ms                                                | 20.9 ms: 1.24x faster                                 |
| nqueens                 | 106 ms                                                 | 87.0 ms: 1.22x faster                                 |
| regex_v8                | 27.8 ms                                                | 23.0 ms: 1.21x faster                                 |
| sqlite_synth            | 3.02 us                                                | 2.51 us: 1.21x faster                                 |
| sympy_sum               | 196 ms                                                 | 163 ms: 1.20x faster                                  |
| sympy_str               | 346 ms                                                 | 289 ms: 1.20x faster                                  |
| sympy_expand            | 566 ms                                                 | 481 ms: 1.18x faster                                  |
| json                    | 5.69 ms                                                | 5.00 ms: 1.14x faster                                 |
| meteor_contest          | 120 ms                                                 | 106 ms: 1.13x faster                                  |
| pickle_list             | 5.08 us                                                | 4.51 us: 1.13x faster                                 |
| json_dumps              | 14.2 ms                                                | 12.6 ms: 1.12x faster                                 |
| pathlib                 | 20.5 ms                                                | 18.2 ms: 1.12x faster                                 |
| json_loads              | 31.2 us                                                | 28.1 us: 1.11x faster                                 |
| pickle                  | 10.7 us                                                | 9.69 us: 1.10x faster                                 |
| xml_etree_iterparse     | 115 ms                                                 | 105 ms: 1.10x faster                                  |
| xml_etree_parse         | 168 ms                                                 | 156 ms: 1.07x faster                                  |
| unpickle_list           | 5.20 us                                                | 4.92 us: 1.06x faster                                 |
| pickle_dict             | 29.6 us                                                | 28.1 us: 1.05x faster                                 |
| telco                   | 7.27 ms                                                | 6.92 ms: 1.05x faster                                 |
| regex_effbot            | 3.63 ms                                                | 3.49 ms: 1.04x faster                                 |
| regex_dna               | 227 ms                                                 | 221 ms: 1.03x faster                                  |
| python_startup_no_site  | 5.93 ms                                                | 6.07 ms: 1.02x slower                                 |
| pidigits                | 191 ms                                                 | 208 ms: 1.09x slower                                  |
| unpack_sequence         | 60.0 ns                                                | 131 ns: 2.18x slower                                  |
| Geometric mean          | (ref)                                                  | 1.29x faster                                          |

Benchmark hidden because not significant (1): unpickle
Ignored benchmarks (41) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, async_generators, async_tree_cpu_io_mixed, async_tree_io, async_tree_memoization, async_tree_none, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, bench_mp_pool, bench_thread_pool, comprehensions, coroutines, coverage, create_gc_cycles, dask, deepcopy, deepcopy_memo, deepcopy_reduce, djangocms, docutils, flaskblogging, gc_traversal, generators, genshi_text, genshi_xml, gunicorn, mdp, mypy2, pprint_pformat, pprint_safe_repr, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, sqlglot_normalize, sqlglot_optimize, sqlglot_parse, sqlglot_transpile, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.28x
- 95% likely to have a speedup of 1.27x
- 99% likely to have a speedup of 1.24x


# Memory

- memory change: 1.09x