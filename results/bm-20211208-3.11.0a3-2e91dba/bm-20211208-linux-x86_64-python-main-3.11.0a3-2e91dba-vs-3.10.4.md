
# Results vs. 3.10.4

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: 2e91dba
- commit date: 2021-12-08
- overall geometric mean: 1.29x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.22x faster
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211208-linux-x86_64-python-main-3.11.0a3-2e91dba |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| 2to3           | 348 ms                                                 | 264 ms: 1.32x faster                                  |
| chameleon      | 9.68 ms                                                | 7.44 ms: 1.30x faster                                 |
| html5lib       | 88.9 ms                                                | 68.5 ms: 1.30x faster                                 |
| tornado_http   | 136 ms                                                 | 108 ms: 1.26x faster                                  |
| Geometric mean | (ref)                                                  | 1.30x faster                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211208-linux-x86_64-python-main-3.11.0a3-2e91dba |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| nbody          | 154 ms                                                 | 96.1 ms: 1.60x faster                                 |
| float          | 117 ms                                                 | 79.2 ms: 1.48x faster                                 |
| pidigits       | 191 ms                                                 | 198 ms: 1.04x slower                                  |
| Geometric mean | (ref)                                                  | 1.32x faster                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211208-linux-x86_64-python-main-3.11.0a3-2e91dba |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 139 ms: 1.36x faster                                  |
| regex_v8       | 27.8 ms                                                | 24.5 ms: 1.13x faster                                 |
| regex_effbot   | 3.63 ms                                                | 3.21 ms: 1.13x faster                                 |
| regex_dna      | 227 ms                                                 | 212 ms: 1.07x faster                                  |
| Geometric mean | (ref)                                                  | 1.17x faster                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211208-linux-x86_64-python-main-3.11.0a3-2e91dba |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 347 us: 1.40x faster                                  |
| xml_etree_process    | 79.1 ms                                                | 57.8 ms: 1.37x faster                                 |
| unpickle_pure_python | 331 us                                                 | 251 us: 1.32x faster                                  |
| xml_etree_generate   | 99.4 ms                                                | 80.8 ms: 1.23x faster                                 |
| json_loads           | 31.2 us                                                | 25.6 us: 1.22x faster                                 |
| json_dumps           | 14.2 ms                                                | 12.6 ms: 1.12x faster                                 |
| xml_etree_iterparse  | 115 ms                                                 | 105 ms: 1.10x faster                                  |
| pickle_list          | 5.08 us                                                | 4.68 us: 1.09x faster                                 |
| xml_etree_parse      | 168 ms                                                 | 156 ms: 1.08x faster                                  |
| pickle               | 10.7 us                                                | 9.95 us: 1.07x faster                                 |
| pickle_dict          | 29.6 us                                                | 27.7 us: 1.07x faster                                 |
| unpickle             | 14.4 us                                                | 14.6 us: 1.01x slower                                 |
| Geometric mean       | (ref)                                                  | 1.15x faster                                          |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211208-linux-x86_64-python-main-3.11.0a3-2e91dba |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 8.00 ms: 1.82x faster                                 |
| python_startup_no_site | 5.93 ms                                                | 5.78 ms: 1.03x faster                                 |
| Geometric mean         | (ref)                                                  | 1.37x faster                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211208-linux-x86_64-python-main-3.11.0a3-2e91dba |
|-----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| mako            | 16.3 ms                                                | 11.9 ms: 1.37x faster                                 |
| django_template | 48.2 ms                                                | 36.5 ms: 1.32x faster                                 |
| Geometric mean  | (ref)                                                  | 1.34x faster                                          |

