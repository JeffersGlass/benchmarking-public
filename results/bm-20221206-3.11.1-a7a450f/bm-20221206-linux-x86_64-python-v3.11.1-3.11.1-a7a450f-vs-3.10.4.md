
# Results vs. 3.10.4

- fork: python
- ref: v3.11.1
- machine: linux-x86_64
- commit hash: a7a450f
- commit date: 2022-12-06
- overall geometric mean: 1.32x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.26x faster
- Memory change: 1.09x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-linux-x86_64-python-v3.11.1-3.11.1-a7a450f |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 258 ms: 1.35x faster                                   |
| chameleon      | 9.68 ms                                                | 6.63 ms: 1.46x faster                                  |
| docutils       | 3.30 sec                                               | 2.57 sec: 1.28x faster                                 |
| html5lib       | 88.9 ms                                                | 63.4 ms: 1.40x faster                                  |
| tornado_http   | 136 ms                                                 | 99.8 ms: 1.37x faster                                  |
| Geometric mean | (ref)                                                  | 1.37x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-linux-x86_64-python-v3.11.1-3.11.1-a7a450f |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 523 ms: 1.39x faster                                   |
| async_tree_memoization  | 870 ms                                                 | 627 ms: 1.39x faster                                   |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 742 ms: 1.37x faster                                   |
| async_tree_io           | 1.77 sec                                               | 1.31 sec: 1.35x faster                                 |
| Geometric mean          | (ref)                                                  | 1.38x faster                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-linux-x86_64-python-v3.11.1-3.11.1-a7a450f |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| nbody          | 154 ms                                                 | 95.4 ms: 1.61x faster                                  |
| float          | 117 ms                                                 | 76.0 ms: 1.54x faster                                  |
| pidigits       | 191 ms                                                 | 190 ms: 1.01x faster                                   |
| Geometric mean | (ref)                                                  | 1.36x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-linux-x86_64-python-v3.11.1-3.11.1-a7a450f |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 137 ms: 1.37x faster                                   |
| regex_v8       | 27.8 ms                                                | 22.3 ms: 1.25x faster                                  |
| regex_dna      | 227 ms                                                 | 200 ms: 1.13x faster                                   |
| regex_effbot   | 3.63 ms                                                | 3.31 ms: 1.10x faster                                  |
| Geometric mean | (ref)                                                  | 1.21x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-linux-x86_64-python-v3.11.1-3.11.1-a7a450f |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 310 us: 1.56x faster                                   |
| xml_etree_process    | 79.1 ms                                                | 53.7 ms: 1.47x faster                                  |
| unpickle_pure_python | 331 us                                                 | 229 us: 1.45x faster                                   |
| json_loads           | 31.2 us                                                | 24.0 us: 1.30x faster                                  |
| xml_etree_generate   | 99.4 ms                                                | 76.6 ms: 1.30x faster                                  |
| pickle_list          | 5.08 us                                                | 4.17 us: 1.22x faster                                  |
| json_dumps           | 14.2 ms                                                | 12.6 ms: 1.12x faster                                  |
| xml_etree_iterparse  | 115 ms                                                 | 103 ms: 1.12x faster                                   |
| pickle               | 10.7 us                                                | 9.72 us: 1.10x faster                                  |
| unpickle             | 14.4 us                                                | 13.4 us: 1.08x faster                                  |
| xml_etree_parse      | 168 ms                                                 | 158 ms: 1.07x faster                                   |
| unpickle_list        | 5.20 us                                                | 4.95 us: 1.05x faster                                  |
| pickle_dict          | 29.6 us                                                | 31.1 us: 1.05x slower                                  |
| Geometric mean       | (ref)                                                  | 1.20x faster                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-linux-x86_64-python-v3.11.1-3.11.1-a7a450f |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 8.49 ms: 1.72x faster                                  |
| python_startup_no_site | 5.93 ms                                                | 5.98 ms: 1.01x slower                                  |
| Geometric mean         | (ref)                                                  | 1.30x faster                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-linux-x86_64-python-v3.11.1-3.11.1-a7a450f |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako            | 16.3 ms                                                | 9.92 ms: 1.65x faster                                  |
| django_template | 48.2 ms                                                | 33.2 ms: 1.45x faster                                  |
| genshi_text     | 31.8 ms                                                | 22.1 ms: 1.44x faster                                  |
| genshi_xml      | 66.0 ms                                                | 52.5 ms: 1.26x faster                                  |
| Geometric mean  | (ref)                                                  | 1.44x faster                                           |

