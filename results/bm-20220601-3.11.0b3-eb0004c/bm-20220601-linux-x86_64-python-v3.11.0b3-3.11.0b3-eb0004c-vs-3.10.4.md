
# Results vs. 3.10.4

- fork: python
- ref: v3.11.0b3
- machine: linux-x86_64
- commit hash: eb0004c
- commit date: 2022-06-01
- overall geometric mean: 1.33x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.27x faster
- Memory change: 1.09x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220601-linux-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 256 ms: 1.36x faster                                       |
| chameleon      | 9.68 ms                                                | 6.42 ms: 1.51x faster                                      |
| docutils       | 3.30 sec                                               | 2.56 sec: 1.29x faster                                     |
| html5lib       | 88.9 ms                                                | 62.8 ms: 1.41x faster                                      |
| tornado_http   | 136 ms                                                 | 94.7 ms: 1.44x faster                                      |
| Geometric mean | (ref)                                                  | 1.40x faster                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220601-linux-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 525 ms: 1.39x faster                                       |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 735 ms: 1.38x faster                                       |
| async_tree_memoization  | 870 ms                                                 | 636 ms: 1.37x faster                                       |
| async_tree_io           | 1.77 sec                                               | 1.30 sec: 1.36x faster                                     |
| Geometric mean          | (ref)                                                  | 1.37x faster                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220601-linux-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| nbody          | 154 ms                                                 | 94.9 ms: 1.62x faster                                      |
| float          | 117 ms                                                 | 73.9 ms: 1.59x faster                                      |
| pidigits       | 191 ms                                                 | 194 ms: 1.02x slower                                       |
| Geometric mean | (ref)                                                  | 1.36x faster                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220601-linux-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 136 ms: 1.38x faster                                       |
| regex_v8       | 27.8 ms                                                | 21.4 ms: 1.30x faster                                      |
| regex_effbot   | 3.63 ms                                                | 2.92 ms: 1.24x faster                                      |
| regex_dna      | 227 ms                                                 | 194 ms: 1.17x faster                                       |
| Geometric mean | (ref)                                                  | 1.27x faster                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220601-linux-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 301 us: 1.61x faster                                       |
| xml_etree_process    | 79.1 ms                                                | 53.6 ms: 1.48x faster                                      |
| unpickle_pure_python | 331 us                                                 | 227 us: 1.45x faster                                       |
| xml_etree_generate   | 99.4 ms                                                | 76.7 ms: 1.30x faster                                      |
| json_loads           | 31.2 us                                                | 24.9 us: 1.26x faster                                      |
| pickle_list          | 5.08 us                                                | 4.27 us: 1.19x faster                                      |
| pickle_dict          | 29.6 us                                                | 26.0 us: 1.14x faster                                      |
| pickle               | 10.7 us                                                | 9.37 us: 1.14x faster                                      |
| json_dumps           | 14.2 ms                                                | 12.7 ms: 1.12x faster                                      |
| unpickle             | 14.4 us                                                | 13.3 us: 1.08x faster                                      |
| xml_etree_iterparse  | 115 ms                                                 | 108 ms: 1.07x faster                                       |
| xml_etree_parse      | 168 ms                                                 | 158 ms: 1.06x faster                                       |
| unpickle_list        | 5.20 us                                                | 4.96 us: 1.05x faster                                      |
| Geometric mean       | (ref)                                                  | 1.21x faster                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220601-linux-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 8.51 ms: 1.71x faster                                      |
| python_startup_no_site | 5.93 ms                                                | 6.01 ms: 1.01x slower                                      |
| Geometric mean         | (ref)                                                  | 1.30x faster                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220601-linux-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| mako            | 16.3 ms                                                | 9.99 ms: 1.63x faster                                      |
| django_template | 48.2 ms                                                | 33.0 ms: 1.46x faster                                      |
| genshi_text     | 31.8 ms                                                | 22.0 ms: 1.44x faster                                      |
| genshi_xml      | 66.0 ms                                                | 52.3 ms: 1.26x faster                                      |
| Geometric mean  | (ref)                                                  | 1.44x faster                                               |

