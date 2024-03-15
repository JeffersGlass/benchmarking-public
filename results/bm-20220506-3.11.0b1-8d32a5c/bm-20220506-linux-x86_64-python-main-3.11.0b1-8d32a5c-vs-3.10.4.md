
# Results vs. 3.10.4

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: 8d32a5c
- commit date: 2022-05-06
- overall geometric mean: 1.38x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.28x faster
- Memory change: 1.04x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220506-linux-x86_64-python-main-3.11.0b1-8d32a5c |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| 2to3           | 348 ms                                                 | 256 ms: 1.36x faster                                  |
| chameleon      | 9.68 ms                                                | 6.57 ms: 1.47x faster                                 |
| html5lib       | 88.9 ms                                                | 60.1 ms: 1.48x faster                                 |
| tornado_http   | 136 ms                                                 | 94.6 ms: 1.44x faster                                 |
| Geometric mean | (ref)                                                  | 1.44x faster                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220506-linux-x86_64-python-main-3.11.0b1-8d32a5c |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| nbody          | 154 ms                                                 | 93.1 ms: 1.65x faster                                 |
| float          | 117 ms                                                 | 72.5 ms: 1.61x faster                                 |
| pidigits       | 191 ms                                                 | 190 ms: 1.01x faster                                  |
| Geometric mean | (ref)                                                  | 1.39x faster                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220506-linux-x86_64-python-main-3.11.0b1-8d32a5c |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 135 ms: 1.40x faster                                  |
| regex_v8       | 27.8 ms                                                | 21.6 ms: 1.29x faster                                 |
| regex_effbot   | 3.63 ms                                                | 2.93 ms: 1.24x faster                                 |
| regex_dna      | 227 ms                                                 | 204 ms: 1.11x faster                                  |
| Geometric mean | (ref)                                                  | 1.25x faster                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220506-linux-x86_64-python-main-3.11.0b1-8d32a5c |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 305 us: 1.59x faster                                  |
| xml_etree_process    | 79.1 ms                                                | 53.6 ms: 1.48x faster                                 |
| unpickle_pure_python | 331 us                                                 | 229 us: 1.45x faster                                  |
| xml_etree_generate   | 99.4 ms                                                | 76.5 ms: 1.30x faster                                 |
| json_loads           | 31.2 us                                                | 25.4 us: 1.23x faster                                 |
| pickle_list          | 5.08 us                                                | 4.26 us: 1.19x faster                                 |
| pickle_dict          | 29.6 us                                                | 25.6 us: 1.16x faster                                 |
| json_dumps           | 14.2 ms                                                | 12.4 ms: 1.15x faster                                 |
| pickle               | 10.7 us                                                | 9.56 us: 1.11x faster                                 |
| xml_etree_iterparse  | 115 ms                                                 | 104 ms: 1.11x faster                                  |
| unpickle             | 14.4 us                                                | 13.4 us: 1.08x faster                                 |
| xml_etree_parse      | 168 ms                                                 | 157 ms: 1.07x faster                                  |
| unpickle_list        | 5.20 us                                                | 5.05 us: 1.03x faster                                 |
| Geometric mean       | (ref)                                                  | 1.21x faster                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220506-linux-x86_64-python-main-3.11.0b1-8d32a5c |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 8.25 ms: 1.77x faster                                 |
| python_startup_no_site | 5.93 ms                                                | 6.16 ms: 1.04x slower                                 |
| Geometric mean         | (ref)                                                  | 1.30x faster                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220506-linux-x86_64-python-main-3.11.0b1-8d32a5c |
|-----------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| mako            | 16.3 ms                                                | 9.88 ms: 1.65x faster                                 |
| django_template | 48.2 ms                                                | 32.8 ms: 1.47x faster                                 |
| Geometric mean  | (ref)                                                  | 1.56x faster                                          |