All benchmarks:
===============

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-linux-x86_64-python-v3.11.1-3.11.1-a7a450f |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| deltablue               | 7.91 ms                                                | 3.67 ms: 2.16x faster                                  |
| scimark_sor             | 220 ms                                                 | 116 ms: 1.90x faster                                   |
| logging_silent          | 190 ns                                                 | 102 ns: 1.86x faster                                   |
| crypto_pyaes            | 128 ms                                                 | 72.6 ms: 1.76x faster                                  |
| scimark_monte_carlo     | 118 ms                                                 | 68.4 ms: 1.73x faster                                  |
| raytrace                | 507 ms                                                 | 294 ms: 1.72x faster                                   |
| pyflate                 | 716 ms                                                 | 415 ms: 1.72x faster                                   |
| go                      | 240 ms                                                 | 140 ms: 1.72x faster                                   |
| python_startup          | 14.6 ms                                                | 8.49 ms: 1.72x faster                                  |
| richards                | 79.3 ms                                                | 46.9 ms: 1.69x faster                                  |
| spectral_norm           | 170 ms                                                 | 101 ms: 1.68x faster                                   |
| chaos                   | 115 ms                                                 | 69.6 ms: 1.66x faster                                  |
| mako                    | 16.3 ms                                                | 9.92 ms: 1.65x faster                                  |
| scimark_lu              | 176 ms                                                 | 107 ms: 1.64x faster                                   |
| hexiom                  | 10.4 ms                                                | 6.46 ms: 1.61x faster                                  |
| nbody                   | 154 ms                                                 | 95.4 ms: 1.61x faster                                  |
| sqlglot_parse           | 2.17 ms                                                | 1.38 ms: 1.57x faster                                  |
| deepcopy_memo           | 58.5 us                                                | 37.2 us: 1.57x faster                                  |
| pickle_pure_python      | 484 us                                                 | 310 us: 1.56x faster                                   |
| float                   | 117 ms                                                 | 76.0 ms: 1.54x faster                                  |
| sqlglot_transpile       | 2.57 ms                                                | 1.68 ms: 1.53x faster                                  |
| xml_etree_process       | 79.1 ms                                                | 53.7 ms: 1.47x faster                                  |
| pprint_pformat          | 2.10 sec                                               | 1.44 sec: 1.46x faster                                 |
| chameleon               | 9.68 ms                                                | 6.63 ms: 1.46x faster                                  |
| pprint_safe_repr        | 1.02 sec                                               | 700 ms: 1.45x faster                                   |
| django_template         | 48.2 ms                                                | 33.2 ms: 1.45x faster                                  |
| unpickle_pure_python    | 331 us                                                 | 229 us: 1.45x faster                                   |
| genshi_text             | 31.8 ms                                                | 22.1 ms: 1.44x faster                                  |
| scimark_fft             | 466 ms                                                 | 327 ms: 1.42x faster                                   |
| scimark_sparse_mat_mult | 6.47 ms                                                | 4.59 ms: 1.41x faster                                  |
| html5lib                | 88.9 ms                                                | 63.4 ms: 1.40x faster                                  |
| thrift                  | 1.07 ms                                                | 765 us: 1.40x faster                                   |
| logging_simple          | 8.30 us                                                | 5.95 us: 1.39x faster                                  |
| async_tree_none         | 728 ms                                                 | 523 ms: 1.39x faster                                   |
| logging_format          | 9.09 us                                                | 6.54 us: 1.39x faster                                  |
| async_tree_memoization  | 870 ms                                                 | 627 ms: 1.39x faster                                   |
| coroutines              | 35.1 ms                                                | 25.3 ms: 1.39x faster                                  |
| fannkuch                | 532 ms                                                 | 384 ms: 1.38x faster                                   |
| regex_compile           | 188 ms                                                 | 137 ms: 1.37x faster                                   |
| deepcopy                | 479 us                                                 | 349 us: 1.37x faster                                   |
| aiohttp                 | 1.44 ms                                                | 1.05 ms: 1.37x faster                                  |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 742 ms: 1.37x faster                                   |
| tornado_http            | 136 ms                                                 | 99.8 ms: 1.37x faster                                  |
| gunicorn                | 1.53 ms                                                | 1.13 ms: 1.36x faster                                  |
| pycparser               | 1.58 sec                                               | 1.16 sec: 1.35x faster                                 |
| async_tree_io           | 1.77 sec                                               | 1.31 sec: 1.35x faster                                 |
| 2to3                    | 348 ms                                                 | 258 ms: 1.35x faster                                   |
| deepcopy_reduce         | 4.17 us                                                | 3.09 us: 1.35x faster                                  |
| unpack_sequence         | 60.0 ns                                                | 44.6 ns: 1.34x faster                                  |
| dulwich_log             | 84.3 ms                                                | 63.5 ms: 1.33x faster                                  |
| sqlglot_normalize       | 143 ms                                                 | 108 ms: 1.32x faster                                   |
| json_loads              | 31.2 us                                                | 24.0 us: 1.30x faster                                  |
| sqlglot_optimize        | 69.2 ms                                                | 53.3 ms: 1.30x faster                                  |
| xml_etree_generate      | 99.4 ms                                                | 76.6 ms: 1.30x faster                                  |
| sqlalchemy_imperative   | 23.3 ms                                                | 18.0 ms: 1.30x faster                                  |
| docutils                | 3.30 sec                                               | 2.57 sec: 1.28x faster                                 |
| genshi_xml              | 66.0 ms                                                | 52.5 ms: 1.26x faster                                  |
| nqueens                 | 106 ms                                                 | 85.0 ms: 1.25x faster                                  |
| regex_v8                | 27.8 ms                                                | 22.3 ms: 1.25x faster                                  |
| async_generators        | 444 ms                                                 | 358 ms: 1.24x faster                                   |
| sympy_integrate         | 25.8 ms                                                | 21.0 ms: 1.23x faster                                  |
| json                    | 5.69 ms                                                | 4.63 ms: 1.23x faster                                  |
| sqlite_synth            | 3.02 us                                                | 2.47 us: 1.23x faster                                  |
| pickle_list             | 5.08 us                                                | 4.17 us: 1.22x faster                                  |
| sqlalchemy_declarative  | 172 ms                                                 | 141 ms: 1.22x faster                                   |
| bench_thread_pool       | 986 us                                                 | 813 us: 1.21x faster                                   |
| flaskblogging           | 8.58 ms                                                | 7.07 ms: 1.21x faster                                  |
| dask                    | 441 ms                                                 | 365 ms: 1.21x faster                                   |
| sympy_expand            | 566 ms                                                 | 472 ms: 1.20x faster                                   |
| sympy_str               | 346 ms                                                 | 289 ms: 1.20x faster                                   |
| pylint                  | 551 ms                                                 | 461 ms: 1.19x faster                                   |
| sympy_sum               | 196 ms                                                 | 166 ms: 1.18x faster                                   |
| djangocms               | 38.4 us                                                | 33.1 us: 1.16x faster                                  |
| regex_dna               | 227 ms                                                 | 200 ms: 1.13x faster                                   |
| pathlib                 | 20.5 ms                                                | 18.1 ms: 1.13x faster                                  |
| meteor_contest          | 120 ms                                                 | 106 ms: 1.13x faster                                   |
| json_dumps              | 14.2 ms                                                | 12.6 ms: 1.12x faster                                  |
| xml_etree_iterparse     | 115 ms                                                 | 103 ms: 1.12x faster                                   |
| pickle                  | 10.7 us                                                | 9.72 us: 1.10x faster                                  |
| regex_effbot            | 3.63 ms                                                | 3.31 ms: 1.10x faster                                  |
| generators              | 80.1 ms                                                | 73.3 ms: 1.09x faster                                  |
| create_gc_cycles        | 1.62 ms                                                | 1.48 ms: 1.09x faster                                  |
| telco                   | 7.27 ms                                                | 6.66 ms: 1.09x faster                                  |
| mdp                     | 2.85 sec                                               | 2.64 sec: 1.08x faster                                 |
| unpickle                | 14.4 us                                                | 13.4 us: 1.08x faster                                  |
| xml_etree_parse         | 168 ms                                                 | 158 ms: 1.07x faster                                   |
| unpickle_list           | 5.20 us                                                | 4.95 us: 1.05x faster                                  |
| asyncio_tcp             | 922 ms                                                 | 889 ms: 1.04x faster                                   |
| pidigits                | 191 ms                                                 | 190 ms: 1.01x faster                                   |
| python_startup_no_site  | 5.93 ms                                                | 5.98 ms: 1.01x slower                                  |
| pickle_dict             | 29.6 us                                                | 31.1 us: 1.05x slower                                  |
| gc_traversal            | 3.62 ms                                                | 4.26 ms: 1.17x slower                                  |
| coverage                | 79.4 ms                                                | 104 ms: 1.31x slower                                   |
| Geometric mean          | (ref)                                                  | 1.32x faster                                           |

Benchmark hidden because not significant (1): bench_mp_pool
Ignored benchmarks (7) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp_ssl, asyncio_websockets, comprehensions, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.30x
- 95% likely to have a speedup of 1.29x
- 99% likely to have a speedup of 1.26x


# Memory

- memory change: 1.09x