All benchmarks:
===============

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220601-linux-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| deltablue               | 7.91 ms                                                | 3.65 ms: 2.17x faster                                      |
| scimark_sor             | 220 ms                                                 | 114 ms: 1.92x faster                                       |
| logging_silent          | 190 ns                                                 | 101 ns: 1.87x faster                                       |
| scimark_monte_carlo     | 118 ms                                                 | 66.6 ms: 1.78x faster                                      |
| pyflate                 | 716 ms                                                 | 409 ms: 1.75x faster                                       |
| richards                | 79.3 ms                                                | 45.3 ms: 1.75x faster                                      |
| spectral_norm           | 170 ms                                                 | 97.5 ms: 1.74x faster                                      |
| crypto_pyaes            | 128 ms                                                 | 73.6 ms: 1.74x faster                                      |
| raytrace                | 507 ms                                                 | 292 ms: 1.73x faster                                       |
| go                      | 240 ms                                                 | 139 ms: 1.72x faster                                       |
| python_startup          | 14.6 ms                                                | 8.51 ms: 1.71x faster                                      |
| chaos                   | 115 ms                                                 | 68.2 ms: 1.69x faster                                      |
| scimark_lu              | 176 ms                                                 | 107 ms: 1.64x faster                                       |
| mako                    | 16.3 ms                                                | 9.99 ms: 1.63x faster                                      |
| hexiom                  | 10.4 ms                                                | 6.36 ms: 1.63x faster                                      |
| nbody                   | 154 ms                                                 | 94.9 ms: 1.62x faster                                      |
| pickle_pure_python      | 484 us                                                 | 301 us: 1.61x faster                                       |
| float                   | 117 ms                                                 | 73.9 ms: 1.59x faster                                      |
| deepcopy_memo           | 58.5 us                                                | 36.9 us: 1.58x faster                                      |
| chameleon               | 9.68 ms                                                | 6.42 ms: 1.51x faster                                      |
| xml_etree_process       | 79.1 ms                                                | 53.6 ms: 1.48x faster                                      |
| pprint_safe_repr        | 1.02 sec                                               | 694 ms: 1.47x faster                                       |
| django_template         | 48.2 ms                                                | 33.0 ms: 1.46x faster                                      |
| unpickle_pure_python    | 331 us                                                 | 227 us: 1.45x faster                                       |
| pprint_pformat          | 2.10 sec                                               | 1.45 sec: 1.45x faster                                     |
| genshi_text             | 31.8 ms                                                | 22.0 ms: 1.44x faster                                      |
| tornado_http            | 136 ms                                                 | 94.7 ms: 1.44x faster                                      |
| logging_format          | 9.09 us                                                | 6.35 us: 1.43x faster                                      |
| logging_simple          | 8.30 us                                                | 5.82 us: 1.43x faster                                      |
| scimark_fft             | 466 ms                                                 | 328 ms: 1.42x faster                                       |
| html5lib                | 88.9 ms                                                | 62.8 ms: 1.41x faster                                      |
| scimark_sparse_mat_mult | 6.47 ms                                                | 4.57 ms: 1.41x faster                                      |
| deepcopy                | 479 us                                                 | 340 us: 1.41x faster                                       |
| thrift                  | 1.07 ms                                                | 763 us: 1.40x faster                                       |
| deepcopy_reduce         | 4.17 us                                                | 2.98 us: 1.40x faster                                      |
| async_tree_none         | 728 ms                                                 | 525 ms: 1.39x faster                                       |
| regex_compile           | 188 ms                                                 | 136 ms: 1.38x faster                                       |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 735 ms: 1.38x faster                                       |
| async_tree_memoization  | 870 ms                                                 | 636 ms: 1.37x faster                                       |
| gunicorn                | 1.53 ms                                                | 1.12 ms: 1.36x faster                                      |
| 2to3                    | 348 ms                                                 | 256 ms: 1.36x faster                                       |
| async_tree_io           | 1.77 sec                                               | 1.30 sec: 1.36x faster                                     |
| aiohttp                 | 1.44 ms                                                | 1.06 ms: 1.36x faster                                      |
| fannkuch                | 532 ms                                                 | 393 ms: 1.35x faster                                       |
| coroutines              | 35.1 ms                                                | 26.0 ms: 1.35x faster                                      |
| pycparser               | 1.58 sec                                               | 1.18 sec: 1.34x faster                                     |
| dulwich_log             | 84.3 ms                                                | 63.0 ms: 1.34x faster                                      |
| sqlglot_normalize       | 143 ms                                                 | 109 ms: 1.31x faster                                       |
| sqlalchemy_imperative   | 23.3 ms                                                | 17.8 ms: 1.31x faster                                      |
| xml_etree_generate      | 99.4 ms                                                | 76.7 ms: 1.30x faster                                      |
| regex_v8                | 27.8 ms                                                | 21.4 ms: 1.30x faster                                      |
| docutils                | 3.30 sec                                               | 2.56 sec: 1.29x faster                                     |
| sqlglot_optimize        | 69.2 ms                                                | 54.0 ms: 1.28x faster                                      |
| genshi_xml              | 66.0 ms                                                | 52.3 ms: 1.26x faster                                      |
| sqlglot_transpile       | 2.57 ms                                                | 2.04 ms: 1.26x faster                                      |
| nqueens                 | 106 ms                                                 | 83.8 ms: 1.26x faster                                      |
| sqlalchemy_declarative  | 172 ms                                                 | 137 ms: 1.26x faster                                       |
| json_loads              | 31.2 us                                                | 24.9 us: 1.26x faster                                      |
| unpack_sequence         | 60.0 ns                                                | 48.0 ns: 1.25x faster                                      |
| async_generators        | 444 ms                                                 | 356 ms: 1.25x faster                                       |
| sympy_integrate         | 25.8 ms                                                | 20.7 ms: 1.25x faster                                      |
| regex_effbot            | 3.63 ms                                                | 2.92 ms: 1.24x faster                                      |
| sqlglot_parse           | 2.17 ms                                                | 1.75 ms: 1.24x faster                                      |
| flaskblogging           | 8.58 ms                                                | 7.04 ms: 1.22x faster                                      |
| sympy_sum               | 196 ms                                                 | 162 ms: 1.21x faster                                       |
| sympy_str               | 346 ms                                                 | 285 ms: 1.21x faster                                       |
| bench_thread_pool       | 986 us                                                 | 816 us: 1.21x faster                                       |
| sympy_expand            | 566 ms                                                 | 469 ms: 1.21x faster                                       |
| json                    | 5.69 ms                                                | 4.74 ms: 1.20x faster                                      |
| dask                    | 441 ms                                                 | 368 ms: 1.20x faster                                       |
| sqlite_synth            | 3.02 us                                                | 2.53 us: 1.19x faster                                      |
| pickle_list             | 5.08 us                                                | 4.27 us: 1.19x faster                                      |
| pylint                  | 551 ms                                                 | 465 ms: 1.19x faster                                       |
| regex_dna               | 227 ms                                                 | 194 ms: 1.17x faster                                       |
| djangocms               | 38.4 us                                                | 33.2 us: 1.16x faster                                      |
| meteor_contest          | 120 ms                                                 | 105 ms: 1.14x faster                                       |
| pickle_dict             | 29.6 us                                                | 26.0 us: 1.14x faster                                      |
| pickle                  | 10.7 us                                                | 9.37 us: 1.14x faster                                      |
| pathlib                 | 20.5 ms                                                | 18.1 ms: 1.13x faster                                      |
| json_dumps              | 14.2 ms                                                | 12.7 ms: 1.12x faster                                      |
| comprehensions          | 28.8 us                                                | 25.9 us: 1.11x faster                                      |
| telco                   | 7.27 ms                                                | 6.59 ms: 1.10x faster                                      |
| generators              | 80.1 ms                                                | 73.8 ms: 1.09x faster                                      |
| unpickle                | 14.4 us                                                | 13.3 us: 1.08x faster                                      |
| create_gc_cycles        | 1.62 ms                                                | 1.51 ms: 1.07x faster                                      |
| xml_etree_iterparse     | 115 ms                                                 | 108 ms: 1.07x faster                                       |
| xml_etree_parse         | 168 ms                                                 | 158 ms: 1.06x faster                                       |
| mdp                     | 2.85 sec                                               | 2.69 sec: 1.06x faster                                     |
| unpickle_list           | 5.20 us                                                | 4.96 us: 1.05x faster                                      |
| asyncio_tcp             | 922 ms                                                 | 888 ms: 1.04x faster                                       |
| python_startup_no_site  | 5.93 ms                                                | 6.01 ms: 1.01x slower                                      |
| pidigits                | 191 ms                                                 | 194 ms: 1.02x slower                                       |
| gc_traversal            | 3.62 ms                                                | 3.79 ms: 1.05x slower                                      |
| Geometric mean          | (ref)                                                  | 1.33x faster                                               |

Benchmark hidden because not significant (1): bench_mp_pool
Ignored benchmarks (7) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp_ssl, asyncio_websockets, coverage, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.30x
- 95% likely to have a speedup of 1.29x
- 99% likely to have a speedup of 1.27x


# Memory

- memory change: 1.09x