All benchmarks:
===============

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211208-linux-x86_64-python-main-3.11.0a3-2e91dba |
|-------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| python_startup          | 14.6 ms                                                | 8.00 ms: 1.82x faster                                 |
| deltablue               | 7.91 ms                                                | 4.54 ms: 1.74x faster                                 |
| logging_silent          | 190 ns                                                 | 110 ns: 1.72x faster                                  |
| scimark_sor             | 220 ms                                                 | 130 ms: 1.68x faster                                  |
| spectral_norm           | 170 ms                                                 | 104 ms: 1.64x faster                                  |
| scimark_monte_carlo     | 118 ms                                                 | 74.0 ms: 1.60x faster                                 |
| nbody                   | 154 ms                                                 | 96.1 ms: 1.60x faster                                 |
| scimark_lu              | 176 ms                                                 | 112 ms: 1.58x faster                                  |
| chaos                   | 115 ms                                                 | 73.9 ms: 1.56x faster                                 |
| hexiom                  | 10.4 ms                                                | 6.77 ms: 1.54x faster                                 |
| go                      | 240 ms                                                 | 158 ms: 1.52x faster                                  |
| raytrace                | 507 ms                                                 | 333 ms: 1.52x faster                                  |
| pyflate                 | 716 ms                                                 | 477 ms: 1.50x faster                                  |
| float                   | 117 ms                                                 | 79.2 ms: 1.48x faster                                 |
| richards                | 79.3 ms                                                | 54.5 ms: 1.45x faster                                 |
| crypto_pyaes            | 128 ms                                                 | 88.1 ms: 1.45x faster                                 |
| scimark_fft             | 466 ms                                                 | 332 ms: 1.40x faster                                  |
| logging_format          | 9.09 us                                                | 6.49 us: 1.40x faster                                 |
| pickle_pure_python      | 484 us                                                 | 347 us: 1.40x faster                                  |
| logging_simple          | 8.30 us                                                | 5.97 us: 1.39x faster                                 |
| fannkuch                | 532 ms                                                 | 386 ms: 1.38x faster                                  |
| mako                    | 16.3 ms                                                | 11.9 ms: 1.37x faster                                 |
| xml_etree_process       | 79.1 ms                                                | 57.8 ms: 1.37x faster                                 |
| regex_compile           | 188 ms                                                 | 139 ms: 1.36x faster                                  |
| scimark_sparse_mat_mult | 6.47 ms                                                | 4.77 ms: 1.36x faster                                 |
| 2to3                    | 348 ms                                                 | 264 ms: 1.32x faster                                  |
| django_template         | 48.2 ms                                                | 36.5 ms: 1.32x faster                                 |
| thrift                  | 1.07 ms                                                | 814 us: 1.32x faster                                  |
| unpickle_pure_python    | 331 us                                                 | 251 us: 1.32x faster                                  |
| chameleon               | 9.68 ms                                                | 7.44 ms: 1.30x faster                                 |
| html5lib                | 88.9 ms                                                | 68.5 ms: 1.30x faster                                 |
| pycparser               | 1.58 sec                                               | 1.24 sec: 1.27x faster                                |
| tornado_http            | 136 ms                                                 | 108 ms: 1.26x faster                                  |
| dulwich_log             | 84.3 ms                                                | 67.2 ms: 1.25x faster                                 |
| nqueens                 | 106 ms                                                 | 84.6 ms: 1.25x faster                                 |
| xml_etree_generate      | 99.4 ms                                                | 80.8 ms: 1.23x faster                                 |
| unpack_sequence         | 60.0 ns                                                | 49.2 ns: 1.22x faster                                 |
| json_loads              | 31.2 us                                                | 25.6 us: 1.22x faster                                 |
| sympy_integrate         | 25.8 ms                                                | 21.7 ms: 1.19x faster                                 |
| json                    | 5.69 ms                                                | 4.83 ms: 1.18x faster                                 |
| meteor_contest          | 120 ms                                                 | 104 ms: 1.15x faster                                  |
| sympy_sum               | 196 ms                                                 | 172 ms: 1.14x faster                                  |
| regex_v8                | 27.8 ms                                                | 24.5 ms: 1.13x faster                                 |
| regex_effbot            | 3.63 ms                                                | 3.21 ms: 1.13x faster                                 |
| json_dumps              | 14.2 ms                                                | 12.6 ms: 1.12x faster                                 |
| sympy_str               | 346 ms                                                 | 308 ms: 1.12x faster                                  |
| sympy_expand            | 566 ms                                                 | 509 ms: 1.11x faster                                  |
| telco                   | 7.27 ms                                                | 6.56 ms: 1.11x faster                                 |
| sqlite_synth            | 3.02 us                                                | 2.74 us: 1.11x faster                                 |
| xml_etree_iterparse     | 115 ms                                                 | 105 ms: 1.10x faster                                  |
| pickle_list             | 5.08 us                                                | 4.68 us: 1.09x faster                                 |
| xml_etree_parse         | 168 ms                                                 | 156 ms: 1.08x faster                                  |
| pickle                  | 10.7 us                                                | 9.95 us: 1.07x faster                                 |
| regex_dna               | 227 ms                                                 | 212 ms: 1.07x faster                                  |
| pickle_dict             | 29.6 us                                                | 27.7 us: 1.07x faster                                 |
| pathlib                 | 20.5 ms                                                | 19.4 ms: 1.05x faster                                 |
| python_startup_no_site  | 5.93 ms                                                | 5.78 ms: 1.03x faster                                 |
| unpickle                | 14.4 us                                                | 14.6 us: 1.01x slower                                 |
| pidigits                | 191 ms                                                 | 198 ms: 1.04x slower                                  |
| Geometric mean          | (ref)                                                  | 1.29x faster                                          |

Benchmark hidden because not significant (1): unpickle_list
Ignored benchmarks (41) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, async_generators, async_tree_cpu_io_mixed, async_tree_io, async_tree_memoization, async_tree_none, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, bench_mp_pool, bench_thread_pool, comprehensions, coroutines, coverage, create_gc_cycles, dask, deepcopy, deepcopy_memo, deepcopy_reduce, djangocms, docutils, flaskblogging, gc_traversal, generators, genshi_text, genshi_xml, gunicorn, mdp, mypy2, pprint_pformat, pprint_safe_repr, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, sqlglot_normalize, sqlglot_optimize, sqlglot_parse, sqlglot_transpile, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.26x
- 95% likely to have a speedup of 1.25x
- 99% likely to have a speedup of 1.22x


# Memory

- memory change: 1.07x