All benchmarks:
===============

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220506-linux-x86_64-python-main-3.11.0b1-8d32a5c |
|-------------------------|:------------------------------------------------------:|:-----------------------------------------------------:|
| deltablue               | 7.91 ms                                                | 3.61 ms: 2.19x faster                                 |
| logging_silent          | 190 ns                                                 | 98.2 ns: 1.93x faster                                 |
| scimark_sor             | 220 ms                                                 | 115 ms: 1.92x faster                                  |
| scimark_monte_carlo     | 118 ms                                                 | 66.5 ms: 1.78x faster                                 |
| python_startup          | 14.6 ms                                                | 8.25 ms: 1.77x faster                                 |
| go                      | 240 ms                                                 | 136 ms: 1.76x faster                                  |
| pyflate                 | 716 ms                                                 | 411 ms: 1.74x faster                                  |
| spectral_norm           | 170 ms                                                 | 97.6 ms: 1.74x faster                                 |
| raytrace                | 507 ms                                                 | 294 ms: 1.72x faster                                  |
| crypto_pyaes            | 128 ms                                                 | 74.3 ms: 1.72x faster                                 |
| richards                | 79.3 ms                                                | 46.4 ms: 1.71x faster                                 |
| chaos                   | 115 ms                                                 | 68.6 ms: 1.68x faster                                 |
| hexiom                  | 10.4 ms                                                | 6.29 ms: 1.65x faster                                 |
| mako                    | 16.3 ms                                                | 9.88 ms: 1.65x faster                                 |
| nbody                   | 154 ms                                                 | 93.1 ms: 1.65x faster                                 |
| scimark_lu              | 176 ms                                                 | 109 ms: 1.61x faster                                  |
| float                   | 117 ms                                                 | 72.5 ms: 1.61x faster                                 |
| pickle_pure_python      | 484 us                                                 | 305 us: 1.59x faster                                  |
| html5lib                | 88.9 ms                                                | 60.1 ms: 1.48x faster                                 |
| xml_etree_process       | 79.1 ms                                                | 53.6 ms: 1.48x faster                                 |
| chameleon               | 9.68 ms                                                | 6.57 ms: 1.47x faster                                 |
| django_template         | 48.2 ms                                                | 32.8 ms: 1.47x faster                                 |
| thrift                  | 1.07 ms                                                | 741 us: 1.45x faster                                  |
| unpickle_pure_python    | 331 us                                                 | 229 us: 1.45x faster                                  |
| tornado_http            | 136 ms                                                 | 94.6 ms: 1.44x faster                                 |
| scimark_fft             | 466 ms                                                 | 325 ms: 1.43x faster                                  |
| scimark_sparse_mat_mult | 6.47 ms                                                | 4.57 ms: 1.42x faster                                 |
| logging_format          | 9.09 us                                                | 6.44 us: 1.41x faster                                 |
| logging_simple          | 8.30 us                                                | 5.89 us: 1.41x faster                                 |
| regex_compile           | 188 ms                                                 | 135 ms: 1.40x faster                                  |
| fannkuch                | 532 ms                                                 | 385 ms: 1.38x faster                                  |
| 2to3                    | 348 ms                                                 | 256 ms: 1.36x faster                                  |
| unpack_sequence         | 60.0 ns                                                | 44.3 ns: 1.36x faster                                 |
| dulwich_log             | 84.3 ms                                                | 62.8 ms: 1.34x faster                                 |
| pycparser               | 1.58 sec                                               | 1.18 sec: 1.33x faster                                |
| xml_etree_generate      | 99.4 ms                                                | 76.5 ms: 1.30x faster                                 |
| regex_v8                | 27.8 ms                                                | 21.6 ms: 1.29x faster                                 |
| sympy_integrate         | 25.8 ms                                                | 20.5 ms: 1.26x faster                                 |
| nqueens                 | 106 ms                                                 | 84.7 ms: 1.25x faster                                 |
| regex_effbot            | 3.63 ms                                                | 2.93 ms: 1.24x faster                                 |
| json_loads              | 31.2 us                                                | 25.4 us: 1.23x faster                                 |
| sympy_sum               | 196 ms                                                 | 161 ms: 1.22x faster                                  |
| sympy_str               | 346 ms                                                 | 284 ms: 1.22x faster                                  |
| sympy_expand            | 566 ms                                                 | 468 ms: 1.21x faster                                  |
| sqlite_synth            | 3.02 us                                                | 2.53 us: 1.20x faster                                 |
| pickle_list             | 5.08 us                                                | 4.26 us: 1.19x faster                                 |
| json                    | 5.69 ms                                                | 4.91 ms: 1.16x faster                                 |
| pickle_dict             | 29.6 us                                                | 25.6 us: 1.16x faster                                 |
| json_dumps              | 14.2 ms                                                | 12.4 ms: 1.15x faster                                 |
| pathlib                 | 20.5 ms                                                | 17.9 ms: 1.14x faster                                 |
| meteor_contest          | 120 ms                                                 | 105 ms: 1.14x faster                                  |
| pickle                  | 10.7 us                                                | 9.56 us: 1.11x faster                                 |
| regex_dna               | 227 ms                                                 | 204 ms: 1.11x faster                                  |
| xml_etree_iterparse     | 115 ms                                                 | 104 ms: 1.11x faster                                  |
| unpickle                | 14.4 us                                                | 13.4 us: 1.08x faster                                 |
| xml_etree_parse         | 168 ms                                                 | 157 ms: 1.07x faster                                  |
| telco                   | 7.27 ms                                                | 6.84 ms: 1.06x faster                                 |
| unpickle_list           | 5.20 us                                                | 5.05 us: 1.03x faster                                 |
| pidigits                | 191 ms                                                 | 190 ms: 1.01x faster                                  |
| python_startup_no_site  | 5.93 ms                                                | 6.16 ms: 1.04x slower                                 |
| Geometric mean          | (ref)                                                  | 1.38x faster                                          |
Ignored benchmarks (41) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, async_generators, async_tree_cpu_io_mixed, async_tree_io, async_tree_memoization, async_tree_none, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, bench_mp_pool, bench_thread_pool, comprehensions, coroutines, coverage, create_gc_cycles, dask, deepcopy, deepcopy_memo, deepcopy_reduce, djangocms, docutils, flaskblogging, gc_traversal, generators, genshi_text, genshi_xml, gunicorn, mdp, mypy2, pprint_pformat, pprint_safe_repr, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, sqlglot_normalize, sqlglot_optimize, sqlglot_parse, sqlglot_transpile, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.34x
- 95% likely to have a speedup of 1.32x
- 99% likely to have a speedup of 1.28x


# Memory

- memory change: 1.04x